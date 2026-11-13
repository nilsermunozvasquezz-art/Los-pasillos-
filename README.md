# Los Pasillos

Juego de terror 2D con vista cenital. Despiertas en un complejo a oscuras y
debes encontrar las **5 llaves** escondidas en los pasillos para abrir la
**puerta** y escapar... mientras algo te persigue en la oscuridad.

## Cómo jugar

Abre `index.html` en cualquier navegador (no requiere instalación).

- **Moverse:** WASD o flechas (en móvil, joystick en pantalla)
- **Objetivo:** recoge las 5 llaves y llega a la puerta
- **Cuidado:** el monstruo te detecta si te acercas. Si te atrapa, pierdes.

## Características

- Laberinto generado al azar en cada partida
- Oscuridad con linterna (campo de visión limitado)
- Enemigo con IA que patrulla y persigue (pathfinding BFS)
- Sonido ambiental y latido que se acelera con el peligro (WebAudio, sin archivos)
- Cronómetro y pantallas de inicio / victoria / derrota
