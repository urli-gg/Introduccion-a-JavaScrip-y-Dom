# Como aplicar estilos _**CSS**_ dinámicamente a un elemento _**HTML**_?

Para aplicar estilos CSS dinámicamente a un elemento HTML es necesario usar JavaScript, lo que permite modificar visualmente cualquier elemento de la página en tiempo real, en respuesta a eventos o condiciones.

Supongamos que, por algún motivo, quiero que este párrafo que estás leyendo pase a tener un fondo de color fucsia. Pongamos que su HTML es algo así:

```js
<p id="intro">Para aplicar estilos CSS…</p>
var intro = document.getElementById('intro');
intro.style.backgroundColor = '#cb00fdff';
```
Para ejecutar la línea de código anterior sería de esta fomra:

```js
<p id="intro" style="background-color: rgba(247, 0, 255, 1);">
Para aplicar estilos CSS...
</p>
```
En dado caso que queramos borrar todo rastro de color, se le asigna null a la propiedad, e.j:

```js
intro.style.backgroundColor = null;
```
Modificar una propiedad directa:
Utiliza el atributo style sobre el elemento:

```js
document.getElementById('miElemento').style.color = '#cb00fdff';
```
Esto hace que cambie el color del texto con el id "miElemento" a rosa.

Ejemplo con un boton:

```js
<button id="btn">Clic</button>
<script>
document.getElementById('btn').onclick = funtion() {this.style.backgroundColor = 'black';}
</script>
```

En caso de que queramos cambiar el color del texto, su tamaño y el tipo de letra sería de esta foma:

```js
document.getElementById('miElemento').style.color = 'blue'; 
document.getElementById('miElemento').style.fontFamily = 'Arial';
document.getElementById('miElemento').style.fontSize = '18px';
```

Aqui con el ejemplo del botón añadido

```js
<button id="btn">Clic</button>
<p id="texto">Este es el texto</p>

<script>
  document.getElementById('btn').onclick = function() {
    const texto = document.getElementById('texto');
    texto.style.color = 'white';
    texto.style.fontWeight = 'bold';
    texto.style.fontFamily = 'Verdana';
    texto.style.backgroundColor = 'black';
  }
</script>
```

Entrellaves. (2018, diciembre 2). *Tres técnicas sencillas para cambiar estilos CSS con Javascript*. Recuperado de https://entrellaves.com/javascript/cambiar-css-con-javascript

[Chat con IA](https://www.perplexity.ai/search/como-aplicar-estilos-css-dinam-OhnhKkeEScmp7j8LTjin_w#7) 
