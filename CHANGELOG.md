# Changelog

Todos los cambios notables en este proyecto serán documentados en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/) y este proyecto se adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-10-25

### 🎉 Lanzamiento Oficial

Primera versión pública y abierta de **ARKA Fábrica de Carruseles**, el sistema de ingeniería de prompts y control de calidad visual para crear carruseles hiperrealistas de alto impacto en Instagram, TikTok y YouTube Shorts.

### ✨ Añadido
- **Skill Universal `.agents/skills/arka-carrusel`**:
  - Detección automática de estado: Modo Onboarding (configuración inicial) vs Modo Producción (generación diaria).
  - Capacidad de lectura y extracción de propuesta de valor, catálogo y ofertas desde URL del sitio web de la marca.
  - Generador automatizado de `BRAND_BIBLE.md` y `CATALOGO.md`.
- **Catálogo de 15 Formatos Universales (`references/formatos.md`)**:
  - Formatos probados desde F1 hasta F15 (4 Momentos, Un Día Con, Mito vs Realidad, Guía Paso a Paso, Pregunta Difícil, Comparativa A vs B, Trazabilidad, etc.).
- **Matriz de Layouts Visuales (`references/layouts.md`)**:
  - Cuatro composiciones cinematográficas (A, B, C, D) en formato cuadrado 1080x1080 px para evitar la fatiga visual de plantillas rígidas.
- **Los 4 Candados Anti-Alucinación (`references/candados.md`)**:
  - **Candado de Logo:** Bloqueo de alucinaciones (sin ramas, marcos ni halos blancos; 100 % fiel al PNG oficial).
  - **Candado de Empaque/Producto:** Fidelidad letra por letra en etiquetas, respetando materiales (vidrio, kraft, tela, metal).
  - **Candado de Modelo Consistente:** Soporte para embajadores reales o modelos IA utilizando fotografías multi-ángulo de referencia.
  - **Candado de Idioma y Renderizado:** Renderizado 100 % en español, sin palabras en inglés y sin etiquetas meta en la imagen.
- **Estándar de Copy Móvil (`references/copy-standards.md`)**:
  - Integración nativa de **Negritas Matemáticas Unicode** (`𝟭.`, `𝟮.`, etc.) para evitar el Markdown roto con asteriscos en Instagram y TikTok.
  - Párrafos cortos de 2 líneas con doble espaciado para lectura móvil.
  - Límite de 5 hashtags hiperenfocados para proteger las cuentas de sanciones por spam.
  - Disclaimer ético de IA: `Imágenes ilustrativas creadas con IA.`
- **Protocolo de Auditoría Visual Milimétrica (`references/qa-checklist.md`)**:
  - Lista de verificación obligatoria de 6 puntos de control antes de dar por terminado cualquier contenido.
  - Regla de reintento puntual: regeneración aislada de slides con fallas.
  - Entrega interactiva mediante carrusel deslizable en Markdown.
- **Estructura de Carpetas para el Usuario**:
  - `brand/referencias/logo/`: Logo en PNG transparente.
  - `brand/referencias/productos/`: Fotos reales de productos y empaques.
  - `brand/referencias/modelo/`: Guía para modelos consistentes multi-ángulo.
  - `plan/`: Calendario editorial de 15, 30, 60 o 90 carruseles.
  - `carruseles/`: Directorio de salida organizada con imágenes, prompts y copys listos.
- **Ejemplo Demostrativo Completo (`examples/D01-demo-cafe-origen/`)**:
  - Caso de uso real con `copy.md` listo para publicar y los 5 prompts (`01.md` a `05.md`) completamente formulados.
- **Documentación Completa**:
  - `README.md` estético y detallado con la explicación del principio 50 % IA / 50 % Humano, guía de inicio en 3 pasos y compatibilidad con Google Antigravity y Cursor.
  - Licencia MIT abierta.
