[index.html](https://github.com/user-attachments/files/34443663/index.html)
<!-- Sección Interactiva: Mensaje del Día / Oráculo -->
    <section style="text-align: center; background: #fff5f7; border: 2px dashed var(--accent); border-radius: 12px; padding: 2rem; margin: 2rem auto;">
        <h2 style="color: var(--primary); border: none;">🔮 Mensaje del Día para tu Alma</h2>
        <p id="textoMensaje" style="font-size: 1.1rem; font-style: italic; color: var(--primary); margin: 1.5rem 0;">
            "Hacé clic en el botón para recibir la energía y el mensaje que necesitás hoy en tu proceso."
        </p>
        <button onclick="mostrarMensaje()" class="btn-green" style="padding: 0.8rem 1.5rem; font-size: 1rem;">Sacar mi Mensaje del Día</button>
    </section>

    <script>
        const mensajesHolisticos = [
            "Flores de Bach: Hoy permitite soltar el control y confiar en tu proceso natural de sanación y armonización interior.",
            "Reiki: Inhala luz dorada y exhala toda tensión acumulada. Tu energía vital se está equilibrando.",
            "Mesa Radiónica: Tu campo energético se está reordenando hacia la vibración de la paz, la claridad y la abundancia.",
            "Esencia de Mimulus: El coraje no es la ausencia de miedo, sino la decisión consciente de avanzar a pesar de él.",
            "Esencia de Walnut: Te protegés de las influencias externas y avanzás firme hacia tu verdadera misión y propósito de vida.",
            "Reiki y Cristales: La vibración de los cristales amplifica tu sanción. Conectá con tu centro de poder."
        ];

        function mostrarMensaje() {
            const aleatorio = Math.floor(Math.random() * mensajesHolisticos.length);
            document.getElementById('textoMensaje').innerText = mensajesHolisticos[aleatorio];
        }
    </script>
[!-- Sección Interactiva Elige tu Ca.txt](https://github.com/user-attachments/files/34443839/--.Seccion.Interactiva.Elige.tu.Ca.txt)
<!-- Sección Interactiva: Elige tu Carta de Tarot ($2.000) -->
    <section style="text-align: center; background: #fff5f7; border: 2px solid var(--accent); border-radius: 12px; padding: 2rem; margin: 2rem auto;">
        <h2 style="color: var(--primary); border: none;">🃏 Oráculo de Tarot Interactivo ($2.000)</h2>
        <p style="color: #4a5568; margin-bottom: 1.5rem;">Elegí una de las 3 cartas ocultas para recibir guía y claridad en tu camino de hoy.</p>
        
        <!-- Cartas para elegir -->
        <div style="display: flex; justify-content: center; gap: 1rem; flex-wrap: wrap; margin-bottom: 1.5rem;">
            <div onclick="elegirCarta(1)" style="background: var(--primary); color: white; padding: 2rem 1.5rem; border-radius: 8px; cursor: pointer; font-weight: bold; font-size: 1.2rem; transition: transform 0.2s; box-shadow: 0 4px 6px rgba(0,0,0,0.1);" onmouseover="this.style.transform='translateY(-5px)'" onmouseout="this.style.transform='translateY(0)'">
                Carta 1 ✨
            </div>
            <div onclick="elegirCarta(2)" style="background: var(--primary); color: white; padding: 2rem 1.5rem; border-radius: 8px; cursor: pointer; font-weight: bold; font-size: 1.2rem; transition: transform 0.2s; box-shadow: 0 4px 6px rgba(0,0,0,0.1);" onmouseover="this.style.transform='translateY(-5px)'" onmouseout="this.style.transform='translateY(0)'">
                Carta 2 🌙
            </div>
            <div onclick="elegirCarta(3)" style="background: var(--primary); color: white; padding: 2rem 1.5rem; border-radius: 8px; cursor: pointer; font-weight: bold; font-size: 1.2rem; transition: transform 0.2s; box-shadow: 0 4px 6px rgba(0,0,0,0.1);" onmouseover="this.style.transform='translateY(-5px)'" onmouseout="this.style.transform='translateY(0)'">
                Carta 3 🔥
            </div>
        </div>

        <!-- Resultado de la carta elegida -->
        <div id="resultadoTarot" style="background: white; padding: 1.5rem; border-radius: 8px; border: 1px dashed var(--accent); display: none; margin-top: 1.5rem;">
            <h3 id="tituloCarta" style="color: var(--primary); margin-top: 0;"></h3>
            <p id="significadoCarta" style="font-style: italic; color: #2d3748; font-size: 1.1rem;"></p>
            <div style="margin-top: 1.2rem;">
                <p><strong>Valor de la lectura: $2.000</strong></p>
                <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Lectura de Tarot ($2.000)</a>
            </div>
        </div>
    </section>

    <script>
        function elegirCarta(numero) {
            const resultados = {
                1: {
                    nombre: "El Mago 🪄 (Carta 1)",
                    significado: "Tenés todo el poder y los recursos internos necesarios para manifestar lo que deseás. Es momento de tomar la iniciativa y confiar en tus talentos."
                },
                2: {
                    nombre: "La Sacerdotisa 🌙 (Carta 2)",
                    significado: "Conectá con tu intuición y tu sabiduría interior. Hay respuestas que ya sabés pero necesitás darte el espacio de silencio para escucharlas."
                },
                3: {
                    nombre: "El Sol ☀️ (Carta 3)",
                    significado: "Vibración de claridad, alegría y éxito renovado. Todo aquello que estaba bloqueado comienza a iluminarse y resolverse con armonía."
                }
            };

            const cartaSeleccionada = resultados[numero];
            document.getElementById('tituloCarta').innerText = cartaSeleccionada.nombre;
            document.getElementById('significadoCarta').innerText = `"${cartaSeleccionada.significado}"`;
            document.getElementById('resultadoTarot').style.display = 'block';
        }
    </script>
<!-- Sección Interactiva: Elige tu Carta de Tarot ($2.000) -->
    <section style="text-align: center; background: #fff5f7; border: 2px solid var(--accent); border-radius: 12px; padding: 2rem; margin: 2rem auto;">
        <h2 style="color: var(--primary); border: none;">🃏 Oráculo de Tarot Interactivo ($2.000)</h2>
        <p style="color: #4a5568; margin-bottom: 1.5rem;">Elegí una de las 3 cartas ocultas para recibir guía y claridad en tu camino de hoy.</p>
        
        <!-- Cartas para elegir -->
        <div style="display: flex; justify-content: center; gap: 1rem; flex-wrap: wrap; margin-bottom: 1.5rem;">
            <div onclick="elegirCarta(1)" style="background: var(--primary); color: white; padding: 2rem 1.5rem; border-radius: 8px; cursor: pointer; font-weight: bold; font-size: 1.2rem; transition: transform 0.2s; box-shadow: 0 4px 6px rgba(0,0,0,0.1);" onmouseover="this.style.transform='translateY(-5px)'" onmouseout="this.style.transform='translateY(0)'">
                Carta 1 ✨
            </div>
            <div onclick="elegirCarta(2)" style="background: var(--primary); color: white; padding: 2rem 1.5rem; border-radius: 8px; cursor: pointer; font-weight: bold; font-size: 1.2rem; transition: transform 0.2s; box-shadow: 0 4px 6px rgba(0,0,0,0.1);" onmouseover="this.style.transform='translateY(-5px)'" onmouseout="this.style.transform='translateY(0)'">
                Carta 2 🌙
            </div>
            <div onclick="elegirCarta(3)" style="background: var(--primary); color: white; padding: 2rem 1.5rem; border-radius: 8px; cursor: pointer; font-weight: bold; font-size: 1.2rem; transition: transform 0.2s; box-shadow: 0 4px 6px rgba(0,0,0,0.1);" onmouseover="this.style.transform='translateY(-5px)'" onmouseout="this.style.transform='translateY(0)'">
                Carta 3 🔥
            </div>
        </div>

        <!-- Resultado de la carta elegida -->
        <div id="resultadoTarot" style="background: white; padding: 1.5rem; border-radius: 8px; border: 1px dashed var(--accent); display: none; margin-top: 1.5rem;">
            <h3 id="tituloCarta" style="color: var(--primary); margin-top: 0;"></h3>
            <p id="significadoCarta" style="font-style: italic; color: #2d3748; font-size: 1.1rem;"></p>
            <div style="margin-top: 1.2rem;">
                <p><strong>Valor de la lectura: $2.000</strong></p>
                <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Lectura de Tarot ($2.000)</a>
            </div>
        </div>
    </section>

    <script>
        function elegirCarta(numero) {
            const resultados = {
                1: {
                    nombre: "El Mago 🪄 (Carta 1)",
                    significado: "Tenés todo el poder y los recursos internos necesarios para manifestar lo que deseás. Es momento de tomar la iniciativa y confiar en tus talentos."
                },
                2: {
                    nombre: "La Sacerdotisa 🌙 (Carta 2)",
                    significado: "Conectá con tu intuición y tu sabiduría interior. Hay respuestas que ya sabés pero necesitás darte el espacio de silencio para escucharlas."
                },
                3: {
                    nombre: "El Sol ☀️ (Carta 3)",
                    significado: "Vibración de claridad, alegría y éxito renovado. Todo aquello que estaba bloqueado comienza a iluminarse y resolverse con armonía."
                }
            };

            const cartaSeleccionada = resultados[numero];
            document.getElementById('tituloCarta').innerText = cartaSeleccionada.nombre;
            document.getElementById('significadoCarta').innerText = `"${cartaSeleccionada.significado}"`;
            document.getElementById('resultadoTarot').style.display = 'block';
        }
    </script>
    
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Viaje de Vida - Terapias Holísticas y Evolución Personal</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,600;1,400&family=Plus+Jakarta+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #581c87;
            --secondary: #9333ea;
            --accent: #f472b6;
            --bg-light: #fef7f9;
            --text-dark: #2d3748;
        }
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-light);
            color: var(--text-dark);
            margin: 0;
            padding: 0;
            line-height: 1.6;
        }
        header {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            text-align: center;
            padding: 4rem 1.5rem;
            border-bottom: 5px solid var(--accent);
        }
        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 2.8rem;
            margin-bottom: 0.5rem;
        }
        header p {
            font-size: 1.2rem;
            opacity: 0.95;
            max-width: 600px;
            margin: 0 auto;
        }
        .container {
            max-width: 1000px;
            margin: 0 auto;
            padding: 2.5rem 1.5rem;
        }
        section {
            background: white;
            border-radius: 16px;
            padding: 2.5rem;
            margin-bottom: 2.5rem;
            box-shadow: 0 10px 25px rgba(88, 28, 135, 0.06);
            border: 1px solid rgba(244, 114, 182, 0.2);
        }
        h2 {
            font-family: 'Playfair Display', serif;
            color: var(--primary);
            font-size: 2rem;
            margin-top: 0;
            text-align: center;
            margin-bottom: 1.5rem;
        }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
        }
        .card {
            background: var(--bg-light);
            border: 1px solid #f3e8ff;
            border-radius: 12px;
            padding: 1.8rem;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 20px rgba(147, 51, 234, 0.12);
        }
        .card h3 {
            color: var(--primary);
            margin-top: 0;
            font-size: 1.4rem;
        }
        .btn-mp {
            display: inline-block;
            background: linear-gradient(135deg, var(--secondary), var(--primary));
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            margin-top: 1.2rem;
            transition: opacity 0.2s;
            box-shadow: 0 4px 10px rgba(147, 51, 234, 0.2);
        }
        .btn-mp:hover {
            opacity: 0.9;
        }
        .tarot-box {
            background: linear-gradient(135deg, #fff1f2, #fdf4f8);
            border: 2px dashed var(--accent);
            text-align: center;
            border-radius: 16px;
            padding: 2.5rem;
        }
        .tarot-options {
            display: flex;
            justify-content: center;
            gap: 1rem;
            flex-wrap: wrap;
            margin: 1.5rem 0;
        }
        .tarot-btn {
            background: var(--primary);
            color: white;
            border: none;
            padding: 1rem 1.5rem;
            border-radius: 10px;
            cursor: pointer;
            font-weight: bold;
            font-size: 1.1rem;
            transition: background 0.2s, transform 0.2s;
        }
        .tarot-btn:hover {
            background: var(--secondary);
            transform: scale(1.05);
        }
        footer {
            text-align: center;
            padding: 2rem;
            color: #6b7280;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <header>
        <h1>Viaje de Vida</h1>
        <p>Terapias Holísticas, Formaciones y Canales de Evolución Personal para armonizar tu energía.</p>
    </header>

    <div class="container">

        <!-- Sección Interactiva: Oráculo de Tarot Interactivo -->
        <section class="tarot-box">
            <h2>🔮 Oráculo de Tarot Interactivo</h2>
            <p style="color: #4b5563; margin-bottom: 1.5rem;">Elegí una de las 3 cartas ocultas para recibir una guía angelical y claridad en tu camino de hoy.</p>
            
            <div class="tarot-options">
                <button class="tarot-btn" onclick="elegirCarta(1)">Carta 1 ✨</button>
                <button class="tarot-btn" onclick="elegirCarta(2)">Carta 2 🌙</button>
                <button class="tarot-btn" onclick="elegirCarta(3)">Carta 3 🔥</button>
            </div>

            <div id="resultadoTarot" style="background: white; padding: 2rem; border-radius: 12px; border: 1px solid #f472b6; display: none; margin-top: 1.5rem; text-align: left;">
                <h3 id="tituloCarta" style="color: var(--primary); margin-top: 0; text-align: center;"></h3>
                <p id="significadoCarta" style="font-style: italic; color: #4b5563; font-size: 1.1rem; text-align: center; line-height: 1.8;"></p>
                <div style="text-align: center; margin-top: 1.5rem; border-top: 1px solid #f3e8ff; padding-top: 1rem;">
                    <p style="margin: 0 0 0.5rem 0; font-weight: 600;">Valor de la lectura interpretativa: $2.000</p>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Abonar Lectura de Tarot ($2.000)</a>
                </div>
            </div>
        </section>

        <!-- Terapias y Sesiones -->
        <section>
            <h2>✨ Terapias y Sesiones Individuales</h2>
            <div class="grid">
                <div class="card">
                    <div>
                        <h3>Flores de Bach</h3>
                        <p>Armonización emocional profunda a través del sistema tradicional de 38 esencias florales.</p>
                    </div>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Sesión</a>
                </div>
                <div class="card">
                    <div>
                        <h3>Reiki y Cristales</h3>
                        <p>Canalización de energía universal y vibración cristalina para restaurar tu paz interior.</p>
                    </div>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Sesión</a>
                </div>
                <div class="card">
                    <div>
                        <h3>Mesas Radiónicas</h3>
                        <p>Limpieza y reestructuración energética cuántica para disolver bloqueos y elevar tu frecuencia.</p>
                    </div>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Pagar Sesión</a>
                </div>
            </div>
        </section>

        <!-- Cursos y Formaciones -->
        <section>
            <h2>📚 Cursos y Formaciones</h2>
            <div class="grid">
                <div class="card">
                    <div>
                        <h3>Reiki Nivel 1</h3>
                        <p>Formación inicial teórico-práctica orientada al despertar y canalización de energía vital.</p>
                    </div>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Inscribirme al Curso</a>
                </div>
                <div class="card">
                    <div>
                        <h3>Terapeuta Floral</h3>
                        <p>Capacitación profesional completa en el sistema internacional de Flores de Bach.</p>
                    </div>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Inscribirme al Curso</a>
                </div>
                <div class="card">
                    <div>
                        <h3>Mesas Radiónicas</h3>
                        <p>Entrenamiento intensivo y especializado para operadoras y operadores del sistema.</p>
                    </div>
                    <a href="https://mpago.la/1kYbut7" target="_blank" class="btn-mp">Inscribirme al Curso</a>
                </div>
            </div>
        </section>

    </div>

    <footer>
        <p>&copy; 2026 Viaje de Vida. Todos los derechos reservados.</p>
    </footer>

    <script>
        function elegirCarta(numero) {
            const resultados = {
                1: {
                    nombre: "El Mago 🪄",
                    significado: "Tenés todo el poder, la capacidad y los recursos internos necesarios para manifestar lo que deseás. Es el momento perfecto para tomar la iniciativa y confiar en tus talentos creadores."
                },
                2: {
                    nombre: "La Sacerdotisa 🌙",
                    significado: "Conectá profundamente con tu intuición y tu sabiduría interior. Hay respuestas que ya habitan en vos; solo necesitás regalarte un espacio de silencio para escucharlas."
                },
                3: {
                    nombre: "El Sol ☀️",
                    significado: "Vibración absoluta de claridad, alegría, vitalidad y éxito renovado. Todo aquello que sentías bloqueado comienza a iluminarse y resolverse con total armonía."
                }
            };

            const cartaSeleccionada = resultados[numero];
            document.getElementById('tituloCarta').innerText = cartaSeleccionada.nombre;
            document.getElementById('significadoCarta').innerText = `"${cartaSeleccionada.significado}"`;
            document.getElementById('resultadoTarot').style.display = 'block';
        }
    </script>
</body>
</html>
