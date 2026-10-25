# Protocolo de Auditoría Visual Milimétrica (Filtro de Seguridad ARKA)

En la Fábrica de Carruseles de ARKA está **estrictamente prohibido afirmar que un carrusel está terminado** sin haber abierto y auditado cada una de las imágenes generadas.

---

## 🔍 Checklist de Inspección Visual (Slide por Slide)

El agente debe abrir cada archivo `01.jpg` a `05.jpg` y contrastarlo contra estos 6 puntos de control:

| Punto de Control | Pregunta de Verificación | Criterio de Aprobación |
|---|---|---|
| **1. Logo Oficial** | ¿Es exactamente el logo de `logo.png`? | ✅ Sin ramas, hojas, flores o subrayados alucinados bajo las letras. Sin marcos cuadrados, halos blancos o stickers. |
| **2. Empaque / Producto** | ¿Es idéntico a las fotos reales de referencia? | ✅ Material real (kraft, vidrio, tela, metal), colores corporativos, tipografía y textos de la etiqueta fieles sin distorsiones ni inventos. |
| **3. Anatomía Humana** | ¿Los personajes lucen naturales y proporcionados? | ✅ Manos con exactamente 5 dedos anatómicos. Rostros con expresión relajada y textura de piel real (cero plástico o cera). |
| **4. Modelo Ancla** | ¿Mantiene la identidad de la persona de referencia? | ✅ Mismas facciones, tono de piel, contextura y edad del archivo de modelo de referencia. |
| **5. Texto en Imagen** | ¿La tipografía es legible y sin errores? | ✅ 100 % en el idioma objetivo con tildes correctas. Cero palabras en inglés no deseadas. Cero palabras meta como "Título", "Kicker" o "CIERRE". |
| **6. Composición y Luz** | ¿Cumple con el Layout (A, B, C o D)? | ✅ Iluminación fotográfica natural, profundidad de campo cinematográfica, sin zonas quemadas ni artefactos extraños. |

---

## 🛠️ Procedimiento de Corrección (Regla de Reintento Puntual)

1. **Aislamiento:** Si una slide (ejemplo: Slide 02) falla en alguno de los 6 puntos, **NO se regenera todo el carrusel**. Se trabaja únicamente sobre esa slide.
2. **Diagnóstico y Prompt Correctivo:**  
   Se identifica la causa exacta de la falla y se añade una directiva prohibitiva explícita en el prompt:
   - *Si alucinó hojas en el logo:* `PROHIBIDO terminantemente dibujar ramas, tallos o guirnaldas de hojas subrayando la palabra [MARCA]`.
   - *Si deformó el empaque:* `PROHIBIDO sustituir el frasco de vidrio por una caja de cartón; reproducir fielmente el envase cilíndrico de la Imagen 2`.
   - *Si dibujó manos con 6 dedos:* `Manos anatómicamente perfectas con exactamente cinco dedos visibles`.
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
