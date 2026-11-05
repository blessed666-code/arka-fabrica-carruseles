# Estándares de Copy para Redes Sociales (Instagram, TikTok, Shorts y Facebook)

El copy generado por la Fábrica de Carruseles de ARKA está diseñado para ser **copiado y pegado directamente** en las aplicaciones móviles y administradores de páginas sin requerir edición manual.

A partir de la versión para e-commerce, cada contenido genera **dos bloques de copy independientes**:
- **Bloque A:** Calibrado para Instagram, TikTok y YouTube Shorts (donde los enlaces en el caption no son clicables).
- **Bloque B:** Calibrado para Fan Pages de Facebook (donde los enlaces son 100 % clicables y permiten trazabilidad con parámetros UTM).

---

## 🚫 Por Qué el Markdown Crudo Está Prohibido en Redes Sociales

En aplicaciones móviles como Instagram y TikTok, el texto en Markdown (`**negrita**` o `*cursiva*`) **no se formatea**. El usuario ve asteriscos feos y rotos que restan profesionalismo.

Por eso, este sistema utiliza **Negritas Matemáticas Unicode nativas**, que se visualizan como negrita real en cualquier teléfono Android, iPhone o navegador web sin necesidad de etiquetas.

### Control de Integridad UTF-8 (Anti-`U+FFFD`):
Al convertir texto en español con vocales tildadas (`á`, `é`, `í`, `ó`, `ú`, `ñ`) a caracteres matemáticos Unicode, algunos generadores insertan el carácter corrupto de reemplazo `` (`U+FFFD`). Para evitarlo:
- Las vocales acentuadas deben conservarse en su carácter UTF-8 limpio estándar si el generador no cuenta con el glifo matemático exacto.
- Toda la codificación de archivos debe guardarse estrictamente en UTF-8 sin BOM.

---

## 🔤 Tabla de Referencia Rápida Unicode

### Números en Negrita (para listas ordenadas):
`𝟭.` · `𝟮.` · `𝟯.` · `𝟰.` · `𝟱.` · `𝟲.` · `𝟳.` · `𝟴.` · `𝟵.` · `𝟭𝟬.`

### Abecedario Mayúsculo en Negrita:
`𝗔 𝗕 𝗖 𝗗 𝗘 𝗙 𝗚 𝗛 𝗜 𝗝 𝗞 𝗟 𝗠 𝗡 𝗢 𝗣 𝗤 𝗥 𝗦 𝗧 𝗨 𝗩 𝗪 𝗫 𝗬 𝗭`

### Abecedario Minúsculo en Negrita:
`𝗮 𝗯 𝗰 𝗱 𝗲 𝗳 𝗴 𝗵 𝗶 𝗷 𝗸 𝗹 𝗺 𝗻 𝗼 𝗽 𝗾 𝗿 𝘀 𝘁 𝘂 𝘃 𝘄 𝘅 𝘆 𝘇`

---

## 📐 Estructura Dual del Archivo `copy.md`

Cada carpeta de carrusel (`carruseles/DNN-slug/copy.md`) debe contener los dos bloques listos para publicar:

### Bloque A · Caption para Instagram, TikTok y YouTube Shorts
```text
[1. GANCHO / HOOK VISUAL (1 línea potente con emoji)]
¿Sientes la piel [problema o síntoma del cliente]? 🤔✨

[2. CONEXIÓN Y CONTEXTO (2 a 3 líneas)]
Explicación corta del porqué el tema de hoy transforma su día o resuelve su duda.

[3. DESARROLLO EN LISTA CON NEGRITAS UNICODE]
𝟭. 𝗣𝘂𝗻𝘁𝗼 𝗖𝗹𝗮𝘃𝗲: explicación directa de una o dos oraciones.

𝟮. 𝗦𝗲𝗴𝘂𝗻𝗱𝗼 𝗣𝘂𝗻𝘁𝗼: sin rodeos ni tecnicismos aburridos.

𝟯. 𝗧𝗲𝗿𝗰𝗲𝗿 𝗣𝘂𝗻𝘁𝗼: el detalle práctico que marca la diferencia.

[4. LLAMADO A LA ACCIÓN (CTA DIRECTO A BIOGRAFÍA Y WHATSAPP)]
👉 Escríbenos por WhatsApp al [Número internacional] o visita el enlace de nuestra biografía para pedir tu [Nombre de Producto] con envío a todo el país.

[5. TRANSPARENCIA Y HASHTAGS (MÁXIMO 5)]
Imágenes ilustrativas creadas con IA.

#marca #producto #beneficio #categoria #nicho
```

### Bloque B · Caption para Fan Page de Facebook (Con Enlaces Directos y UTMs)
Facebook es un canal de tráfico directo porque permite enlaces clicables dentro de la publicación. Cada enlace de producto debe llevar sus parámetros de seguimiento para Google Analytics 4 (GA4):

```text
[1. GANCHO VISUAL CONTEXTUALIZADO PARA FACEBOOK]
¿Sientes la piel [problema o síntoma del cliente]? 🫧✨

[2. CONEXIÓN CORTA Y BENEFICIOS]
Resumen de los puntos clave de la solución y por qué funciona.

[3. OFERTA Y PRECIO CLARO]
🎁 𝗣𝗿𝗲𝗰𝗶𝗼 𝘆 𝗕𝗲𝗻𝗲𝗳𝗶𝗰𝗶𝗼: $XX.XXX COP + [Obsequio o Envío Gratis].

[4. ENLACE DIRECTO DE COMPRA CON PARÁMETROS UTM]
🛒 𝗖𝗼𝗺𝗽𝗿𝗮𝗿 𝗲𝗻 𝗹𝗮 𝘁𝗶𝗲𝗻𝗱𝗮 𝘄𝗲𝗯:
https://tu-dominio.com/producto/slug-producto?utm_source=facebook&utm_medium=organic_social&utm_campaign=d01_slug_carrusel

[5. ENLACE DIRECTO A WHATSAPP]
📲 𝗣𝗲𝗱𝗶𝗿 𝗽𝗼𝗿 𝗪𝗵𝗮𝘁𝘀𝗔𝗽𝗽 𝗕𝘂𝘀𝗶𝗻𝗲𝘀𝘀:
https://wa.me/573001234567?text=Hola%20quiero%20el%20producto%20de%20la%20publicacion

[6. COBERTURA, MEDIOS DE PAGO Y TRANSPARENCIA]
🚚 Despacho asegurado a toda Colombia (Pago Contraentrega o Nequi).

Imágenes ilustrativas creadas con IA.

#marca #producto #categoria #beneficio #nicho
```

---

## 📌 Reglas Inquebrantables de Formato
1. **Doble Salto de Línea:** Siempre dejar una línea en blanco entre párrafos. Los bloques compactos ahuyentan la lectura en pantallas móviles.
2. **Máximo 5 Hashtags:** Usar entre 3 y 5 hashtags de nicho para evitar penalización por spam algorítmico.
3. **Cero Guiones Largos:** Prohibido usar rayas (`—`) o semirrayas (`–`). Usar guion corto (`-`), dos puntos (`:`) o punto (`.`).
4. **Disclaimer de IA:** Incluir siempre al final: `Imágenes ilustrativas creadas con IA.`
