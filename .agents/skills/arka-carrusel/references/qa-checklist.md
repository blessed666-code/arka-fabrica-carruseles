# Protocolo de Auditoría Visual Milimétrica y de Copy (Filtro de Seguridad ARKA)

En la Fábrica de Carruseles de ARKA está **estrictamente prohibido afirmar que un carrusel está terminado** sin haber abierto y auditado cada una de las imágenes generadas y los dos bloques de copy.

---

## 🔍 Checklist de Inspección Visual (Slide por Slide)

El agente debe abrir cada archivo `01.jpg` a `05.jpg` y contrastarlo contra estos 8 puntos de control:

| Punto de Control | Pregunta de Verificación | Criterio de Aprobación |
|---|---|---|
| **1. Logo Oficial (Variante Correcta)** | ¿Aplica la variante correspondiente? | ✅ Slide 1 y 5: Logotipo Completo (12%-15% ancho). Slides 2, 3 y 4: Emblema/Isotipo sutil (8%-10% ancho). Cero recuadros negros, ramas, hojas añadidas o halos blancos de sticker. |
| **2. Empaque / Producto** | ¿Es idéntico a las fotos reales de referencia? | ✅ Material real (vidrio, cartón rígido, tubo, gotero), colores corporativos y textos fieles sin deformaciones ni envases genéricos de stock. |
| **3. Aislamiento de Fondo de Estudio** | ¿Aisló el producto de su foto original? | ✅ Si la foto de referencia venía con fondo negro o blanco de estudio, la escena final debe situarlo naturalmente sobre la encimera/tocador bajo luz natural sin manchones oscuros. |
| **4. Zona Segura Móvil (Safe Zone)** | ¿El texto respeta el tercio inferior? | ✅ Margen inferior libre del 10 % en el borde de abajo. Ningún título ni botón queda tapado por la interfaz nativa de TikTok o Instagram. |
| **5. Contraste de Texto** | ¿El ratio de contraste supera 10:1? | ✅ Texto nítido y legible al primer golpe de vista sobre la superficie, sin zonas quemadas ni fondos confusos. |
| **6. Anatomía Humana** | ¿Los personajes lucen naturales y proporcionados? | ✅ Manos con exactamente 5 dedos anatómicos. Rostros con expresión relajada y textura de piel real con poros visibles (cero plástico o cera). |
| **7. Modelo Ancla** | ¿Mantiene la identidad de la persona de referencia? | ✅ Mismas facciones, tono de piel, contextura y edad del archivo de modelo de referencia en todas las slides. |
| **8. Ortografía y Cero Guiones Largos** | ¿La tipografía es impecable en español? | ✅ 100 % en español con tildes correctas. Cero palabras meta como "Título", "Kicker" o "CIERRE". Cero comillas o guiones largos ("—" o "–"). |

---

## 📝 Checklist del Archivo `copy.md` (Copy Dual)

- [ ] **Bloque A (Instagram / TikTok / Shorts):**
  - Negritas Matemáticas Unicode nativas (`𝟭.`, `𝟮.`, `𝗧𝗶́𝘁𝘂𝗹𝗼:`).
  - Cero asteriscos rotos de Markdown (`**texto**`).
  - Cero caracteres corruptos de codificación (`U+FFFD`).
  - Doble salto de línea entre párrafos para lectura móvil ágil.
  - Máximo 5 hashtags hipersegmentados.
  - Disclaimer obligatorio: `Imágenes ilustrativas creadas con IA.`
- [ ] **Bloque B (Facebook Fan Page):**
  - Enlaces directos clicables a la tienda web con parámetros de campaña UTM (`?utm_source=facebook&utm_medium=organic_social&utm_campaign=...`).
  - Enlace directo a WhatsApp con formato internacional (`https://wa.me/...`).

---

## 🛠️ Procedimiento de Corrección (Regla de Reintento Puntual)

1. **Aislamiento:** Si una slide (ejemplo: Slide 02) falla en alguno de los puntos, **NO se regenera todo el carrusel**. Se trabaja únicamente sobre esa slide.
2. **Diagnóstico y Prompt Correctivo:**  
   Se identifica la causa exacta de la falla y se añade una directiva prohibitiva explícita en el prompt:
   - *Si alucinó hojas en el logo:* `PROHIBIDO terminantemente dibujar ramas, tallos o guirnaldas de hojas subrayando la marca`.
   - *Si arrastró el fondo negro del producto:* `AISLAMIENTO TOTAL: Ignorar el fondo negro de estudio (#000000) de la Imagen 2; extraer únicamente el envase`.
   - *Si el texto quedó muy abajo:* `ZONA SEGURA: Elevar el bloque de texto 120 píxeles por encima del borde inferior`.
3. **Re-generación y Re-auditoría:** Se ejecuta nuevamente la generación y se vuelve a auditar hasta que esté impecable.

---

## 📊 Presentación al Usuario

Una vez que todas las slides han superado la auditoría al 100 %, el agente genera el informe de verificación interactivo utilizando el componente ````carousel```` de Markdown:

````markdown
````carousel
![Slide 01 — Portada](/ruta/absoluta/01.jpg)
<!-- slide -->
![Slide 02 — Desarrollo](/ruta/absoluta/02.jpg)
<!-- slide -->
![Slide 03 — Detalle](/ruta/absoluta/03.jpg)
<!-- slide -->
![Slide 04 — Beneficio](/ruta/absoluta/04.jpg)
<!-- slide -->
![Slide 05 — Cierre y CTA](/ruta/absoluta/05.jpg)
````
````
