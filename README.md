# Godot

## Introducción a Godot

Godot es un motor de juegos que utiliza una estructura de nodos para componer los elementos del juego. Cada nodo cumple una función específica dentro del juego y se organiza en un árbol de nodos, donde los árboles de nodos se conocen como escenas. Las escenas pueden ser manejadas de manera aislada para un manejo modular y también se pueden introducir escenas dentro de otras escenas.

## Configuración del Proyecto en Godot

Para configurar el tamaño del viewport en Godot, sigue estos pasos:

1. Ve a `Proyecto` > `Configuración de Proyecto`.
2. En la pestaña `Ventana`, puedes cambiar el ancho y alto del viewport, así como otras opciones adicionales.

## Nodos en Godot

Los nodos son los componentes fundamentales en Godot:

- Selecciona la opción de `Nodo` en la parte derecha de la ventana.
- Elige el tipo de nodo adecuado para tu necesidad.
- En el inspector, puedes asignar texturas arrastrando tus activos y manejar la transformación del nodo para ajustar su posición, rotación y escala.

## Relaciones de Nodos

- Toda escena en Godot parte de un nodo raíz, que actúa como padre de todos los nodos dentro de la escena.
- Los nodos hijos heredan transformaciones del nodo padre, pero los cambios en los nodos hijos no afectan al padre.

## Métodos en Godot

- `_ready()`: Se ejecuta al iniciar la escena y es útil para inicializar variables o mostrar mensajes.
- `_process()`: Se ejecuta una vez por frame, es decir, cada vez que se actualiza la pantalla.
- `_physics_process(delta)`: Se ejecuta en cada actualización de las físicas, donde `delta` representa el tiempo entre las ejecuciones.

## Movimiento en Godot

- `move_and_slide()`: Método para mover un nodo basado en la velocidad asignada y resolver colisiones con deslizamiento.
- `move_and_collide()`: Método similar a `move_and_slide()` pero detiene el cuerpo al colisionar y proporciona información sobre la colisión.

## Otros Conceptos

- `Delta`: Representa el tiempo entre ejecuciones sucesivas de `_physics_process()`, útil para sincronizar la física del juego.
- `Randi`: Método para generar un número entero aleatorio positivo.
- `Area2D`: Nodo que funciona como un trigger, activando ciertas acciones cuando algo entra en su área.
- `Signals`: Eventos manejados en Godot.

## Atajos Útiles

- Puedes presionar `F5` para ejecutar el proyecto.
