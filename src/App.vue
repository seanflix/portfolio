<template>
  <canvas class="absolute z-10 w-full h-full inset-0 opacity-50" id="demo-canvas"></canvas>
  <div class="relative h-screen overflow-y-scroll bg-gray-950 text-slate-400">
    <div class="relative z-20">
        <div class="mx-auto min-h-screen max-w-screen-xl px-6 py-12 font-sans md:px-12 md:py-16 lg:py-0">
            <div class="lg:flex lg:justify-between lg:gap-4">
                <Navbar />
                <main id="content" class="pt-24 lg:w-[52%] lg:py-24">
                    <About />
                    <Experience />
                </main>
            </div>
        </div>
      
      <!-- <Hero />
      <About />
      <Services />
      <Portfolio />
      <Work />
      <Testimonial />
      <Contact />
      <Footer /> -->
    </div>
  </div>
</template>

<script setup>

import { onMounted } from 'vue'

import Navbar from './components/NavbarSection.vue'
// import Hero from './components/HeroSection.vue'
import About from './components/AboutSection.vue'
import Experience from './components/ExperienceSection.vue'
// import Services from './components/ServicesSection.vue'
// import Portfolio from './components/PortfolioSection.vue'
// import Work from './components/WorkSection.vue'
// import Testimonial from './components/TestimonialSection.vue'
// import Contact from './components/ContactSection.vue'
// import Footer from './components/FooterSection.vue'

import { TweenLite, Circ } from 'gsap'

onMounted(() => {
  (function() {
    var width, height, canvas, ctx, points, target, animateHeader = true;

    // Main
    initHeader();
    initAnimation();
    addListeners();

    function initHeader() {
        width = window.innerWidth;
        height = window.innerHeight;
        target = {x: width/2, y: height/2};

        canvas = document.getElementById('demo-canvas');
        canvas.width = width;
        canvas.height = height;
        ctx = canvas.getContext('2d');

        // create points
        points = [];
        for(var x = 0; x < width; x = x + width/15) {
            for(var y = 0; y < height; y = y + height/15) {
                var px = x + Math.random()*width/15;
                var py = y + Math.random()*height/15;
                var p = {x: px, originX: px, y: py, originY: py };
                points.push(p);
            }
        }

        // for each point find the 5 closest points
        for(var i = 0; i < points.length; i++) {
            var closest = [];
            var p1 = points[i];
            for(var j = 0; j < points.length; j++) {
                var p2 = points[j]
                if(!(p1 == p2)) {
                    var placed = false;
                    for(var index = 0; index < 5; index++) {
                        if(!placed) {
                            if(closest[index] == undefined) {
                                closest[index] = p2;
                                placed = true;
                            }
                        }
                    }

                    for(var indexx = 0; indexx < 5; indexx++) {
                        if(!placed) {
                            if(getDistance(p1, p2) < getDistance(p1, closest[indexx])) {
                                closest[indexx] = p2;
                                placed = true;
                            }
                        }
                    }
                }
            }
            p1.closest = closest;
        }

        // assign a circle to each point
        for(var ii in points) {
            var c = new Circle(points[ii], 2+Math.random()*2, 'rgba(255,255,255,0.3)');
            points[ii].circle = c;
        }
    }

    // Event handling
    function addListeners() {
        if(!('ontouchstart' in window)) {
            window.addEventListener('mousemove', mouseMove);
        }
        window.addEventListener('scroll', scrollCheck);
        window.addEventListener('resize', resize);
    }

    function mouseMove(e) {
        var posx = 0;
        var posy = 0;
        if (e.pageX || e.pageY) {
            posx = e.pageX;
            posy = e.pageY;
        }
        else if (e.clientX || e.clientY)    {
            posx = e.clientX + document.body.scrollLeft + document.documentElement.scrollLeft;
            posy = e.clientY + document.body.scrollTop + document.documentElement.scrollTop;
        }
        target.x = posx;
        target.y = posy;
    }

    function scrollCheck() {
        animateHeader = true;
    }

    function resize() {
        width = window.innerWidth;
        height = window.innerHeight;
        canvas.width = width;
        canvas.height = height;
    }

    // animation
    function initAnimation() {
        animate();
        for(var iii in points) {
            shiftPoint(points[iii]);
        }
    }

    function animate() {
        if(animateHeader) {
            ctx.clearRect(0,0,width,height);
            for(var iiii in points) {
                // detect points in range
                if(Math.abs(getDistance(target, points[iiii])) < 4000) {
                    points[iiii].active = 0.3;
                    points[iiii].circle.active = 0.6;
                } else if(Math.abs(getDistance(target, points[iiii])) < 20000) {
                    points[iiii].active = 0.1;
                    points[iiii].circle.active = 0.3;
                } else if(Math.abs(getDistance(target, points[iiii])) < 40000) {
                    points[iiii].active = 0.02;
                    points[iiii].circle.active = 0.1;
                } else {
                    points[iiii].active = 0;
                    points[iiii].circle.active = 0;
                }

                drawLines(points[iiii]);
                points[iiii].circle.draw();
            }
        }
        requestAnimationFrame(animate);
    }

    function shiftPoint(p) {
        TweenLite.to(p, 1+1*Math.random(), {x:p.originX-50+Math.random()*100,
            y: p.originY-50+Math.random()*100, ease:Circ.easeInOut,
            onComplete: function() {
                shiftPoint(p);
            }});
    }

    // Canvas manipulation
    function drawLines(p) {
        if(!p.active) return;
        for(var iiiii in p.closest) {
            ctx.beginPath();
            ctx.moveTo(p.x, p.y);
            ctx.lineTo(p.closest[iiiii].x, p.closest[iiiii].y);
            ctx.strokeStyle = 'rgba(156,217,249,'+ p.active+')';
            ctx.stroke();
        }
    }

    function Circle(pos,rad,color) {
        var _this = this;

        // constructor
        (function() {
            _this.pos = pos || null;
            _this.radius = rad || null;
            _this.color = color || null;
        })();

        this.draw = function() {
            if(!_this.active) return;
            ctx.beginPath();
            ctx.arc(_this.pos.x, _this.pos.y, _this.radius, 0, 2 * Math.PI, false);
            ctx.fillStyle = 'rgba(156,217,249,'+ _this.active+')';
            ctx.fill();
        };
    }

    // Util
    function getDistance(p1, p2) {
        return Math.pow(p1.x - p2.x, 2) + Math.pow(p1.y - p2.y, 2);
    }

    })();
})

</script>