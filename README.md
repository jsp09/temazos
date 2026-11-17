# Temazos

Juego de fiesta para adivinar en qué año salió cada canción. Suena un tema, lo colocas en la línea del tiempo y gana quien consiga antes 10 cartas.

**Jugar:** https://jsp09.github.io/temazos/

Funciona en el navegador del móvil, sin instalar nada. Con Spotify Premium las canciones suenan sin que nadie vea el título.

## Cómo se juega

1. Elige jugadores o equipos, las reglas y las barajas, y pulsa **Empezar partida**.
2. En cada turno suena una canción. El jugador elige el hueco de la línea del tiempo donde cree que va y confirma.
3. Antes de revelar el año, los demás pueden gastar un comodín 🃏 para apostar por otro hueco. Si el jugador falla y uno de ellos acierta, se lleva la carta.
4. Se revela el año. Si la canción es del mismo año que otra carta, vale ponerla a cualquiera de sus dos lados.
5. Gana quien llegue primero al número de cartas elegido.

### Niveles

Se elige en Reglas y es el mismo para todos:

- **Fácil:** basta con colocar la canción. Si además dices título y artista, ganas un comodín.
- **Medio:** colocarla y decir el artista o el título. Si dices los dos, ganas un comodín.
- **Pro:** colocarla y decir artista y título.
- **Experto:** además, el año exacto. Antes de sonar, el jugador elige de qué década quiere la canción.
- **Al azar:** de cada 10 turnos, 4 Fácil, 3 Medio, 2 Pro y 1 Experto, igual para todos.

Al revelar, la tarjeta sale en verde si está todo acertado, en naranja si falta confirmar lo que se ha dicho y en rojo si es un fallo.

### Comodines

- 1 comodín: saltar una canción.
- 3 comodines: comprar la carta, que se coloca sola.
- Robar: apostar por otro hueco cuando juega otro. En Medio, Pro y Experto, quien roba también tiene que cumplir su nivel (artista o título en Medio; artista y título en Pro y Experto), y si lo consigue recupera el comodín.

## Opciones

- Línea del tiempo compartida o una por jugador.
- Número de comodines y de cartas para ganar.
- Temporizador de 30, 45 o 60 segundos.
- Filtro por décadas.
- Modo tele: pantalla en horizontal y en grande, para duplicar el móvil en la tele.
- ✏️ para corregir un año que esté mal (se guarda para siguientes partidas) y ↶ para deshacer.
- Estadísticas al final de la partida.

## Música

**Sin Premium:** el botón abre la canción en Spotify y la pone otro jugador (el DJ), sin enseñar la pantalla.

**Con Premium:** pulsa **Conectar Spotify** en el menú. La canción suena en tu Spotify (móvil, altavoz o tele) sin salir del juego, puede empezar hacia el segundo 40, se puede pausar y seguir, y se para al revelar el año o al acabar el temporizador.

El juego viene configurado con mi app de Spotify, que en modo desarrollo solo admite 5 cuentas autorizadas. Para usar tu propia app:

1. Entra en [developer.spotify.com/dashboard](https://developer.spotify.com/dashboard) y pulsa **Create app**.
2. En **Redirect URIs** pon `https://jsp09.github.io/temazos/`.
3. Marca **Web API** y guarda.
4. Copia el **Client ID** y pégalo en el juego, en "Usar mi propia app de Spotify".

## Barajas

Trae varias barajas ya cargadas y se pueden mezclar. Para añadir una playlist propia, expórtala como CSV en [exportify.net](https://exportify.net) e impórtala desde el menú. Los años vienen de Spotify y a veces corresponden a una remasterización; se pueden corregir durante la partida.

## Instalar como app

En el iPhone, abre la web en Safari y pulsa **Compartir → Añadir a pantalla de inicio**. En Android, menú de Chrome → **Añadir a pantalla de inicio**. La app instalada guarda sus datos aparte de Safari, así que la primera vez hay que volver a conectar Spotify.

## Archivos

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | El juego completo, con las barajas incluidas |
| `manifest.webmanifest` | Nombre e icono al instalarlo en la pantalla de inicio |
| `icon-180.png`, `icon-512.png` | Iconos de la app |

Proyecto personal sin ánimo de lucro, no afiliado a Spotify.
