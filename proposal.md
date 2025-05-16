# Propuesta TP DSW

## Grupo
### Integrantes
52450 - Di Bernardo, Franco

### Repositorios
* [frontend app](https://github.com/FDB-52450/proyectoDSW-frontend)
* [backend app](https://github.com/FDB-52450/proyectoDSW-backend)

## Tema
### Descripción
  El sistema a modelar consiste en una página de computación, llamada TECH NEXUS, que vende varios tipos de hardware de computación, como monitores, placas de video, notebooks y demás, inspirado en diferentes paginas de computacion como Hardcore Computacion (https://hardcorecomputacion.com.ar/) o CompraGamer (https://compragamer.com/)
  Los usuarios de la página podrán ser capaces de visualizar todos los productos disponibles (con stock) que ofrece el local, siendo capaces de agregarlos a sus carritos de compras para posteriormente poder realizar un pedido con los mismos.
  Los administradores de la página serán capaces de gestionar los productos, marcas y categorias de la pagina, pudiendo crear, borrar o modificar atributos existentes de los mismos. Además, se encargarán de confirmar la finalización de los pedidos en el sistema.


### Modelo
![(https://github.com/FDB-52450/tp/blob/main/modeloDominio-paginaHardware.png?raw=true)]()

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Marca<br>2. CRUD Categoria<br>3. CRUD Pedido<br>4. CRUD Administrador|
|CRUD dependiente|1. CRUD Producto {depende de} CRUD Marca y CRUD Categoria<br>2. CRUD PedidoProd {depende de} CRUD Producto y CRUD Pedido|
|Listado<br>+<br>detalle| 1. Listado de productos filtrado por nombre, categoria, rango de precio y/o marca => detalle muestra datos completos del producto<br> 2. Listado de pedidos filtrado por numero de pedido, rango de fecha y/o estado => detalle muestra datos completos del pedido|
|CUU/Epic|1. Agregar un producto al carrito<br>2. Finalizar la compra de un pedido|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Marca<br>2. CRUD Categoria<br>3. CRUD Pedido<br>4. CRUD Administrador<br>5. CRUD Producto<br>6. CRUD PedidoProd|
|CUU/Epic|1. Agregar un producto al carrito<br>2. Finalizar la compra de un pedido<br>3. Confirmar pedido hecho con exito|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Listado de productos (para administradores) filtrado por id, nombre y/o stock => detalle muestra datos completos de producto y CRUD producto|
|CUU/Epic|1. Crear producto|
|Otros|1. Uso de imagenes para mostrar productos y marcas|

