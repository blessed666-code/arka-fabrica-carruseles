# Changelog

Todos los cambios notables en este proyecto serán documentados en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/) y este proyecto se adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.1.0] - 2026-11-05

### ✨ Añadido (Mejoras para E-Commerce y Redes Sociales)
- **Candado de Aislamiento de Fondo de Estudio (`references/candados.md`)**:
  - Directiva obligatoria para aislar envases fotografiados sobre fondos negros de estudio (`#000000`) o blancos de recorte, evitando que la IA oscurezca o manche la escena generada.
- **Zona Segura Móvil del 10 % (`references/layouts.md`, `references/candados.md`)**:
  - Margen libre obligatorio en el tercio inferior para evitar que la interfaz nativa de TikTok e Instagram (nombre de usuario, audio, botones de like/comentar) tape el texto renderizado.
- **Estructura de Copy Dual (`references/copy-standards.md`, `references/qa-checklist.md`)**:
  - **Bloque A:** Optimizado para Instagram, TikTok y Shorts con negritas Unicode nativas y llamado a biografía/WhatsApp.
  - **Bloque B:** Optimizado para Facebook Fan Page con enlaces directos y clicables al producto con parámetros UTM completos para medición en Google Analytics 4 (GA4).
- **Protocolo de Doble Variante de Logotipo (`references/candados.md`, `references/layouts.md`)**:
  - Reglas para alternar entre el Logotipo Completo (Slide 1 y 5, 12 % a 15 % del ancho) y el Emblema/Isotipo sutil (Slides 2, 3 y 4, 8 % a 10 % del ancho en esquina).
- **Ficha Morfológica y Cromática en Catálogo (`templates/catalogo.md`)**:
  - Guía detallada para registrar materiales de envase (vidrio, cartón rígido, tubo, gotero), acabado y tipo de dispensador para evitar envases genéricos.
- **Control de Integridad UTF-8 Anti-`U+FFFD` (`references/copy-standards.md`)**:
  - Estandarización de negritas matemáticas Unicode en español evitando caracteres corruptos en vocales tildadas.
- **Guía de Contraste WCAG > 10:1 (`references/layouts.md`)**:
  - Parámetros de contraste tipográfico sobre superficies claras u oscuras.

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
