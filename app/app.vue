<template>
  <div class="min-h-screen bg-[#09090d] text-zinc-200 p-4 md:p-8 lg:p-12 font-sans selection:bg-purple-500 selection:text-white relative overflow-hidden flex flex-col justify-between">
    
    <!-- ================= 1. BACKGROUND TEXTURES & GLOW ================= -->
    <!-- Tech Grid Lines -->
    <div 
      class="absolute inset-0 pointer-events-none opacity-[0.07]"
      style="background-image: linear-gradient(to right, #ffffff 1px, transparent 1px), linear-gradient(to bottom, #ffffff 1px, transparent 1px); background-size: 48px 48px; mask-image: radial-gradient(ellipse 70% 60% at 50% 40%, #000 70%, transparent 100%);"
    ></div>

    <!-- Aurora Glow Atas Tengah -->
    <div class="absolute -top-40 left-1/2 -translate-x-1/2 w-[800px] h-[450px] bg-gradient-to-b from-purple-600/30 to-indigo-600/10 blur-[140px] pointer-events-none rounded-full"></div>
    
    <!-- Aurora Glow Samping Kanan -->
    <div class="absolute top-1/3 -right-36 w-[500px] h-[500px] bg-blue-600/10 blur-[150px] pointer-events-none rounded-full"></div>

    <!-- ================= 2. FLOATING HEADER (STATUS BAR) ================= -->
    <header class="max-w-7xl mx-auto w-full mb-8 relative z-20 flex items-center justify-between">
      <div class="flex items-center gap-2.5">
        <img src="/images/avatar.png" alt="Avatar" class="w-7 h-7 rounded-full object-cover border border-purple-500/40" />
        <span class="text-xs font-semibold text-zinc-200">Matthew Natanael</span>
      </div>

      <div class="hidden sm:flex items-center gap-3 px-4 py-1.5 rounded-full bg-[#141418]/80 border border-zinc-800/80 backdrop-blur-md text-xs shadow-sm">
        <span class="w-2 h-2 rounded-full bg-emerald-400 animate-ping"></span>
        <span class="text-zinc-300 font-medium">Ready for Semester 5 Enrichment</span>
        <span class="text-zinc-600">•</span>
        <span class="text-zinc-400 font-mono text-[11px]">Nuxt 3 + Tailwind</span>
      </div>
    </header>

    <!-- ================= 3. BENTO GRID UTAMA ================= -->
    <main class="max-w-7xl mx-auto w-full grid grid-cols-1 lg:grid-cols-12 gap-5 relative z-10 flex-1">
      
      <!-- ================= KOLOM KIRI (3 SPAN) ================= -->
      <div class="lg:col-span-3 flex flex-col gap-5 order-2 lg:order-1">
        
        <!-- Skills & Tools -->
        <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-3xl p-5 hover:border-purple-500/40 transition-colors">
          <div class="flex items-center gap-2 mb-4 text-xs font-semibold uppercase tracking-wider text-zinc-400">
            <svg class="w-4 h-4 text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
            </svg>
            <span>Skills & Tools</span>
          </div>
          
          <div class="grid grid-cols-2 gap-2.5">
            <!-- Node.js -->
            <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-xl p-2.5 flex items-center gap-2.5 hover:border-zinc-700 transition-colors">
              <div class="w-6 h-6 rounded-lg bg-emerald-500/10 border border-emerald-500/20 flex items-center justify-center shrink-0">
                <svg class="w-3.5 h-3.5 text-emerald-400 fill-current" viewBox="0 0 24 24">
                  <path d="M12 2l9 5.2v10.4L12 23l-9-5.2V7.2L12 2zm0 2.31L5 8.35v7.3L12 19.69l7-4.04V8.35L12 4.31z" />
                </svg>
              </div>
              <span class="text-xs font-medium text-zinc-300">Node.js</span>
            </div>

            <!-- Nuxt.js -->
            <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-xl p-2.5 flex items-center gap-2.5 hover:border-zinc-700 transition-colors">
              <div class="w-6 h-6 rounded-lg bg-emerald-500/10 border border-emerald-500/20 flex items-center justify-center shrink-0">
                <svg class="w-3.5 h-3.5 text-emerald-400 fill-current" viewBox="0 0 24 24">
                  <path d="M10.93 4.25a2 2 0 0 0-3.46 0L.37 16.5a2 2 0 0 0 1.73 3h7.24a2 2 0 0 0 1.73-1l4.04-7.05-4.18-7.2zm4.4 7.67-2.3 4.02a1 1 0 0 0 .86 1.5h8.24a1 1 0 0 0 .87-1.5l-6.52-11.4a1 1 0 0 0-1.74 0l-1.2 2.1 1.79 5.28z" />
                </svg>
              </div>
              <span class="text-xs font-medium text-zinc-300">Nuxt.js</span>
            </div>

            <!-- Laravel -->
            <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-xl p-2.5 flex items-center gap-2.5 hover:border-zinc-700 transition-colors">
              <div class="w-6 h-6 rounded-lg bg-red-500/10 border border-red-500/20 flex items-center justify-center shrink-0">
                <svg class="w-3.5 h-3.5 text-red-500 fill-current" viewBox="0 0 24 24">
                  <path d="M11.75 2.17a.5.5 0 0 0-.5 0L3.6 6.58a.5.5 0 0 0-.25.43v8.83a.5.5 0 0 0 .25.44l7.65 4.41a.5.5 0 0 0 .5 0l7.65-4.41a.5.5 0 0 0 .25-.44V7.01a.5.5 0 0 0-.25-.43L11.75 2.17zm-.25 1.58 6.4 3.7-6.4 3.7-6.4-3.7 6.4-3.7zM4.85 8.1l6.15 3.55v7.2L4.85 15.3V8.1zm14.3 0v7.2l-6.15 3.55v-7.2l6.15-3.55z" />
                </svg>
              </div>
              <span class="text-xs font-medium text-zinc-300">Laravel</span>
            </div>

            <!-- Python -->
            <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-xl p-2.5 flex items-center gap-2.5 hover:border-zinc-700 transition-colors">
              <div class="w-6 h-6 rounded-lg bg-yellow-500/10 border border-yellow-500/20 flex items-center justify-center shrink-0">
                <svg class="w-3.5 h-3.5" viewBox="0 0 24 24">
                  <path fill="#38bdf8" d="M11.9 2c-5.2 0-4.9 2.2-4.9 2.2l.01 2.3h5V7.2H5.1S2 6.8 2 12c0 5.1 2.7 4.9 2.7 4.9h1.6v-2.3c0-2.6 2.3-2.6 2.3-2.6h5c2.3 0 2.3-2.2 2.3-2.2V4.2S16.3 2 11.9 2zm-1.4 1.4c.5 0 .9.4.9.9s-.4.9-.9.9-.9-.4-.9-.9.4-.9.9-.9z" />
                  <path fill="#facc15" d="M12.1 22c5.2 0 4.9-2.2 4.9-2.2l-.01-2.3h-5v-.7h6.9s3.1.4 3.1-4.8c0-5.1-2.7-4.9-2.7-4.9h-1.6v2.3c0 2.6-2.3 2.6-2.3 2.6h-5c-2.3 0-2.3 2.2-2.3 2.2v7.6s-.4 2.2 4 2.2zm1.4-1.4c-.5 0-.9-.4-.9-.9s.4-.9.9-.9.9.4.9.9-.4.9-.9.9z" />
                </svg>
              </div>
              <span class="text-xs font-medium text-zinc-300">Python</span>
            </div>

            <!-- Git -->
            <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-xl p-2.5 flex items-center gap-2.5 hover:border-zinc-700 transition-colors">
              <div class="w-6 h-6 rounded-lg bg-orange-500/10 border border-orange-500/20 flex items-center justify-center shrink-0">
                <svg class="w-3.5 h-3.5 text-orange-500 fill-current" viewBox="0 0 24 24">
                  <path d="M21.62 10.95L13.06 2.4a1.5 1.5 0 0 0-2.12 0L8.8 4.54l2.69 2.69a1.76 1.76 0 0 1 2.23 2.24l2.58 2.59a1.75 1.75 0 1 1-1.07 1.04l-2.4-2.4v5.33a1.75 1.75 0 1 1-1.5 0V10.4a1.77 1.77 0 0 1-.95-.97L7.69 6.74 2.38 12.05a1.5 1.5 0 0 0 0 2.12l8.56 8.55a1.5 1.5 0 0 0 2.12 0l8.56-8.55a1.5 1.5 0 0 0 0-2.12z" />
                </svg>
              </div>
              <span class="text-xs font-medium text-zinc-300">Git</span>
            </div>

            <!-- Tailwind CSS -->
            <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-xl p-2.5 flex items-center gap-2.5 hover:border-zinc-700 transition-colors">
              <div class="w-6 h-6 rounded-lg bg-sky-500/10 border border-sky-500/20 flex items-center justify-center shrink-0">
                <svg class="w-3.5 h-3.5 text-sky-400 fill-current" viewBox="0 0 24 24">
                  <path d="M12.001 4.8c-3.2 0-5.2 1.6-6 4.8 1.2-1.6 2.6-2.2 4.2-1.8.913.228 1.565.89 2.288 1.624C13.666 10.618 15.027 12 18.001 12c3.2 0 5.2-1.6 6-4.8-1.2 1.6-2.6 2.2-4.2 1.8-.913-.228-1.565-.89-2.288-1.624C16.337 6.182 14.976 4.8 12.001 4.8zm-6 7.2c-3.2 0-5.2 1.6-6 4.8 1.2-1.6 2.6-2.2 4.2-1.8.913.228 1.565.89 2.288 1.624 1.177 1.194 2.538 2.576 5.512 2.576 3.2 0 5.2-1.6 6-4.8-1.2 1.6-2.6 2.2-4.2 1.8-.913-.228-1.565-.89-2.288-1.624C10.337 13.382 8.976 12 6.001 12z" />
                </svg>
              </div>
              <span class="text-xs font-medium text-zinc-300">Tailwind</span>
            </div>
          </div>
        </div>

        <!-- Education & Coursework -->
        <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-3xl p-5 hover:border-purple-500/40 transition-colors flex-1 flex flex-col justify-between">
          <div>
            <div class="flex items-center gap-2 mb-3 text-xs font-semibold uppercase tracking-wider text-zinc-400">
              <svg class="w-4 h-4 text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M12 14l9-5-9-5-9 5 9 5z" />
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z" />
              </svg>
              <span>Education</span>
            </div>
            <h3 class="text-base font-bold text-white">BINUS University</h3>
            <p class="text-xs text-purple-400 font-medium mt-0.5">Computer Science</p>
            <p class="text-xs text-zinc-500 mt-0.5">Semester 5 • Ready for Enrichment</p>

            <div class="mt-5">
              <p class="text-[11px] font-semibold uppercase tracking-wider text-zinc-400 mb-2">Relevant Coursework</p>
              <ul class="space-y-1.5 text-xs text-zinc-300">
                <li class="flex items-center gap-2">
                  <span class="text-purple-400 font-mono text-[10px]">#</span>
                  <span>Data Structures & Algorithms</span>
                </li>
                <li class="flex items-center gap-2">
                  <span class="text-purple-400 font-mono text-[10px]">#</span>
                  <span>Object-Oriented Programming</span>
                </li>
                <li class="flex items-center gap-2">
                  <span class="text-purple-400 font-mono text-[10px]">#</span>
                  <span>Database Technology</span>
                </li>
                <li class="flex items-center gap-2">
                  <span class="text-purple-400 font-mono text-[10px]">#</span>
                  <span>Web Based Programming</span>
                </li>
                <li class="flex items-center gap-2">
                  <span class="text-purple-400 font-mono text-[10px]">#</span>
                  <span>Mobile Programming</span>
                </li>
                <li class="flex items-center gap-2">
                  <span class="text-purple-400 font-mono text-[10px]">#</span>
                  <span>Cloud Services & Computing</span>
                </li>
                <li class="flex items-center gap-2">
                  <span class="text-purple-400 font-mono text-[10px]">#</span>
                  <span>Artificial Intelligence</span>
                </li>
              </ul>
            </div>
          </div>
        </div>

        <!-- Online Presence -->
        <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-3xl p-5 hover:border-purple-500/40 transition-colors">
          <div class="flex items-center gap-2 mb-3 text-xs font-semibold uppercase tracking-wider text-zinc-400">
            <svg class="w-4 h-4 text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9" />
            </svg>
            <span>Online Presence</span>
          </div>
          <div class="flex flex-col gap-2">
            <a href="https://github.com/mattnael" target="_blank" class="bg-[#1a1a21]/90 hover:bg-zinc-800 border border-zinc-800/80 px-3.5 py-2 rounded-xl flex items-center justify-between text-xs text-zinc-300 transition-colors">
              <span class="font-medium">GitHub</span>
              <span class="text-zinc-500 text-[11px]">mattnael ↗</span>
            </a>
            <a href="https://linkedin.com/in/matthew-natanael" target="_blank" class="bg-[#1a1a21]/90 hover:bg-zinc-800 border border-zinc-800/80 px-3.5 py-2 rounded-xl flex items-center justify-between text-xs text-zinc-300 transition-colors">
              <span class="font-medium">LinkedIn</span>
              <span class="text-zinc-500 text-[11px]">matthew-natanael ↗</span>
            </a>
            <a href="https://instagram.com/matt_nael" target="_blank" class="bg-[#1a1a21]/90 hover:bg-zinc-800 border border-zinc-800/80 px-3.5 py-2 rounded-xl flex items-center justify-between text-xs text-zinc-300 transition-colors">
              <span class="font-medium">Instagram</span>
              <span class="text-zinc-500 text-[11px]">@matt_nael ↗</span>
            </a>
          </div>
        </div>

      </div>

      <!-- ================= KOLOM TENGAH (5 SPAN) ================= -->
      <div class="lg:col-span-5 flex flex-col gap-5 order-1 lg:order-2">
        
        <!-- Metrics -->
        <div class="grid grid-cols-3 gap-3">
          <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-2xl p-4 text-center">
            <div class="text-2xl font-extrabold text-white">05+</div>
            <div class="text-[11px] text-zinc-400 mt-1">Projects Built</div>
          </div>
          <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-2xl p-4 text-center">
            <div class="text-2xl font-extrabold text-white">02</div>
            <div class="text-[11px] text-zinc-400 mt-1">Roles at BNCC</div>
          </div>
          <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-2xl p-4 text-center">
            <div class="text-2xl font-extrabold text-purple-400">Sem 5</div>
            <div class="text-[11px] text-zinc-400 mt-1">Enrichment Ready</div>
          </div>
        </div>

        <!-- Profile Card -->
        <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-3xl p-6 hover:border-purple-500/40 transition-colors">
          <div class="flex items-start gap-4">
            <img 
              src="/images/avatar.png" 
              alt="Matthew Natanael" 
              class="w-20 h-20 rounded-2xl object-cover border border-purple-500/30 shrink-0 bg-zinc-800 shadow-md shadow-black/50"
            />
            <div class="flex-1">
              <div class="inline-flex items-center gap-1.5 px-2.5 py-0.5 rounded-full text-[11px] font-medium bg-emerald-500/10 text-emerald-400 border border-emerald-500/20 mb-2">
                <span class="w-1.5 h-1.5 rounded-full bg-emerald-400 animate-pulse"></span>
                <span>Open for Internship</span>
              </div>
              <h1 class="text-xl font-bold text-white">Matthew Natanael</h1>
              <p class="text-xs text-zinc-400 mt-0.5">Computer Science Undergraduate</p>
              <p class="text-xs text-zinc-500">BINUS University</p>
            </div>
          </div>
          <div class="mt-5">
            <a 
              href="/resume.pdf" 
              download 
              class="w-full inline-flex items-center justify-center gap-2 py-2.5 rounded-xl text-xs font-semibold bg-gradient-to-r from-purple-600 to-indigo-600 hover:from-purple-500 hover:to-indigo-500 text-white shadow-lg shadow-purple-600/25 transition-all"
            >
              <span>Download CV</span>
              <svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3" />
              </svg>
            </a>
          </div>
        </div>

        <!-- Featured Projects Showcase -->
        <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-3xl p-6 hover:border-purple-500/40 transition-colors flex-1 flex flex-col justify-between">
          <div>
            <div class="flex items-center justify-between mb-4">
              <div class="flex items-center gap-2 text-xs font-semibold uppercase tracking-wider text-zinc-400">
                <svg class="w-4 h-4 text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M8 9l3 3-3 3m5 0h3M5 20h14a2 2 0 002-2V6a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                </svg>
                <span>Featured Projects</span>
              </div>
              <span class="text-[11px] text-purple-400 font-mono">Real-world & Automation</span>
            </div>

            <!-- List Proyek -->
            <div class="space-y-3">
              <!-- Proyek 1 -->
              <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-2xl p-3.5 hover:border-zinc-700 transition-colors">
                <div class="flex items-start justify-between gap-2">
                  <div>
                    <h3 class="text-xs font-bold text-white">Dragon Nest Raid Salary Bot</h3>
                    <p class="text-[11px] text-zinc-400 mt-1 leading-relaxed">
                      Bot Discord untuk kalkulasi dan pembagian gaji/loot tim raid Dragon Nest secara otomatis, transparan, dan terstruktur.
                    </p>
                  </div>
                  <a href="https://github.com/mattnael/discord-raid-salary-bot" target="_blank" class="text-zinc-400 hover:text-purple-400 text-xs shrink-0 px-2.5 py-1 bg-zinc-800/80 hover:bg-zinc-800 rounded-lg border border-zinc-700/60 transition-colors flex items-center gap-1">
                    <span>Repo</span>
                    <span>↗</span>
                  </a>
                </div>
                <div class="flex flex-wrap gap-1.5 mt-2.5">
                  <span class="text-[10px] bg-[#22222b] text-purple-300 border border-purple-500/20 px-2 py-0.5 rounded-md">Discord API</span>
                  <span class="text-[10px] bg-[#22222b] text-emerald-300 border border-emerald-500/20 px-2 py-0.5 rounded-md">Automation</span>
                  <span class="text-[10px] bg-[#22222b] text-zinc-300 border border-zinc-700/50 px-2 py-0.5 rounded-md">Python / Node</span>
                </div>
              </div>

              <!-- Proyek 2 -->
              <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-2xl p-3.5 hover:border-zinc-700 transition-colors">
                <div class="flex items-start justify-between gap-2">
                  <div>
                    <h3 class="text-xs font-bold text-white">Discord Reminder Bot</h3>
                    <p class="text-[11px] text-zinc-400 mt-1 leading-relaxed">
                      Bot pengingat tugas dan jadwal terjadwal yang fleksibel, mendukung pengingat berupa server broadcast.
                    </p>
                  </div>
                  <a href="https://github.com/mattnael/reminder-dc-bot" target="_blank" class="text-zinc-400 hover:text-purple-400 text-xs shrink-0 px-2.5 py-1 bg-zinc-800/80 hover:bg-zinc-800 rounded-lg border border-zinc-700/60 transition-colors flex items-center gap-1">
                    <span>Repo</span>
                    <span>↗</span>
                  </a>
                </div>
                <div class="flex flex-wrap gap-1.5 mt-2.5">
                  <span class="text-[10px] bg-[#22222b] text-purple-300 border border-purple-500/20 px-2 py-0.5 rounded-md">Discord API</span>
                  <span class="text-[10px] bg-[#22222b] text-yellow-300 border border-yellow-500/20 px-2 py-0.5 rounded-md">Scheduler</span>
                  <span class="text-[10px] bg-[#22222b] text-zinc-300 border border-zinc-700/50 px-2 py-0.5 rounded-md">Productivity</span>
                </div>
              </div>

              <!-- Proyek 3 -->
              <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-2xl p-3.5 hover:border-zinc-700 transition-colors">
                <div class="flex items-start justify-between gap-2">
                  <div>
                    <h3 class="text-xs font-bold text-white">E-Archive Management System</h3>
                    <p class="text-[11px] text-zinc-400 mt-1 leading-relaxed">
                      Sistem manajemen arsip digital berbasis web untuk sentralisasi penyimpanan dokumen, tata kelola berkas, dan pencarian cepat.
                    </p>
                  </div>
                  <a href="https://github.com/Hilmee15/e-archive" target="_blank" class="text-zinc-400 hover:text-purple-400 text-xs shrink-0 px-2.5 py-1 bg-zinc-800/80 hover:bg-zinc-800 rounded-lg border border-zinc-700/60 transition-colors flex items-center gap-1">
                    <span>Repo</span>
                    <span>↗</span>
                  </a>
                </div>
                <div class="flex flex-wrap gap-1.5 mt-2.5">
                  <span class="text-[10px] bg-[#22222b] text-red-300 border border-red-500/20 px-2 py-0.5 rounded-md">Fullstack Web</span>
                  <span class="text-[10px] bg-[#22222b] text-blue-300 border border-blue-500/20 px-2 py-0.5 rounded-md">Database</span>
                  <span class="text-[10px] bg-[#22222b] text-zinc-300 border border-zinc-700/50 px-2 py-0.5 rounded-md">Management</span>
                </div>
              </div>
            </div>
          </div>

          <div class="mt-4 pt-3 border-t border-zinc-800/80 flex items-center justify-between">
            <span class="text-[11px] text-zinc-500">Lihat repositori lainnya di profil:</span>
            <a href="https://github.com/mattnael" target="_blank" class="text-xs font-semibold text-purple-400 hover:text-purple-300 flex items-center gap-1 transition-colors">
              <span>github.com/mattnael</span>
              <span>→</span>
            </a>
          </div>
        </div>

      </div>

      <!-- ================= KOLOM KANAN (4 SPAN) ================= -->
      <div class="lg:col-span-4 flex flex-col gap-5 order-3 lg:order-3">
        
        <!-- Campus Organizational -->
        <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-3xl p-5 hover:border-purple-500/40 transition-colors">
          <div class="flex items-center gap-2 mb-4 text-xs font-semibold uppercase tracking-wider text-zinc-400">
            <svg class="w-4 h-4 text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z" />
            </svg>
            <span>Campus Organizational</span>
          </div>

          <div class="flex flex-col gap-3">
            <!-- Event 1: Manager -->
            <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-2xl p-3.5">
              <div class="flex justify-between items-start">
                <span class="text-xs font-bold text-white leading-tight">Manager External Event Organizer</span>
                <span class="text-[10px] text-zinc-500 shrink-0">Oct 2025 – Present</span>
              </div>
              <div class="flex gap-2.5 items-center mt-2.5">
                <img 
                  src="/images/techdive.png" 
                  alt="BNCC TechDive 2025" 
                  class="w-12 h-12 rounded-lg object-cover border border-zinc-700/60 shrink-0 bg-zinc-800"
                />
                <div>
                  <p class="text-xs font-semibold text-purple-400 line-clamp-1">
                    BNCC TechDive 2025: Cloud-Powered Transformation
                  </p>
                  <p class="text-[11px] text-zinc-400 line-clamp-2 mt-0.5 leading-snug">
                    Memimpin acara sebagai Koordinator Divisi Acara & Perlengkapan.
                  </p>
                </div>
              </div>
            </div>

            <!-- Event 2: Activist -->
            <div class="bg-[#1a1a21]/90 border border-zinc-800/80 rounded-2xl p-3.5">
              <div class="flex justify-between items-start">
                <span class="text-xs font-bold text-white leading-tight">Activist External Event Organizer</span>
                <span class="text-[10px] text-zinc-500 shrink-0">Jan 2025 – Sep 2025</span>
              </div>
              <div class="flex gap-2.5 items-center mt-2.5">
                <img 
                  src="/images/smart-ai.png" 
                  alt="Smart Learning AI" 
                  class="w-12 h-12 rounded-lg object-cover border border-zinc-700/60 shrink-0 bg-zinc-800"
                />
                <div>
                  <p class="text-xs font-semibold text-purple-400 line-clamp-1">
                    Smart Learning Based on AI: Roadmap to Tomorrow
                  </p>
                  <p class="text-[11px] text-zinc-400 line-clamp-2 mt-0.5 leading-snug">
                    Membuat struktur acara dan menjadi operator teknis saat acara berlangsung.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Contact Me -->
        <div class="bg-gradient-to-b from-[#17171c] to-[#121215] border border-white/[0.08] shadow-xl shadow-black/40 rounded-3xl p-6 hover:border-emerald-500/30 transition-colors flex-1 flex flex-col justify-between">
          <div>
            <div class="flex items-center justify-between mb-3">
              <div class="flex items-center gap-2 text-xs font-semibold uppercase tracking-wider text-zinc-400">
                <svg class="w-4 h-4 text-emerald-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z" />
                </svg>
                <span>Contact Me</span>
              </div>
              <span class="inline-flex items-center gap-1 text-[10px] text-emerald-400 bg-emerald-500/10 border border-emerald-500/20 px-2 py-0.5 rounded-full">
                <span class="w-1.5 h-1.5 rounded-full bg-emerald-400 animate-pulse"></span>
                Fast Response
              </span>
            </div>

            <h3 class="text-base font-bold text-white">Let's Connect for Enrichment</h3>
            <p class="text-xs text-zinc-400 mt-1 leading-relaxed">
              Terbuka untuk diskusi peluang internship. Hubungi langsung lewat WhatsApp atau Email di bawah.
            </p>
          </div>

          <div class="flex flex-col gap-2.5 mt-5">
            <!-- Tombol WhatsApp -->
            <a 
              href="https://wa.me/6282215174801?text=Halo%20Matthew,%20saya%20tertarik%20dengan%20portofolio%20Anda" 
              target="_blank" 
              class="w-full py-2.5 rounded-xl text-xs font-semibold bg-emerald-600 hover:bg-emerald-500 text-white shadow-lg shadow-emerald-600/20 transition-all text-center inline-flex items-center justify-center gap-2"
            >
              <svg class="w-4 h-4 fill-current" viewBox="0 0 24 24">
                <path d="M17.472 14.382c-.301-.15-1.78-.879-2.056-.98-.276-.1-.477-.15-.678.15-.2.3-.778.98-.953 1.18-.175.201-.351.226-.652.076-.301-.15-1.272-.469-2.423-1.496-.896-.798-1.501-1.784-1.677-2.085-.175-.301-.019-.464.132-.613.136-.134.301-.35.451-.525.151-.176.201-.301.301-.502.1-.2.05-.376-.025-.526-.075-.15-.678-1.633-.929-2.238-.244-.59-.492-.51-.678-.52l-.578-.01c-.2 0-.526.075-.802.376-.276.301-1.053 1.029-1.053 2.509 0 1.48 1.078 2.909 1.229 3.11.15.2 2.122 3.24 5.141 4.544.718.31 1.279.496 1.716.635.722.23 1.379.197 1.898.12.578-.087 1.78-.727 2.031-1.43.251-.703.251-1.304.176-1.43-.076-.125-.276-.2-.577-.35zM12.004 2C6.48 2 2 6.48 2 12c0 1.956.564 3.784 1.542 5.332L2 22l4.82-1.263C8.307 21.564 10.098 22 12.004 22 17.524 22 22 17.52 22 12s-4.476-10-9.996-10z" />
              </svg>
              <span>Chat via WhatsApp</span>
              <span>↗</span>
            </a>

            <!-- Alamat Email -->
            <div class="flex items-center justify-between px-3.5 py-2.5 rounded-xl bg-[#1a1a21]/90 border border-zinc-800/80">
              <div class="flex items-center gap-2 min-w-0">
                <svg class="w-3.5 h-3.5 text-zinc-400 shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.8" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                </svg>
                <span class="text-xs text-zinc-300 font-mono truncate select-all">mattnael07@gmail.com</span>
              </div>
              <span class="text-[10px] text-zinc-500 uppercase tracking-wider font-semibold shrink-0 ml-2">Email</span>
            </div>
          </div>
        </div>

      </div>
    </main>

    <!-- ================= 4. MINIMALIST FOOTER ================= -->
    <footer class="max-w-7xl mx-auto w-full mt-10 pt-4 border-t border-zinc-800/60 relative z-20 flex flex-col sm:flex-row items-center justify-between text-[11px] text-zinc-500 gap-2">
      <p>© 2026 Matthew Natanael. Crafted with Nuxt 3 & Tailwind CSS.</p>
      <div class="flex items-center gap-4">
        <span class="hover:text-zinc-300 transition-colors">Bandung, Indonesia</span>
        <span>•</span>
        <span class="text-emerald-400 font-medium">Available for Opportunities</span>
      </div>
    </footer>

  </div>
</template>