## 1. Crear un archivo HTML

Abre tu editor de texto o IDE preferido (como Visual Studio Code, Sublime Text, o incluso el bloc de notas) y crea un nuevo archivo llamado `ejercicio.html`.

---

## 2. Estructura base del archivo

Copia y pega la siguiente estructura básica HTML en tu archivo:

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Ejercicio simple DOM</title>
</head>
<body>
  </body>
</html>
```

---

## 3. Agregar el párrafo al `<body>`

Dentro de la etiqueta `<body>`, agrega el siguiente párrafo con un identificador. El atributo `id="miParrafo"` es fundamental porque nos permite seleccionar este elemento desde JavaScript.

```html
<p id="miParrafo">Este es el texto original.</p>
```

---

## 4. Agregar el botón al `<body>`

Justo debajo del párrafo, añade el botón que activará el cambio.

```html
<button id="btnCambiar">Cambiar Texto y Color</button>
```

---

## 5. Insertar el script JavaScript

Al final del `<body>`, justo antes de la etiqueta de cierre `</body>`, añade el siguiente código JavaScript. Esto asegura que el script se ejecute después de que los elementos HTML (párrafo y botón) se hayan cargado.

```javascript
<script>
  // Seleccionar el párrafo usando su id
  const parrafo = document.getElementById("miParrafo");

  // Seleccionar el botón usando su id
  const boton = document.getElementById("btnCambiar");

  // Escuchar el evento click en el botón y cambiar el texto y estilo del párrafo
  boton.addEventListener("click", function() {
    parrafo.textContent = "El texto ha sido cambiado!";
    parrafo.style.color = "blue";
  });
</script>
```

---

## 6. Guardar y probar el ejercicio

1.  **Guarda** el archivo `ejercicio.html`.
2.  **Ábrelo** en tu navegador web (puedes hacer doble clic sobre el archivo).
3.  Al abrirlo, verás el texto original y el botón.
4.  Cuando presiones el botón "Cambiar Texto y Color", el texto del párrafo cambiará a "El texto ha sido cambiado!" y su color se volverá azul.
