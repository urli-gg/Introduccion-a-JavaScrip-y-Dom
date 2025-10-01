# Introducción a JavaScript y el DOM

## ¿Cómo obtener o modificar contenido de un elemento HTML? 
“Para obtener o modificar el contenido de un elemento HTML con JavaScript, usamos principalmente dos propiedades: textContent y innerHTML.

textContent sirve para leer o cambiar el texto puro de un elemento, es decir, solo las palabras, sin HTML dentro. Por ejemplo, si tenemos este párrafo:

![Codigo1](./Imagenes/290.png)

Podemos acceder y modificar su texto así:

![Codigo2](./Imagenes/291.png)

Lo que hace este código es: primero seleccionamos el párrafo con (getElementById.) Después, al usar (parrafo.textContent = 'Nuevo texto simple';) cambiamos lo que se ve, poniendo solo texto, sencillo, sin formato especial.

Por otro lado, innerHTML se usa cuando queremos leer o modificar el contenido incluyendo etiquetas HTML, como negritas, enlaces, imágenes, etc. Usando el mismo párrafo:

![Codigo3](./Imagenes/292.png)

Aquí no solo cambiamos el texto, sino que también le decimos al navegador que esa parte debe ir en negritas, gracias a la etiqueta <b>. O sea, con innerHTML, podemos darle formato y estructura al contenido.
