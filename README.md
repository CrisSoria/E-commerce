### [Live Site](https://compu-henry.netlify.app)

# E-commerce Compu Henry

Página web para venta de insumos informáticos con todas las funcionalidades de un e-commerce.
Trabajo en equipo de 7 personas utilizando metodologías ágiles
(SCRUM). Un mes de duración total, con springs semanales
presentados a un Product Owner.

<img align="right" alt="img" src="https://i.ibb.co/rwk20kr/ecommerce.png" width="50%" height="auto" />

## Objetivos del Proyecto

- Construir una App JavaScript desde cero.
- Afirmar y conectar los conceptos aprendidos en la carrera.
- Aprender mejores prácticas.
- Aprender y practicar el workflow de GIT.
- Utilizar Metodologías Ágiles.
- Trabajar en equipo.
- Usar y practicar testing.

<br/> 
<hr/>

<img src="https://i.ibb.co/5nz078q/ecomm-favs.png" alt="ecomm-favs" border="0" width="49%" ><img src="https://i.ibb.co/6g4YN8S/ecom-login.png" alt="ecom-login" border="0" width="49%">

<br/> 
<hr/>
<br/> 
<br/> 
<img src="https://i.ibb.co/Fq2Vy9L/ecomm-armar-PC.png" alt="ecomm-armar-PC" border="0" width="32%" align="right" >

<p aling="center">
Uno de las principales problemáticas para la venta de insumos informáticos, es el desconocimiento por parte del comprador frete a la amplia gama de opciones existentes para satisfacer sus necesidades.
Para ello ideamos un sistema de productos asociados compatibles. Permitiendo así a cualquier usuario armar su computadora independientemente de sus conocimietos en cuestiones de hadware.
</p>
  
<br/> 
<br/> 
<br/>

<br/> 
<hr/>
<br/>

<span style="display:block">

<img src="https://i.ibb.co/ggt95G1/ecomm-carrito.png" alt="ecomm-carrito" border="0" width="69%" >
<img src="https://i.ibb.co/SJg4K4V/ecomm-mercado-Pago.png" alt="ecomm-mercado-Pago" border="0" width="29%" >
</span>

<br/> 
<hr/>
<br/>

### Usuarios no Autenticados

Un Visitante anónimo debería poder navegar tu e-commerce, ver y buscar productos.

###### Como un Guest yo puedo...

- PRODUCTOS:

  - ...ver la lista completa de productos (catálogo), para ver todo lo disponible para comprar.
  - ...refinar el listado por categorías, para poder ver los items en los que estoy interesado.
  - ...buscas productos, para poder encontrar rápido los productos que quiero comprar.
  - ...ver los detalles de un producto individual (incluida las fotos, descripciones, reviews, etc...), asi puede determinar si quiero ese producto o no.

- CARRITO:
  - ...poder agregar items a mi carrito de compras desde el listado o desde a página de detalles de un producto, para poder comprarlos despues.
  - ...sacar items de mi carrito, en caso que decida no quererlos.
  - ...editar cantidades de los items de mi carrito, en caso que quiera mas o menos cantidad de un item en particular.
  - ...refrescar la página, o irme y volver, y todavía tener mi carrito de compras (sin haberme creado una cuenta). (Podés usar sessionStorage, localStorage, cookies, o JWT).
  - ...poder crearme una cuenta, loguearme y seguir editando ese mismo carrito, asi no pierdo los items seleccionados.
- CHECKOUT:
  - ...poder comprar todos los items de un mi carrito.
  - ...especificar una dirección de envio y un email cuando hago el checkout, asi me envien la compra a lugar que dije.
  - ...recibir un email de confirmación que hice la compra.
  - ...recibir un email de notificación cuando la orden fue despachada.
- GESTION DE CUENTA:
  - ...poder crear una cuenta, asi puede hacer otras cosas como dejar un review.
  - ...poder logearme usando Google o Github, para no tener que acordarme de un password nuevo.

### Usuarios Autenticados

Los usuarios que hayan creado su cuenta, podrán hacer todo lo que puede hacer un usuario guest y además:

###### Como un Usuario Autenticado yo puedo...

- GESTION DE CUENTA:
  - ...poder desloguearme, asi nadie más pueda usar mi sesión.
  - ...ver el historial de ordenes previas, asi puede reever las ordenes que hice en el pasado.
  - ...ver los detalles de una orden que hice en el pasado, incluyendo:
    - Los items comprados, con sus cantidades.
    - Links a la página del producto comprado.
    - Fecha y hora de la compra.
- REVIEWS:
  - ...poder dejar reviews a los productos, que incluyan texto y un sistema de cinco estrellas.

### Admin

Los usuarios administradores pueden manejar el sitio, los productos que se listan y los items que están disponibles.

###### Como un administrador yo puedo...

- GESTION DE PRODUCTOS:

  - ...poder crear y editar productos, con nombre, descripción, precio y uno o más fotos, tal que los visitantes puedan ver la última información de lo que se vende.
  - ...poder crear categorías, para que los usuarios puedan filtrar los items.
  - ...poder agregar o sacar categorías de los items (los items deben poder aceptar múltiples categorías).
  - ...gestionar la disponibilidad de un item. (un item que no esta disponible, no deberá estar listado en la página, pero su detalle debe seguir siendo accesible desde el historial de compras o con su URL, pero debe mencionar que el item no está disponible).

- GESTION DE ORDENES:

  - ...poder ver una lista de todas las ordenes, para poder ver y revisar las ordener.
  - ...poder filtrar as ordenes por su estado (creada, procesando, cancelada, completa).
  - ver los detalles de una orden específica, asi puedo revisarla y actualizar su estado.
  - ...poder cambiar el estado de una orden (creada => procesando, procesando => cancelada || completa).

- GESTION DE USUARIOS:
  - ...poder hacer que un usuario se convierta en admin.
  - ...borrar a un usuario, asi no puedan logearse más.
  - ...forzar una password reset para un usuario.
