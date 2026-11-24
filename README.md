# Hacemos la Tarea · Sistema de diseño

Guía de marca de Hacemos la Tarea (movimiento ciudadano de Bogotá, vocero Christiam Torres) para el equipo de diseño y contenido.

## Cómo usarlo

- **Ver la guía:** descarga el repositorio (Code → Download ZIP) y abre `index.html` en el navegador. Tiene vista clara y vista noche.
- **Diseñar:** los isotipos están en `logos/` y la tipografía Montserrat en `fonts/` (licencia SIL Open Font, ver `fonts/OFL.txt`). Los valores de color están en la sección Color de la guía.
- **Maquetar en web:** carga `tokens.css` y `componentes.css`. El HTML de cada componente está en la sección Componentes de la guía.
- **Proponer un cambio:** abre un issue o un pull request. `tokens.json` es la fuente de los valores; `tokens.css` se deriva de él.

| Archivo | Contenido |
| --- | --- |
| `index.html` | La guía visual, autocontenida |
| `logos/` | Isotipo HT en PNG transparente, versión para fondo claro y para fondo oscuro |
| `fonts/` | Montserrat recta y cursiva, todos los pesos |
| `tokens.css` · `tokens.json` | Colores, espacios, radios y estilos de texto |
| `componentes.css` | Clases de los seis componentes |
| `avatares/` | Avatar conversacional: dirección seleccionada, exploraciones, referencias de animación y manual de uso |
| `referencia/` | Hoja de color original |

## Pendiente

- Isotipo en vectorial (el PNG mide 568 × 328 px, no alcanza para impresión).
- Logotipo horizontal con el nombre.
- Confirmar Montserrat como tipografía oficial: se identificó a partir de la hoja de color.

# Reglas de la marca

Hacemos la Tarea es un movimiento ciudadano de Bogotá cuyo vocero es Christiam Torres. Este sistema rige todo lo que se produzca para el movimiento y para Christiam: piezas de redes, videos, documentos, presentaciones y web.

## Voz y contenido

- **La marca es el movimiento.** Firma como «Hacemos la Tarea». Christiam Torres aparece como vocero, con nombre y cargo en estilo `nota`, nunca como titular de la pieza.
- **Ciudadano, no político ni institucional.** Habla como un vecino que se informó: frases cortas, verbos de acción, segunda persona («Cuéntanos», «Revisa», «Participa»). Sin jerga de entidad ni promesas.
- **Dato con fuente.** Toda cifra lleva su fuente visible en estilo `nota`. Sin fuente verificable, no se publica.
- **Nombra barrios y lugares concretos.** Nunca escribas la palabra «estrato» en una pieza pública.
- **Lemas.** «Nuestra ciudad, nuestro compromiso» es el lema principal. «Participar · Actuar · Avanzar» es el secundario; sus tres verbos se separan con punto medio.
- **Frentes.** Cada pieza pertenece a un frente y lo declara con una `Etiqueta`: Educación vial, Víctimas o SITP.
- **Mayúsculas.** Titulares de portada y etiquetas van en mayúsculas. Texto corrido y subtítulos, en alta y baja. Escribe siempre «Hacemos la Tarea» con H y T mayúsculas.
- **Sin emojis en las piezas gráficas.** La flecha del isotipo (`.ht-flecha`) hace de viñeta, de indicador de «desliza» y de señal de continuidad.

## Color

Cuatro colores, tomados de la hoja de color de la marca (`referencia/paleta-oficial.jpg`):

| Token | Valor | Papel |
| --- | --- | --- |
| `azul-noche` | #00002E | Color principal. Fondo de piezas oscuras y tinta sobre blanco. |
| `verde-activo` | #B4F000 | Acción y resalte. Solo como relleno. |
| `gris` | #646464 | Texto de apoyo sobre blanco. |
| `blanco` | #FFFFFF | Fondo claro y texto sobre azul. |

- Compón con los tokens de función (`fondo`, `tinta`, `tinta-suave`, `acento`, `sobre-acento`), no con los de marca, para que la pieza funcione en el tema Claro y en el tema Noche.
- **Proporción.** En una pieza, `azul-noche` o `blanco` ocupan el fondo; `verde-activo` no pasa de un tercio de la superficie. Es el color que guía el ojo: un resalte, un botón, una banda.
- **Combinaciones permitidas para texto:** `azul-noche` sobre `blanco`, `blanco` sobre `azul-noche`, `azul-noche` sobre `verde-activo`, `verde-activo` sobre `azul-noche`, `gris` sobre `blanco`.
- **Prohibidas:** `verde-activo` como texto sobre `blanco` (1,4:1), `blanco` sobre `verde-activo`, `gris` sobre `azul-noche` (usa `tinta-suave`).
- `verde-flecha` existe solo dentro del motivo de la flecha. No lo uses en texto, fondos ni botones.
- No añadas colores. Sin degradados ni sombras: la marca es de tintas planas.

## Tipografía

Una sola familia: **Montserrat** (`--font-sans`), en dos voces.

- **Voz de titular:** cursiva, pesos 800 y 900 (`cifra`, `titular-xl`, `titular-l`, `titular-m`). La cursiva pesada repite la inclinación del isotipo. Interlínea apretada, de 0,9 a 1,1.
- **Voz de texto:** recta, pesos 400 y 500 (`cuerpo-l`, `cuerpo`, `nota`). `titular-s` y `etiqueta` son rectas en peso 800.
- Resalta con el componente `Titular` (`.ht-resalte`), no con subrayado ni con otro color de letra.
- Líneas de texto corrido de 65 caracteres como máximo. Alinea a la izquierda; no justifiques ni centres párrafos.
- No uses cursiva ligera, ni otra familia, ni contornos o sombras en la letra.

## Isotipo

El isotipo es la H y la T unidas por una flecha que avanza. Hay dos archivos en `logos/`:

- `ht-isotipo-fondo-claro.png`: H en azul. Para fondo `blanco` y `fondo-alterno` del tema Claro.
- `ht-isotipo-fondo-oscuro.png`: H en blanco. Para fondo `azul-noche` y sobre foto oscurecida.

Reglas:

- Usa el archivo tal cual. No lo redibujes, recolorees, gires, estires ni le quites la flecha.
- Nunca lo pongas sobre `verde-activo` ni sobre una foto clara: la T se pierde.
- Deja libre a su alrededor, como mínimo, el ancho de la flecha.
- Ancho mínimo: 48 px en pantalla, 15 mm en impreso.
- No hay logotipo horizontal con el nombre entre los archivos de marca. Cuando necesites nombre e isotipo juntos, usa el componente `Firma`.

## Forma

- **Aristas vivas.** Todo va en `radio-recto`. `radio-suave` y `radio-circulo` quedan para campos de formulario y fotos de perfil.
- **Inclinación.** Bloques, bandas y etiquetas se inclinan con `inclinacion` (−12°), el ángulo de las astas del isotipo. El texto corrido y las fotos no se inclinan.
- **La flecha** (`.ht-flecha`) es el único motivo gráfico. Apunta siempre a la derecha: hacia adelante.
- Las fotos van a sangre o en rectángulo recto, sin marcos ni esquinas redondeadas. Sobre foto, el texto lleva debajo un velo `azul-noche` al 60 % como mínimo.

## Espaciado

Usa la escala `espacio-1` a `espacio-6` (4, 8, 16, 24, 40, 64 px). El módulo de bloques y flechas es `espacio-6`. Margen lateral mínimo en móvil: `espacio-3`.

## Formatos

| Formato | Tamaño | Margen de seguridad |
| --- | --- | --- |
| Post y carrusel | 1080 × 1350 px | 96 px por lado |
| Historia, reel y TikTok | 1080 × 1920 px | 96 px a los lados, 250 px arriba, 340 px abajo |
| Presentación | 1920 × 1080 px | 96 px por lado |
| Documento | Carta | 20 mm |

- **Carrusel:** portada con `PiezaSocial`, láminas interiores con un `Titular` y máximo 40 palabras, un `Dato` cuando haya cifra, y `Firma` en la última lámina.
- **Video:** subtítulos en Montserrat 800 recta, `blanco` sobre placa `azul-noche`; la palabra clave de cada frase con `.ht-resalte`. Cierre con `Firma` sobre `azul-noche` durante 2 segundos como mínimo.
- **Documento y presentación:** fondo `blanco`, titulares en `titular-l` o `titular-m`, portada y separadores sobre `azul-noche`.

## Componentes

`Boton`, `Etiqueta`, `Titular`, `Dato`, `PiezaSocial` y `Firma` son HTML con las clases de `componentes.css`. No hay JavaScript. Su HTML de ejemplo y sus reglas están en `index.html`, sección Componentes.

## Avatar conversacional

La dirección seleccionada, las exploraciones y las referencias para animación están documentadas en [avatares/README.md](avatares/README.md). Consulta también el [manual de uso del avatar](avatares/manual-de-uso.md).

## Accesibilidad

- Texto a 4,5:1 como mínimo sobre su fondo; 3:1 para titulares de 24 px o más.
- El anillo de foco es `foco`, sólido de 3 px, separado 3 px del control.
- El color nunca es la única señal: una etiqueta activa también es la primera de su fila, y un dato siempre lleva su texto.
