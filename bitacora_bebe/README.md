# Bitácora de José Gabriel

App de un solo archivo (`index.html`) para registrar la rutina y la salud del bebé desde el teléfono, con botones grandes y pocos toques.

## Qué registra
- **Alimentación:** pecho (temporizador por lado y lado sugerido), biberón (leche materna o fórmula, en **ml u oz**), sólidos y extracción de leche.
- **Pañales:** pipí y popó, con color (tarjeta colorimétrica) y consistencia.
- **Sueño:** temporizador, calidad, lugar y ventana de vigilia según la edad.
- **Tiempo de barriga** con meta diaria por edad.
- **Salud:** temperatura, medicinas, suplementos diarios (vitamina D), síntomas, baño y notas.
- **Vacunas:** Esquema de Vacunación Universal (Cartilla Nacional de Salud) con fecha de cada dosis y su estado.
- **Crecimiento:** peso, talla y perímetro cefálico con percentiles OMS (niños, 0–12 meses).
- **Consultas:** tamizajes, consultas de niño sano y un registro de consultas y estudios.

Avisa cuando se registra lo mismo dos veces en poco tiempo (en medicinas, dentro de 4 h) y muestra alertas como fiebre en menores de 3 meses, heces pálidas o pocos pañales mojados.

## Dónde se guardan los datos
| Dónde se abre | Datos |
|---|---|
| Página publicada en Claude (compartida con permiso de Editor) | Compartidos y sincronizados en vivo entre los teléfonos |
| Este `index.html` (GitHub Pages o el archivo en el teléfono) | Solo en el navegador de ese teléfono |

Para pasar datos de una versión a otra: **Ajustes → Exportar / Importar** (archivo `.json`).

## Publicarlo con GitHub Pages
1. En el repo: **Settings → Pages**.
2. En *Branch*, elige la rama que tenga esta carpeta y la carpeta `/ (root)`.
3. La app queda en `https://<tu-usuario>.github.io/<repo>/bitacora_bebe/`.

Ábrela en el teléfono y usa "Agregar a pantalla de inicio".

> Herramienta de observación; no sustituye la valoración del pediatra.
