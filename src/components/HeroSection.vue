<template>
    <div class="w-full relative pt-32">
        <div class="max-w-7xl mx-auto px-5 py-40">
            <div class="max-w-4xl">
                <h1 class="font-light sm:text-5xl text-3xl mb-4 text-white">
                    Hello! I'm Sean
                </h1>
                <h3 class="text-3xl font-thin">
                    A <span class="text-sky-300" id="autotype"></span>
                </h3>
                <p class="mt-4 mb-8 leading-relaxed">
                    A passionate frontend web developer dedicated to crafting immersive and user-friendly digital experiences. With expertise in HTML, CSS, JavaScript, and cutting-edge frameworks like Vue.js, React and Angular, I bring ideas to life with a perfect blend of creativity and functionality. Explore my projects and let's create digital experiences that captivate and resonate 🚀
                </p>
                <div class="flex flex-col md:flex-row md:space-x-4 space-y-2 md:space-y-0">
                    <button class="inline-flex text-white bg-sky-500 py-2 px-6 hover:bg-sky-600 rounded text-lg transition-all duration-200">
                        Let's Connect
                    </button>
                    <button class="inline-flex text-gray-400 bg-gray-800 py-2 px-6 hover:bg-gray-700 hover:text-white rounded text-lg transition-all duration-200">See Portfolios</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Typed from 'typed.js'

export default {
    mounted() {
        new Typed('#autotype', {
            strings: [
                'Software Engineer', 
                'Web Developer', 
                'UI/UX Designer', 
                'Multimedia Expert'
            ],
            typeSpeed: 50,
            startDelay: 100,
            backSpeed: 30,
            backDelay: 1500,
            loop: true
        });
    }
}

</script>