# Ω Sensory · NeuroGPU-SNN

An experimental, standalone browser visualization of a self-organizing neural field. The page processes microphone, audio/video-file, or synthetic demo input locally in the browser and renders the network with JavaScript and WebGL. It does not require a server or external runtime dependencies.

[![License: GPL v3](https://img.shields.io/badge/license-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.html)
[![Rendering: WebGL](https://img.shields.io/badge/rendering-WebGL-990000.svg)](https://developer.mozilla.org/docs/Web/API/WebGL_API)

---

## 🔬 El Paradigma: Conexión Sináptica Local

**NeuroGPU-SNN** ejecuta su demostración y visualización localmente en el navegador; no envía las entradas de audio a un servicio remoto. Es un prototipo experimental, no una herramienta clínica ni un modelo validado para el diagnóstico o tratamiento de pacientes.

### Características Clave
* **Red autoorganizada escalable:** Perfiles de `P1 (32)` a `P9 (50,000)` neuronas, con reducción automática del perfil si el rendimiento cae.
* **Visualización neural y holográfica:** rejilla cúbica 3D con perspectiva y giro continuo, bandas con actividad, avatar neural y dos salidas para ilusiones Pepper's Ghost: una figura central para una pantalla tipo vitrina y cuatro figuras orientadas en cruz para una pirámide DIY de cuatro caras. El avatar tiene una superficie texturizada continua, responde al campo y se adapta a la pantalla; la proyección holográfica permite ajustar giro, espejo y tamaño, y usar pantalla completa sobre fondo negro.
* **Dinámica de red experimental:** incluye inhibición lateral, aprendizaje cooperativo y una cascada de error/energía `ω → ε`.
* **Perfiles y rendimiento:** selecciona de 32 a 50 000 neuronas; los perfiles altos pueden reducirse automáticamente si la tasa de fotogramas cae.
* **Controles de red:** ajusta la mezcla de bandas y los controles disponibles en la interfaz; guarda, exporta e importa topologías desde el navegador.

---

## 🛠️ Arquitectura del Sistema

La aplicación está contenida en un único documento HTML. JavaScript procesa la entrada y actualiza la red; shaders WebGL dibujan el fondo, las conexiones y las neuronas, y aplican los efectos visuales. La entrada de micrófono usa la API de audio del navegador y requiere permiso del usuario.

## Usar la aplicación

1. Abre [`index.html`](./index.html) en un navegador compatible con WebGL, o habilita GitHub Pages para publicar el documento.
2. Elige **Demo** para generar una señal sintética, **Archivos** para cargar audio o video, o **Micrófono** y concede permiso para capturar audio.
3. Selecciona un perfil de neuronas y una vista: rejilla cúbica 3D, bandas con actividad, avatar en el campo, holograma central o pirámide DIY de cuatro caras.

La captura de micrófono normalmente requiere un contexto seguro (`https://` o `localhost`). El acceso a dispositivos y el rendimiento dependen del navegador y del equipo.

### Proyección holográfica DIY

Para una pirámide reflectante de cuatro lados, selecciona **Holograma: pirámide DIY · 4 caras**, coloca la pirámide transparente centrada sobre la pantalla, ajusta giro/espejo/tamaño y activa pantalla completa. Una pantalla con brillo alto y la habitación oscura mejoran el reflejo. Para una vitrina o pantalla holográfica de una sola vista, selecciona **Holograma: vista central (AVA)**. Estas opciones generan una ilusión óptica 2D tipo Pepper's Ghost; no son hologramas volumétricos reales y el resultado depende de la geometría del reflector.

## Publicar en GitHub Pages

La aplicación se publica desde `index.html` en la raíz del repositorio. En **Settings → Pages → Build and deployment**, selecciona **Deploy from a branch**, la rama `main` y la carpeta `/(root)`. El archivo fuente original también está disponible como [`Ω Sensory Shader — NN autoorganizada - Latest 0.1.html`](./Ω%20Sensory%20Shader%20—%20NN%20autoorganizada%20-%20Latest%200.1.html).
