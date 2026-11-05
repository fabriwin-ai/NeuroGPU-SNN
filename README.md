# Ω Sensory · NeuroGPU-SNN 🧠⚡

An open-source, bare-metal framework designed for real-time Self-Organizing Neural Networks (SNN/SOM) and digital twin patient modeling (MDP). Powered entirely on the edge via WebGPU and WGSL to process neuro-acoustic, bio-synaptic, and bioengineering signals with absolute autonomy.

[![License: GPL v3](https://shields.io)](https://gnu.org)
[![Framework: WebGPU](https://shields.io)](https://github.io)
[![Field: Bioengineering](https://shields.io)](https://github.com/fabriwin-ai/NeuroGPU-SNN)

---

## 🔬 El Paradigma: Conexión Sináptica Local

**NeuroGPU-SNN** rompe la dependencia de la nube y los modelos comerciales controlados por las corporaciones tecnológicas. Al mapear y procesar dinámicas celulares y neuronales directamente sobre el silicio local, esta plataforma permite simular, filtrar y corregir bio-señales en tiempo real sin intermediarios industriales.

### Características Clave
* **Red autoorganizada escalable:** Perfiles de `P1 (32)` a `P9 (50,000)` neuronas, con reducción automática del perfil si el rendimiento cae.
* **Tres modos visuales:** rejilla 2.5D, bandas con actividad neuronal y avatar holográfico texturizado, anclado al centro de actividad del campo NN sin rotación orbital. El render WebGL aplica bloom de varias pasadas y antialias FXAA. En el modo avatar, nodos locales perciben actividad, bandas, fase y distribución espacial de la red; seis niveles de profundidad NN desplazan el avatar en Z. Efectos XZ enmascarados mantienen la altura Y, con ondas al caminar/correr, flujo y ruido sutiles y aparición progresiva por un campo lineal Z. El avatar responde con acciones automáticas (caminar, correr, escuchar, pensar, señalar, descansar y más).
* **Mecánica Neurobiológica Nativa:** Implementación matemática integrada de **Inhibición Lateral**, sistemas de aprendizaje cooperativo y la cascada de error/energía `ω → ε`.
* **Procesamiento de Atención Modular (NN LOD):** Niveles de detalle computacional que van desde predicciones y gradientes básicos (LOD 1) hasta optimizaciones iterativas críticas de alta densidad (LOD 3).

---

## 🛠️ Arquitectura del Sistema

El núcleo del shader emula el comportamiento de una cóclea biológica y redes neuronales *Spiking* de disparo temporal:

## Publicar en GitHub Pages

La aplicación se publica desde `index.html` en la raíz del repositorio. En **Settings → Pages → Build and deployment**, selecciona **Deploy from a branch**, la rama `main` y la carpeta `/(root)`. El archivo fuente original también está disponible como `Ω Sensory Shader — NN autoorganizada - Latest 0.1.html`.
