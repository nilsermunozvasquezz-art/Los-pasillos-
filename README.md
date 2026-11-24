# Los Pasillos

Juego de terror 2D con vista cenital. Baja por los pisos de un complejo a oscuras:
en cada uno reúne las **5 llaves** y cruza la **puerta**, mientras algo te caza
(y la luz lo atrae). El último piso da a la superficie.

## Cómo jugar

Abre `index.html` en cualquier navegador (no requiere instalación).

- **Mover:** WASD / flechas (joystick en móvil, o control/gamepad 🎮)
- **Espacio / botón:** disparar (o ACCIÓN si tienes algo delante) · **E:** acción
- **Shift:** correr · **F:** linterna · **Q:** señuelo · **R:** radar · **P:** pausa
- **Objetivo de cada piso:** ① junta las **5 llaves** · ② activa el **generador** (E) · ③ entra al **ascensor** y baja. El ascensor solo abre con las 5 llaves **y** con energía (su luz pasa de roja a verde). Al bajar del último piso escapas.

## Características

- Varios **pisos** temáticos (El Complejo, La Biblioteca, La Enfermería) con habitaciones y un monstruo por piso
- **3 compas** (Nico, Rulo y Checo) que te siguen y disparan solos, con **barra de vida** encima: aguantan **2 zarpazos** del monstruo y al segundo se los lleva **en tu lugar**. Heridos cojean y disparan más lento; se curan solos si el monstruo anda lejos (+2,2 %/s) y +40 % al bajar de piso. El que cae no vuelve
- **Comportamiento de escuadrón**: con calma, uno se adelanta a **revisar** un rincón cercano y vuelve a la formación, los dos trayectos **a paso normal**. Si uno **ve al monstruo y dispara**, si el monstruo hiere a alguno, o si **el monstruo te persigue a ti**, **los tres corren a ayudar**; cuando se aleja, todos regresan contigo
- **Embestida**: de vez en cuando (no más de una cada ~1-1,5 min, y nunca al empezar el piso) el monstruo se olvida de ti y **va expresamente a por un compa**, avisando en pantalla. Mientras embiste, los disparos le frenan menos, así que hay que reaccionar rápido
- **Órdenes al escuadrón** (`C` o el botón COMPAS): alterna entre **CONMIGO** y **CUBRIENDO**, que los deja aguantando el punto donde estabas; ahí solo acuden a un aviso si cae a menos de 170 px
- **Carácter propio**: Nico se adelanta y explora, Rulo se queda atrás y dispara de lejos, Checo apunta mejor (245 px de alcance y más cadencia)
- **Hablan**: bocadillos cortos — "¡a tu espalda!", "casi sin pila", "voy a echar un ojo", "¡ayuda!"
- **Compa derribado**: cuando el monstruo lo deja sin vida y no se lo lleva, queda **malherido en el suelo** sangrando; tienes **20 s** para llegar y levantarlo (**E**). Si el monstruo lo alcanza antes, se lo lleva
- **Eventos de piso** (45 % de las veces): **inundado**, **apagón total** (sin focos hasta el generador) o **niebla** (conos al 62 %)
- El **piso inundado** va con agua de verdad: suelo oscurecido y verdoso, línea de agua contra cada muro, moho en la base de las paredes, lámina de reflejos moviéndose, **ondas que se abren con cada pisada** (tuya, de los compas y del monstruo), **chapoteos** en vez de pisadas secas y goteras del techo. Todos vais al 78 % de velocidad y **al monstruo se le oye llegar mejor** por el agua
- **Resumen de partida** al terminar: tiempo, pisos, llaves, compas perdidos/levantados/rescatados, puntería, golpes, notas y objetos
- **Rescate**: al compa que se lleva el monstruo puedes recuperarlo. Aparece **atado y solo** en una habitación del **piso siguiente**, con dos minis guardándolo. Tienes **ese piso** para llegar hasta él (**E** para soltarlo); si bajas sin rescatarlo, lo pierdes
- **Minis explosivos**: bichos verdes que te detectan a 210 px, **corren hacia ti y revientan** salpicando verde y rojo el suelo **y las paredes**. Un tiro los hace estallar a distancia
- **Vida del jugador**: aguantas **2 zarpazos** del monstruo (3 reventones de mini); el contacto ya no te mata de uno. Se recupera sola si el monstruo anda lejos
- **Rastro de sangre**: tras llevarse a un compa, el monstruo se va herido y va **goteando por los pasillos** unos 25 s
- **Muerte arrastrada** (50 % de las veces): en vez de caer ahí, el monstruo **se lo lleva a la oscuridad** con la linterna encendida dando tumbos, mientras grita, hasta que se apaga
- Cada compa lleva **su propia linterna** con cono direccional: se abren en abanico (izquierda, frente y derecha) y barren el pasillo. Se apagan y encienden **con la tuya (F)**, para que apagar la luz siga sirviendo para esconderse, y **gastan pila al mismo ritmo que la tuya**: igual que a ti, el cono se les va acortando y a 0 no se apaga, se queda al mínimo. Cada **pila** recogida te da +45% y reparte +30% a cada compa
- **Arma de fuego** con munición limitada: los disparos hacen retroceder al monstruo (no lo matan) pero el estruendo **delata tu posición**; cajas de munición repartidas por el piso
- **Botón contextual**: pone DISPARAR normalmente y cambia a ACCIÓN (sin disparar) al tener delante el generador, un armario o la consola
- **Habitaciones con puertas automáticas** que se abren al acercarte tú, tus compas o el monstruo
- **Sala de control** en una esquina de cada piso: su consola de **cámaras** marca en el minimapa dónde están las llaves que faltan, el generador y el ascensor (20 s) y localiza al monstruo (8 s). Reutilizable cada 25 s — no dibuja los pasillos, solo los objetivos
- **Ascensor** para bajar de piso, con cinemática dentro de la cabina
- **Mobiliario** según el escenario: cajas en el complejo, mesas en la biblioteca, camillas en la enfermería
- Suelos y muros con **texturas continuas** (hormigón, tablones de madera, baldosas)
- Laberinto generado al azar; linterna direccional (cono 110°) con parpadeos y apagones
- **La luz atrae al monstruo**: apágala para pasar desapercibido · pilas, armarios, trampas
- Ítems: llave maestra (+2), señuelos, botas (correr), radar (ubica al monstruo 3 s), mapa del piso (dibuja los pasillos en el minimapa)
- **Niebla en el minimapa** (se revela lo explorado) y **generador** que da energía a la puerta
- **Partida guardada**: continúa en el piso donde ibas
- Barra de **cordura** (distorsiona la pantalla), **huellas** y gruñido direccional
- **Focos en las paredes** que parpadean y dan luz alrededor
- **Clima al azar**: lluvia con sonido, truenos y relámpagos que iluminan la escena
- **Eventos de guion**: sustos, mensajes, sangre en paredes, apagones de luz
- **Notas** con historia + **final secreto** si las reúnes todas
- **Logros**, **tabla de récords** por dificultad, **dificultades** (Fácil/Normal/Pesadilla)
- **Menú de opciones** (volumen de música/efectos, brillo, pausa) + **tutorial**
- Cinemáticas: intro, transición de piso, final al escapar y al morir
- Música de fondo y pasos (más rápidos al correr) · soporte de gamepad
