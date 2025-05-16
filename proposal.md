# Propuesta TP DSW

## Grupo
### Integrantes
52450 - Di Bernardo, Franco

### Repositorios
* [frontend app](https://github.com/FDB-52450/proyectoDSW-frontend)
* [backend app](https://github.com/FDB-52450/proyectoDSW-backend)
*Nota*: si utiliza un monorepo indicar un solo link con fullstack app.

## Tema
### Descripción
*2 a 6 líneas describiendo el negocio (menos es más)*

### Modelo
![imagen del modelo]()

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Marca<br>2. CRUD Categoria<br>3. CRUD Pedido<br>4. CRUD Administrador|
|CRUD dependiente|1. CRUD Producto {depende de} CRUD Marca y CRUD Categoria<br>2. CRUD PedidoProd {depende de} CRUD Producto y CRUD Pedido<br>3. CRUD HistorialPrecio {depende de} CRUD Producto<br>4. CRUD Carrito {depende de} CRUD Producto|
|Listado<br>+<br>detalle| 1. Listado de productos filtrado por categoria, rango de precio y marca => detalle CRUD Habitacion<br> 2. Listado de pedidos filtrado por numero de pedido, rango de fecha y estado|
|CUU/Epic|1. Agregar un producto al carrito<br>2. Finalizar la compra de un pedido|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Marca<br>2. CRUD Categoria<br>3. CRUD Pedido<br>4. CRUD Administrador<br>5. CRUD Producto<br>6. CRUD PedidoProd<br>7. CRUD HistorialPrecio<br>8. CRUD Carrito (solo memoria)|
|CUU/Epic|1. Agregar un producto al carrito<br>2. Finalizar la compra de un pedido<br>3. Confirmar pedido hecho con exito|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|

