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
