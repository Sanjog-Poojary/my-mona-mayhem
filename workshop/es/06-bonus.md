<!-- l10n-sync: source-file="workshop/06-bonus.md" -->
# 🎉 Bonus y extensiones

---

¡Has creado una aplicación de GitHub Battle completamente funcional! Ahora es el momento de ir más allá con **desafíos abiertos**.

<!-- track:vscode:start -->
Usa **Agent Mode** para todos ellos: describe lo que quieres y deja que Copilot te ayude a construirlo.
<!-- track:vscode:end -->

<!-- track:cli:start -->
Usa Copilot CLI para todos ellos: combina el contexto con `@file`, `/plan`, el modo normal y `/review` según sea necesario.
<!-- track:cli:end -->

---

## 🏆 Desafío 1: Banner del ganador

Después de que se carguen ambos gráficos de contribuciones, compara los totales y muestra un anuncio dinámico del ganador.

**Qué construir:**
- Compara las contribuciones totales de ambos usuarios.
- Muestra **"🏆 {username} WINS! 🏆"** con un estilo festivo si hay un ganador claro.
- Muestra **"🤝 IT'S A TIE! 🤝"** si las contribuciones son iguales.
- Añade animación o confeti para darle un toque especial.

**Sugerencia de prompt:**
> After both users' contribution data loads, compare total contributions and display a winner banner. Show "🏆 {username} WINS! 🏆" if one user has more contributions, or "🤝 IT'S A TIE! 🤝" if equal. Make it visually exciting with CSS animations.

---

## 🏆 Desafío 2: Contador de racha

Calcula y muestra la racha de contribuciones consecutivas más larga de cada usuario.

**Qué construir:**
- Analiza los datos de contribuciones día a día.
- Encuentra la serie más larga de días consecutivos con al menos una contribución.
- Muestra de forma destacada el número de días de la racha de cada usuario.
- Destaca quién tiene la racha más larga.

**Sugerencia de prompt:**
> Add a streak counter feature that analyzes each user's contribution data to find their longest consecutive contribution streak. Display "🔥 Longest Streak: X days" for each user below their contribution graph.

---

## 🏆 Desafío 3: Historial de batallas

Conserva los resultados de las batallas para que los usuarios puedan ver sus enfrentamientos anteriores.

**Qué construir:**
- Guarda cada resultado de batalla en `localStorage` (nombres de usuario, totales, ganador y marca de tiempo).
- Añade una sección **"Recent Battles"** debajo del área principal de batalla.
- Muestra las últimas 5–10 batallas con sus resultados.
- Añade un botón «Clear History».

**Sugerencia de prompt:**
> Save battle results to localStorage after each comparison. Add a "Recent Battles" section that displays the last 10 battles with usernames, contribution totals, the winner, and when the battle happened. Include a "Clear History" button.

---

## 🏆 Desafío 4: Efectos de sonido

Añade efectos de sonido de arcade retro mediante la Web Audio API, sin necesidad de archivos externos.

**Qué construir:**
- Sonido de **insertar moneda** al hacer clic en el botón «Battle!».
- Sonido de **power up** cuando los resultados se carguen correctamente.
- Sonido de **explosión** cuando se produzca un error (usuario no encontrado o fallo de la API).
- Un botón para activar o silenciar el sonido.

**Sugerencia de prompt:**
> Add retro arcade sound effects using the Web Audio API (no audio files). Play a coin insert sound on battle start, a power-up sound when results load, and an explosion sound on errors. Generate the sounds programmatically with oscillators and gain nodes. Include a mute toggle.

---

## 🏆 Desafío 5: Secuencia de batalla animada

Crea expectación con una cuenta atrás dramática antes de mostrar los resultados.

**Qué construir:**
- Al hacer clic en «Battle!», muestra una superposición a pantalla completa.
- Anima: **«3...»** → **«2...»** → **«1...»** → **«⚡ FIGHT! ⚡»**.
- Después, muestra los gráficos de contribuciones con una entrada espectacular.
- Usa animaciones CSS o temporización con JavaScript.

**Sugerencia de prompt:**
> Add an animated battle sequence when the user clicks "Battle!". Show a countdown overlay: "3..." then "2..." then "1..." then "⚡ FIGHT! ⚡" with each step lasting about 1 second. After the countdown, reveal the results with a slide-in animation.

---

## 🏆 Desafío 6: Leyenda de contribuciones

Añade una leyenda de escala de colores que coincida con la paleta del gráfico de contribuciones.

**Qué construir:**
- Una leyenda horizontal que muestre los niveles de intensidad de las contribuciones.
- Etiquetas desde **«Less»** hasta **«More»**.
- Usa la paleta de colores real de la respuesta de la API de contribuciones.
- Colócala cerca de los gráficos de contribuciones.

**Sugerencia de prompt:**
> Add a contribution legend below the graphs showing the color scale from the API's color palette. Display a row of colored squares ranging from "Less" (lightest) to "More" (darkest), matching the actual contribution level colors returned by the API.

---

## 🏆 Desafío 7: Compartir resultados

Permite que los usuarios compartan sus resultados de batalla con un solo clic.

**Qué construir:**
- Un botón **«📋 Share Results»** que aparezca después de una batalla.
- Copia un resumen de texto con formato en el portapapeles.
- Incluye los nombres de usuario, los totales de contribuciones y el ganador.
- Muestra brevemente un mensaje de confirmación «Copied!».

**Sugerencia de prompt:**
> Add a "📋 Share Results" button that copies a formatted battle summary to the clipboard. The summary should include both usernames, their contribution totals, and who won. Use the Clipboard API and show a brief "Copied to clipboard!" confirmation.

---

<!-- track:cli:start -->
## 💻 Extras del CLI

Si quieres explorar más funcionalidades de Copilot CLI después del taller principal:

- Usa `copilot -p "Write a conventional commit message for the current git diff"` para generar una respuesta única que puedas pegar en Git.
- Ejecuta `/share file` para guardar tu sesión como Markdown y consultarla más adelante.
- Usa `/session` y `/session plan` para inspeccionar cómo CLI sigue tu trabajo actual.
<!-- track:cli:end -->

## 🎊 ¡Enhorabuena!

¡Has completado el taller **Mona Mayhem: GitHub Battle**! Esto es lo que has conseguido:

### Lo que has construido

- ✅ Una **aplicación web completa de varias páginas** a partir de una especificación de diseño.
- ✅ Una **página de inicio** con temática de arcade retro y diseño responsivo.
- ✅ Una **arena de batalla** que obtiene y compara datos reales de contribuciones de GitHub.
- ✅ **Gráficos de contribuciones interactivos** con niveles de actividad codificados por colores.
- ✅ **Manejo de errores, estados de carga y mejoras de accesibilidad**.
- ✅ **Diseño responsivo** que funciona en distintos dispositivos.

### Lo que has practicado

| Habilidad | Qué has practicado |
|---|---|
| **Ingeniería de contexto** | Dar a Copilot los archivos, instrucciones y restricciones adecuados |
| **Planificación** | Generar y refinar planes de implementación antes de programar |
| **Programación agéntica** | Delegar en Copilot trabajo de varios archivos y varios pasos |
| **Iteración de diseño** | Partir de una dirección visual y refinarla hasta obtener un resultado pulido |
| **Disciplina de revisión** | Inspeccionar los cambios generados por IA antes de hacer commit |

### 🚀 Sigue avanzando

- 📺 [Canal de YouTube de VS Code](https://www.youtube.com/@code): consejos, tutoriales y novedades.
- 📖 [Documentación de GitHub Copilot](https://docs.github.com/en/copilot): documentación oficial y guías.
- 💻 [Documentación de GitHub Copilot CLI](https://docs.github.com/en/copilot/how-tos/copilot-cli): instalación, comandos slash y prácticas recomendadas.
- 🌟 [Awesome GitHub Copilot](https://github.com/stefanprodan/awesome-github-copilot): recursos y ejemplos de la comunidad.
- 🛠️ [Talleres de Copilot Dev Days](https://github.com/github/copilot-dev-days): más talleres prácticos como este.

---

## 🙏 ¡Gracias!

¡Gracias por participar en este taller! Has comprobado cómo GitHub Copilot puede acelerar cada fase del desarrollo, desde la planificación y el diseño hasta la implementación y el pulido. Las técnicas que has practicado aquí se aplican a cualquier proyecto, framework y escala. ¡Ahora ve y construye algo increíble! 🚀
