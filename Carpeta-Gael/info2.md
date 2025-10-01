# Métodos para Seleccionar Elementos HTML en JavaScript

- **getElementById(id):** Selecciona un único elemento por su atributo `id`.

const elemento = document.getElementById('mi-id');

- **getElementsByClassName(clase):** Selecciona todos los elementos que tienen una clase específica, devuelve una colección.

const elementos = document.getElementsByClassName('mi-clase');

- **getElementsByTagName(etiqueta):** Selecciona todos los elementos de un tipo de etiqueta, devuelve una colección.

const elementos = document.getElementsByTagName('p');

- **getElementsByName(nombre):** Selecciona todos los elementos cuyo atributo `name` coincide. Útil para formularios.

const inputs = document.getElementsByName('nombre');

- **querySelector(selector):** Selecciona el primer elemento que coincide con un selector CSS.

const primerElemento = document.querySelector('.mi-clase');

- **querySelectorAll(selector):** Selecciona todos los elementos que coinciden con un selector CSS, devuelve una lista de nodos.

const elementos = document.querySelectorAll('div.mi-clase');
