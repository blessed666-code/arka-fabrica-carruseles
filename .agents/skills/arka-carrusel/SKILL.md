---
name: arka-carrusel
description: Fábrica universal de carruseles y posts de alto impacto para Instagram, TikTok y YouTube Shorts desarrollada por ARKA. Diseña planes editoriales (15 a 90 contenidos), audita referencias reales (logos, productos y modelos), genera prompts hiperrealistas con candados anti-alucinación, inspecciona visualmente cada imagen con control de calidad milimétrico y redacta copy listo para publicar con negritas Unicode y llamadas a la acción directas.
---

# ARKA Fábrica de Carruseles · Skill Universal

Motor de creación de contenido visual y persuasivo para marcas, productos y servicios en **Instagram, TikTok y YouTube Shorts**. Diseñado para operar de forma nativa en **Google Antigravity** o **Cursor** utilizando modelos de generación de imagen por llamada de herramientas como **Nano Banana 2** (`gemini-3.1-flash-image` / `GenerateImage`).

Desarrollado y compartido abiertamente por **Danniel Mena / ARKA** ([arkadigital.co](https://arkadigital.co) · GitHub: [blessed666-code](https://github.com/blessed666-code)).

---

## ⚡ Filosofía del Sistema (50% Automatizado / 50% Humano)

Este sistema automatiza el **50% más técnico y exigente** del trabajo:
1. Extracción estratégica del contexto de la marca (desde URL o cuestionario).
2. Estructuración del calendario editorial con 15 formatos probados (F1 a F15).
3. Redacción de prompts fotorrealistas con candados estrictos para empaque, logo y modelo.
4. Generación de imágenes en proporción 1:1 con lentes ópticos y luz cinematográfica.
5. Control de calidad visual milimétrico (auditoría obligatoria antes de entregar).
6. Copy optimizado para móviles (sin asteriscos de Markdown, con negritas Unicode).

El **50% humano** restante consiste en:
- Aprobación final del contenido generado.
- Programación y subida a las plataformas sociales.
- Atención a las ventas y mensajes de clientes que llegan por WhatsApp o DM.

---

## 🚦 Regla de Oro: Prohibido decir "Listo" antes de Auditar

El agente **NUNCA** presenta un carrusel o post como terminado sin antes haber abierto e inspeccionado visualmente cada imagen generada con su herramienta de lectura de imágenes. Si alguna slide presenta:
- Ramas, marcos, subrayados o halos inventados en el logo.
- Empaques deformados o convertidos en cajas/latas genéricas.
- Rostros de cera plástica o manos con más o menos de 5 dedos.
- Palabras en inglés o errores ortográficos en el texto renderizado.

El agente tiene la orden estricta de **regenerar únicamente la slide con error** aplicando un prompt correctivo antes de notificar al usuario.

---

## 🔄 Los Dos Modos de Operación

Al activarse, la skill evalúa si la marca ya está configurada revisando si existen `brand/BRAND_BIBLE.md` y archivos dentro de `brand/referencias/`:

### MODO 1: Onboarding y Configuración de Marca (Primera vez)
Si la marca no ha sido configurada o el usuario dice *"configurar marca"*, *"iniciar"*, *"nueva marca"* o pasa una URL:
1. **Inspección Web:** Si el usuario tiene sitio web (ej. `https://mi-tienda.com`), lee el sitio para extraer catálogo, propuestas de valor, ofertas/combos, precios y tono de voz.
2. **Recepción de Fotos de Referencia:**
   - Logo oficial: `brand/referencias/logo/logo.png` (PNG transparente).
   - Fotos de productos: `brand/referencias/productos/` (fotos de frente, etiqueta legible, materiales reales).
   - Modelo (opcional): `brand/referencias/modelo/` (fotos multi-ángulo de persona real o modelo IA).
3. **Formato Preferido:** Pregunta si desea carruseles de 5 slides o posts individuales de 1 slide.
4. **Volumen de Contenido:** Pregunta cuántos contenidos planear (15, 30, 60 o 90 piezas).
5. **Generación de Archivos:** Compila `brand/BRAND_BIBLE.md`, `brand/CATALOGO.md` y `plan/PLAN-EDITORIAL.md`.

### MODO 2: Producción de Contenido (Día a día)
Cuando el usuario pide un contenido (ej. *"haz el D01"*, *"siguiente carrusel"*, *"ejecuta el D05"*):
1. Lee la ficha del contenido en `plan/PLAN-EDITORIAL.md`.
2. Lee `brand/BRAND_BIBLE.md` y `brand/CATALOGO.md`.
3. Audita las referencias visuales correspondientes en `brand/referencias/`.
4. Crea la carpeta `carruseles/DNN-slug/` y redacta:
   - `copy.md`: caption con negritas Unicode, doble espacio y CTA a WhatsApp/Bio.
   - `prompts/01.md` ... `05.md`: prompts independientes con sus candados.
5. Genera las imágenes en 1:1 (`01.jpg` a `05.jpg`) pasando las referencias exactas.
6. Ejecuta la auditoría visual milimétrica. Si hay error, regenera la slide fallida.
7. Presenta el informe con el componente interactivo de carrusel en Markdown.

---

## 🎯 Canales Objetivos y Formato de Copy

Este sistema está diseñado exclusivamente para **Instagram, TikTok y YouTube Shorts**.
- **Cero asteriscos (`*` o `**`):** Las aplicaciones sociales no renderizan Markdown, mostrando asteriscos rotos y antiestéticos.
- **Negritas Matemáticas Unicode:** Se usan caracteres nativos legibles en cualquier celular:
  - `𝟭.`, `𝟮.`, `𝟯.` para listas numeradas.
  - `𝗧𝗶́𝘁𝘂𝗹𝗼 𝗱𝗲 𝗘𝗷𝗲𝗺𝗽𝗹𝗼:` para encabezados.
- **Doble espaciado:** Párrafos de 1 a 2 oraciones con salto de línea doble para lectura ágil en móviles.
- **Máximo 5 hashtags:** Hiperenfocados en el nicho y producto para evitar penalizaciones por spam.
- **Disclaimer obligatorio:** `Imágenes ilustrativas creadas con IA.`

---

## 👤 Módulo de Modelo Consistente (Persona Real o Modelo IA)

Si la marca desea que una persona o personaje recurrente protagonice las publicaciones:
1. **Requisito estricto de referencias:** Se deben incluir fotos nítidas en `brand/referencias/modelo/`:
   - Rostro de frente mirando a cámara con buena luz.
   - Rostro en ángulo de 3/4 izquierdo y derecho.
   - Perfil lateral.
   - Cuerpo entero (si las escenas requieren planos generales).
2. **Uso en Prompts:** Se pasa la imagen de referencia como ancla de identidad (`Imagen X = ancla_rostro.jpg`) con la directiva:
   *«Reproducir con absoluta fidelidad los rasgos faciales, tono de piel, contextura, peinado y edad del modelo de la Imagen X. Prohibido alterar la identidad o deformar la anatomía»*.
