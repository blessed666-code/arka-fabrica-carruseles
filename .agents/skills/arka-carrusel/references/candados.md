# Candados Anti-Alucinación ARKA

Los "Candados" son fórmulas y directivas de prompt diseñadas para **bloquear las alucinaciones habituales de los modelos generativos** (como agregar ramas o subrayados al logo, transformar bolsas en cajas, inventar etiquetas o crear manos con 6 dedos).

Deben insertarse obligatoriamente en los prompts de cada slide según los elementos presentes.

---

## 🔒 1. Candado de Logo Oficial

Se pasa siempre el archivo `brand/referencias/logo/logo.png` como Imagen 1.

```text
Imagen 1 = logo oficial de la marca (logo.png).
Reproducir con fidelidad idéntica el logotipo oficial:
1) Formas, iconos, tipografía y colores exactamente como aparecen en la Imagen 1.
2) PROHIBIDO terminantemente dibujar ramas, coronas de hojas, tallos, marcos, círculos o subrayados inventados debajo o alrededor de las letras.
3) Un solo grupo limpio, transparente, integrado orgánicamente en la iluminación de la escena.
4) PROHIBIDO añadir halos blancos, bordes de sticker o fondos opacos detrás del logo.
5) Ubicado en la [Esquina superior derecha / Esquina superior izquierda / Centro superior] ocupando el 12 % del ancho con un margen del 5 %.
```

---

## 📦 2. Candado de Empaque y Producto

Se pasa la fotografía real del producto desde `brand/referencias/productos/`.

```text
FIDELIDAD DEL EMPAQUE Y PRODUCTO (obligatorio):
Reproducir el producto/empaque de la imagen adjunta manteniendo fielmente su forma física real, materiales (vidrio, bolsa kraft, aluminio, tela, cartón), proporciones, colores corporativos, tipografía, sellos y TODO el texto de la etiqueta frontal, letra por letra, sin cambiar, traducir, resumir, reordenar ni inventar ningún elemento.
No sustituir por un envase genérico de banco de imágenes ni convertir una bolsa en caja o lata.
El producto debe reposar de pie, nítido y de frente sobre la superficie, sin nada que tape su etiqueta frontal.
```

---

## 👤 3. Candado de Modelo Consistente (Persona Real o Modelo IA)

Aplica cuando la marca cuenta con un embajador, influencer o modelo de catálogo y se aportan fotos multi-ángulo en `brand/referencias/modelo/`.

```text
CONSISTENCIA DE MODELO / IDENTIDAD:
Reproducir fielmente a la persona que aparece en las referencias adjuntas (ancla de rostro / modelo).
1) Rostro idéntico: facciones faciales exactas, tono de piel, color y forma de ojos, estructura ósea, peinado y color de cabello.
2) Contextura y edad: mantener la misma fisionomía, complexión corporal y rango de edad en todas las tomas.
3) Anatomía humana perfecta: manos perfectamente anatómicas con exactamente 5 dedos en cada mano, uñas naturales, textura de piel realista con poros visibles.
4) Expresión genuina y relajada: mirada natural, sin muecas forzadas ni aspecto de muñeco de cera o render 3D plástico.
```

---

## 🌐 4. Candado de Idioma y Renderizado de Texto

```text
ADVERTENCIA DE IDIOMA Y TEXTO:
TODO el texto visible integrado en la imagen debe estar renderizado exactamente en ESPAÑOL (o idioma oficial de la marca), con ortografía impecable y tildes correspondientes.
PROHIBIDO escribir palabras o carteles en inglés.
PROHIBIDO escribir etiquetas meta del prompt como "Título:", "Kicker:", "Pastilla:", "CIERRE" o comillas dentro de la imagen.
El texto debe leerse limpio, nítido y con alto contraste sobre la composición.
```

---

## 🚫 5. Bloque Prohibido Universal (Negative Constraints)

Pegar al final de cada prompt:

```text
[PROHIBIDO]
Ramas o guirnaldas subrayando el logotipo, halo blanco o borde de sticker en el logo, empaque deformado o sustituido por objeto genérico, manos con más o menos de 5 dedos, rostros de cera plástica deformes, palabras en inglés, textos meta ("Kicker", "Título"), precios numéricos flotantes, marcas de agua.
```
