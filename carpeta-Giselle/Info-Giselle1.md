## Estructuras de control: Condicionales y Ciclos en Java

Son las instrucciones que permiten decidir qué código ejecutar y cuántas veces repetirlo

- Condicionales: if/else, switch, operador ternario.

- Ciclos: while, do…while, for, foreach.

```js
public class EjemploCondicionales {
    public static void main(String[] args) {
        int edad = 20;

        // if - else if - else
        if (edad < 13) {
            System.out.println("Eres un niño");
        } else if (edad < 18) {
            System.out.println("Eres un adolescente");
        } else {
            System.out.println("Eres un adulto");
        }

        // switch
        int dia = 6; // 1 = lunes ... 7 = domingo
        switch (dia) {
            case 1:
                System.out.println("Es lunes");
                break;
            case 6:
                System.out.println("Es sábado");
                break;
            case 7:
                System.out.println("Es domingo");
                break;
            default:
                System.out.println("Es un día entre semana");
        }

        // operador ternario
        String permiso = (edad >= 18) ? "Tienes permiso para conducir" : "No puedes conducir";
        System.out.println(permiso);
    }
}
```
### ¿Qué está haciendo?

- if – else if – else: Clasifica la edad y decide si eres niño, adolescente o adulto.
Sirve para evaluar rangos o condiciones múltiples.

- switch: Dependiendo del número del día, imprime si es lunes, sábado, domingo o entre semana.
Sirve cuando hay muchas opciones fijas de un mismo valor.

- Operador ternario: Evalúa en una sola línea si puedes o no conducir según la edad.
Sirve para asignaciones rápidas de valores.

## Los condicionales permiten tomar decisiones en el flujo del programa.


```js
public class EjemploCiclos {
    public static void main(String[] args) {
        
        // while
        int i = 1;
        while (i <= 3) {
            System.out.println("while: número " + i);
            i++;
        }

        // do...while
        int j = 1;
        do {
            System.out.println("do...while: número " + j);
            j++;
        } while (j <= 3);

        // for
        for (int k = 1; k <= 3; k++) {
            System.out.println("for: número " + k);
        }

        // foreach (for mejorado)
        int[] numeros = {10, 20, 30};
        for (int n : numeros) {
            System.out.println("foreach: valor " + n);
        }
    }
}
```
### ¿Qué está haciendo?

- while: Empieza con i = 1 y repite hasta que i <= 3. Imprime 1, 2, 3. Sirve cuando no sabemos cuántas veces se repetirá y depende de una condición.

- do…while: Hace lo mismo, pero garantiza al menos una ejecución aunque la condición sea falsa.
Útil para menús o validaciones que deben mostrarse al menos una vez.

- for: Usa un contador k que va de 1 a 3 e imprime los números.
Sirve cuando sabemos exactamente cuántas veces queremos repetir.

- foreach (for mejorado): Recorre directamente un arreglo ({10,20,30}) y muestra sus valores. Sirve para recorrer colecciones y arreglos de manera sencilla.

## Los ciclos permiten repetir acciones de forma controlada.