# Cebollin

Página web (landing + demo jugable) del videojuego **Cebollin**, de **Pablo Saúl
/ Treehouse Studios**. Este repositorio contiene el sitio contenedor; el juego es
un export web de Godot Engine incrustado en `game/`.

## El juego

Cebollin es un juego de acción/plataformas con una historia de superación,
familia y sacrificio. Recorre **5 etapas en 5 biomas mutados** — Valle Verdura,
Rio Riviera, Cordilleras Acoyote, Cuevas Andinas y Abitio Bosque — enfrentando a
las criaturas mutadas del bosque.

**Personajes:** Cebollin (protagonista), Dr. Rabadin, Lily Tlacuache.

## Jugar

- En el sitio, botón **«▶ Jugar demo»**, o directamente `game/index.html`.
- El juego es un export HTML5 de **Godot Engine** (WebAssembly).

## Correr en local

    python -m http.server 8000

Luego abre `http://localhost:8000/`. Conviene servir por HTTP: abrir `index.html`
desde el disco (`file://`) puede fallar por las rutas absolutas y el service
worker del juego.

## Estructura

    index.html      Landing (esta página web)
    game/           Juego Cebollin — export web de Godot (wasm, pck, service worker)
    assets/         Arte, concept art, universo, pitch deck, logo, personajes
    tracks/         Música (mp3)
    *.png           Arte de la raíz

## Créditos

- Juego y arte: **Pablo Saúl** — Treehouse Studios · [pablosaul2312@gmail.com](mailto:pablosaul2312@gmail.com) · [@cebollingame](https://www.instagram.com/cebollingame/)
- Música: **Fernando «Junfez»** · [@junfez](https://www.instagram.com/junfez/)

## Licencia

El código de la página contenedora (`index.html`) es **MIT** (ver
[`LICENSE`](LICENSE)). El arte, la música y el juego exportado (`assets/`,
`tracks/`, `game/`, `*.png`) son propiedad de Pablo Saúl / Treehouse Studios y de
sus respectivos autores, y **no** están cubiertos por MIT — usados con permiso.
Detalle en [`LICENSE`](LICENSE).
