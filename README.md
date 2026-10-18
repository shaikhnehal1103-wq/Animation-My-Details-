<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Shaikh Nehal | Full-Stack Developer & AI Enthusiast</title>
  
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <!-- Font Awesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Fira+Code:wght@400;500;600&display=display" rel="stylesheet">

  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: {
              50: '#f5f3ff',
              100: '#ede9fe',
              200: '#ddd6fe',
              300: '#c4b5fd',
              400: '#a78bfa',
              500: '#8b5cf6',
              600: '#7c3aed',
              700: '#6d28d9',
              800: '#5b21b6',
              900: '#4c1d95',
              accent: '#8B7BD8'
            }
          },
          fontFamily: {
            sans: ['"Plus Jakarta Sans"', 'sans-serif'],
            mono: ['"Fira Code"', 'monospace'],
          }
        }
      }
    }
  </script>

  <style>
    body {
      background-color: #0b0914;
      color: #f3f4f6;
      font-family: 'Plus Jakarta Sans', sans-serif;
      overflow-x: hidden;
    }

    /* Custom Glassmorphism */
    .glass-card {
      background: rgba(23, 18, 41, 0.6);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border: 1px solid rgba(139, 123, 216, 0.15);
    }
    
    .glass-card:hover {
      border-color: rgba(167, 139, 250, 0.4);
      box-shadow: 0 10px 30px -10px rgba(139, 123, 216, 0.2);
    }

    .glass-nav {
      background: rgba(11, 9, 20, 0.8);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(139, 123, 216, 0.1);
    }

    /* Glow Effects */
    .glow-bg {
      position: absolute;
      border-radius: 50%;
      filter: blur(120px);
      z-index: 0;
      opacity: 0.35;
      pointer-events: none;
    }

    .text-gradient {
      background: linear-gradient(135deg, #ffffff 0%, #A78BFA 50%, #8B7BD8 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    /* Typing Animation Cursor */
    .cursor {
      display: inline-block;
      width: 3px;
      background-color: #A78BFA;
      animation: blink 0.8s infinite;
    }

    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }
  </style>
</head>
<body class="relative min-h-screen selection:bg-brand-500 selection:text-white">

  <!-- Glow Elements -->
  <div class="glow-bg bg-purple-600 w-96 h-96 -top-20 -left-20"></div>
  <div class="glow-bg bg-brand-accent w-[500px] h-[500px] top-1/3 -right-32"></div>
  <div class="glow-bg bg-indigo-600 w-80 h-80 bottom-10 left-10"></div>

  <!-- Header / Navigation -->
  <header class="sticky top-0 z-50 glass-nav transition-all duration-300">
    <div class="max-w-6xl mx-auto px-6 h-20 flex items-center justify-between">
      <a href="#" class="text-2xl font-bold font-mono tracking-tight text-white flex items-center gap-2">
        <span class="text-brand-400">&lt;</span>ShaikhNehal<span class="text-brand-400">/&gt;</span>
      </a>

      <nav class="hidden md:flex items-center space-x-8 text-sm font-medium text-gray-300">
        <a href="#about" class="hover:text-brand-300 transition-colors">About</a>
        <a href="#skills" class="hover:text-brand-300 transition-colors">Tech Stack</a>
        <a href="#projects" class="hover:text-brand-300 transition-colors">Projects</a>
        <a href="#stats" class="hover:text-brand-300 transition-colors">GitHub</a>
        <a href="#connect" class="px-5 py-2.5 rounded-full bg-brand-600 hover:bg-brand-500 text-white font-semibold shadow-lg shadow-brand-600/30 transition-all hover:scale-105">Contact Me</a>
      </nav>

      <!-- Mobile Menu Button -->
      <button id="mobileMenuBtn" class="md:hidden text-gray-300 hover:text-white text-2xl focus:outline-none">
        <i class="fa-solid fa-bars"></i>
      </button>
    </div>

    <!-- Mobile Dropdown -->
    <div id="mobileMenu" class="hidden md:hidden glass-card border-x-0 border-t-0 px-6 py-4 flex flex-col gap-4 text-gray-300">
      <a href="#about" class="hover:text-brand-300 py-1">About</a>
      <a href="#skills" class="hover:text-brand-300 py-1">Tech Stack</a>
      <a href="#projects" class="hover:text-brand-300 py-1">Projects</a>
      <a href="#stats" class="hover:text-brand-300 py-1">GitHub</a>
      <a href="#connect" class="text-brand-400 font-semibold py-1">Contact Me</a>
    </div>
  </header>

  <main class="relative z-10 max-w-6xl mx-auto px-6">

    <!-- Hero Section -->
    <section class="min-h-[85vh] flex flex-col justify-center items-center text-center py-20">
      
      <!-- Badges -->
      <div class="flex flex-wrap justify-center gap-3 mb-8">
        <span class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full text-xs font-semibold bg-brand-900/50 text-brand-200 border border-brand-500/30">
          <i class="fa-solid fa-location-dot text-brand-400"></i> Islamabad, Pakistan
        </span>
        <span class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full text-xs font-semibold bg-brand-900/50 text-brand-200 border border-brand-500/30">
          <i class="fa-solid fa-certificate text-brand-400"></i> Certified AI Specialist
        </span>
        <span class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full text-xs font-semibold bg-emerald-950/60 text-emerald-300 border border-emerald-500/30">
          <span class="w-2 h-2 rounded-full bg-emerald-400 animate-pulse"></span> Open to Collaboration
        </span>
      </div>

      <!-- Main Headline -->
      <h1 class="text-5xl md:text-7xl font-extrabold tracking-tight mb-6">
        Hi, I'm <span class="text-gradient">Shaikh Nehal</span>
      </h1>

      <!-- Dynamic Typing Text -->
      <div class="h-12 mb-8 flex items-center justify-center">
        <p class="font-mono text-lg md:text-2xl text-brand-200">
          <span id="typing-text"></span><span class="cursor">&nbsp;</span>
        </p>
      </div>

      <!-- Description -->
      <p class="max-w-2xl text-gray-400 text-base md:text-lg leading-relaxed mb-10">
        An 18-year-old developer & designer crafting high-performance digital experiences. Blending clean code with functional UI/UX design and AI integration.
      </p>

      <!-- CTA Buttons -->
      <div class="flex flex-wrap justify-center gap-4">
        <a href="#projects" class="px-8 py-3.5 rounded-full bg-brand-600 hover:bg-brand-500 text-white font-semibold shadow-lg shadow-brand-600/30 transition-all hover:scale-105 flex items-center gap-2">
          View Featured Work <i class="fa-solid fa-arrow-down text-sm"></i>
        </a>
        <a href="#connect" class="px-8 py-3.5 rounded-full glass-card text-white font-semibold hover:bg-white/10 transition-all hover:scale-105 border border-brand-400/30 flex items-center gap-2">
          Let's Talk <i class="fa-solid fa-paper-plane text-sm text-brand-400"></i>
        </a>
      </div>
    </section>

    <!-- About Me Section -->
    <section id="about" class="py-20 border-t border-gray-800/60">
      <div class="grid grid-cols-1 md:grid-cols-12 gap-10 items-center">
        <div class="md:col-span-5 flex justify-center">
          <div class="relative group">
            <div class="absolute -inset-1 bg-gradient-to-r from-brand-500 to-indigo-600 rounded-3xl blur opacity-30 group-hover:opacity-75 transition duration-1000"></div>
            <div class="relative glass-card p-8 rounded-3xl text-center">
              <div class="w-32 h-32 mx-auto mb-6 rounded-2xl bg-gradient-to-tr from-brand-600 to-indigo-500 flex items-center justify-center text-5xl text-white shadow-xl">
                <i class="fa-solid fa-laptop-code"></i>
              </div>
              <h3 class="text-xl font-bold text-white mb-1">Shaikh Nehal</h3>
              <p class="text-brand-400 font-mono text-sm mb-4">18 y/o Developer & Designer</p>
              <div class="p-3 rounded-xl bg-black/30 border border-white/5 font-mono text-xs text-gray-400">
                ⚡ Motto: <span class="text-brand-200">"One small coding step at a time"</span>
              </div>
            </div>
          </div>
        </div>

        <div class="md:col-span-7 space-y-6">
          <h2 class="text-3xl md:text-4xl font-bold text-white">
            🚀 About <span class="text-brand-400">Me</span>
          </h2>
          <p class="text-gray-300 text-lg leading-relaxed">
            Hey! I'm Nehal, based in Islamabad. I specialize in building web applications that blend reliable full-stack architecture with visually polished front-end design.
          </p>
          
          <ul class="space-y-4">
            <li class="flex items-start gap-3 text-gray-300">
              <span class="p-1.5 rounded-lg bg-brand-500/20 text-brand-400 mt-0.5"><i class="fa-solid fa-seedling"></i></span>
              <span>Currently levelling up my <b>JavaScript & React</b> architecture skills.</span>
            </li>
            <li class="flex items-start gap-3 text-gray-300">
              <span class="p-1.5 rounded-lg bg-brand-500/20 text-brand-400 mt-0.5"><i class="fa-solid fa-robot"></i></span>
              <span>Exploring real-world <b>AI integration</b> to power smart applications.</span>
            </li>
            <li class="flex items-start gap-3 text-gray-300">
              <span class="p-1.5 rounded-lg bg-brand-500/20 text-brand-400 mt-0.5"><i class="fa-solid fa-palette"></i></span>
              <span>Passionate about UI/UX design, modern branding, and digital media editing.</span>
            </li>
          </ul>
        </div>
      </div>
    </section>

    <!-- Tech Stack Section -->
    <section id="skills" class="py-20 border-t border-gray-800/60">
      <div class="text-center mb-16">
        <h2 class="text-3xl md:text-4xl font-bold text-white mb-4">💻 Tech Stack & Tools</h2>
        <p class="text-gray-400 max-w-lg mx-auto">Technologies and creative tools I use to bring ideas into digital reality.</p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- Development Stack -->
        <div class="glass-card p-8 rounded-3xl">
          <div class="flex items-center gap-3 mb-6">
            <div class="p-3 rounded-xl bg-brand-500/20 text-brand-400 text-xl">
              <i class="fa-solid fa-code"></i>
            </div>
            <h3 class="text-xl font-bold text-white">Development</h3>
          </div>
          <div class="grid grid-cols-2 sm:grid-cols-4 gap-4">
            <div class="p-4 rounded-2xl bg-white/5 border border-white/5 text-center hover:bg-white/10 transition-colors">
              <i class="fa-brands fa
