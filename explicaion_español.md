# Sistema de Inventario
## Buenas tardes o buenos días (depende de cuándo veas esto). Aquí voy a explicar cómo funciona mi programa en Python
### Diagrama de flujo

### Este programa es un script simple de inventario que le pide al usuario algunos datos sobre el producto:
1. ¿Cuál es su nombre?
2. ¿Cuál es su precio?
3. ¿Cuál es su cantidad?

### Luego le pregunta al usuario si quiere ver solo el precio final o los detalles completos de la compra. Si el usuario elige "solo el precio final", el sistema imprime "tienes que pagar...". Pero si elige la otra opción, imprime toda la información completa.

#### ejemplo:
```
¿cuál es el nombre del producto que quieres comprar?
Manzanas
```
```
¿cuál es su precio?
$5.40
```
```
¿cuál es su cantidad?
3
```
```
¿qué quieres ver?

1.el precio final
2.el detalle completo de la compra

2
```
```
Producto: Manzanas
Precio: $5.40
Cantidad: 3
costo total: 16.2
```


### ¿Cómo funciona?
#### Primero, el programa comienza con un bucle ```while true```, lo que significa que el programa seguirá ejecutándose hasta que una condición específica lo detenga.

#### Lo primero que el programa pregunta es cuál es el _nombre del producto_. El usuario introduce el nombre del producto y el programa verifica si el nombre es válido usando la función ```isalpha()```. Esta función revisa la entrada y verifica que solo contenga letras. Si el nombre no es válido, el programa vuelve a pedir el nombre del producto.

#### Luego, el programa pide el _precio del producto_ (el producto seleccionado). Este proceso está dentro de un bloque ```try-except```. El bloque try intenta convertir la entrada en un número tipo float, por lo que si el usuario introduce un valor inválido como un string (texto), el programa captura el error y vuelve a pedir el precio del producto. También verifica que el precio no sea un valor negativo.

#### Después de eso, el programa pide _la cantidad del producto_ (usando un proceso de validación similar), convierte la entrada en un número entero y verifica que no sea un número negativo.

#### Una vez que el programa tiene el precio y la cantidad, calcula el costo final multiplicando el precio por la cantidad.

#### Finalmente, el programa le pregunta al usuario qué información quiere ver. Puede elegir entre ver solo el costo final o el detalle completo de la compra. Dependiendo de la elección del usuario, el programa muestra el resultado correspondiente.
