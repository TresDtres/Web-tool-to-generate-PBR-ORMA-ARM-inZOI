# Generador de Texturas ORMA/ARM para inzoi & Unreal Engine 5 🎨

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Platform](https://img.shields.io/badge/platform-Web-orange.svg)

Una herramienta web gratuita y de código abierto para generar texturas PBR (Physically Based Rendering) optimizadas para **inzoi** y **Unreal Engine 5.4/5.6**.

Esta herramienta permite crear mapas empaquetados **ORMA** (Occlusion, Roughness, Metallic, Alpha) y **ARM** directamente desde el navegador, sin necesidad de instalar software complejo.

## 🚀 Características Principales

*   **Generación Procedural:** Crea mapas de Oclusión Ambiental (AO), Rugosidad y Metálico a partir de una sola imagen de color base.
*   **Empaquetado ORMA/ARM:** Exporta texturas con los canales correctos para UE5 e inzoi:
    *   🔴 **R:** Ambient Occlusion
    *   🟢 **G:** Roughness
    *   🔵 **B:** Metallic
    *   ⚪ **A:** Alpha / Height
*   **Presets de Materiales:** Configuraciones listas para usar: Lana, Seda, Cuero, Metal, Plástico, Cabello, etc.
*   **Ruido Perlin:** Añade imperfecciones realistas y micro-detalles al canal de rugosidad para evitar el efecto "plástico".
*   **Mapas de Normales:** Generación automática de mapas de normales con control de intensidad.
*   **Vista Previa en Tiempo Real:** Visualiza los cambios al instante mientras ajustas los sliders.
*   **Internacionalización:** Traducido automáticamente a múltiples idiomas mediante Google Translate.
*   **100% Cliente:** Funciona en tu navegador. Tus imágenes no se suben a ningún servidor.

## 🛠️ Cómo Usar

1.  **Carga tu imagen:** Sube una textura base (Base Color).
2.  **Elige un Preset:** Selecciona el tipo de material (ej. "Fabric: Wool") o ajusta los valores manualmente.
3.  **Ajusta:** Usa los sliders para refinar la rugosidad, el metalizado o la intensidad del ruido.
4.  **Descarga:**
    *   Baja las texturas individuales.
    *   O descarga el paquete **ORMA** listo para el motor del juego.

## 📦 Instalación

No requiere instalación. Simplemente abre el archivo `index.html` en cualquier navegador web moderno o alójalo en GitHub Pages.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - mira el archivo LICENSE para más detalles.

---

*Creado para la comunidad de modding de inzoi.*