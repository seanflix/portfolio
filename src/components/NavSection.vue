<template>
    <header class="lg:sticky lg:top-0 lg:flex lg:max-h-screen lg:w-[48%] lg:flex-col lg:justify-between lg:py-24">
        <div>
            <h1 class="text-4xl font-bold tracking-tight text-slate-200 sm:text-5xl">
                <a href="/">
                    John Sean Blanco
                </a>
            </h1>
            <h2 class="mt-3 text-lg font-medium tracking-tight text-slate-200 sm:text-xl inline-flex h-5" id="autotype"></h2>
            <p class="mt-4 max-w-xs leading-normal">
                Crafting seamless, visually engaging digital solutions across web and multimedia platforms.
            </p>
            <nav class="nav hidden lg:block" aria-label="In-page jump links">
                <ul class="mt-16 w-max">
                    <li>
                        <a class="group flex items-center py-3 active" href="#about">
                            <span class="nav-indicator mr-4 h-px w-8 bg-slate-600 transition-all group-hover:w-16 group-hover:bg-slate-200 group-focus-visible:w-16 group-focus-visible:bg-slate-200 motion-reduce:transition-none"></span>
                            <span class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200">About</span>
                        </a>
                    </li>
                    <li>
                        <a class="group flex items-center py-3" href="#experience">
                            <span class="nav-indicator mr-4 h-px w-8 bg-slate-600 transition-all group-hover:w-16 group-hover:bg-slate-200 group-focus-visible:w-16 group-focus-visible:bg-slate-200 motion-reduce:transition-none"></span>
                            <span class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200">Experience</span>
                        </a>
                    </li>
                    <li>
                        <a class="group flex items-center py-3" href="#projects">
                            <span class="nav-indicator mr-4 h-px w-8 bg-slate-600 transition-all group-hover:w-16 group-hover:bg-slate-200 group-focus-visible:w-16 group-focus-visible:bg-slate-200 motion-reduce:transition-none"></span>
                            <span class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200">Projects</span>
                        </a>
                    </li>
                    <li>
                        <a class="group flex items-center py-3" href="#designs">
                            <span class="nav-indicator mr-4 h-px w-8 bg-slate-600 transition-all group-hover:w-16 group-hover:bg-slate-200 group-focus-visible:w-16 group-focus-visible:bg-slate-200 motion-reduce:transition-none"></span>
                            <span class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200">Designs</span>
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
        <ul class="ml-1 mt-8 flex items-center" aria-label="Social media">
            <li class="mr-5 shrink-0 text-xs">
                <a class="block hover:text-slate-200" href="https://github.com/seanflix" target="_blank" rel="noreferrer noopener" title="GitHub">
                    <span class="sr-only">GitHub</span>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor" class="h-6 w-6" aria-hidden="true"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
                </a>
            </li>
            <li class="mr-5 shrink-0 text-xs">
                <a class="block hover:text-slate-200" href="mailto:dev.seanflix@gmail.com" rel="noreferrer noopener" title="Gmail">
                    <span class="sr-only">Gmail</span><svg class="h-6 w-6 fill-slate-400 hover:fill-slate-200" viewBox="0 0 24 24" role="img" xmlns="http://www.w3.org/2000/svg"><path d="M24 5.457v13.909c0 .904-.732 1.636-1.636 1.636h-3.819V11.73L12 16.64l-6.545-4.91v9.273H1.636A1.636 1.636 0 0 1 0 19.366V5.457c0-2.023 2.309-3.178 3.927-1.964L5.455 4.64 12 9.548l6.545-4.91 1.528-1.145C21.69 2.28 24 3.434 24 5.457z"/></svg>
                </a>
            </li>
            <li class="mr-5 shrink-0 text-xs">
                <a class="block hover:text-slate-200" href="https://wa.me/639610285561" target="_blank" rel="noreferrer noopener" title="Whatsapp">
                    <span class="sr-only">Whatsapp</span><svg fill="#000000" class="h-6 w-6 fill-slate-400 hover:fill-slate-200" viewBox="-2 -2 24 24" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMinYMin"><path d='M9.516.012C4.206.262.017 4.652.033 9.929a9.798 9.798 0 0 0 1.085 4.465L.06 19.495a.387.387 0 0 0 .47.453l5.034-1.184a9.981 9.981 0 0 0 4.284 1.032c5.427.083 9.951-4.195 10.12-9.58C20.15 4.441 15.351-.265 9.516.011zm6.007 15.367a7.784 7.784 0 0 1-5.52 2.27 7.77 7.77 0 0 1-3.474-.808l-.701-.347-3.087.726.65-3.131-.346-.672A7.62 7.62 0 0 1 2.197 9.9c0-2.07.812-4.017 2.286-5.48a7.85 7.85 0 0 1 5.52-2.271c2.086 0 4.046.806 5.52 2.27a7.672 7.672 0 0 1 2.287 5.48c0 2.052-.825 4.03-2.287 5.481z'/><path d='M14.842 12.045l-1.931-.55a.723.723 0 0 0-.713.186l-.472.478a.707.707 0 0 1-.765.16c-.913-.367-2.835-2.063-3.326-2.912a.694.694 0 0 1 .056-.774l.412-.53a.71.71 0 0 0 .089-.726L7.38 5.553a.723.723 0 0 0-1.125-.256c-.539.453-1.179 1.14-1.256 1.903-.137 1.343.443 3.036 2.637 5.07 2.535 2.349 4.566 2.66 5.887 2.341.75-.18 1.35-.903 1.727-1.494a.713.713 0 0 0-.408-1.072z'/></svg>
                </a>
            </li>
        </ul>
    </header>
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