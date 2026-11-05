---
name: arka-carrusel
description: Fábrica universal de carruseles y posts de alto impacto para Instagram, TikTok, YouTube Shorts y Facebook Fan Page desarrollada por ARKA. Diseña planes editoriales (15 a 90 contenidos), audita referencias reales (logos con canal alfa transparente, morfología de productos y modelos), genera prompts hiperrealistas con 6 candados anti-alucinación (incluyendo aislamiento de fondo de estudio y zona segura móvil), inspecciona visualmente cada imagen con control de calidad milimétrico y redacta copy dual (IG/TikTok + Facebook con UTMs) con negritas matemáticas Unicode limpias y llamadas a la acción directas.
---

# ARKA Fábrica de Carruseles · Skill Universal

Motor de creación de contenido visual y persuasivo para marcas, productos y servicios en **Instagram, TikTok, YouTube Shorts y Fan Page de Facebook**. Diseñado para operar de forma nativa en **Google Antigravity** o **Cursor** utilizando modelos de generación de imagen por llamada de herramientas como **Nano Banana 2** (`gemini-3.1-flash-image` / `GenerateImage`).

Desarrollado y compartido abiertamente por **Danniel Mena / ARKA** ([arkadigital.co](https://arkadigital.co) · GitHub: [blessed666-code](https://github.com/blessed666-code)).

---

## ⚡ Filosofía del Sistema (50% Automatizado / 50% Humano)

Este sistema automatiza el **50% más técnico y exigente** del trabajo:
1. Extracción estratégica del contexto de la marca (desde URL o cuestionario).
2. Estructuración del calendario editorial con 15 formatos probados (F1 a F15).
3. Redacción de prompts fotorrealistas con **6 candados estrictos**:
   - Transparencia real con canal alfa en logos.
   - Fidelidad de empaque + aislamiento de fondo negro o blanco de estudio.
   - Zona segura móvil (margen inferior del 10 % para interfaz de redes).
   - Consistencia de modelo y anatomía humana (5 dedos).
   - Idioma español y regla de guiones cortos.
   - Bloque prohibitivo universal de negativas.
4. Generación de imágenes en proporción `1:1` (1080x1080 px) o `4:5` (1080x1350 px) con lentes ópticos y luz cinematográfica.
5. Control de calidad visual milimétrico (auditoría obligatoria antes de entregar).
6. **Copy dual optimizado**:
   - **Bloque A:** Para Instagram, TikTok y Shorts con negritas matemáticas Unicode (sin asteriscos rotos y sin caracteres corruptos `U+FFFD`).
   - **Bloque B:** Para Facebook Fan Page con enlaces directos clicables y parámetros UTM para atribución en analítica web.

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
- Palabras en inglés, errores ortográficos o textos que invadan la zona segura móvil.

El agente tiene la orden estricta de **regenerar únicamente la slide con error** aplicando un prompt correctivo antes de notificar al usuario.

---

## 🔄 Los Dos Modos de Operación

Al activarse, la skill evalúa si la marca ya está configurada revisando si existen `brand/BRAND_BIBLE.md` y archivos dentro de `brand/referencias/`:

### MODO 1: Onboarding y Configuración de Marca (Primera vez)
Si la marca no ha sido configurada o el usuario dice *"configurar marca"*, *"iniciar"*, *"nueva marca"* o pasa una URL:
1. **Inspección Web:** Si el usuario tiene sitio web (ej. `https://mi-tienda.com`), lee el sitio para extraer catálogo, propuestas de valor, ofertas/combos, precios y tono de voz.
2. **Recepción de Fotos de Referencia:**
   - Logo oficial: `brand/referencias/logo/logo.png` (o variantes `logo-completo.png` y `logo-emblema.png`).
   - Fotos de productos: `brand/referencias/productos/` (fotos de frente, etiqueta legible, materiales reales).
   - Modelo (opcional): `brand/referencias/modelo/` (fotos multi-ángulo de persona real o modelo IA).
3. **Formato Preferido:** Pregunta si desea carruseles de 5 slides o posts individuales de 1 slide.
4. **Volumen de Contenido:** Pregunta cuántos contenidos planear (15, 30, 60 o 90 piezas).
5. **Generación de Archivos:** Compila `brand/BRAND_BIBLE.md`, `brand/CATALOGO.md` (con ficha morfológica) y `plan/PLAN-EDITORIAL.md`.

### MODO 2: Producción de Contenido (Día a día)
Cuando el usuario pide un contenido (ej. *"haz el D01"*, *"siguiente carrusel"*, *"ejecuta el D05"*):
1. Lee la ficha del contenido en `plan/PLAN-EDITORIAL.md`.
2. Lee `brand/BRAND_BIBLE.md` y `brand/CATALOGO.md`.
3. Audita las referencias visuales correspondientes en `brand/referencias/`.
4. Crea la carpeta `carruseles/DNN-slug/` y redacta:
   - `copy.md`: estructura dual (Bloque A para IG/TikTok/Shorts y Bloque B para Facebook con UTMs).
   - `prompts/01.md` ... `05.md`: prompts independientes con sus candados y zona segura móvil.
5. Genera las imágenes en 1:1 o 4:5 pasando las referencias exactas.
6. Ejecuta la auditoría visual milimétrica (`references/qa-checklist.md`). Si hay error, regenera la slide fallida.
7. Presenta el informe con el componente interactivo de carrusel en Markdown.
