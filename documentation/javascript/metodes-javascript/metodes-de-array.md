# Métodes de array

## Método reduce

El méotdo **reduce** sirve para acumular un valor 

```
const array1 = [1, 2, 3]
function acumular(acumulador, siguienteNumero) {
   return acumulador + siguienteNumero
}
const sumaTotal = array1.reduce(acumular)
```
La función **acumular** se va a invocar 3 veces, una por cada elemento del array.
En el parámetro **acumulador** se va a ir guardando el valor correspondiente a la **evaluación del return de la línea 8**
Es decir, acumulador pasará a valer: 1, luego 3, y luego 6

### Caso práctico

Imaginar que tenemos en un array el total de gastos de una factura.
Podríamos utilizar el método **reduce** para sumar todos sus valores.

```
const gastos = [13.99, 11.00, 5.00]
const reducer = (accumulator, currentValue) => accumulator + currentValue;
const gastoTotal = gastos.reduce(reducer)
```

## Referencias

[Ejemplos Mozilla Método Reduce](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Objetos_globales/Array/reduce)



