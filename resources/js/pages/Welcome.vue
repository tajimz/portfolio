<script setup lang="ts">
import { ref } from 'vue';
import { Head } from '@inertiajs/vue3';
import { Github, Linkedin, Globe, Smartphone, Code, Mail, Menu, X } from 'lucide-vue-next';

const isMenuOpen = ref(false);
</script>

<template>
    <Head title="TR Tajim | Full Stack Developer" />

    <div class="min-h-screen bg-slate-50 text-slate-900 font-sans selection:bg-indigo-500 selection:text-white overflow-x-hidden">
        
        <div class="fixed inset-0 z-0 pointer-events-none">
            <div class="absolute inset-0 opacity-[0.03] [mask-image:radial-gradient(ellipse_at_center,black,transparent)]" 
                 style="background-image: url('data:image/svg+xml,%3Csvg width=\'60\' height=\'60\' viewBox=\'0 0 60 60\' xmlns=\'http://www.w3.org/2000/svg\'%3E%3Cpath d=\'M30 0L30 60M0 30L60 30\' fill=\'none\' stroke=\'%234f46e5\' stroke-width=\'1\'/%3E%3C/svg%3E');">
            </div>
            
            <div class="absolute top-[-10%] left-[-10%] w-[50%] h-[50%] rounded-full bg-indigo-200/40 blur-[120px] animate-pulse"></div>
            <div class="absolute bottom-[10%] right-[-5%] w-[40%] h-[40%] rounded-full bg-violet-200/30 blur-[100px]"></div>
        </div>

        <nav class="sticky top-0 z-50 bg-white/70 backdrop-blur-md border-b border-slate-200/60">
            <div class="max-w-6xl mx-auto px-6 py-4 flex justify-between items-center">
                <span class="text-xl font-black tracking-tighter text-indigo-600">TR.TAJIM</span>
                
                <div class="hidden md:flex space-x-8 font-bold text-xs uppercase tracking-widest text-slate-600">
                    <a href="#work" class="hover:text-indigo-600 transition">Work</a>
                    <a href="#skills" class="hover:text-indigo-600 transition">Skills</a>
                    <a href="#contact" class="hover:text-indigo-600 transition">Contact</a>
                </div>

                <button @click="isMenuOpen = !isMenuOpen" class="md:hidden p-2 text-slate-600">
                    <Menu v-if="!isMenuOpen" class="w-6 h-6" />
                    <X v-else class="w-6 h-6" />
                </button>
            </div>

            <div v-show="isMenuOpen" class="md:hidden bg-white border-b border-slate-200 p-6 space-y-4 font-bold">
                <a href="#work" @click="isMenuOpen = false" class="block">Work</a>
                <a href="#skills" @click="isMenuOpen = false" class="block">Skills</a>
                <a href="#contact" @click="isMenuOpen = false" class="block">Contact</a>
            </div>
        </nav>

        <header class="relative z-10 max-w-6xl mx-auto px-6 pt-16 pb-24 md:pt-32 md:pb-40 grid md:grid-cols-2 gap-16 items-center">
            <div class="text-center md:text-left">
                <div class="inline-block px-4 py-1.5 mb-6 text-xs font-bold tracking-widest text-indigo-600 uppercase bg-indigo-50 rounded-full border border-indigo-100">
                    Full Stack Developer
                </div>
                <h1 class="text-5xl md:text-7xl font-black leading-[1.1] mb-8 tracking-tight">
                    Building robust <br/>
                    <span class="text-transparent bg-clip-text bg-gradient-to-r from-indigo-600 to-violet-500">
                        Android & Web
                    </span> experiences.
                </h1>
                <p class="text-lg text-slate-600 mb-10 max-w-md mx-auto md:mx-0 leading-relaxed">
                    I'm TR Tajim, specializing in Laravel, Vue.js, and native Android. I turn complex problems into elegant digital solutions.
                </p>
                <div class="flex flex-col sm:flex-row gap-4 justify-center md:justify-start">
                    <a href="https://github.com/tajimz" target="_blank" class="px-8 py-4 bg-indigo-600 text-white font-bold rounded-2xl shadow-lg shadow-indigo-200 hover:shadow-indigo-300 hover:-translate-y-1 transition-all text-center">View My Work</a>
                    <a href="https://www.linkedin.com/in/tajimz/" target="_blank" class="px-8 py-4 bg-white border border-slate-200 font-bold rounded-2xl hover:bg-slate-50 transition-all text-center">Get in Touch</a>
                </div>
            </div>

            <div class="relative group">
                <div class="absolute -inset-4 bg-gradient-to-r from-indigo-500 to-violet-600 rounded-3xl blur-2xl opacity-20 group-hover:opacity-40 transition duration-1000"></div>
                <div class="relative bg-slate-900 rounded-3xl overflow-hidden shadow-2xl p-8 font-mono text-sm border border-slate-800">
                    <div class="flex gap-2 mb-8">
                        <div class="w-3 h-3 rounded-full bg-red-500"></div>
                        <div class="w-3 h-3 rounded-full bg-amber-500"></div>
                        <div class="w-3 h-3 rounded-full bg-emerald-500"></div>
                    </div>
                    <div class="space-y-4">
                        <p class="text-emerald-400">$ <span class="text-slate-100">fetch skills --profile=tr_tajim</span></p>
                        <div class="grid grid-cols-2 gap-3 text-indigo-300">
                            <span class="flex items-center gap-2 font-semibold"><span class="text-slate-600">01</span> Laravel</span>
                            <span class="flex items-center gap-2 font-semibold"><span class="text-slate-600">02</span> Vue.js</span>
                            <span class="flex items-center gap-2 font-semibold"><span class="text-slate-600">03</span> Java</span>
                            <span class="flex items-center gap-2 font-semibold"><span class="text-slate-600">04</span> Inertia.js</span>
                            <span class="flex items-center gap-2 font-semibold"><span class="text-slate-600">05</span> Tailwind</span>
                            <span class="flex items-center gap-2 font-semibold"><span class="text-slate-600">06</span> MySQL</span>
                        </div>
                        <p class="text-slate-500 mt-6 animate-pulse">_</p>
                        <div class="absolute bottom-8 right-8 opacity-10 group-hover:opacity-30 transition-opacity">
                            <Code class="w-24 h-24 text-white" />
                        </div>
                    </div>
                </div>
            </div>
        </header>

        <section id="skills" class="relative z-10 py-32 bg-white/60 backdrop-blur-sm border-y border-slate-200">
            <div class="max-w-6xl mx-auto px-6">
                <div class="grid md:grid-cols-3 gap-8">
                    <div class="group p-10 rounded-3xl bg-white border border-slate-100 shadow-sm hover:shadow-xl hover:-translate-y-2 transition-all duration-300">
                        <div class="w-14 h-14 bg-indigo-50 text-indigo-600 rounded-2xl flex items-center justify-center mb-8 group-hover:scale-110 group-hover:bg-indigo-600 group-hover:text-white transition-all">
                            <Smartphone class="w-7 h-7" />
                        </div>
                        <h3 class="text-xl font-bold mb-4">Android Dev</h3>
                        <p class="text-slate-500 text-sm leading-relaxed">High-performance mobile applications built with Kotlin and modern architectural patterns.</p>
                    </div>

                    <div class="group p-10 rounded-3xl bg-white border border-slate-100 shadow-sm hover:shadow-xl hover:-translate-y-2 transition-all duration-300">
                        <div class="w-14 h-14 bg-emerald-50 text-emerald-600 rounded-2xl flex items-center justify-center mb-8 group-hover:scale-110 group-hover:bg-emerald-600 group-hover:text-white transition-all">
                            <Code class="w-7 h-7" />
                        </div>
                        <h3 class="text-xl font-bold mb-4">Laravel & Vue</h3>
                        <p class="text-slate-500 text-sm leading-relaxed">Seamless SPA development using the TALL stack or Inertia.js for modern, reactive web apps.</p>
                    </div>

                    <div class="group p-10 rounded-3xl bg-white border border-slate-100 shadow-sm hover:shadow-xl hover:-translate-y-2 transition-all duration-300">
                        <div class="w-14 h-14 bg-violet-50 text-violet-600 rounded-2xl flex items-center justify-center mb-8 group-hover:scale-110 group-hover:bg-violet-600 group-hover:text-white transition-all">
                            <Globe class="w-7 h-7" />
                        </div>
                        <h3 class="text-xl font-bold mb-4">API Design</h3>
                        <p class="text-slate-500 text-sm leading-relaxed">Scalable RESTful and GraphQL APIs designed for speed, security, and integration.</p>
                    </div>
                </div>
            </div>
        </section>

        <footer id="contact" class="relative z-10 py-32 text-center px-6">
            <div class="max-w-4xl mx-auto">
                <h2 class="text-4xl md:text-5xl font-black mb-8 tracking-tight">Let's build something <br/> amazing together.</h2>
                <a href="mailto:hello@tajimz.xyz" class="inline-block text-2xl md:text-4xl font-black text-indigo-600 hover:text-indigo-700 transition-colors border-b-4 border-indigo-100 hover:border-indigo-600 pb-2 mb-16">
                    hello@tajimz.xyz
                </a>
                
                <div class="pt-12 border-t border-slate-200 flex flex-col md:flex-row justify-between items-center gap-6">
                    <p class="text-slate-500 font-medium">© 2026 TR Tajim. Built with Passion.</p>
                    <div class="flex gap-8">
                        <a href="https://github.com/tajimz" target="_blank" class="text-slate-400 hover:text-indigo-600 transition-colors"><Github class="w-6 h-6" /></a>
                        <a href="https://www.linkedin.com/in/tajimz/" target="_blank" class="text-slate-400 hover:text-indigo-600 transition-colors"><Linkedin class="w-6 h-6" /></a>
                        <a href="mailto:hello@tajimz.xyz" target="_blank" class="text-slate-400 hover:text-indigo-600 transition-colors"><Mail class="w-6 h-6" /></a>
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
/* Custom selection color */
::selection {
    background-color: #4f46e5;
    color: white;
}
</style>