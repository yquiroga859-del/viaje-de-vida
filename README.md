<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Viaje de Vida - Terapias Holísticas y Evolución Personal</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,600;0,700;1,400&family=Plus+Jakarta+Sans:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #4c1d95; /* Violeta profundo */
            --secondary: #581c87; /* Violeta oscuro */
            --accent: #facc15; /* Amarillo vibrante */
            --bg-light: #fef9c3; /* Fondo amarillo muy suave */
            --card-bg: #ffffff;
            --text-dark: #111827; /* Negro / Gris muy oscuro para lectura */
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.7;
        }

        header {
            background: linear-gradient(135deg, #2e1065, var(--primary), var(--secondary));
            color: white;
            text-align: center;
            padding: 5rem 1.5rem;
            position: relative;
            border-bottom: 4px solid var(--accent);
        }

        .logo-container {
            margin-bottom: 1.5rem;
        }

        .logo-container img {
            width: 130px;
            height: 130px;
            border-radius: 50%;
            object-fit: cover;
            border: 3px solid var(--accent);
            box-shadow: 0 4px 15px rgba(0,0,0,0.25);
            background: white;
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3.2rem;
            margin-bottom: 0.8rem;
            color: #ffffff;
        }

        header p {
            font-size: 1.25rem;
            opacity: 0.95;
            max-width: 700px;
            margin: 0 auto;
            font-weight: 300;
            color: #f3f4f6;
        }

        .container {
            max-width: 1100px;
            margin: -2rem auto 3rem auto;
            padding: 0 1.5rem;
            position: relative;
            z-index: 10;
        }

        section {
            background: var(--card-bg);
            border-radius: 20px;
            padding: 3rem 2.5rem;
            margin-bottom: 2.5rem;
            box-shadow: 0 15px 35px rgba(76, 29, 149, 0.1);
            border: 2px solid #fef08a;
        }

        h2 {
            font-family: 'Playfair Display', serif;
            color: var(--primary);
            font-size: 2.3rem;
            margin-top: 0;
            text-align: center;
            margin-bottom: 2rem;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .card {
            background: #fefce8;
            border: 1px solid #fde047;
            border-radius: 16px;
            padding: 2.2rem;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            transition: all 0.3s ease;
        }

        .card:hover {
            transform: translateY(-8px);
            background: #ffffff;
            box-shadow: 0 15px 30px rgba(76, 29, 149, 0.15);
            border-color: var(--primary);
        }

        .card h3 {
            color: var(--primary);
            margin-top: 0;
            font-size: 1.5rem;
            margin-bottom: 1rem;
            font-family: 'Playfair Display', serif;
        }

        .card p {
            color: #374151;
            font-size: 0.98rem;
            margin-bottom: 1.5rem;
        }

        .price-tag {
            font-size: 1.25rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .btn-mp {
            display: inline-block;
            background: linear-gradient(135deg, var(--secondary), var(--primary));
            color: #ffffff;
            padding: 0.85rem 1.8rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(76, 29, 149, 0.25);
            border: 1px solid #facc15;
        }

        .btn-mp:hover {
            transform: scale(1.04);
            opacity: 0.95;
            background: #3b0764;
        }

        .interactive-box {
            background: linear-gradient(135deg, #fefce8, #fef9c3);
            border: 2px dashed #facc15;
            text-align: center;
            border-radius: 20px;
            padding: 3rem 2rem;
        }

        .tarot-options {
            display: flex;
            justify-content: center;
            gap: 1.2rem;
            flex-wrap: wrap;
            margin: 2rem 0;
        }

        .tarot-btn {
            background: var(--primary);
            color: #ffffff;
            border: none;
            padding: 1.1rem 2rem;
            border-radius: 12px;
            cursor: pointer;
            font-weight: 600;
            font-size: 1.15rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(76, 29, 149, 0.2);
            text-decoration: none;
            display: inline-block;
        }

        .tarot-btn:hover {
            background: var(--secondary);
            transform: translateY(-4px);
            color: var(--accent);
        }

        .elementos-magicos {
            text-align: center;
            font-size: 1.8rem;
            margin: 1.5rem 0;
            letter-spacing: 0.8rem;
        }

        /* Botón Flotante de WhatsApp */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: #25d366;
            color: white;
            border-radius: 50px;
            padding: 12px 22px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.3);
            z-index: 1000;
            display: flex;
            align-items: center;
            gap: 10px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1rem;
            transition: all 0.3s ease;
        }

        .whatsapp-float:hover {
            background-color: #20ba5a;
            transform: scale(1.05);
        }

        footer {
            text-align: center;
            padding: 3rem 1rem;
            color: #1f2937;
            font-size: 0.95rem;
            border-top: 2px solid #fef08a;
            background: #ffffff;
            font-weight: 500;
        }
    </style>
</head>
<body>

    <header>
        <div class="logo-container">
            <img src="https://i.ibb.co/6y18195/logo-viaje-de-vida.png" alt="Logo Viaje de Vida">
        </div>
        <h1>Viaje de Vida</h1>
        <p>Terapias Holísticas, Formaciones y Canales de Evolución Personal para armonizar tu energía y transformar tu realidad.</p>
    </header>

    <div class="container">
        <!-- Elementos Mágicos Decorativos -->
        <div class="elementos-magicos">
            🌸 🔮 ✨ 🌿 🃏 💫
        </div>

        <!-- Mensaje del Día -->
        <section class="interactive-box" style="border-color: var(--primary); background: linear-gradient(135deg, #fefce8, #fef08a);">
            <h2>✨ Mensaje del Día para tu Alma ($2.000)</h2>
            <p style="color: #1f2937; margin-bottom: 1.5rem;">Hacé clic en el botón para abonar tu mensaje sincrónico y recibir la guía exacta que necesitás hoy.</p>
            <div id="textoMensajeContainer" style="font-size: 1.2rem; font-style: italic; color: var(--primary); margin: 1.5rem auto; max-width: 750px; background: white; padding: 2rem; border-radius: 14px; border: 2px solid var(--accent); box-shadow: 0 4px 15px rgba(0,0,0,0.05);">
                "Aboná para revelar tu mensaje sincrónico de hoy."
            </div>
            <a href="https://mpago.la/1kYbut7" target="_blank" class="tarot-btn" style="background: var(--primary);" onclick="mostrarMensaje()">🌟 Abonar y Revelar Mi Mensaje ($2.000)</a>
        </section>

        <!-- Juego Interactivo: El Laberinto de los Chakras ($3.000) -->
        <section class="interactive-box" style="background: linear-gradient(135deg, #fef08a, #fef9c3); border-color: var(--primary);">
            <h2>🎮 Juego Interactivo: El Laberinto de los Chakras ($3.000)</h2>
            <p style="color: #1f2937; margin-bottom: 1.5rem;">Elegí un portal energético para descubrir cuál es el chakra que te pide atención hoy y desbloquear tu bienestar.</p>
            <div class="tarot-options">
                <button class="tarot-btn" onclick="jugarChakras(1)">Portal Raíz 🔴</button>
                <button class="tarot-btn" onclick="jugarChakras(2)">Portal Heart 💚</button>
                <button class="tarot-btn" onclick="jugarChakras(3)">Portal Corona 💜</button>
            </div>
            <div id="resultadoChakras" style="background: white; padding: 2.5rem; border-radius: 14px; border: 2px solid var(--primary); display: none; margin-top: 2rem; text-align: left; box-shadow: 0 10px 30px rgba(0,0,0,0.08);">
                <h3 id="tituloChakra" style="color: var(--primary); margin-top: 0; text-align: center; font-family: 'Playfair Display', serif; font-size: 1.8rem;"></h3>
                <p id="significadoChakra" style="font-style: italic; color: #374151; font-size: 1.15rem; text-align: center; line-height: 1.8; margin-top: 1rem;"></p>
                
                <!-- Pregunta orientada a formaciones con salto a la sección de cursos -->
                <div style="background: #fefce8; border: 1px dashed var(--primary); padding: 1.5rem; border-radius: 12px; margin-top: 2rem; text-align: center;">
                    <p style="color: var(--primary); font-weight: 700; font-size: 1.05rem; margin-bottom: 1rem;">✨ ¿Sentís el llamado de profundizar en este camino y querés ver los cursos y precios disponibles?</p>
                    <div style="display: flex; justify-content: center; gap: 1rem; flex-wrap: wrap;">
                        <a href="#seccion-cursos" class="btn-mp">Ver Cursos y Precios 📚</a>
                    </div>
                </div>

                <div style="text-align: center; margin-top: 2rem; border-top: 1px solid #fef08a; padding-top: 1.5rem;">
                    <p style="margin: 0 0 1rem 0; font-weight: 700; color: var(--primary);">Valor de la partida y calibración energética: $3.000</p>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Abonar para Jugar y Avanzar ($3.000)</a>
                </div>
            </div>
        </section>

        <!-- Rueda de lo que Tenés que Saber Hoy ($5.000) -->
        <section class="interactive-box" style="background: linear-gradient(135deg, #fefce8, #fef08a); border-color: var(--primary);">
            <h2>🎡 La Rueda de lo que Tenés que Saber Hoy</h2>
            <p style="color: #1f2937; margin-bottom: 1.5rem;">Elegí una posición en la rueda energética y descubrí el mensaje clave que debés saber hoy ($5.000).</p>
            <div class="tarot-options">
                <button class="tarot-btn" onclick="girarRueda(1)">Posición 1 🌸</button>
                <button class="tarot-btn" onclick="girarRueda(2)">Posición 2 💫</button>
                <button class="tarot-btn" onclick="girarRueda(3)">Posición 3 🔮</button>
                <button class="tarot-btn" onclick="girarRueda(4)">Posición 4 ✨</button>
            </div>
            <div id="resultadoRueda" style="background: white; padding: 2.5rem; border-radius: 14px; border: 2px solid var(--primary); display: none; margin-top: 2rem; text-align: left; box-shadow: 0 10px 30px rgba(0,0,0,0.08);">
                <h3 id="tituloRueda" style="color: var(--primary); margin-top: 0; text-align: center; font-family: 'Playfair Display', serif; font-size: 1.8rem;"></h3>
                <p id="significadoRueda" style="font-style: italic; color: #374151; font-size: 1.15rem; text-align: center; line-height: 1.8; margin-top: 1rem;"></p>
                <div style="text-align: center; margin-top: 2rem; border-top: 1px solid #fef08a; padding-top: 1.5rem;">
                    <p style="margin: 0 0 1rem 0; font-weight: 700; color: var(--primary);">Valor de la revelación de la Rueda: $5.000</p>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Abonar para Desbloquear ($5.000)</a>
                </div>
            </div>
        </section>

        <!-- Oráculo de Tarot Interactivo ($2.000) -->
        <section class="interactive-box">
            <h2>🃏 Oráculo de Tarot Interactivo ($2.000)</h2>
            <p style="color: #1f2937; margin-bottom: 1.5rem;">Elegí una de las 3 cartas ocultas para recibir guía y claridad inmediata en tu camino.</p>
            <div class="tarot-options">
                <button class="tarot-btn" onclick="elegirCarta(1)">Carta 1 🎴</button>
                <button class="tarot-btn" onclick="elegirCarta(2)">Carta 2 🌙</button>
                <button class="tarot-btn" onclick="elegirCarta(3)">Carta 3 🔥</button>
            </div>
            <div id="resultadoTarot" style="background: white; padding: 2.5rem; border-radius: 14px; border: 2px solid var(--primary); display: none; margin-top: 2rem; text-align: left; box-shadow: 0 10px 30px rgba(0,0,0,0.08);">
                <h3 id="tituloCarta" style="color: var(--primary); margin-top: 0; text-align: center; font-family: 'Playfair Display', serif; font-size: 1.8rem;"></h3>
                <p id="significadoCarta" style="font-style: italic; color: #374151; font-size: 1.15rem; text-align: center; line-height: 1.8; margin-top: 1rem;"></p>
                <div style="text-align: center; margin-top: 2rem; border-top: 1px solid #fef08a; padding-top: 1.5rem;">
                    <p style="margin: 0 0 1rem 0; font-weight: 700; color: var(--primary);">Valor de la lectura interpretativa: $2.000</p>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Abonar Lectura de Tarot ($2.000)</a>
                </div>
            </div>
        </section>

        <!-- Terapias y Sesiones ($15.000 cada una) -->
        <section>
            <h2>🌿 Terapias y Sesiones Individuales</h2>
            <div class="grid">
                <div class="card">
                    <div>
                        <h3>Flores de Bach 🌸</h3>
                        <p>Armonización emocional profunda a través del sistema tradicional de 38 esencias florales.</p>
                    </div>
                    <div>
                        <div class="price-tag">$15.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Sesión</a>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <h3>Reiki y Cristales 💎</h3>
                        <p>Canalización de energía universal y vibración cristalina para restaurar tu paz interior.</p>
                    </div>
                    <div>
                        <div class="price-tag">$15.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Sesión</a>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <h3>Mesas Radiónicas 🔮</h3>
                        <p>Limpieza y reestructuración energética cuántica para disolver bloqueos y elevar tu frecuencia.</p>
                    </div>
                    <div>
                        <div class="price-tag">$15.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Sesión</a>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <h3>Registros Akáshicos 📖</h3>
                        <p>Lectura profunda del alma para recibir guía, respuestas y sanación desde los planos superiores.</p>
                    </div>
                    <div>
                        <div class="price-tag">$15.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Sesión</a>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <h3>Tarot Evolutivo 🎴</h3>
                        <p>Orientación y claridad consciente a través de la sabiduría simbólica de los arcanos.</p>
                    </div>
                    <div>
                        <div class="price-tag">$15.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Sesión</a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Cursos y Formaciones ($60.000 cada uno) -->
        <section id="seccion-cursos">
            <h2>📚 Cursos y Formaciones</h2>
            <div class="grid">
                <div class="card">
                    <div>
                        <h3>Reiki Nivel 1 🕯️</h3>
                        <p>Formación inicial teórico-práctica orientada al despertar y canalización de energía vital.</p>
                    </div>
                    <div>
                        <div class="price-tag">$60.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Inscribirme al Curso</a>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <h3>Reiki Nivel 2 ⚡</h3>
                        <p>Expansión energética con símbolos sagrados y sanación a distancia y emocional.</p>
                    </div>
                    <div>
                        <div class="price-tag">$60.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Inscribirme al Curso</a>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <h3>Reiki Nivel 3 🌟</h3>
                        <p>Maestría interior y activación de la maestría sanadora para la evolución profunda.</p>
                    </div>
                    <div>
                        <div class="price-tag">$60.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Inscribirme al Curso</a>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <h3>Terapeuta Floral 🌸</h3>
                        <p>Capacitación profesional completa en el sistema internacional de Flores de Bach.</p>
                    </div>
                    <div>
                        <div class="price-tag">$60.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Inscribirme al Curso</a>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <h3>Registros Akáshicos 🕊️</h3>
                        <p>Formación para aprender a canalizar y leer los archivos del alma con precisión y guía.</p>
                    </div>
                    <div>
                        <div class="price-tag">$60.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Inscribirme al Curso</a>
                    </div>
                </div>
                <div class="card">
                    <div>
                        <h3>Mesas Radiónicas 💫</h3>
                        <p>Entrenamiento intensivo y especializado para operadoras y operadores del sistema.</p>
                    </div>
                    <div>
                        <div class="price-tag">$60.000</div>
                        <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Inscribirme al Curso</a>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- Botón Flotante de WhatsApp -->
    <a href="https://wa.me/5493541334168?text=Hola%20Yanina,%20quiero%20más%20información%20sobre%20tus%20terapias%20y%20cursos" class="whatsapp-float" target="_blank">
        💬 WhatsApp
    </a>

    <footer>
        <p>&copy; 2026 Viaje de Vida. Todos los derechos reservados.</p>
    </footer>

    <script>
        const mensajesHolisticos = [
            "Flores de Bach: Hoy permitite soltar el control y confiar en tu proceso natural de sanación y armonización interior.",
            "Reiki: Inhala luz dorada y exhala toda tensión acumulada. Tu energía vital se está equilibrando.",
            "Mesa Radiónica: Tu campo energético se está reordenando hacia la vibración de la paz, la claridad y la abundancia.",
            "Esencia de Mimulus: El coraje no es la ausencia de miedo, sino la decisión consciente de avanzar a pesar de él.",
            "Esencia de Walnut: Te protegés de las influencias externas y avanzás firme hacia tu verdadera misión y propósito de vida.",
            "Reiki y Cristales: La vibración de los cristales amplifica tu sanación. Conectá con tu centro de poder."
        ];

        function mostrarMensaje() {
            const aleatorio = Math.floor(Math.random() * mensajesHolisticos.length);
            document.getElementById('textoMensajeContainer').innerText = `"${mensajesHolisticos[aleatorio]}"`;
        }

        function jugarChakras(numero) {
            const chakras = {
                1: { nombre: "Chakra Raíz (Muladhara) 🔴", significado: "Elegiste el portal de la tierra y la estabilidad. Tu desafío actual es afianzar tu seguridad, soltar el miedo al futuro y conectar fuertemente con el presente." },
                2: { nombre: "Chakra del Corazón (Anahata) 💚", significado: "Elegiste el portal del amor incondicional y la compasión. El juego te revela que es el momento perfecto para perdonar, abrir tu sentir y darte el afecto que mereces." },
                3: { nombre: "Chakra Corona (Sahasrara) 💜", significado: "Elegiste el portal de la conexión espiritual superior. Tu energía se eleva para recibir inspiración pura, guía divina y claridad absoluta en tu camino." }
            };
            const seleccionado = chakras[numero];
            document.getElementById('tituloChakra').innerText = seleccionado.nombre;
            document.getElementById('significadoChakra').innerText = `"${seleccionado.significado}"`;
            document.getElementById('resultadoChakras').style.display = 'block';
        }

        function girarRueda(numero) {
            const revelacionesRueda = {
                1: { nombre: "Ciclo de Crecimiento y Apertura 🌸", significado: "La energía de la rueda marca que estás entrando en un periodo de expansión donde tus proyectos florecen. Es momento de soltar las dudas y dar el paso con confianza absoluta." },
                2: { nombre: "Sanación y Reordenamiento Interno 💫", significado: "El mensaje central de hoy te invita a priorizar tu paz mental. Lo que parecía un obstáculo externo es en realidad una invitación a habitar tu centro con más amor propio." },
                3: { nombre: "Sincronía y Propósito 🔮", significado: "Estás alineada con las respuestas correctas. Las señales que venías pidiendo se manifiestan hoy de forma clara; prestá atención a tus intuiciones y corazonadas." },
                4: { nombre: "Renovación Energética Total ✨", significado: "Se disuelven cargas del pasado que ya no te pertenecen. La rueda gira a tu favor, trayendo una brisa de aire fresco, vitalidad y nuevas oportunidades a tu vida." }
            };
            const itemElegido = revelacionesRueda[numero];
            document.getElementById('tituloRueda').innerText = itemElegido.nombre;
            document.getElementById('significadoRueda').innerText = `"${itemElegido.significado}"`;
            document.getElementById('resultadoRueda').style.display = 'block';
        }

        function elegirCarta(numero) {
            const resultados = {
                1: { nombre: "El Mago 🪄", significado: "Tenés todo el poder, la capacidad y los recursos internos necesarios para manifestar lo que deseás. Es el momento perfecto para tomar la iniciativa y confiar en tus talentos creadores." },
                2: { nombre: "La Sacerdotisa 🌙", significado: "Conectá profundamente con tu intuición y tu sabiduría interior. Hay respuestas que ya habitan en vos; solo necesitás regalarte un espacio de silencio para escucharlas." },
                3: { nombre: "El Sol ☀️", significado: "Vibración absoluta de claridad, alegría, vitalidad y éxito renovado. Todo aquello que sentías bloqueado comienza a iluminarse y resolverse con total armonía." }
            };
            const cartaSeleccionada = resultados[numero];
            document.getElementById('tituloCarta').innerText = cartaSeleccionada.nombre;
            document.getElementById('significadoCarta').innerText = `"${cartaSeleccionada.significado}"`;
            document.getElementById('resultadoTarot').style.display = 'block';
        }
    </script>
</body>
</html>
