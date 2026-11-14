# Los Pasillos

Juego de terror 2D con vista cenital. Despiertas en un complejo a oscuras y
debes encontrar las **5 llaves** escondidas en los pasillos para abrir la
**puerta** y escapar... mientras algo te caza en la oscuridad (y la luz lo atrae).

## Cómo jugar

Abre `index.html` en cualquier navegador (no requiere instalación).

- **Mover:** WASD / flechas (o joystick en móvil, o **control/gamepad** 🎮)
- **Shift:** correr (necesitas las botas)
- **F:** encender / apagar la linterna
- **E:** esconderte en un armario
- **Q:** lanzar un señuelo para distraer al monstruo
- **Objetivo:** reúne las 5 llaves y llega a la puerta sin que te atrape

## Características

- Laberinto generado al azar en cada partida
- Linterna direccional (cono 110°) con parpadeos y apagones; se gasta con pilas
- **La luz atrae al monstruo**: apágala para pasar desapercibido
- Enemigo con IA (pathfinding BFS), huellas que deja al caminar y gruñido direccional
- Barra de **cordura**: baja con el miedo, distorsiona la pantalla; se recupera escondido
- **Sustos** y sonidos ambientales aleatorios
- Cinemáticas: intro con la historia, final al escapar (amanecer) y al morir (jumpscare)
- Armarios para esconderte · trampas que lo atraen
- Ítems: pilas, **llave maestra** (+2), **señuelos** y **botas** (correr)
- 3 dificultades (Fácil / Normal / Pesadilla)
- Récord de mejor tiempo guardado por dificultad (localStorage)
- Pantalla de historia y créditos · minimapa con pistas · soporte de gamepad
