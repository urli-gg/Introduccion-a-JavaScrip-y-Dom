##  Que es el manejo de eventos ???

En JavaScript, el manejo de eventos se refiere a la forma en que tu código “escucha” e interactúa con acciones del usuario o del sistema, como:
- Hacer clic en un botón (click)

-   Escribir en un campo de texto (input)

- Pasar el mouse por encima de un elemento (mouseover)

- Cargar la página (load)

-   Presionar una tecla (keydown)

Un evento es simplemente “algo que pasa” en la página, y el manejo de eventos es la lógica que defines para reaccionar a eso.


### Ejemplo básico en JavaScript con DOM

El DOM (Document Object Model) es la representación de la página como una estructura de nodos (árbol). Gracias al DOM puedes seleccionar elementos y añadirles eventos.

```js
<!DOCTYPE html>
<html>
  <body>
    <button id="miBoton">Haz clic aquí</button>

    <script>
      // Seleccionamos el botón en el DOM
      const boton = document.getElementById("miBoton");

      // Añadimos un "manejador de evento"
      boton.addEventListener("click", function() {
        alert("¡Le diste clic al botón!");
      });
    </script>
  </body>
</html>
```
En este ejemplo:

Se selecciona el botón con getElementById.

Se le añade un listener (escuchador de evento) para el evento click.

Cuando ocurre el evento → se ejecuta la función (mostrar alerta).

Resumen rápido:

-    JavaScript maneja eventos para reaccionar a lo que hace el usuario o el navegador.

- El DOM te da acceso a los elementos de la página para poder asignarles esos eventos.

- La función que responde al evento se llama manejador de evento (event handler).
