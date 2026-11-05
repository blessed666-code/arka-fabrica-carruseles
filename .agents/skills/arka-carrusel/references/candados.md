# Candados Anti-Alucinación ARKA

Los "Candados" son fórmulas y directivas de prompt diseñadas para **bloquear las alucinaciones habituales de los modelos generativos** (como agregar ramas o subrayados al logo, arrastrar fondos negros de estudio, transformar envases, inventar etiquetas o crear manos con 6 dedos).

Deben insertarse obligatoriamente en los prompts de cada slide según los elementos presentes.

---

## 🔒 1. Candado de Logo Oficial y Protocolo de Doble Variante

Se pasa el archivo de logotipo en PNG transparente (`brand/referencias/logo/`).

### Regla de Transparencia Real (Canal Alfa):
El archivo tiene fondo 100 % transparente. La IA debe integrarlo directamente sobre la superficie clara superior de la escena. **PROHIBIDO terminantemente renderizar un recuadro negro, gris o blanco detrás del logo.**

### Protocolo de Doble Variante (si la marca cuenta con isotipo y logotipo completo):
- **Logotipo Completo (Icono + Tipografía):** Se usa en **Slide 1** (portada) y **Slide 5** (cierre / llamada a la acción), ocupando entre el 12 % y el 15 % del ancho superior.
- **Emblema / Isotipo Sutil (Solo Icono sin letras):** Se usa en **Slides 2, 3 y 4** como una marca de agua discreta y elegante en la esquina superior (8 % a 10 % del ancho) con margen del 5 %, evitando competir con el contenido pedagógico.

```text
Imagen 1 = logo oficial de la marca (logo.png).
Reproducir con total fidelidad idéntica el logotipo oficial:
1) Formas, iconos, tipografía y colores exactamente como aparecen en la Imagen 1.
2) TRANSPARENCIA REAL (CANAL ALFA): Fondo 100 % transparente integrado directamente sobre la zona luminosa superior de la escena. PROHIBIDO terminantemente renderizar un recuadro negro, gris o blanco detrás del logo.
3) PROHIBIDO terminantemente dibujar ramas, coronas de hojas, tallos, marcos, círculos o subrayados inventados debajo o alrededor de las letras.
4) PROHIBIDO añadir halos blancos, bordes de sticker o fondos opacos detrás del logo.
5) Ubicado en [Centro superior (12 % a 15 % del ancho) / Esquina superior derecha (8 % a 10 % del ancho)] con margen superior del 5 %.
```

---

## 📦 2. Candado de Empaque, Producto y Aislamiento de Fondo de Estudio

A menudo las fotos de producto de catálogo ecommerce vienen sobre fondo negro de estudio (`#000000`) o blanco de recorte. Este candado garantiza que la IA reproduzca fielmente el producto **sin contaminar la escena con el fondo de la foto**.

```text
FIDELIDAD DEL EMPAQUE Y AISLAMIENTO DE FONDO (obligatorio):
Reproducir el producto/empaque de la imagen adjunta manteniendo fielmente su forma física real, materiales (vidrio, cartón rígido, tubo depresible, aluminio, tela), proporciones, colores corporativos, tipografía, sellos y TODO el texto de la etiqueta frontal, letra por letra, sin cambiar, traducir, resumir, reordenar ni inventar ningún elemento.
AISLAMIENTO DE FONDO: Ignorar por completo el fondo negro (#000000) o blanco de recorte de la foto de referencia; extraer únicamente el envase y colocarlo de pie sobre la superficie de la escena bajo iluminación natural matutina.
No sustituir por un envase genérico de banco de imágenes ni alterar el tipo de dispensador, gotero o tapa.
El producto debe reposar de pie, nítido y de frente sobre la superficie, sin nada que tape su etiqueta frontal.
```

---

## 📱 3. Candado de Zona Segura Móvil (Mobile UI Safe Zone)

En Instagram, TikTok y YouTube Shorts, la interfaz nativa de la aplicación (nombre de cuenta, descripción, botón de audio y barra lateral de me gusta/comentarios) ocupa el tercio inferior y los laterales.

```text
ZONA SEGURA MÓVIL (obligatorio):
El tercio inferior de la imagen debe reservar un margen libre de texto del 10 % en el borde inferior.
Los textos integrados deben colocarse sobre una zona despejada y contrastada con ratio superior a 10:1 respecto al fondo, garantizando lectura nítida sin ser tapados por la interfaz de las aplicaciones móviles.
```

---

## 👤 4. Candado de Modelo Consistente (Persona Real o Modelo IA)

Aplica cuando la marca cuenta con un embajador, influencer o modelo recurrente y se aportan fotos multi-ángulo en `brand/referencias/modelo/`.

```text
CONSISTENCIA DE MODELO / IDENTIDAD:
Reproducir fielmente a la persona que aparece en las referencias adjuntas (ancla de rostro / modelo).
1) Rostro idéntico: facciones faciales exactas, tono de piel, color y forma de ojos, estructura ósea, peinado y color de cabello.
2) Contextura y edad: mantener la misma fisionomía, complexión corporal y rango de edad en todas las tomas.
3) Anatomía humana perfecta: manos perfectamente anatómicas con exactamente 5 dedos en cada mano, uñas naturales, textura de piel realista con poros visibles.
4) Expresión genuina y relajada: mirada natural, sin muecas forzadas ni aspecto de muñeco de cera o render 3D plástico.
```

---

## 🌐 5. Candado de Idioma, Tipografía y Regla de Guiones

```text
ADVERTENCIA DE IDIOMA Y TEXTO:
TODO el texto visible integrado en la imagen debe estar renderizado exactamente en ESPAÑOL (o idioma oficial de la marca), con ortografía impecable y tildes correspondientes.
PROHIBIDO escribir palabras o carteles en inglés.
PROHIBIDO escribir etiquetas meta del prompt como "Título:", "Kicker:", "Pastilla:", "CIERRE", "Línea 1" o comillas dentro de la imagen.
PROHIBIDO usar guiones largos (ni raya "—" ni semirraya "–"); usar siempre guion corto ("-"), dos puntos (":") o punto (".").
El texto debe leerse limpio, nítido y con alto contraste sobre la composición.
```

---

## 🚫 6. Bloque Prohibido Universal (Negative Constraints)

Pegar al final de cada prompt:

```text
[PROHIBIDO]
Recuadro negro o blanco detrás del logo, arrastrar el fondo negro de estudio del producto, ramas o guirnaldas subrayando el logotipo, halo blanco o borde de sticker en el logo, empaque deformado o sustituido por objeto genérico, manos con más o menos de 5 dedos, rostros de cera plástica deformes, palabras en inglés, textos meta ("Kicker", "Título", "Línea 1"), comillas, guiones largos, precios numéricos flotantes, marcas de agua extrañas.
```
