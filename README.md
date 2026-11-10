# Simulador optocinético MdDS

Reproduce en un televisor o monitor grande los parámetros publicados de la
readaptación vestíbulo-ocular para el síndrome del mal de desembarque (MdDS),
conocida como protocolo de Dai: franjas en movimiento a velocidad angular
constante, metrónomo para la inclinación de cabeza, bloques cronometrados y
registro de síntomas antes y después.

> **Herramienta de apoyo, no un tratamiento validado.** Las mejorías publicadas
> (64% a 78% inmediatas) se lograron en clínica, con un terapeuta moviendo la
> cabeza de la paciente y franjas que llenan todo el campo visual. No hay datos
> publicados de eficacia ni de seguridad de versiones caseras. Úsese con el
> visto bueno del médico tratante.

## Cómo usarlo

1. Descargar `index.html` (o clonar el repositorio) y abrirlo con doble clic en
   Chrome, Edge, Firefox o Safari. No necesita instalación ni servidor; solo
   usa internet para cargar la tipografía.
2. Conectar la computadora al televisor por HDMI y mover la ventana del
   navegador a esa pantalla.
3. Capturar el ancho de la imagen y la distancia de los ojos a la pantalla.
   El simulador calcula el campo visual; la meta es ±45° o más
   (un televisor de 55 pulgadas a 60 cm).
4. Marcar las cinco condiciones de seguridad, elegir la dirección con la guía
   y la prueba de 30 segundos, e iniciar el bloque. Cualquier tecla o toque
   detiene las franjas.

El registro se guarda solo en el navegador del equipo donde se usa. El botón
«Copiar como CSV» permite compartirlo con el médico.

## No usar si

- Hay embarazo, o el médico no ha autorizado el ejercicio después del parto.
- No hay síntomas activos ese día: sin ellos no se puede elegir la dirección
  ni medir la respuesta.
- Hay epilepsia o antecedentes de crisis provocadas por luces o patrones.
- No hay otra persona presente.

Detener de inmediato ante náusea, dolor de cabeza o un balanceo que suba
2 puntos o más.

## Parámetros y de dónde salen

| Parámetro | Valor | Fuente |
| --- | --- | --- |
| Velocidad de las franjas | 10 °/s, ajustable | Dai 2014; Schoenmaekers 2024 |
| Velocidad con visor | 5 °/s, campo de ±45° | Yakushin 2020 |
| Ancho de franja | 1.4° | Dai 2014 |
| Inclinación de cabeza | ±20° de hombro a hombro | Dai 2014; Schoenmaekers 2024 |
| Frecuencia de la cabeza | La del balanceo de la paciente (0.2 ± 0.1 Hz) o 0.167 Hz fija | Dai 2014; Schoenmaekers 2024 |
| Metrónomo | Escala de ocho notas ascendente y descendente | Yakushin 2020 |
| Bloques | 2 de 4 minutos, mañana y tarde, 3 días seguidos | Schoenmaekers 2024 |
| Dirección | Contraria al giro en la prueba de Fukuda; se invierte si empeora o no responde | Dai 2014; Schoenmaekers 2024 |
| Después | Evitar viajes largos, barcos y estrés intenso 2 semanas | Dai 2017 |

Fuentes:

- Dai 2014: <https://pmc.ncbi.nlm.nih.gov/articles/PMC4097942/>
- Dai 2017: <https://pmc.ncbi.nlm.nih.gov/articles/PMC5418223/>
- Yakushin 2020: <https://pmc.ncbi.nlm.nih.gov/articles/PMC7461907/>
- Schoenmaekers 2024: <https://pmc.ncbi.nlm.nih.gov/articles/PMC10985174/>

## Diferencias con la clínica

- Una pantalla plana cubre menos campo visual que la sala circular del estudio
  original. El simulador lo compensa dibujando las franjas en perspectiva: su
  velocidad angular es la misma en el centro y en los bordes para quien se
  sienta a la distancia capturada.
- En los estudios la cabeza la mueve el terapeuta. Aquí la mueve un
  acompañante siguiendo el metrónomo, y nadie verifica el ángulo ni el ritmo.
- No incluye modo de visor con celular: las franjas deben permanecer verticales
  respecto a la gravedad aunque la cabeza se incline, y eso exige leer el
  giroscopio del teléfono.

## Estado de las pruebas

Probado en Chromium de escritorio: inicio y paro de bloques, prueba de
30 segundos y registro. Sin probar: sonido, pantalla completa en un televisor
real, Safari y navegadores de televisores inteligentes.
