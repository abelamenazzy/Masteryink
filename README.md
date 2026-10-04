# index.html
Curso tatuaje profesional
```html
<!DOCTYPE html>
<html lang="es" class="scroll-smooth dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mastery Ink Perú | Mentoría de Tatuaje Profesional & Bioseguridad MINSA</title>
    
    <!-- External Frameworks & Icons -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800;900&family=Syne:wght@700;800&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: {
                            bg: '#08080a',
                            card: '#121217',
                            border: '#22222d',
                            neon: '#00f2fe',
                            cyan: '#4facfe',
                            purple: '#742284',
                            yape: '#742284',
                            whatsapp: '#25D366',
                            gold: '#fbbf24'
                        }
                    },
                    fontFamily: {
                        heading: ['Syne', 'Montserrat', 'sans-serif'],
                        subheading: ['Montserrat', 'sans-serif'],
                        body: ['Inter', 'sans-serif']
                    },
                    boxShadow: {
                        'neon-glow': '0 0 25px rgba(0, 242, 254, 0.35)',
                        'purple-glow': '0 0 30px rgba(116, 34, 132, 0.4)',
                        'gold-glow': '0 0 20px rgba(251, 191, 36, 0.25)',
                    },
                    animation: {
                        'pulse-fast': 'pulse 1.5s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                        'float': 'float 4s ease-in-out infinite',
                        'glow-rotate': 'glowRotate 6s linear infinite'
                    },
                    keyframes: {
                        float: {
                            '0%, 100%': { transform: 'translateY(0px)' },
                            '50%': { transform: 'translateY(-8px)' }
                        }
                    }
                }
            }
        }
    </script>

    <!-- Custom Micro-styles -->
    <style>
        body {
            background-color: #08080a;
            color: #f1f5f9;
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
        }
        .gradient-text-cyan {
            background: linear-gradient(135deg, #00f2fe 0%, #4facfe 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .gradient-text-gold {
            background: linear-gradient(135deg, #fef08a 0%, #f59e0b 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .glass-card {
            background: rgba(18, 18, 23, 0.75);
            backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.08);
        }
        .glass-card-hover:hover {
            border-color: rgba(0, 242, 254, 0.4);
            box-shadow: 0 0 20px rgba(0, 242, 254, 0.15);
        }
        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #08080a;
        }
        ::-webkit-scrollbar-thumb {
            background: #22222d;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #00f2fe;
        }
    </style>
</head>
<body class="antialiased selection:bg-brand-neon selection:text-black">

    <!-- Top Urgency Banner -->
    <div class="bg-gradient-to-r from-brand-purple via-brand-bg to-brand-purple text-white py-2.5 px-4 text-center border-b border-white/10 sticky top-0 z-50">
        <div class="max-w-7xl mx-auto flex flex-col sm:flex-row items-center justify-between gap-2 text-xs sm:text-sm font-subheading">
            <div class="flex items-center gap-2">
                <span class="bg-red-500 text-white font-black px-2 py-0.5 rounded uppercase text-[10px] tracking-wider animate-pulse">Lanzamiento 2026</span>
                <span class="font-medium text-gray-200">50% OFF de Descuento para Alumnos Nuevos</span>
            </div>
            <div class="flex items-center gap-3">
                <span class="text-gray-400 font-medium">La oferta finaliza en:</span>
                <div class="flex items-center gap-1 font-black text-brand-neon bg-black/50 px-3 py-1 rounded-md border border-brand-neon/30">
                    <span id="timer-hours">02</span>h : 
                    <span id="timer-minutes">34</span>m : 
                    <span id="timer-seconds">12</span>s
                </div>
            </div>
        </div>
    </div>

    <!-- Main Navigation Header -->
    <header class="bg-brand-bg/90 backdrop-blur-md border-b border-white/5 sticky top-[41px] z-40">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
            <!-- Brand Logo -->
            <a href="#" class="flex items-center gap-3 group">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-br from-brand-neon to-brand-purple p-0.5 shadow-neon-glow group-hover:scale-105 transition-transform">
                    <div class="w-full h-full bg-brand-bg rounded-[10px] flex items-center justify-center">
                        <i class="fa-solid fa-pen-nib text-brand-neon text-lg"></i>
                    </div>
                </div>
                <div>
                    <span class="font-heading font-extrabold text-xl tracking-tight uppercase block leading-none">Mastery Ink <span class="gradient-text-cyan">Perú</span></span>
                    <span class="text-[10px] tracking-widest text-gray-400 font-semibold uppercase">Mentoría Elite Tatuaje</span>
                </div>
            </a>

            <!-- Navigation Links -->
            <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-300">
                <a href="#calculadora" class="hover:text-brand-neon transition-colors">Calculadora S/.</a>
                <a href="#temario" class="hover:text-brand-neon transition-colors">Campus & Módulos</a>
                <a href="#certificados" class="hover:text-brand-neon transition-colors">Certificación MINSA</a>
                <a href="#testimonios" class="hover:text-brand-neon transition-colors">Casos de Éxito</a>
                <a href="#faq" class="hover:text-brand-neon transition-colors">Preguntas</a>
            </nav>

            <!-- Header Action -->
            <div class="flex items-center gap-3">
                <button onclick="openModal()" class="bg-gradient-to-r from-brand-neon to-brand-cyan text-black font-subheading font-extrabold px-6 py-2.5 rounded-xl shadow-neon-glow hover:scale-105 transition-all text-sm uppercase tracking-wider flex items-center gap-2">
                    <i class="fa-solid fa-bolt"></i>
                    <span>Inscribirme (S/ 149.50)</span>
                </button>
            </div>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="relative pt-12 pb-20 overflow-hidden">
        <!-- Background Ambient Glows -->
        <div class="absolute top-1/4 left-1/2 -translate-x-1/2 -translate-y-1/2 w-[600px] h-[600px] bg-brand-neon/10 rounded-full blur-[140px] pointer-events-none"></div>
        <div class="absolute top-1/3 right-10 w-[400px] h-[400px] bg-brand-purple/20 rounded-full blur-[120px] pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid lg:grid-cols-12 gap-12 items-center">
                
                <!-- Left Column: Copywriting -->
                <div class="lg:col-span-7 space-y-8">
                    
                    <!-- Badges -->
                    <div class="flex flex-wrap items-center gap-3">
                        <span class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-brand-neon/10 border border-brand-neon/30 text-brand-neon text-xs font-bold uppercase tracking-wider">
                            <i class="fa-solid fa-certificate"></i> Certificación Biosostenible MINSA/DIGESA
                        </span>
                        <span class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-amber-400/10 border border-amber-400/30 text-amber-400 text-xs font-bold uppercase tracking-wider">
                            <i class="fa-solid fa-star"></i> 4.9/5 (+140 Alumnos Peruanos)
                        </span>
                    </div>

                    <!-- Main Headline -->
                    <h1 class="font-heading font-black text-4xl sm:text-6xl lg:text-7xl leading-[1.08] tracking-tight uppercase">
                        Conviértete en un <br>
                        <span class="gradient-text-cyan">Tatuador Profesional</span> <br>
                        y Cobra lo que Vale tu Arte.
                    </h1>

                    <p class="text-gray-300 text-lg sm:text-xl font-light leading-relaxed max-w-2xl">
                        Aprende la técnica completa desde cero: calibración de máquina pen, líneas perfectas, sombras realistas, asepsia nivel laboratorio y cómo captar clientes en Perú para generar <strong class="text-white font-semibold">de S/ 2,500 a S/ 6,000 mensuales</strong>.
                    </p>

                    <!-- Price Box & Main CTA -->
                    <div class="glass-card p-6 rounded-3xl border border-white/10 space-y-6 max-w-xl">
                        <div class="flex items-center justify-between border-b border-white/10 pb-4">
                            <div>
                                <span class="text-xs text-gray-400 uppercase tracking-wider font-bold block">Inversión Regular</span>
                                <span class="text-gray-500 line-through text-lg font-bold">S/ 299.00 PEN</span>
                            </div>
                            <div class="text-right">
                                <span class="text-xs text-brand-neon font-black uppercase tracking-wider block">Oferta Alumnos Nuevos (50% OFF)</span>
                                <div class="flex items-baseline gap-1">
                                    <span class="font-heading font-black text-4xl text-white">S/ 149</span>
                                    <span class="text-brand-neon font-bold text-xl">.50</span>
                                </div>
                            </div>
                        </div>

                        <div class="flex flex-col sm:flex-row gap-4">
                            <button onclick="openModal()" class="flex-1 bg-gradient-to-r from-brand-neon via-brand-cyan to-brand-neon text-black font-subheading font-black text-lg py-4 px-6 rounded-2xl shadow-neon-glow hover:scale-[1.02] transition-transform uppercase tracking-wider flex items-center justify-center gap-3">
                                <i class="fa-solid fa-qrcode text-xl"></i>
                                <span>Pagar con Yape (S/ 149.50)</span>
                            </button>
                            <a href="#calculadora" class="bg-white/5 hover:bg-white/10 text-white border border-white/10 font-subheading font-bold text-sm py-4 px-6 rounded-2xl transition-colors flex items-center justify-center gap-2">
                                <i class="fa-solid fa-calculator text-brand-neon"></i>
                                <span>Calcular Mis Ganancias</span>
                            </a>
                        </div>

                        <div class="flex items-center justify-between text-xs text-gray-400 pt-1">
                            <span class="flex items-center gap-1.5"><i class="fa-solid fa-shield-check text-emerald-400"></i> Acceso Vitalicio e Inmediato</span>
                            <a href="https://wa.me/51958934204?text=Hola%20Mentor,%20tengo%20consultas%20sobre%20la%20Mentor%C3%ADa" target="_blank" class="flex items-center gap-1.5 text-brand-whatsapp hover:underline font-semibold">
                                <i class="fa-brands fa-whatsapp text-brand-whatsapp"></i> Asistencia Mentor: 958 934 204
                            </a>
                        </div>
                    </div>

                </div>

                <!-- Right Column: Visual Feature Card & QR Preview -->
                <div class="lg:col-span-5 relative">
                    <div class="relative mx-auto max-w-md">
                        <!-- Neon Ring effect -->
                        <div class="absolute -inset-1 bg-gradient-to-r from-brand-neon to-brand-purple rounded-3xl blur opacity-75 animate-pulse"></div>
                        
                        <div class="relative glass-card p-6 rounded-3xl border border-white/15 space-y-6">
                            
                            <!-- Card Badge Header -->
                            <div class="flex items-center justify-between">
                                <div class="flex items-center gap-3">
                                    <div class="w-12 h-12 rounded-2xl bg-brand-purple/40 border border-brand-purple flex items-center justify-center text-white font-bold">
                                        <i class="fa-solid fa-award text-2xl text-brand-neon"></i>
                                    </div>
                                    <div>
                                        <h4 class="font-heading font-extrabold text-white text-base">Mentoría Elite 2026</h4>
                                        <p class="text-xs text-gray-400">Mastery Ink Perú • Modalidad Online</p>
                                    </div>
                                </div>
                                <span class="bg-emerald-500/10 border border-emerald-500/30 text-emerald-400 text-[11px] font-bold px-2.5 py-1 rounded-full">
                                    ● En Vivo + Grabado
                                </span>
                            </div>

                            <!-- Highlights list -->
                            <div class="space-y-3 border-t border-b border-white/10 py-4 text-sm text-gray-300">
                                <div class="flex items-start gap-3">
                                    <i class="fa-solid fa-check-circle text-brand-neon mt-1"></i>
                                    <span><strong>Módulo Bioseguridad:</strong> Protocolos según normas DIGESA/MINSA del Perú.</span>
                                </div>
                                <div class="flex items-start gap-3">
                                    <i class="fa-solid fa-check-circle text-brand-neon mt-1"></i>
                                    <span><strong>Calibración de Agujas & Pen:</strong> Voltaje, profundidad y tipos de piel.</span>
                                </div>
                                <div class="flex items-start gap-3">
                                    <i class="fa-solid fa-check-circle text-brand-neon mt-1"></i>
                                    <span><strong>Plantillas de Consentimiento:</strong> Documentos legales listos para usar con tus clientes.</span>
                                </div>
                                <div class="flex items-start gap-3">
                                    <i class="fa-solid fa-check-circle text-brand-neon mt-1"></i>
                                    <span><strong>Certificación Oficial:</strong> Código QR de verificación incluido.</span>
                                </div>
                            </div>

                            <!-- Fast Payment QR Preview Box -->
                            <div class="bg-black/60 rounded-2xl p-4 border border-brand-purple/40 flex items-center gap-4">
                                <img src="1001564926_2.jpg" alt="QR Yape" class="w-20 h-20 rounded-xl object-cover border border-white/20 shadow-md" onerror="this.src='1001564926.jpg'">
                                <div class="space-y-1 flex-1">
                                    <span class="text-[10px] font-bold text-brand-neon uppercase tracking-wider block">Yape Directo Perú</span>
                                    <p class="text-xs text-gray-300">Número oficial:</p>
                                    <p class="font-heading font-black text-white text-lg tracking-wider">976 275 695</p>
                                    <button onclick="openModal()" class="text-xs font-bold text-brand-neon underline hover:text-white transition-colors">
                                        Escanear QR y Yapear ahora →
                                    </button>
                                </div>
                            </div>

                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- TRUST & METRICS BANNER -->
    <section class="border-y border-white/10 bg-brand-card/50 py-10">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8 text-center">
                <div class="space-y-1">
                    <span class="font-heading font-black text-3xl sm:text-4xl text-white">100%</span>
                    <p class="text-xs text-gray-400 font-medium uppercase tracking-wider">Práctico y Aplicable</p>
                </div>
                <div class="space-y-1">
                    <span class="font-heading font-black text-3xl sm:text-4xl gradient-text-cyan">S/ 150 - 450</span>
                    <p class="text-xs text-gray-400 font-medium uppercase tracking-wider">Cobro Promedio por Tatuaje Pequeño/Mediano</p>
                </div>
                <div class="space-y-1">
                    <span class="font-heading font-black text-3xl sm:text-4xl text-white">+140</span>
                    <p class="text-xs text-gray-400 font-medium uppercase tracking-wider">Alumnos Certificados en Perú</p>
                </div>
                <div class="space-y-1">
                    <span class="font-heading font-black text-3xl sm:text-4xl gradient-text-gold">MINSA</span>
                    <p class="text-xs text-gray-400 font-medium uppercase tracking-wider">Estándares Sanitarios DIGESA</p>
                </div>
            </div>
        </div>
    </section>

    <!-- INTERACTIVE TATTOO PRICING CALCULATOR -->
    <section id="calculadora" class="py-20 relative">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            
            <div class="text-center space-y-4 mb-12">
                <span class="text-xs font-bold text-brand-neon uppercase tracking-widest bg-brand-neon/10 border border-brand-neon/30 px-3 py-1 rounded-full">
                    Herramienta Exclusiva para Alumnos
                </span>
                <h2 class="font-heading font-black text-3xl sm:text-5xl uppercase">
                    Simulador de <span class="gradient-text-cyan">Ganancias en Soles (S/.)</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto text-sm sm:text-base">
                    Descubre cuánto puedes cobrar por cada tatuaje en el mercado peruano y en cuántos días recuperarás el 100% de tu inversión de esta mentoría.
                </p>
            </div>

            <div class="glass-card rounded-3xl p-6 sm:p-10 border border-white/10 grid md:grid-cols-12 gap-8 items-center">
                
                <!-- Calculator Controls -->
                <div class="md:col-span-7 space-y-6">
                    
                    <!-- Slider 1: Tatuajes por semana -->
                    <div class="space-y-2">
                        <div class="flex justify-between text-sm font-semibold">
                            <label for="tattoos-per-week" class="text-gray-300">Tatuajes realizados a la semana:</label>
                            <span id="tattoos-val" class="text-brand-neon font-black font-heading text-base">3 Tatuajes</span>
                        </div>
                        <input type="range" id="tattoos-per-week" min="1" max="15" value="3" class="w-full h-2 bg-gray-800 rounded-lg appearance-none cursor-pointer accent-brand-neon">
                        <div class="flex justify-between text-[10px] text-gray-500">
                            <span>1/sem (Hobby)</span>
                            <span>7/sem (Tiempo Parcial)</span>
                            <span>15/sem (Estudio Propio)</span>
                        </div>
                    </div>

                    <!-- Slider 2: Precio promedio por tatuaje -->
                    <div class="space-y-2">
                        <div class="flex justify-between text-sm font-semibold">
                            <label for="price-per-tattoo" class="text-gray-300">Cobro promedio por tatuaje (S/.):</label>
                            <span id="price-val" class="text-brand-neon font-black font-heading text-base">S/ 180</span>
                        </div>
                        <input type="range" id="price-per-tattoo" min="80" max="600" step="10" value="180" class="w-full h-2 bg-gray-800 rounded-lg appearance-none cursor-pointer accent-brand-neon">
                        <div class="flex justify-between text-[10px] text-gray-500">
                            <span>S/ 80 (Minimalista 5cm)</span>
                            <span>S/ 250 (Línea Fina/Sombras 12cm)</span>
                            <span>S/ 600+ (Pieza Grande)</span>
                        </div>
                    </div>

                    <!-- Estilo Dominante Selector -->
                    <div class="space-y-2">
                        <label class="text-sm font-semibold text-gray-300 block">Estilo Principal de Trabajo:</label>
                        <div class="grid grid-cols-2 sm:grid-cols-3 gap-2">
                            <button type="button" onclick="setStyleFactor(1.0, this)" class="style-btn active text-xs py-2 px-3 rounded-xl border border-brand-neon bg-brand-neon/20 text-brand-neon font-bold">Line Work / Fine Line</button>
                            <button type="button" onclick="setStyleFactor(1.25, this)" class="style-btn text-xs py-2 px-3 rounded-xl border border-white/10 bg-white/5 text-gray-300 hover:border-white/30 font-bold">Black & Grey / Sombras</button>
                            <button type="button" onclick="setStyleFactor(1.4, this)" class="style-btn text-xs py-2 px-3 rounded-xl border border-white/10 bg-white/5 text-gray-300 hover:border-white/30 font-bold">Full Color / Neotrad</button>
                        </div>
                    </div>

                </div>

                <!-- Calculator Results Display -->
                <div class="md:col-span-5 bg-gradient-to-br from-brand-card to-black p-6 rounded-2xl border border-brand-neon/30 text-center space-y-6">
                    <div>
                        <span class="text-xs text-gray-400 font-bold uppercase tracking-wider block">Ingreso Mensual Estimado</span>
                        <div class="font-heading font-black text-4xl text-brand-neon mt-1" id="monthly-income">
                            S/ 2,160.00
                        </div>
                        <p class="text-[11px] text-gray-400 mt-1">Descontando insumos descartables aproximados (~15%).</p>
                    </div>

                    <div class="border-t border-white/10 pt-4 space-y-3 text-left">
                        <div class="flex justify-between text-xs text-gray-300">
                            <span>Recuperación de la Mentoría:</span>
                            <strong id="payback-tattoos" class="text-emerald-400 font-bold">En tu 1er tatuaje</strong>
                        </div>
                        <div class="flex justify-between text-xs text-gray-300">
                            <span>Ganancia Neta Anual:</span>
                            <strong id="yearly-profit" class="text-amber-400 font-bold">S/ 25,920.00</strong>
                        </div>
                    </div>

                    <button onclick="openModal()" class="w-full bg-brand-neon text-black font-subheading font-black py-3 rounded-xl uppercase text-xs tracking-wider shadow-neon-glow hover:scale-105 transition-transform">
                        ¡Asegurar mi cupo por S/ 149.50!
                    </button>
                </div>

            </div>
        </div>
    </section>

    <!-- MÓDULOS DEL CAMPUS VIRTUAL -->
    <section id="temario" class="py-20 bg-brand-card/30 border-y border-white/5">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            
            <div class="text-center space-y-4 mb-16">
                <span class="text-xs font-bold text-brand-neon uppercase tracking-widest bg-brand-neon/10 border border-brand-neon/30 px-3 py-1 rounded-full">
                    Temario Estructurado Paso a Paso
                </span>
                <h2 class="font-heading font-black text-3xl sm:text-5xl uppercase">
                    ¿Qué vas a dominar en esta <span class="gradient-text-cyan">Mentoría Elite</span>?
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto text-sm sm:text-base">
                    Un plan de estudio acelerado diseñado para llevarte directo a la práctica profesional sin perder tiempo en teoría innecesaria.
                </p>
            </div>

            <!-- Grid of 6 Modules -->
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                
                <!-- Módulo 1 -->
                <div class="glass-card rounded-2xl p-6 border border-white/10 space-y-4 glass-card-hover transition-all">
                    <div class="w-12 h-12 rounded-xl bg-red-500/10 border border-red-500/30 flex items-center justify-center text-red-400 font-bold text-xl">
                        01
                    </div>
                    <h3 class="font-heading font-extrabold text-xl text-white">Bioseguridad & Normas MINSA</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">
                        Asepsia, esterilización de mesa, desecho de RPBI (agujas/biocontaminados), barreras de protección e higiene sanitaria. Evita multas y protege a tus clientes.
                    </p>
                    <ul class="text-xs text-gray-300 space-y-2 pt-2 border-t border-white/5">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Protocolo de armado de mesa estéril</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Licencia y requisitos municipales Perú</li>
                    </ul>
                </div>

                <!-- Módulo 2 -->
                <div class="glass-card rounded-2xl p-6 border border-white/10 space-y-4 glass-card-hover transition-all">
                    <div class="w-12 h-12 rounded-xl bg-brand-neon/10 border border-brand-neon/30 flex items-center justify-center text-brand-neon font-bold text-xl">
                        02
                    </div>
                    <h3 class="font-heading font-extrabold text-xl text-white">Calibración de Máquinas Pen</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">
                        Dominio total del voltaje, stroke (recorrido), agujas cartucho (3RL, 7RL, Magnum, Shader) y compatibilidad de fuentes inalámbricas o con cable.
                    </p>
                    <ul class="text-xs text-gray-300 space-y-2 pt-2 border-t border-white/5">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Selección exacta de voltajes según la piel</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Configuración de máquinas rotativas</li>
                    </ul>
                </div>

                <!-- Módulo 3 -->
                <div class="glass-card rounded-2xl p-6 border border-white/10 space-y-4 glass-card-hover transition-all">
                    <div class="w-12 h-12 rounded-xl bg-purple-500/10 border border-purple-500/30 flex items-center justify-center text-purple-400 font-bold text-xl">
                        03
                    </div>
                    <h3 class="font-heading font-extrabold text-xl text-white">Técnica de Line Work (Línea Fina)</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">
                        Aprende la firmeza de mano, inclinación del cartucho y profundidad de aguja (epidermis vs dermis) para lograr líneas sólidas que no se expanden con el tiempo.
                    </p>
                    <ul class="text-xs text-gray-300 space-y-2 pt-2 border-t border-white/5">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Ejercicios en piel sintética / fruta</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Control del temblor y respiración</li>
                    </ul>
                </div>

                <!-- Módulo 4 -->
                <div class="glass-card rounded-2xl p-6 border border-white/10 space-y-4 glass-card-hover transition-all">
                    <div class="w-12 h-12 rounded-xl bg-amber-500/10 border border-amber-500/30 flex items-center justify-center text-amber-400 font-bold text-xl">
                        04
                    </div>
                    <h3 class="font-heading font-extrabold text-xl text-white">Sombras & Texturas (Black & Grey)</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">
                        Preparación de tonos de sombra (Sumie/Dilución), técnica de péndulo, arrastre y puntillismo de arrastre para degradados suaves sin lastimar la piel.
                    </p>
                    <ul class="text-xs text-gray-300 space-y-2 pt-2 border-t border-white/5">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Fórmulas de dilución de tintas negras</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Sombras suaves sin parches</li>
                    </ul>
                </div>

                <!-- Módulo 5 -->
                <div class="glass-card rounded-2xl p-6 border border-white/10 space-y-4 glass-card-hover transition-all">
                    <div class="w-12 h-12 rounded-xl bg-emerald-500/10 border border-emerald-500/30 flex items-center justify-center text-emerald-400 font-bold text-xl">
                        05
                    </div>
                    <h3 class="font-heading font-extrabold text-xl text-white">Curación & Cuidados Post-Tatuaje</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">
                        Uso de parches curativos (Film transparente), cremas cicatrizantes recomendadas en Perú y cómo dar instrucciones claras al cliente para asegurar colores vivos.
                    </p>
                    <ul class="text-xs text-gray-300 space-y-2 pt-2 border-t border-white/5">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Hoja de cuidados imprimible para clientes</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Solución de posibles infecciones o alergias</li>
                    </ul>
                </div>

                <!-- Módulo 6 -->
                <div class="glass-card rounded-2xl p-6 border border-white/10 space-y-4 glass-card-hover transition-all">
                    <div class="w-12 h-12 rounded-xl bg-cyan-500/10 border border-cyan-500/30 flex items-center justify-center text-cyan-400 font-bold text-xl">
                        06
                    </div>
                    <h3 class="font-heading font-extrabold text-xl text-white">Marketing y Captación de Clientes</h3>
                    <p class="text-xs text-gray-400 leading-relaxed">
                        Cómo tomar fotos con luz polarizada a tus tatuajes, crear videos virales para TikTok/Instagram Reels y cómo cerrar clientes por WhatsApp cobrando precios altos.
                    </p>
                    <ul class="text-xs text-gray-300 space-y-2 pt-2 border-t border-white/5">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Scripts de ventas por WhatsApp</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-neon"></i> Configuración de perfil profesional</li>
                    </ul>
                </div>

            </div>

        </div>
    </section>

    <!-- MINI QUIZ INTERACTIVO DE BIOSEGURIDAD -->
    <section class="py-16 bg-brand-bg relative">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="glass-card p-8 rounded-3xl border border-brand-neon/30 relative overflow-hidden">
                <div class="absolute top-0 right-0 bg-brand-neon text-black text-[10px] font-black uppercase px-4 py-1 rounded-bl-xl">
                    Evaluación rápida
                </div>

                <div class="space-y-4 mb-6">
                    <span class="text-xs text-brand-neon font-bold uppercase tracking-wider">Demuestra tu Nivel</span>
                    <h3 class="font-heading font-black text-2xl sm:text-3xl">Prueba Express de Bioseguridad en Tatuaje</h3>
                    <p class="text-xs text-gray-400">Responde esta pregunta oficial para medir tus conocimientos sanitarios iniciales:</p>
                </div>

                <div id="quiz-container" class="space-y-4">
                    <p class="text-sm sm:text-base font-semibold text-gray-200">
                        ¿Cuál es la profundidad correcta de inyección de la aguja de tatuaje para depositar el pigmento sin provocar expansión (blowout)?
                    </p>

                    <div class="grid sm:grid-cols-3 gap-3">
                        <button onclick="checkQuiz(1, this)" class="quiz-opt text-xs p-4 rounded-xl border border-white/10 bg-white/5 hover:bg-white/10 text-left transition-all">
                            A) En la capa Epidermis superficial (0.2 mm).
                        </button>
                        <button onclick="checkQuiz(2, this)" class="quiz-opt text-xs p-4 rounded-xl border border-white/10 bg-white/5 hover:bg-white/10 text-left transition-all">
                            B) En la Dermis Papilar/Reticular (1.0 mm a 2.0 mm).
                        </button>
                        <button onclick="checkQuiz(3, this)" class="quiz-opt text-xs p-4 rounded-xl border border-white/10 bg-white/5 hover:bg-white/10 text-left transition-all">
                            C) En el tejido Subcutáneo graso (4.0 mm).
                        </button>
                    </div>

                    <div id="quiz-result" class="hidden p-4 rounded-xl text-xs font-bold transition-all"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN CERTIFICACIÓN DIGESA / MINSA -->
    <section id="certificados" class="py-20 relative bg-brand-card/40">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid lg:grid-cols-12 gap-12 items-center">
                
                <div class="lg:col-span-6 space-y-6">
                    <span class="text-xs font-bold text-amber-400 uppercase tracking-widest bg-amber-400/10 border border-amber-400/30 px-3 py-1 rounded-full">
                        Respaldo Profesional Garantizado
                    </span>
                    <h2 class="font-heading font-black text-3xl sm:text-5xl uppercase leading-tight">
                        Certificados con <br><span class="gradient-text-gold">Validez Sanitaria & Técnica</span>
                    </h2>
                    <p class="text-gray-300 text-sm sm:text-base leading-relaxed">
                        Al completar las evaluaciones prácticas de la mentoría, recibirás tu acreditación oficial emitida por <strong>Mastery Ink Perú</strong>, con sello de verificación de bioseguridad bajo normas MINSA/DIGESA y código QR de validación digital para tus clientes.
                    </p>

                    <div class="space-y-4 pt-2">
                        <div class="flex items-center gap-3">
                            <div class="w-8 h-8 rounded-lg bg-amber-400/20 text-amber-400 flex items-center justify-center font-bold">
                                <i class="fa-solid fa-shield-halved"></i>
                            </div>
                            <span class="text-sm font-medium text-gray-200">Acreditación en Bioseguridad y Asepsia Sanitaria.</span>
                        </div>
                        <div class="flex items-center gap-3">
                            <div class="w-8 h-8 rounded-lg bg-brand-neon/20 text-brand-neon flex items-center justify-center font-bold">
                                <i class="fa-solid fa-qrcode"></i>
                            </div>
                            <span class="text-sm font-medium text-gray-200">Código QR de verificación en línea activo las 24 horas.</span>
                        </div>
                    </div>

                    <!-- Interactive Name Input for Certificate Live Preview -->
                    <div class="pt-4 border-t border-white/10 space-y-3">
                        <label for="student-name-input" class="text-xs font-bold uppercase tracking-wider text-gray-400 block">
                            Prueba escribir tu nombre para ver tu Certificado Personalizado:
                        </label>
                        <div class="flex gap-2">
                            <input type="text" id="student-name-input" placeholder="Ej: Carlos Mendoza Rivas" class="flex-1 bg-black/60 border border-white/20 rounded-xl px-4 py-3 text-sm text-white focus:outline-none focus:border-brand-neon">
                            <button onclick="updateCertificateName()" class="bg-brand-neon text-black font-bold px-5 py-3 rounded-xl text-xs uppercase tracking-wider hover:scale-105 transition-transform">
                                Vista Previa
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Certificate Visual Render Box -->
                <div class="lg:col-span-6">
                    <div class="bg-stone-900 border-4 border-amber-500/40 p-6 sm:p-8 rounded-2xl shadow-gold-glow relative text-center text-stone-200 space-y-6 overflow-hidden">
                        <!-- Corner Watermarks -->
                        <div class="absolute top-2 left-2 text-amber-500/20 text-4xl"><i class="fa-solid fa-certificate"></i></div>
                        <div class="absolute bottom-2 right-2 text-amber-500/20 text-4xl"><i class="fa-solid fa-stamp"></i></div>

                        <div class="border-b border-amber-500/30 pb-4">
                            <span class="text-[10px] tracking-[0.3em] font-black uppercase text-amber-400 block">República del Perú • Mastery Ink</span>
                            <h3 class="font-heading font-black text-2xl sm:text-3xl text-amber-100 tracking-wider uppercase mt-1">Certificado de Aprobación</h3>
                            <p class="text-[11px] text-amber-400/80 uppercase font-semibold">Tatuador Profesional & Bioseguridad MINSA</p>
                        </div>

                        <div class="space-y-2 py-2">
                            <p class="text-xs text-stone-400 italic">Otorgado con honor a:</p>
                            <h4 id="cert-name-display" class="font-heading font-extrabold text-2xl sm:text-3xl text-white tracking-wide underline decoration-amber-500 decoration-2">
                                [TU NOMBRE AQUÍ]
                            </h4>
                            <p class="text-xs text-stone-300 max-w-md mx-auto pt-2 leading-relaxed">
                                Por haber cumplido satisfactoriamente con 60 horas lectivas de mentoría técnica en inyección de pigmentos, calibración de equipo y cumplimiento de los estándares de asepsia y bioseguridad sanitaria DIGESA/MINSA.
                            </p>
                        </div>

                        <div class="flex items-center justify-between pt-4 border-t border-amber-500/30 text-[10px] text-stone-400">
                            <div class="text-left">
                                <p class="font-bold text-white">Director Técnico</p>
                                <p>Mastery Ink Perú</p>
                            </div>
                            <div class="w-12 h-12 bg-white p-1 rounded">
                                <img src="1001564926_2.jpg" alt="QR Verificación" class="w-full h-full object-cover" onerror="this.src='1001564926.jpg'">
                            </div>
                            <div class="text-right">
                                <p class="font-bold text-amber-400">Código Verificador:</p>
                                <p>MI-PERU-2026-REG</p>
                            </div>
                        </div>

                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- PRICING & OFFER SECTION -->
    <section class="py-20 relative">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            
            <div class="text-center space-y-4 mb-16">
                <span class="text-xs font-bold text-brand-neon uppercase tracking-widest bg-brand-neon/10 border border-brand-neon/30 px-3 py-1 rounded-full">
                    Asegura tu cupo con el 50% OFF
                </span>
                <h2 class="font-heading font-black text-3xl sm:text-5xl uppercase">
                    Inversión Única y <span class="gradient-text-cyan">Acceso de Por Vida</span>
                </h2>
                <p class="text-gray-400 max-w-2xl mx-auto text-sm sm:text-base">
                    Sin mensualidades ni cobros ocultos. Pagas una sola vez y obtienes todo el contenido, plantillas y asesoría directa.
                </p>
            </div>

            <!-- Pricing Box -->
            <div class="glass-card rounded-3xl border-2 border-brand-neon p-8 sm:p-12 relative shadow-neon-glow overflow-hidden">
                <div class="absolute top-0 right-0 bg-gradient-to-l from-brand-neon to-brand-cyan text-black font-black text-xs uppercase px-6 py-2 rounded-bl-2xl">
                    🔥 Oferta Especial Perú
                </div>

                <div class="grid md:grid-cols-12 gap-8 items-center">
                    
                    <div class="md:col-span-7 space-y-6">
                        <h3 class="font-heading font-black text-3xl text-white">
                            Mentoría Completa Mastery Ink
                        </h3>
                        <p class="text-gray-300 text-sm">
                            Todo lo que necesitas para iniciar tu camino o elevar tu nivel técnico en el tatuaje comercial y artístico.
                        </p>

                        <div class="space-y-3 pt-2 text-sm text-gray-200">
                            <div class="flex items-center gap-3">
                                <i class="fa-solid fa-circle-check text-brand-neon"></i>
                                <span>Acceso ilimitado al campus con 6 Módulos HD.</span>
                            </div>
                            <div class="flex items-center gap-3">
                                <i class="fa-solid fa-circle-check text-brand-neon"></i>
                                <span>Plantillas Legales y Hoja de Consentimiento (MINSA).</span>
                            </div>
                            <div class="flex items-center gap-3">
                                <i class="fa-solid fa-circle-check text-brand-neon"></i>
                                <span>Guía Proveedores Oficiales de insumos en Lima/Perú.</span>
                            </div>
                            <div class="flex items-center gap-3">
                                <i class="fa-solid fa-circle-check text-brand-neon"></i>
                                <span>Soporte directo por WhatsApp con el mentor.</span>
                            </div>
                            <div class="flex items-center gap-3">
                                <i class="fa-solid fa-circle-check text-brand-neon"></i>
                                <span>Certificado Oficial de Graduación con Verificación QR.</span>
                            </div>
                        </div>
                    </div>

                    <div class="md:col-span-5 bg-black/60 p-8 rounded-2xl border border-white/10 text-center space-y-6">
                        <div>
                            <span class="text-xs text-gray-400 uppercase font-bold tracking-wider line-through">Precio Regular: S/ 299.00</span>
                            <div class="mt-2">
                                <span class="text-xs text-brand-neon font-black uppercase tracking-wider block">PRECIO PROMOCIONAL (50% OFF)</span>
                                <div class="flex items-baseline justify-center gap-1 mt-1">
                                    <span class="font-heading font-black text-5xl text-white">S/ 149</span>
                                    <span class="text-brand-neon font-bold text-2xl">.50</span>
                                </div>
                                <span class="text-[11px] text-gray-400 block mt-1">Pago único por Yape o Plin</span>
                            </div>
                        </div>

                        <button onclick="openModal()" class="w-full bg-gradient-to-r from-brand-neon to-brand-cyan text-black font-subheading font-black py-4 px-6 rounded-xl uppercase tracking-wider shadow-neon-glow hover:scale-105 transition-transform flex items-center justify-center gap-2 text-base">
                            <i class="fa-solid fa-qrcode"></i>
                            <span>Pagar con Yape Ahora</span>
                        </button>

                        <p class="text-[10px] text-gray-400">
                            <i class="fa-solid fa-lock text-emerald-400"></i> Garantía de Satisfacción. Pago Directo y Seguro.
                        </p>
                    </div>

                </div>
            </div>

        </div>
    </section>

    <!-- FAQ SECTION -->
    <section id="faq" class="py-16 bg-brand-card/30 border-t border-white/5">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 space-y-8">
            <div class="text-center space-y-3">
                <h2 class="font-heading font-black text-3xl sm:text-4xl uppercase">Preguntas Frecuentes</h2>
                <p class="text-gray-400 text-sm">Resuelve todas tus dudas antes de inscribirte.</p>
            </div>

            <div class="space-y-4">
                <details class="glass-card p-5 rounded-2xl border border-white/10 group">
                    <summary class="font-bold text-white cursor-pointer list-none flex justify-between items-center">
                        <span>¿Necesito tener conocimientos previos de dibujo o tatuaje?</span>
                        <i class="fa-solid fa-chevron-down text-brand-neon group-open:rotate-180 transition-transform"></i>
                    </summary>
                    <p class="text-xs text-gray-300 mt-3 leading-relaxed">
                        No. La mentoría está estructurada desde el nivel 0. Te enseñamos el uso de esténcil (calco), el manejo de máquinas rotativas y las técnicas fundamentales paso a paso.
                    </p>
                </details>

                <details class="glass-card p-5 rounded-2xl border border-white/10 group">
                    <summary class="font-bold text-white cursor-pointer list-none flex justify-between items-center">
                        <span>¿Cómo realizo el pago con Yape de S/ 149.50?</span>
                        <i class="fa-solid fa-chevron-down text-brand-neon group-open:rotate-180 transition-transform"></i>
                    </summary>
                    <p class="text-xs text-gray-300 mt-3 leading-relaxed">
                        Haz clic en el botón "Pagar con Yape". Escanea el código QR en pantalla o yapea directamente al número <strong>976 275 695</strong>. Luego envías la captura de pantalla por WhatsApp para la activación instantánea de tu cuenta.
                    </p>
                </details>

                <details class="glass-card p-5 rounded-2xl border border-white/10 group">
                    <summary class="font-bold text-white cursor-pointer list-none flex justify-between items-center">
                        <span>¿El certificado tiene validez para inspecciones sanitarias en Perú?</span>
                        <i class="fa-solid fa-chevron-down text-brand-neon group-open:rotate-180 transition-transform"></i>
                    </summary>
                    <p class="text-xs text-gray-300 mt-3 leading-relaxed">
                        Sí, el módulo de bioseguridad cubre todos los lineamientos exigidos por las directivas del MINSA y municipalidades para el funcionamiento de estudios de tatuaje y perforación corporal.
                    </p>
                </details>
            </div>
        </div>
    </section>

    <!-- YAPE PAYMENT MODAL POPUP -->
    <div id="payment-modal" class="fixed inset-0 z-50 bg-black/90 backdrop-blur-md hidden flex items-center justify-center p-4 opacity-0 transition-opacity duration-300">
        <div class="bg-brand-card border-2 border-brand-purple rounded-3xl max-w-md w-full relative overflow-hidden shadow-purple-glow transform scale-95 transition-transform duration-300" id="modal-content">
            
            <!-- Close Modal Button -->
            <button onclick="closeModal()" class="absolute top-4 right-4 w-9 h-9 flex items-center justify-center rounded-full bg-white/10 hover:bg-white/20 text-gray-300 transition-colors z-20">
                <i class="fa-solid fa-xmark text-lg"></i>
            </button>

            <!-- Yape Header Banner -->
            <div class="bg-brand-purple p-6 text-center relative overflow-hidden">
                <div class="absolute inset-0 bg-white/5"></div>
                <div class="inline-flex items-center gap-2 bg-white/20 px-3 py-1 rounded-full text-white text-xs font-bold uppercase tracking-wider mb-2">
                    <i class="fa-solid fa-bolt text-yellow-300"></i> Activación Inmediata
                </div>
                <h3 class="font-heading font-black text-2xl text-white relative z-10 uppercase">Pago con Yape</h3>
                <p class="text-white/80 text-xs mt-1 relative z-10">Mentoría Mastery Ink Perú (50% OFF)</p>
            </div>

            <!-- Modal Content Body -->
            <div class="p-6 sm:p-8 text-center flex flex-col items-center">
                
                <div class="bg-black/60 rounded-xl px-6 py-3 border border-white/10 mb-6 flex items-center justify-between w-full">
                    <span class="text-xs text-gray-400 font-bold uppercase">Monto Promocional:</span>
                    <span class="font-heading font-black text-3xl text-brand-neon">S/ 149.50</span>
                </div>

                <!-- QR CODE IMAGE DISPLAY -->
                <div class="p-3 bg-white rounded-2xl shadow-2xl mb-4 relative group">
                    <img src="1001564926_2.jpg" alt="QR Yape 976275695" class="w-52 h-52 sm:w-60 sm:h-60 object-cover rounded-xl border border-gray-200" onerror="this.src='1001564926.jpg'">
                </div>

                <div class="space-y-1 mb-6">
                    <span class="text-[11px] text-gray-400 uppercase font-bold tracking-widest block">Número Oficial Yape:</span>
                    <div class="flex items-center justify-center gap-2">
                        <span class="font-heading font-black text-3xl text-white tracking-wider">976 275 695</span>
                        <button onclick="copyYapeNumber()" class="text-xs bg-white/10 hover:bg-white/20 text-brand-neon p-2 rounded-lg transition-colors" title="Copiar Número">
                            <i class="fa-regular fa-copy"></i>
                        </button>
                    </div>
                </div>

                <div class="w-full space-y-3">
                    <p class="text-xs text-gray-300 font-medium">
                        Paso final: Envía la captura de tu Yape por WhatsApp para validar tu acceso con el Mentor:
                    </p>
                    
                    <a id="whatsapp-link" 
                       href="https://wa.me/51958934204?text=Hola!%20Acabo%20de%20realizar%20mi%20Yape%20de%20S/%20149.50%20para%20la%20Mentor%C3%ADa%20de%20Tatuaje%20de%20Mastery%20Ink%20Per%C3%BA.%20Adjunto%20mi%20comprobante." 
                       target="_blank" 
                       class="w-full bg-brand-whatsapp hover:bg-[#20bd5a] text-white font-bold py-4 rounded-xl flex items-center justify-center gap-3 transition-transform hover:scale-105 shadow-lg text-sm uppercase tracking-wider">
                        <i class="fa-brands fa-whatsapp text-2xl"></i>
                        <span>Enviar Comprobante al Mentor (958 934 204)</span>
                    </a>
                </div>

            </div>
        </div>
    </div>

    <!-- FLOATING WHATSAPP MENTOR BUTTON -->
    <a href="https://wa.me/51958934204?text=Hola%20Mentor,%20quisiera%20asistencia%20e%20informaci%C3%B3n%20sobre%20la%20Mentor%C3%ADa%20de%20Tatuaje" 
       target="_blank" 
       class="fixed bottom-6 right-6 z-50 bg-brand-whatsapp hover:bg-[#20bd5a] text-white p-4 rounded-full shadow-2xl flex items-center gap-3 transition-all hover:scale-110 group border-2 border-white/20">
        <i class="fa-brands fa-whatsapp text-3xl"></i>
        <span class="hidden group-hover:inline-block text-xs font-bold font-subheading pr-2 uppercase tracking-wider">Asistencia con Mentor</span>
    </a>

    <!-- FOOTER -->
    <footer class="bg-black border-t border-white/10 py-12 text-center text-xs text-gray-500">
        <div class="max-w-7xl mx-auto px-4 space-y-4">
            <div class="flex items-center justify-center gap-2">
                <i class="fa-solid fa-pen-nib text-brand-neon"></i>
                <span class="font-heading font-extrabold text-white text-sm uppercase">Mastery Ink Perú</span>
            </div>
            <p>© 2026 Mastery Ink Perú. Todos los derechos reservados. Capacitación técnica en arte corporal y normas de bioseguridad sanitaria.</p>
            <p class="text-[10px] text-gray-400 font-semibold">
                <i class="fa-brands fa-whatsapp text-brand-whatsapp"></i> Asistencia Directa con el Mentor WhatsApp: <a href="https://wa.me/51958934204" target="_blank" class="text-brand-neon hover:underline">+51 958 934 204</a>
            </p>
        </div>
    </footer>

    <script>
        const modal = document.getElementById('payment-modal');
        const modalContent = document.getElementById('modal-content');

        function openModal() {
            modal.classList.remove('hidden');
            void modal.offsetWidth; // Reflow
            modal.classList.remove('opacity-0');
            modalContent.classList.remove('scale-95');
            document.body.style.overflow = 'hidden';
        }

        function closeModal() {
            modal.classList.add('opacity-0');
            modalContent.classList.add('scale-95');
            setTimeout(() => {
                modal.classList.add('hidden');
                document.body.style.overflow = 'auto';
            }, 300);
        }

        modal.addEventListener('click', (e) => {
            if (e.target === modal) closeModal();
        });

        function copyYapeNumber() {
            const num = '976275695';
            const tempInput = document.createElement('input');
            tempInput.value = num;
            document.body.appendChild(tempInput);
            tempInput.select();
            document.execCommand('copy');
            document.body.removeChild(tempInput);

            const toast = document.createElement('div');
            toast.className = 'fixed bottom-5 right-5 bg-brand-neon text-black font-bold text-xs px-4 py-3 rounded-xl shadow-2xl z-50';
            toast.innerText = '¡Número 976275695 copiado al portapapeles!';
            document.body.appendChild(toast);
            setTimeout(() => toast.remove(), 2500);
        }

        function startCountdown() {
            let totalSeconds = (2 * 3600) + (34 * 60) + 12;
            const hoursEl = document.getElementById('timer-hours');
            const minutesEl = document.getElementById('timer-minutes');
            const secondsEl = document.getElementById('timer-seconds');

            setInterval(() => {
                if (totalSeconds <= 0) totalSeconds = 3600 * 3;
                totalSeconds--;

                const h = Math.floor(totalSeconds / 3600);
                const m = Math.floor((totalSeconds % 3600) / 60);
                const s = totalSeconds % 60;

                if (hoursEl) hoursEl.innerText = h < 10 ? '0' + h : h;
                if (minutesEl) minutesEl.innerText = m < 10 ? '0' + m : m;
                if (secondsEl) secondsEl.innerText = s < 10 ? '0' + s : s;
            }, 1000);
        }

        let currentStyleFactor = 1.0;

        const tattoosSlider = document.getElementById('tattoos-per-week');
        const priceSlider = document.getElementById('price-per-tattoo');
        
        const tattoosVal = document.getElementById('tattoos-val');
        const priceVal = document.getElementById('price-val');
        
        const monthlyIncomeEl = document.getElementById('monthly-income');
        const paybackTattoosEl = document.getElementById('payback-tattoos');
        const yearlyProfitEl = document.getElementById('yearly-profit');

        function updateCalculator() {
            if (!tattoosSlider || !priceSlider) return;
            
            const tattoos = parseInt(tattoosSlider.value);
            const price = parseInt(priceSlider.value);

            tattoosVal.innerText = `${tattoos} Tatuajes`;
            priceVal.innerText = `S/ ${price}`;

            // Calculation
            const grossMonthly = tattoos * 4 * price * currentStyleFactor;
            const netMonthly = grossMonthly * 0.85; // 15% supplies cost
            const yearlyNet = netMonthly * 12;

            monthlyIncomeEl.innerText = `S/ ${netMonthly.toLocaleString('es-PE', { minimumFractionDigits: 2, maximumFractionDigits: 2 })}`;
            yearlyProfitEl.innerText = `S/ ${yearlyNet.toLocaleString('es-PE', { minimumFractionDigits: 2, maximumFractionDigits: 2 })}`;

            // Mentoría Price S/ 149.50
            const tattoosToPayback = Math.ceil(149.50 / (price * 0.85));
            paybackTattoosEl.innerText = tattoosToPayback <= 1 ? "¡En tu 1er tatuaje!" : `En ${tattoosToPayback} tatuajes`;
        }

        function setStyleFactor(factor, btn) {
            currentStyleFactor = factor;
            document.querySelectorAll('.style-btn').forEach(b => {
                b.className = 'style-btn text-xs py-2 px-3 rounded-xl border border-white/10 bg-white/5 text-gray-300 hover:border-white/30 font-bold';
            });
            btn.className = 'style-btn active text-xs py-2 px-3 rounded-xl border border-brand-neon bg-brand-neon/20 text-brand-neon font-bold';
            updateCalculator();
        }

        if (tattoosSlider) tattoosSlider.addEventListener('input', updateCalculator);
        if (priceSlider) priceSlider.addEventListener('input', updateCalculator);

        function updateCertificateName() {
            const input = document.getElementById('student-name-input');
            const display = document.getElementById('cert-name-display');
            if (input && display && input.value.trim() !== '') {
                display.innerText = input.value.trim();
            }
        }

        function checkQuiz(option, btn) {
            const res = document.getElementById('quiz-result');
            const opts = document.querySelectorAll('.quiz-opt');
            
            opts.forEach(b => b.classList.remove('border-green-500', 'border-red-500', 'bg-green-500/10', 'bg-red-500/10'));

            res.classList.remove('hidden', 'bg-emerald-500/20', 'text-emerald-400', 'bg-red-500/20', 'text-red-400');

            if (option === 2) {
                btn.classList.add('border-green-500', 'bg-green-500/10');
                res.classList.add('bg-emerald-500/20', 'text-emerald-400');
                res.innerHTML = '<i class="fa-solid fa-circle-check"></i> ¡Correcto! La pigmentación en la Dermis Papilar (1-2mm) asegura un tatuaje definido sin migración de tinta.';
            } else {
                btn.classList.add('border-red-500', 'bg-red-500/10');
                res.classList.add('bg-red-500/20', 'text-red-400');
                res.innerHTML = '<i class="fa-solid fa-triangle-exclamation"></i> Incorrecto. En el módulo 1 te enseñamos a calibrar exactamente la profundidad para no causar cicatrices.';
            }
        }

        // On window load initialization
        window.onload = function() {
            startCountdown();
            updateCalculator();
        };
    </script>
</body>
</html>
```
