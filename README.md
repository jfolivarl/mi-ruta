# Mi Ruta

**Mi Ruta** convierte el itinerario de un día en un juego para hacerlo a pie en pareja.

Cada parada es un **nivel**, con su ilustración y un texto corto. El **punto azul con el banderín** sois vosotros moviéndoos por el mapa. Cuando entráis en el **círculo de 60 m** de una parada, se pone **OK**. Después hacéis un **reto rápido** (una foto divertida o probar algo), **plantáis la bandera y coronáis el nivel**.

La app va con la **hora real**: dice qué toca ahora, cuánto queda (un anillo que se vacía y se desvanece) y si vais con retraso.

Al abrir la app sale **Mis rutas**, el cuadro de mando inicial. Hay una tarjeta por viaje, con la fecha, los lugares y el estado («Hoy», «Faltan 14 días» o «Terminada»). La que toca según la fecha va marcada y desde ella se entra al juego.

| Ruta | Fechas | Estado |
|---|---|---|
| Conquista Toulouse | 21 de noviembre de 2026 | Lista |
| Valladolid y León | 5–9 de diciembre de 2026 | Próximamente |
| Milán, Lugano, Como y Bernina Express (Nochevieja en los Navigli) | 27–31 de diciembre de 2026 | Próximamente |

Web: https://jfolivarl.github.io/mi-ruta/

Autor: **Juan Felipe Olivar Londoño**

## Qué tiene

- **Dos rutas.** **Completa:** de 10:00 a 18:00, las 10 paradas del itinerario. **Exprés:** de 10:00 a 15:30, solo las prioridades del itinerario más la comida.
- **Círculos por importancia.** Los grandes con doble aro son las prioridades si vais justos de tiempo.
- **Sígueme.** Os sigue con el GPS y os guía hasta el siguiente nivel con una flecha, la distancia y los minutos a pie.
- **Resumen.** Se abre con el botón de las banderas o tocando el reloj. Muestra cómo vais, a qué hora llegasteis a cada sitio y si fuisteis en hora. Si cambia el plan, se toca una hora y todas las paradas siguientes se ajustan solas al nuevo horario.
- **Norte y giro.** El mapa gira con dos dedos. Al tocar la N vuelve al norte. En el ordenador también gira con Mayús + arrastrar.
- **Comida.** Se elige uno de los tres restaurantes y la ruta se recalcula.
- **Hotel.** Se fija tocando el mapa.
- **Apple Watch.** La página `reloj.html` está hecha para el reloj: muestra la hora, qué toca, la cuenta atrás y el horario. El Apple Watch no tiene Safari: os enviáis el enlace por Mensajes y lo abrís en el reloj. En el Resumen hay un botón para copiarlo.
- **Recompensas.** XP, rangos, insignias y un **álbum** con las fotos de los retos.
- **Capas del mapa.** Azul, Callejero, Relieve y Satélite. Abajo aparecen la escala y el autor, como en Mis viajes.
- **Todo dentro de la app.** Se instala en la pantalla de inicio, y el progreso y las fotos se guardan solo en el móvil.

## Archivos (todos sueltos en la raíz)

| Archivo | Para qué sirve |
|---|---|
| `index.html` | Todo el juego: estilo, ilustraciones, datos de la ruta y funcionamiento |
| `reloj.html` | Versión para el Apple Watch: hora, qué toca, cuenta atrás y horario |
| `logo.png` | Logo de Mi Ruta (cabecera, portada y mapa) |
| `leaflet.js`, `leaflet.css`, `LICENSE-leaflet.txt` | Mapa Leaflet 1.9.4 |
| `manifest.webmanifest` | Instalarla como app |
| `icon-192.png`, `icon-512.png`, `icon-maskable.png`, `apple-touch-icon.png` | Iconos de la app |
| `README.md` | Este archivo |

## Cómo actualizar

Todo se cambia dentro de `index.html`:

- **MIS RUTAS**: las tarjetas del cuadro de mando. Para añadir un viaje, se copia una tarjeta y se cambian las fechas y los textos.

- **RUTA DE MAÑANA**: fecha, paradas, horas, textos, coordenadas (`lat` y `lng`), prioridad (`nivel` 3, 2 o 1) y restaurantes.
- **EL JUEGO**: el reto de cada nivel, su insignia y las horas de la ruta exprés.
- **ILUSTRACIONES**: los dibujos de cada nivel.

Si cambias las horas, cámbialas también en `reloj.html` (mismo bloque **RUTA DE MAÑANA**).

Para mover una parada, en Google Maps mantén pulsado el sitio y copia las coordenadas.

Mapas © OpenStreetMap y Esri · Leaflet 1.9.4 (licencia BSD-2).
