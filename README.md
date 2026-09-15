Ejercicio 2.E.1 09 - Producto y Carrito de Compras

Lógica del programa
Para este ejercicio, trabajé con la interacción entre dos clases distintas: `Producto` y `CarritoDeCompras`.

Primero, diseñé la clase `Producto` aplicando el concepto de encapsulamiento. Definí los atributos privados `nombre` (String) y `precio` (double), y armé su respectivo constructor junto con los métodos *getters* y *setters* para acceder a la información de forma segura.

Luego, desarrollé la clase `CarritoDeCompras`. Acá utilicé un `ArrayList` llamado `productos`, diseñado específicamente para almacenar objetos del tipo `Producto`. En el constructor, me aseguré de inicializar esta lista vacía para poder empezar a usarla.

Para el comportamiento del carrito, implementé tres métodos:
1. `agregarProducto(Producto producto)`: Recibe un objeto de tipo `Producto` por parámetro y lo añade directamente a la lista dinámica.
2. `calcularTotal()`: Utiliza un bucle `for-each` para recorrer la lista de productos. En cada iteración, obtiene el precio del producto actual (usando el método `getPrecio()`) y lo acumula en la variable `total`, retornando el monto final.
3. `mostrarDetalle()`: Imprime un listado en pantalla iterando sobre los productos guardados y, al finalizar la lista, llama al método `calcularTotal()` para mostrar el importe final a abonar.

Dentro del método `main`, desarrollé la siguiente lógica de prueba:
1. Instancié un objeto `CarritoDeCompras`.
2. Instancié tres objetos `Producto` independientes (Ramen, Pepsi y Salchichas) pasándoles su nombre y precio correspondiente al constructor.
3. Agregué los tres productos al carrito usando el método `agregarProducto()`.
4. Llamé al método `mostrarDetalle()` para imprimir en consola el ticket de la compra y comprobar que ambas clases interactúan correctamente.

Ejecución en consola
<img width="1366" height="723" alt="imagen" src="https://github.com/user-attachments/assets/cb2fb69c-1a5d-4fc2-958b-a4df85cd56a3" />
