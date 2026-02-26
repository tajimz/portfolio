<script setup lang="ts">
import { ref } from 'vue';
import { Head } from '@inertiajs/vue3';
import { Github, Linkedin, Cpu, Smartphone, Code, FacebookIcon, Menu, X } from 'lucide-vue-next';

const isMenuOpen = ref(false);
</script>

<template>
    <Head title="TR Tajim | Full Stack Developer" />

    <div class="min-h-screen overflow-x-hidden bg-slate-50 font-sans text-slate-900 selection:bg-indigo-500 selection:text-white">
        <div class="pointer-events-none fixed inset-0 z-0">
            <div
                class="absolute inset-0 [mask-image:radial-gradient(ellipse_at_center,black,transparent)] opacity-[0.03]"
                style="
                    background-image: url(&quot;data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M30 0L30 60M0 30L60 30' fill='none' stroke='%234f46e5' stroke-width='1'/%3E%3C/svg%3E&quot;);
                "
            ></div>
            <div class="absolute top-[-10%] left-[-10%] h-[50%] w-[50%] animate-pulse rounded-full bg-indigo-200/40 blur-[120px]"></div>
            <div class="absolute right-[-5%] bottom-[10%] h-[40%] w-[40%] rounded-full bg-violet-200/30 blur-[100px]"></div>
        </div>

        <nav class="sticky top-0 z-50 border-b border-slate-200/60 bg-white/70 backdrop-blur-md">
            <div class="mx-auto flex max-w-6xl items-center justify-between px-6 py-4">
                <span class="text-xl font-black tracking-tighter text-indigo-600">TR.TAJIM</span>

                <div class="hidden space-x-8 text-xs font-bold tracking-widest text-slate-600 uppercase md:flex">
                    <a href="#work" class="transition hover:text-indigo-600">Work</a>
                    <a href="#skills" class="transition hover:text-indigo-600">Skills</a>
                    <a href="#contact" class="transition hover:text-indigo-600">Contact</a>
                </div>

                <button @click="isMenuOpen = !isMenuOpen" class="p-2 text-slate-600 md:hidden">
                    <Menu v-if="!isMenuOpen" class="h-6 w-6" />
                    <X v-else class="h-6 w-6" />
                </button>
            </div>

            <div v-show="isMenuOpen" class="space-y-4 border-b border-slate-200 bg-white p-6 font-bold md:hidden">
                <a href="#work" @click="isMenuOpen = false" class="block">Work</a>
                <a href="#skills" @click="isMenuOpen = false" class="block">Skills</a>
                <a href="#contact" @click="isMenuOpen = false" class="block">Contact</a>
            </div>
        </nav>

        <header class="relative z-10 mx-auto grid max-w-6xl items-center gap-16 px-6 pt-12 pb-24 md:grid-cols-2 md:pt-32 md:pb-40">
            <div class="order-2 text-center md:order-1 md:text-left">
                <div
                    class="mb-6 inline-block rounded-full border border-indigo-100 bg-indigo-50 px-4 py-1.5 text-xs font-bold tracking-widest text-indigo-600 uppercase"
                >
                    Full Stack Developer
                </div>
                <h1 class="mb-8 text-5xl leading-[1.1] font-black tracking-tight md:text-7xl">
                    Building robust <br />
                    <span class="bg-gradient-to-r from-indigo-600 to-violet-500 bg-clip-text text-transparent"> Android, Web & IoT </span>
                    experiences.
                </h1>
                <p class="mx-auto mb-10 max-w-md text-lg leading-relaxed text-slate-600 md:mx-0">
                    I’m TR Tajim, specializing in Laravel, Vue.js, native Android, and Arduino based IoT devices. I turn complex problems into elegant
                    digital solutions.
                </p>
                <div class="flex flex-col justify-center gap-4 sm:flex-row md:justify-start">
                    <a
                        href="https://github.com/tajimz"
                        target="_blank"
                        class="rounded-2xl bg-indigo-600 px-8 py-4 text-center font-bold text-white shadow-lg shadow-indigo-200 transition-all hover:-translate-y-1 hover:shadow-indigo-300"
                        >View My Work</a
                    >
                    <a
                        href="https://www.linkedin.com/in/tajimz/"
                        target="_blank"
                        class="rounded-2xl border border-slate-200 bg-white px-8 py-4 text-center font-bold transition-all hover:bg-slate-50"
                        >Get in Touch</a
                    >
                </div>
            </div>

            <div class="order-1 flex justify-center md:order-2">
                <div class="relative h-64 w-64 md:h-[450px] md:w-[450px]">
                    <div
                        class="animate-spin-slow absolute -inset-4 rounded-[30%_70%_70%_30%/30%_30%_70%_70%] bg-gradient-to-tr from-indigo-200 to-violet-200 blur-2xl"
                    ></div>

                    <div
                        class="relative h-full w-full overflow-hidden rounded-[30%_70%_70%_30%/30%_30%_70%_70%] border-2 border-white bg-slate-200 shadow-2xl transition-all duration-700 hover:rounded-3xl"
                    >
                        <img
                            src="/images/me5.png"
                            alt="TR Tajim"
                            class="h-full w-full object-cover object-top transition-transform duration-700 hover:scale-105"
                        />
                    </div>

                    <div class="absolute -right-4 -bottom-4 hidden rounded-2xl bg-white p-4 shadow-xl md:block">
                        <div class="flex flex-wrap gap-2">
                            <span class="text-xs font-bold text-indigo-600">Laravel</span>
                            <span class="text-xs font-bold text-violet-600">Vue.js</span>
                            <span class="text-xs font-bold text-emerald-600">Android</span>
                            <span class="text-xs font-bold text-zinc-600">Arduino</span>
                        </div>
                    </div>
                </div>
            </div>
        </header>

        <section id="skills" class="relative z-10 border-y border-slate-200 bg-white/60 py-32 backdrop-blur-sm">
            <div class="mx-auto max-w-6xl px-6">
                <div class="grid gap-8 md:grid-cols-3">
                    <div
                        class="group rounded-3xl border border-slate-100 bg-white p-10 shadow-sm transition-all duration-300 hover:-translate-y-2 hover:shadow-xl"
                    >
                        <div
                            class="mb-8 flex h-14 w-14 items-center justify-center rounded-2xl bg-indigo-50 text-indigo-600 transition-all group-hover:scale-110 group-hover:bg-indigo-600 group-hover:text-white"
                        >
                            <Smartphone class="h-7 w-7" />
                        </div>
                        <h3 class="mb-4 text-xl font-bold">Android Dev</h3>
                        <p class="text-sm leading-relaxed text-slate-500">
                            High-performance mobile applications built with Java and modern architectural patterns.
                        </p>
                    </div>

                    <div
                        class="group rounded-3xl border border-slate-100 bg-white p-10 shadow-sm transition-all duration-300 hover:-translate-y-2 hover:shadow-xl"
                    >
                        <div
                            class="mb-8 flex h-14 w-14 items-center justify-center rounded-2xl bg-emerald-50 text-emerald-600 transition-all group-hover:scale-110 group-hover:bg-emerald-600 group-hover:text-white"
                        >
                            <Code class="h-7 w-7" />
                        </div>
                        <h3 class="mb-4 text-xl font-bold">Laravel & Vue</h3>
                        <p class="text-sm leading-relaxed text-slate-500">
                            Seamless SPA development using the TALL stack or Inertia.js for modern, reactive web apps.
                        </p>
                    </div>

                    <div
                        class="group rounded-3xl border border-slate-100 bg-white p-10 shadow-sm transition-all duration-300 hover:-translate-y-2 hover:shadow-xl"
                    >
                        <div
                            class="mb-8 flex h-14 w-14 items-center justify-center rounded-2xl bg-violet-50 text-violet-600 transition-all group-hover:scale-110 group-hover:bg-violet-600 group-hover:text-white"
                        >
                            <Cpu class="h-7 w-7" />
                        </div>
                        <h3 class="mb-4 text-xl font-bold">IoT Devices</h3>
                        <p class="text-sm leading-relaxed text-slate-500">Arduino-based IoT devices connecting hardware and software seamlessly.</p>
                    </div>
                </div>
            </div>
        </section>

        <footer id="contact" class="relative z-10 px-6 py-32 text-center">
            <div class="mx-auto max-w-4xl">
                <h2 class="mb-8 text-4xl font-black tracking-tight md:text-5xl">
                    Let's build something <br />
                    amazing together.
                </h2>
                <a
                    href="mailto:hello@tajimz.xyz"
                    class="mb-16 inline-block border-b-4 border-indigo-100 pb-2 text-2xl font-black text-indigo-600 transition-colors hover:border-indigo-600 hover:text-indigo-700 md:text-4xl"
                >
                    hello@tajimz.xyz
                </a>

                <div class="flex flex-col items-center justify-between gap-6 border-t border-slate-200 pt-12 md:flex-row">
                    <p class="font-medium text-slate-500">© 2026 TR Tajim. Built with Passion.</p>
                    <div class="flex gap-8">
                        <a href="https://github.com/tajimz" target="_blank" class="text-slate-400 transition-colors hover:text-indigo-600"
                            ><Github class="h-6 w-6"
                        /></a>
                        <a href="https://www.linkedin.com/in/tajimz/" target="_blank" class="text-slate-400 transition-colors hover:text-indigo-600"
                            ><Linkedin class="h-6 w-6"
                        /></a>
                        <a href="https://facebook.com/trtajim" target="_blank" class="text-slate-400 transition-colors hover:text-indigo-600"
                            ><FacebookIcon class="h-6 w-6"
                        /></a>
                    </div>
                </div>
            </div>
        </footer>
    </div>
</template>

<style>
html {
    scroll-behavior: smooth;
}

@keyframes spin-slow {
    from {
        transform: rotate(0deg);
    }
    to {
        transform: rotate(360deg);
    }
}

.animate-spin-slow {
    animation: spin-slow 12s linear infinite;
}

::selection {
    background-color: #4f46e5;
    color: white;
}
</style>
