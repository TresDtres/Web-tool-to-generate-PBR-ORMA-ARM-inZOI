# ORMA/ARM Texture Generator for inZOI & Unreal Engine 5 🎨

![License](https://img.shields.io/badge/license-MIT-green) ![Platform](https://img.shields.io/badge/platform-Web-blue)

A free and open-source web tool for generating PBR (Physically Based Rendering) textures optimized for **inZOI** and **Unreal Engine 5.4/5.6**.

This tool allows you to create **ORMA** (Occlusion, Roughness, Metallic, Alpha) and **ARM** packaged maps directly from your browser, without the need to install complex software.

## 🚀 Key Features

- **Procedural Generation**: Creates Ambient Occlusion (AO), Roughness, and Metallic maps from a single base color image.
- **ORMA/ARM Packaging**: Exports textures with the correct channels for UE5 and inZOI:
  - 🔴 **R**: Ambient Occlusion
  - 🟢 **G**: Roughness
  - 🔵 **B**: Metallic
  - ⚪ **A**: Alpha / Height
- **Material Presets**: Ready-to-use configurations: Wool, Silk, Leather, Metal, Plastic, Hair, Skin, etc.
- **Perlin Noise**: Adds realistic imperfections and micro-details to the roughness channel to avoid the "plastic" effect.
- **Normal Maps**: Automatic generation of normal maps with intensity control.
- **🆕 RGB → sRGB Converter**: Converts one image or an entire folder to the sRGB color space (embedded ICC profiles are applied, output is properly tagged as sRGB). Includes a **Non-color data** mode for normal maps, roughness and masks: color profiles are ignored and pixel values pass through bit-exact.
- **🆕 T-Shirt Print Extractor**: Removes a solid black or white background from a design and outputs a PNG with real transparency — perfect for printed clothing and decals. Edge colors are mathematically un-blended (no dark fringes), with options for solid white/black/custom print color and alpha cleanup levels.
- **🆕 Lossless Export**: Packed textures (ORMA/ARM) and extracted prints are encoded straight from raw pixel data, avoiding the canvas premultiplied-alpha corruption that normally damages RGB channels wherever alpha < 255.
- **Real-Time Preview**: See changes instantly as you adjust the sliders.
- **Internationalization**: Automatically translated into multiple languages using Google Translate.
- **100% Client-Side**: Works in your browser. Your images are never uploaded to any server.

## 🛠️ How to Use

1. **Upload your image**: Upload a base texture (Base Color).
2. **Choose a Preset**: Select the material type (e.g., "Fabric: Wool") or adjust the values manually.
3. **Adjust**: Use the sliders to refine the roughness, metallic effect, or noise intensity.
4. **Download**: Download the individual textures, or the ORMA package ready for the game engine.

**For printed t-shirts/decals**: drop your design into the *T-Shirt Print Extractor*, remove the background, and use the resulting PNG as the Base Color of a Masked material (opacity from the alpha channel).

**To batch-convert images to sRGB**: use the *RGB → sRGB Image Converter* — select multiple files or a whole folder; results download as a ZIP preserving the folder structure. Enable *Non-color data* for normal maps and masks.

## 📦 Installation

No installation required. Simply open the `index.html` file in any modern web browser (Chrome/Edge recommended) or host it on GitHub Pages.

## 📄 License

This project is under the MIT License — see the `LICENSE` file for details.

*Created for the inZOI modding community.*

---

# Generador de Texturas ORMA/ARM para inZOI & Unreal Engine 5 🎨

Una herramienta web gratuita y de código abierto para generar texturas PBR (Physically Based Rendering) optimizadas para **inZOI** y **Unreal Engine 5.4/5.6**.

Esta herramienta permite crear mapas empaquetados **ORMA** (Occlusion, Roughness, Metallic, Alpha) y **ARM** directamente desde el navegador, sin necesidad de instalar software complejo.

## 🚀 Características Principales

- **Generación Procedural**: Crea mapas de Oclusión Ambiental (AO), Rugosidad y Metálico a partir de una sola imagen de color base.
- **Empaquetado ORMA/ARM**: Exporta texturas con los canales correctos para UE5 e inZOI:
  - 🔴 **R**: Ambient Occlusion
  - 🟢 **G**: Roughness
  - 🔵 **B**: Metallic
  - ⚪ **A**: Alpha / Height
- **Presets de Materiales**: Configuraciones listas para usar: Lana, Seda, Cuero, Metal, Plástico, Cabello, Piel, etc.
- **Ruido Perlin**: Añade imperfecciones realistas y micro-detalles al canal de rugosidad para evitar el efecto "plástico".
- **Mapas de Normales**: Generación automática de mapas de normales con control de intensidad.
- **🆕 Conversor RGB → sRGB**: Convierte una imagen o una carpeta entera al espacio de color sRGB (se aplican los perfiles ICC incrustados y la salida queda correctamente etiquetada como sRGB). Incluye un modo **Non-color data** para normal maps, roughness y máscaras: se ignoran los perfiles de color y los píxeles pasan intactos, bit a bit.
- **🆕 Extractor de Estampados (T-Shirt Print Extractor)**: Elimina el fondo negro o blanco sólido de un diseño y genera un PNG con transparencia real — perfecto para ropa impresa y decals. El color de los bordes se des-mezcla matemáticamente (sin halos oscuros), con opciones de color de tinta blanco/negro/personalizado y niveles de limpieza del alfa.
- **🆕 Exportación Sin Pérdida**: Las texturas empaquetadas (ORMA/ARM) y los estampados extraídos se codifican directamente desde los datos crudos, evitando la corrupción por alfa premultiplicado del canvas que normalmente daña los canales RGB donde el alfa es menor de 255.
- **Vista Previa en Tiempo Real**: Visualiza los cambios al instante mientras ajustas los sliders.
- **Internacionalización**: Traducido automáticamente a múltiples idiomas mediante Google Translate.
- **100% Cliente**: Funciona en tu navegador. Tus imágenes nunca se suben a ningún servidor.

## 🛠️ Cómo Usar

1. **Carga tu imagen**: Sube una textura base (Base Color).
2. **Elige un Preset**: Selecciona el tipo de material (ej. "Fabric: Wool") o ajusta los valores manualmente.
3. **Ajusta**: Usa los sliders para refinar la rugosidad, el metalizado o la intensidad del ruido.
4. **Descarga**: Baja las texturas individuales, o descarga el paquete ORMA listo para el motor del juego.

**Para camisetas impresas/decals**: arrastra tu diseño al *T-Shirt Print Extractor*, elimina el fondo y usa el PNG resultante como Base Color de un material Masked (opacidad desde el canal alfa).

**Para convertir imágenes a sRGB por lotes**: usa el *Conversor RGB → sRGB* — selecciona varios archivos o una carpeta completa; los resultados se descargan en un ZIP conservando la estructura de carpetas. Activa *Non-color data* para normal maps y máscaras.

## 📦 Instalación

No requiere instalación. Simplemente abre el archivo `index.html` en cualquier navegador web moderno (Chrome/Edge recomendados) o alójalo en GitHub Pages.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT — mira el archivo `LICENSE` para más detalles.

*Creado para la comunidad de modding de inZOI.*
