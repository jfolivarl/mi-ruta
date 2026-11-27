# Mi Ruta

**Mi Ruta** convierte el itinerario de un día en un juego para hacerlo a pie en pareja.

Cada parada es un **nivel**, con su ilustración y un texto corto. El **punto azul con el banderín** sois vosotros moviéndoos por el mapa. Cuando entráis en el **círculo de 60 m** de una parada, se pone **OK**. Después hacéis un **reto rápido** (una foto divertida o probar algo), **plantáis la bandera y coronáis el nivel**.

La app va con la **hora real**: dice qué toca ahora, cuánto queda (un anillo que se vacía y se desvanece) y si vais con retraso.

Al abrir la app sale **Mis rutas**, el cuadro de mando inicial. Hay una tarjeta por viaje, con la fecha, los lugares y el estado («Hoy», «Faltan 14 días» o «Terminada»). La que toca según la fecha va marcada y desde ella se entra al juego. Arriba hay un **filtro por país** (Todos, España, Francia, Italia, Suiza).

**Conquista Zaragoza** no tiene fecha fija: se juega el día que elijáis, con la hora real. Recorre el Pilar, el Puente de Piedra, la Seo, el Mercado Central, el tapeo de El Tubo (a elegir entre Bodegas Almau, Doña Casta y Casa Pascualillo), la plaza de España y la Aljafería, y termina con el Pilar iluminado. Cada parada tiene su propio dibujo. El progreso de cada ruta se guarda por separado.

**Viaje de Navidad (27–31 de diciembre).** Cuatro rutas sueltas. **Conquista Lugano** (28, mañana): Ayuntamiento y Piazza della Riforma, mercadillos, lago, Parco Ciani y su puerta al lago, funicular del Monte Brè. **Conquista Como** (28, tarde): Duomo, Città dei Balocchi y el lago iluminado. **Tren Bernina** (29): St. Moritz y el Bernina Express (glaciar de Morteratsch, curva de Montebello, Lago Bianco, Alp Grüm) hasta Tirano. **Conquista Milán** (30): Duomo, Galleria, la Scala, el Camparino, comida a elegir entre Luini, Spontini o Trattoria Milanese, y Aperol en los Navigli. Las horas del bus y del tren son orientativas: se cambian tocándolas en el Resumen.

El filtro de Mis rutas lleva la banderita de cada país.

**Conquista Valladolid** y **Conquista León** son rutas cortas (unas cinco horas), también sin fecha fija y con un dibujo para cada parada. Valladolid: Plaza Mayor, San Pablo y San Gregorio, la catedral y la Antigua, pinchos (Los Zagales, Villa Paramesa o Jero) y el Campo Grande. León: la catedral, Casa Botines, San Isidoro, tapeo en el Barrio Húmedo (El Rebote, La Bicha o El Flechazo) y San Marcos.

| Ruta | Fechas | Estado |
|---|---|---|
| Conquista Zaragoza | Cuando queráis (un día a pie) | Lista |
| Conquista Toulouse | 21 de noviembre de 2026 | Lista |
| Conquista Valladolid | Cuando queráis (ruta corta) | Lista |
| Conquista León | Cuando queráis (ruta corta) | Lista |
| Conquista Lugano | 28 de diciembre de 2026 (mañana) | Lista |
| Conquista Como | 28 de diciembre de 2026 (tarde) | Lista |
| Tren Bernina | 29 de diciembre de 2026 | Lista |
| Conquista Milán | 30 de diciembre de 2026 | Lista |

Web: https://jfolivarl.github.io/mi-ruta/

Autor: **Juan Felipe Olivar Londoño**

## Qué tiene

- **Dos rutas.** **Completa:** de 10:00 a 18:00, las 10 paradas del itinerario. **Exprés:** de 10:00 a 15:30, solo las prioridades del itinerario más la comida.
- **Círculos por importancia.** Los grandes con doble aro son las prioridades si vais justos de tiempo.
- **Sígueme y Llévame.** El punto azul lleva una línea y un arco delante que apuntan hacia donde mira el móvil. Navegación a pie por las calles, como un GPS: una flecha grande dice «gira a la izquierda en 20 m por Rue du Taur», «sigue recto» o «a la derecha», y en el mapa se dibuja la ruta. Las rutas a pie las calcula OpenStreetMap (routing.openstreetmap.de). Si no hay conexión, una flecha de brújula apunta al destino.
- **Copia de seguridad.** En el Resumen, «Guardar copia» guarda el progreso y las fotos en un archivo (Compartir › Guardar en Archivos) y «Recuperar copia» lo vuelve a cargar. «Dar por hechas las paradas anteriores» recupera de golpe las banderas de las paradas ya pasadas.
- **Quitar y añadir paradas.** En el Resumen, la ✕ quita una parada (se puede recuperar). «Añadir parada» pide tocar el mapa, el nombre y la hora, y la parada entra en el juego como un nivel más.
- **Resumen.** Se abre con el botón de las banderas o tocando el reloj. Muestra cómo vais, a qué hora llegasteis a cada sitio y si fuisteis en hora. Si cambia el plan, se toca una hora y todas las paradas siguientes se ajustan solas al nuevo horario.
- **Norte y giro.** El mapa gira con dos dedos. Al tocar la N vuelve al norte. En el ordenador también gira con Mayús + arrastrar.
- **Comida.** Se elige uno de los tres restaurantes y la ruta se recalcula.
- **Hotel.** Se fija tocando el mapa.
- **Recompensas.** XP, rangos, insignias y un **álbum** con las fotos de los retos.
- **Capas del mapa.** Azul, Callejero, Relieve y Satélite. Abajo aparecen la escala y el autor, como en Mis viajes.
- **Todo dentro de la app.** Se instala en la pantalla de inicio, y el progreso y las fotos se guardan solo en el móvil.

## Archivos (todos sueltos en la raíz)

| Archivo | Para qué sirve |
|---|---|
| `index.html` | Todo el juego: estilo, ilustraciones, datos de la ruta y funcionamiento |
| `logo.png` | Logo de Mi Ruta (cabecera, portada y mapa) |
| `leaflet.js`, `leaflet.css`, `LICENSE-leaflet.txt` | Mapa Leaflet 1.9.4 |
| `manifest.webmanifest` | Instalarla como app |
| `icon-192.png`, `icon-512.png`, `icon-maskable.png`, `apple-touch-icon.png` | Iconos de la app |
| `README.md` | Este archivo |

## Cómo actualizar

Todo se cambia dentro de `index.html`:

- **MIS RUTAS**: las tarjetas del cuadro de mando. Para añadir un viaje, se copia una tarjeta y se cambian las fechas y los textos.

- **RUTA POR ZARAGOZA**: paradas, horas, textos, retos y los tres bares de El Tubo. **ILUSTRACIONES DE ZARAGOZA**: sus dibujos.
- **RUTA DE MAÑANA**: fecha, paradas, horas, textos, coordenadas (`lat` y `lng`), prioridad (`nivel` 3, 2 o 1) y restaurantes.
- **EL JUEGO**: el reto de cada nivel, su insignia y las horas de la ruta exprés.
- **ILUSTRACIONES**: los dibujos de cada nivel.


Para mover una parada, en Google Maps mantén pulsado el sitio y copia las coordenadas.

Mapas © OpenStreetMap y Esri · Rutas a pie: FOSSGIS / OSRM · Leaflet 1.9.4 (licencia BSD-2).
