# Operation Cortex — cambios de esta revisión

- El modo de mundo abierto vuelve a ejecutar el juego Three.js incluido en el proyecto; se elimina el iframe externo que impedía corregir la física.
- Personaje 3D articulado con cabeza, rostro sencillo, pelo estilizado, chaqueta, pantalones, botas, brazos y piernas separados; las extremidades se animan al andar.
- Movimiento con WASD/flechas, sprint con Shift, salto con Espacio, dash y joystick táctil.
- Movimiento diagonal normalizado, seguimiento de cámara suavizado, gravedad y apoyo en el suelo/plataformas de salto.
- Botón de pantalla completa y adaptación a móvil.
- Se conserva el sistema de tres portales cognitivos y el guardado local de resultados.

## Comprobaciones realizadas

- `node --check world3d.js`
- `node --check app.js`
- `node --check games-arcade.js`
- `node --check server.mjs`

No se pudo ejecutar una prueba visual automatizada del navegador desde este entorno. Three.js se carga desde cdnjs, por lo que la primera carga del mundo 3D necesita conexión a internet. El personaje es una versión 3D articulada inspirada en el storyboard; no es una réplica facial exacta del dibujo/fotograma.
