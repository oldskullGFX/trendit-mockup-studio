# Trendit Mockup Studio

**El estudio de diseño para estampado, todo en un solo programa.**
Crea mockups realistas, prepara archivos DTF, quita fondos con IA, separa colores para serigrafía y diseña playeras con plantillas profesionales, sin necesidad de saber Photoshop o Illustrator.

[⬇ Descargar la última versión](https://github.com/oldskullGFX/trendit-mockup-studio/releases/latest) · Windows 10/11 (64 bits) · Gratis

Instagram: [@trenditlab](https://www.instagram.com/trenditlab/) · [@holyshirtux](https://www.instagram.com/holyshirtux/)

---

## ¿Qué es?

Trendit Mockup Studio es un programa de escritorio para personas y negocios que **diseñan, imprimen y venden ropa personalizada**: playeras, sudaderas y demás prendas.
Reúne en una sola ventana las herramientas que normalmente necesitarías buscar en varios programas, páginas web o suscripciones de pago. Cada una te guía con pasos claros.

## ¿Cómo ayuda a los diseñadores emergentes?

Empezar un negocio de estampado suele implicar pagar programas caros, aprender a usarlos y perder tiempo en tareas repetitivas. Este programa busca quitar esas barreras:

- **Sin curva de aprendizaje.** Cada herramienta muestra qué hacer en tres pasos y trae valores recomendados. Hay opciones avanzadas para quien quiera más control.
- **Vende antes de imprimir.** Con los mockups realistas muestras tus diseños puestos en la prenda y publicas en redes en los formatos de Instagram, sin tomar fotos ni producir muestras.
- **Archivos listos para el taller.** Prepara diseños a la medida exacta en centímetros y a 300 DPI, con bordes limpios para DTF. También genera positivos para serigrafía y plantillas de corte para pedrería y vinil, así se evitan errores y desperdicio de material.
- **Calcula antes de cobrar.** La guía de medidas acomoda tus diseños a tamaño real sobre la prenda y calcula cuánta película DTF usas y cuánto cuesta.
- **Diseña aunque no seas diseñador.** Más de 50 plantillas editables, hechas con acabado profesional, para playeras, parejas, música y artistas, redes sociales, catálogos y hojas de pedido.
- **Privado y sin internet.** Tus diseños se procesan en tu computadora y no se suben a ningún servidor.
- **Siempre al día.** El programa se actualiza solo con funciones nuevas.

## Funciones

### 👕 Mockups
- **Mockup realista:** coloca tu diseño en playeras y sudaderas reales y cambia el color de la prenda. Respeta las arrugas y la luz de la tela. Exporta en formatos para Instagram (1:1, 4:5, historia).
- **Mockups automáticos:** genera de una vez tu diseño en varias prendas y colores, y descárgalos en un ZIP.
- **Mis plantillas:** usa fotos de tus propias prendas como mockup.
- **Frente y espalda:** divide un diseño que une frente y espalda y míralo puesto en la prenda.

### 🖨️ Preparar para imprimir
- **Archivos DTF:** medida exacta en cm, 300 DPI, limpieza de bordes semitransparentes y revisión de calidad de impresión.
- **Quitar fondo con IA:** fondo automático, selección de objeto con un clic, varita mágica, pincel y **borrar un color en toda la imagen**.
- **Reescalar con IA (Real-ESRGAN):** agranda imágenes pequeñas ×2, ×3 o ×4 para que se impriman nítidas.
- **Mejorar imagen:** corrección automática de luz, color y nitidez.
- **Girar y recortar**, **recorte en forma** (círculo, corazón, estrella, hexágono, insignia) y **conversor de archivos** (PNG, JPG, WEBP, ICO).

### ✨ Efectos
- **Semitonos sin semitransparencias**, incluido el modo para borrar un color con puntos.
- **Umbral**, **viñetas**, **marcos**, **texturas vintage**, **cambio de color**.
- **Contorno y sticker**, con línea de corte para plotter, Cricut o Silhouette.
- **Sombras y brillo** (sombra, neón y sombra larga).
- **Duotono y degradado**, **glitch y retro**, **pixel art**.

### 💎 Especiales
- **Separación de colores para serigrafía:** un positivo por tinta, base blanca para prenda oscura, marcas de registro y descarga en ZIP.
- **Pedrería** y **pedrería sobre DTF:** con conteo de piedras y plantilla de corte.
- **Vinil reflectante:** vista con y sin flash, capa de corte y capa DTF.

### 🅰️ Diseño
- **Editor de plantillas por capas:** textos con degradado, doble contorno y efecto 3D; texto curvo; fotos en círculo o corazón; formas, íconos y tablas. Exporta PNG, JPG o PDF.
- **Plantillas:** playeras (universitario, jersey, retro, Y2K, groovy, graffiti…), parejas («Only You», «Nuestra canción»…), música y artistas (reproductor con letra, estilo bootleg, gira, boleto de concierto), redes sociales, catálogos y hojas de pedido.
- **Guía de medidas:** acomoda los diseños a tamaño real sobre el plano de la prenda y calcula el costo de DTF.
- **Paleta de colores** (códigos HEX), **patrón repetido** para sublimación y **vectorizar a SVG**.

## ¿Cómo está hecho?

- **Aplicación de escritorio con Electron.** La interfaz está hecha con HTML, CSS y JavaScript propios, sin frameworks, para que sea ligera y rápida.
- **Procesamiento de imagen con Canvas**, a nivel de píxel: semitonos, separaciones, contornos (transformada de distancia), sombras y más. La vista previa trabaja a menor resolución para responder al instante, y la descarga se genera a resolución completa.
- **Inteligencia artificial local**, ejecutada en tu propio equipo:
  - Selección de objetos con un modelo tipo SAM (transformers.js).
  - Quitar fondo automático con @imgly/background-removal.
  - Reescalado con Real-ESRGAN en ONNX Runtime, usando la tarjeta gráfica (WebGPU) o varios núcleos del procesador. El programa elige solo lo más rápido para tu equipo.
  - Algunos modelos se descargan una sola vez, la primera vez que los usas.
- **Vectorización** con ImageTracer (dominio público).
- **Actualizaciones automáticas** con electron-updater desde las publicaciones de este repositorio.
- Tus plantillas y diseños guardados se almacenan en tu computadora.

## Instalación

1. Descarga `Trendit-Mockup-Studio-Setup-X.Y.Z.exe` desde [Releases](https://github.com/oldskullGFX/trendit-mockup-studio/releases/latest) y ábrelo.
2. Si Windows muestra un aviso de SmartScreen, haz clic en **Más información → Ejecutar de todas formas**. El programa todavía no está firmado digitalmente.
3. ¿No quieres instalar? Usa `Trendit-Mockup-Studio-Portable-X.Y.Z.exe`. La versión portable no se actualiza sola.

Tus descargas se guardan en **Descargas › Trendit Mockup Studio**.

---

Hecho por **Trendit Lab** para la comunidad de diseño y estampado.
