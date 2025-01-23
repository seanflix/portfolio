<template>
    <section id="designs" class="mb-16 scroll-mt-16 md:mb-24 lg:mb-36 lg:scroll-mt-24" aria-label="Selected projects">
        <div
            class="sticky top-0 z-20 -mx-6 mb-4 w-screen bg-slate-900/75 px-6 py-5 backdrop-blur md:-mx-12 md:px-12 lg:sr-only lg:relative lg:top-auto lg:mx-auto lg:w-full lg:px-0 lg:py-0 lg:opacity-0">
            <h2 class="text-sm font-bold uppercase tracking-widest text-slate-200 lg:sr-only">Designs</h2>
        </div>
        <div>
            <ul class="group/list">
                <li class="mb-12">
                    <div class="group relative grid gap-4 pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:hover:!opacity-100 lg:group-hover/list:opacity-50">
                        <div class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"></div>
                        <div class="z-10 sm:order-2 sm:col-span-6">
                            <h3>
                                <div @click="openModal('web1')" class="inline-flex hover:cursor-pointer items-baseline font-medium leading-tight text-slate-200 hover:text-teal-300 focus-visible:text-teal-300  group/link text-base">
                                    <span class="absolute -inset-x-4 -inset-y-2.5 hidden rounded md:-inset-x-6 md:-inset-y-4 lg:block"></span>
                                    <span>
                                        Photography Site
                                        <span class="inline-block">
                                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="inline-block h-4 w-4 shrink-0 transition-transform group-hover/link:-translate-y-1 group-hover/link:translate-x-1 group-focus-visible/link:-translate-y-1 group-focus-visible/link:translate-x-1 motion-reduce:transition-none ml-1 translate-y-px" aria-hidden="true">
                                                <path fill-rule="evenodd" d="M5.22 14.78a.75.75 0 001.06 0l7.22-7.22v5.69a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75h-7.5a.75.75 0 000 1.5h5.69l-7.22 7.22a.75.75 0 000 1.06z" clip-rule="evenodd"></path>
                                            </svg>
                                        </span>
                                    </span>
                                </div>
                            </h3>
                            <p class="mt-2 text-sm leading-normal">
                                A sleek and modern photography website design crafted to showcase stunning visuals with a clean layout, intuitive navigation, and a focus on enhancing the user experience for photographers and their clients.
                            </p>
                        </div>
                        <img alt="" loading="lazy" width="400" height="100"
                            decoding="async" data-nimg="1"
                            class="aspect-video object-top object-cover rounded border-2 border-slate-200/10 transition group-hover:border-slate-200/30 sm:order-1 sm:col-span-2 sm:translate-y-1"
                            style="color:transparent"
                            src="@/assets/portfolio/photography-site.jpg">
                    </div>
                </li>
                <li class="mb-12">
                    <div class="group relative grid gap-4 pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:hover:!opacity-100 lg:group-hover/list:opacity-50">
                        <div class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"></div>
                        <div class="z-10 sm:order-2 sm:col-span-6">
                            <h3>
                                <div @click="openModal('web2')" class="inline-flex hover:cursor-pointer items-baseline font-medium leading-tight text-slate-200 hover:text-teal-300 focus-visible:text-teal-300  group/link text-base">
                                    <span class="absolute -inset-x-4 -inset-y-2.5 hidden rounded md:-inset-x-6 md:-inset-y-4 lg:block"></span>
                                    <span>
                                        Sports Site
                                        <span class="inline-block">
                                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="inline-block h-4 w-4 shrink-0 transition-transform group-hover/link:-translate-y-1 group-hover/link:translate-x-1 group-focus-visible/link:-translate-y-1 group-focus-visible/link:translate-x-1 motion-reduce:transition-none ml-1 translate-y-px" aria-hidden="true">
                                                <path fill-rule="evenodd" d="M5.22 14.78a.75.75 0 001.06 0l7.22-7.22v5.69a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75h-7.5a.75.75 0 000 1.5h5.69l-7.22 7.22a.75.75 0 000 1.06z" clip-rule="evenodd"></path>
                                            </svg>
                                        </span>
                                    </span>
                                </div>
                            </h3>
                            <p class="mt-2 text-sm leading-normal">
                                A dynamic and engaging sports website design tailored for martial arts and MMA enthusiasts, featuring bold visuals, seamless navigation, and interactive elements to highlight events, fighters, and training programs.
                            </p>
                        </div>
                        <img alt="" loading="lazy" width="400" height="100"
                            decoding="async" data-nimg="1"
                            class="aspect-video object-top object-cover rounded border-2 border-slate-200/10 transition group-hover:border-slate-200/30 sm:order-1 sm:col-span-2 sm:translate-y-1"
                            style="color:transparent"
                            src="@/assets/portfolio/sports-site.jpg">
                    </div>
                </li>
                <li class="mb-12">
                    <div class="group relative grid gap-4 pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:hover:!opacity-100 lg:group-hover/list:opacity-50">
                        <div class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"></div>
                        <div class="z-10 sm:order-2 sm:col-span-6">
                            <h3>
                                <div @click="openModal('web3')" class="inline-flex hover:cursor-pointer items-baseline font-medium leading-tight text-slate-200 hover:text-teal-300 focus-visible:text-teal-300  group/link text-base">
                                    <span class="absolute -inset-x-4 -inset-y-2.5 hidden rounded md:-inset-x-6 md:-inset-y-4 lg:block"></span>
                                    <span>
                                        Modern Ecommerce Site
                                        <span class="inline-block">
                                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="inline-block h-4 w-4 shrink-0 transition-transform group-hover/link:-translate-y-1 group-hover/link:translate-x-1 group-focus-visible/link:-translate-y-1 group-focus-visible/link:translate-x-1 motion-reduce:transition-none ml-1 translate-y-px" aria-hidden="true">
                                                <path fill-rule="evenodd" d="M5.22 14.78a.75.75 0 001.06 0l7.22-7.22v5.69a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75h-7.5a.75.75 0 000 1.5h5.69l-7.22 7.22a.75.75 0 000 1.06z" clip-rule="evenodd"></path>
                                            </svg>
                                        </span>
                                    </span>
                                </div>
                            </h3>
                            <p class="mt-2 text-sm leading-normal">
                                A sleek and modern eCommerce website design, optimized for user experience with intuitive navigation, clean aesthetics, and seamless functionality to enhance online shopping and drive conversions.
                            </p>
                        </div>
                        <img alt="" loading="lazy" width="400" height="100"
                            decoding="async" data-nimg="1"
                            class="aspect-video object-top object-cover rounded border-2 border-slate-200/10 transition group-hover:border-slate-200/30 sm:order-1 sm:col-span-2 sm:translate-y-1"
                            style="color:transparent"
                            src="@/assets/portfolio/web3.png">
                    </div>
                </li>
            </ul>
            <div class="grid grid-cols-2 sm:grid-cols-3 gap-10">
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('logo1')">
                    <img src="@/assets/portfolio/logos/logo1.png" class="aspect-sqaure object-cover rounded-sm group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('logo2')">
                    <img src="@/assets/portfolio/logos/logo2.png" class="aspect-sqaure object-cover rounded-sm group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('logo3')">
                    <img src="@/assets/portfolio/logos/logo3.png" class="aspect-sqaure object-cover rounded-sm group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('logo4')">
                    <img src="@/assets/portfolio/logos/logo4.jpeg" class="aspect-sqaure object-cover rounded-sm group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('logo5')">
                    <img src="@/assets/portfolio/logos/logo5.jpeg" class="aspect-sqaure object-cover rounded-sm group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('logo6')">
                    <img src="@/assets/portfolio/logos/logo6.jpeg" class="aspect-sqaure object-cover rounded-sm group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('logo7')">
                    <img src="@/assets/portfolio/logos/logo7.jpeg" class="aspect-sqaure object-cover rounded-sm group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('logo8')">
                    <img src="@/assets/portfolio/logos/logo8.jpg" class="aspect-sqaure object-cover rounded-sm group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('logo9')">
                    <img src="@/assets/portfolio/logos/logo9.png" class="aspect-sqaure object-cover rounded-sm group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
            </div>
            <div class="space-y-5 mt-10">
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('banner1')">
                    <img src="@/assets/portfolio/banner1.png" class="group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
                <div class="group transition-all ease-in-out hover:cursor-pointer" @click="openModal('banner2')">
                    <img src="@/assets/portfolio/banner2.png" class="group-hover:border-2 group-hover:border-slate-200/30" alt="">
                </div>
            </div>
        </div>
    </section>

    <vs-modal ref="web1" size="l" backdropBlur removeHeader>
        <img src="@/assets/portfolio/photography-site.jpg" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="web2" size="l" backdropBlur removeHeader>
        <img src="@/assets/portfolio/sports-site.jpg" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="web3" size="l" backdropBlur removeHeader>
        <img src="@/assets/portfolio/web3.png" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>

    <vs-modal ref="logo1" backdropBlur removeHeader>
        <img src="@/assets/portfolio/logos/logo1.png" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="logo2" backdropBlur removeHeader>
        <img src="@/assets/portfolio/logos/logo2.png" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="logo3" backdropBlur removeHeader>
        <img src="@/assets/portfolio/logos/logo3.png" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="logo4" backdropBlur removeHeader>
        <img src="@/assets/portfolio/logos/logo4.jpeg" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="logo5" backdropBlur removeHeader>
        <img src="@/assets/portfolio/logos/logo5.jpeg" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="logo6" backdropBlur removeHeader>
        <img src="@/assets/portfolio/logos/logo6.jpeg" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="logo7" backdropBlur removeHeader>
        <img src="@/assets/portfolio/logos/logo7.jpeg" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="logo8" backdropBlur removeHeader>
        <img src="@/assets/portfolio/logos/logo8.jpg" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="logo9" backdropBlur removeHeader>
        <img src="@/assets/portfolio/logos/logo9.png" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="banner1" size="auto" backdropBlur removeHeader>
        <img src="@/assets/portfolio/banner1.png" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
    <vs-modal ref="banner2" size="auto" backdropBlur removeHeader>
        <img src="@/assets/portfolio/banner2.png" class="aspect-sqaure mt-6 mb-2" alt="">
    </vs-modal>
</template>

<script>
  import VsModal from '@vuesimple/vs-modal';

  export default {
    components: {
      VsModal,
    },

    methods: {
      openModal(ref) {
        this.$refs[ref].open();
      },

      closeModal(ref) {
        this.$refs[ref].close();
      },
    },
  };
</script>