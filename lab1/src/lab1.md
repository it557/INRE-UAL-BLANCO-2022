### ***Actividades***

---

#### **Supuesto 1: Horarios➡️**
En una universidad, el personal del PDI, el personal del PAS y los estudiantes pueden consultar horarios. Por su parte, el personal del PAS puede modificar horarios y dar de alta estudiantes. El personal de PDI puede proponer cambios en los horarios y dar de alta estudiantes. La funcionalidad de dar de alta estudiantes del PAS realiza una verificación de los datos del estudiante. Sin embargo, la funcionalidad de dar de alta estudiantes del PDI, además de verificar los datos también permite de forma excepcional realizar la búsqueda en las listas de clase de sus asignaturas.

![Supuesto 1: Horarios](/out/lab0/src/horarios/horarios.svg)
|| |
|-|:-:|
|**ID:**|UC-00|
|**Nombre:**|Modificar Horario|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PAS modificar el horario|
|**Actor:**|PAS|
|**Precondiciones:**|Pertenecer al PAS de esta institucion|
|**Flujo normal:**|Acceder al horario <br> hola|
|**Flujo aternativo:**|Ninguno|
|**Postcondiciones:**|Ninguna|
||


|| |
|-|:-:|
|**ID:**|UC-01|
|**Nombre:**|Dar de alta estudiantes|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PAS <br> dar de alta a los estudiantes|
|**Actor:**|PAS|
|**Precondiciones:**|Pertenecer al PAS de esta institucion|
|**Flujo normal:**|Dar de alta estudiantes|
|**Flujo aternativo:**|No existe el estudiante|
|**Postcondiciones:**|El estudiante ya no esta registrado|

|| |
|-|:-:|
|**ID:**|UC-03|
|**Nombre:**|Validar datos|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PAS modificar el horario|
|**Actor:**|PAS|
|**Precondiciones:**|Pertenecer al PAS de esta institucion|
|**Flujo normal:**|1 Dar de alta estudiantes <br> 2 Validar los datos|
|**Flujo aternativo:**|Ninguno|
|**Postcondiciones:**|Ninguna|
||

|| |
|-|:-:|
|**ID:**|UC-06|
|**Nombre:**|Consultar Horario|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PAS modificar el horario|
|**Actor:**|Estudiante|
|**Precondiciones:**|Ser un estudiante de esta institucion|
|**Flujo normal:**|Consultar el horario|
|**Flujo aternativo:**|Ninguno|
|**Postcondiciones:**|Ninguna|
||
#### **Supuesto 2: Sistema de compras➡️**
En un sistema de compra, existen cuatro tipos de usuarios: comprador, vendedor, proveedor y administrador. Los compradores pueden agregar productos, consultar precios, finalizar la compra y consultar ofertas. Agregar productos implica marcar esos productos como bloqueados. Los vendedores también pueden consultar ofertas y consultar precios. Los proveedores pueden consultar precios, avisar de nuevos productos y consultar ofertas. Avisar de nuevos productos, de forma excepcional, realiza la incorporación de una oferta. Los proveedores también tienen una funcionalidad para avisar del fin de una oferta. Cuando se avisa del fin de una oferta, se ejecuta la funcionalidad de eliminar la oferta. Ambas funcionalidades de avisar del proveedor tienen en común que se encarga de enviar una notificación. Los administradores pueden consultar precios, consultar ofertas y eliminar productos. La funcionalidad de consultar precios incluye una funcionalidad de buscar productos que es similar a la funcionalidad de consultar productos de los compradores. Sin embargo, la funcionalidad de consultar productos añade una funcionalidad para verificar la disponibilidad. Para realizar una venta, un comprador y un vendedor participan de forma conjunta. En dicha operación, se lleva a cabo el acuerdo de un precio; excepcionalmente, durante la realización de la venta, se consultará el histórico de ventas.

![Supuerto 2: Sistema de Compras](/out/lab0/src/SistemaDeCompras/SistemaDeCompras.svg)
| |  |
| ---| :---: |
| **ID**| UC-03 |
| **Nombre**| ConsultarProducto|
| **Fecha**| 07/10/2022 |
| **Autor**| Ioan Stefan Toderic |
| **Descripcion**| Permite consultar el historico de ventas  |
| **Actores**| Comprador |
| **Precondiciones**| El usuario debe estar logueado como productor |
| **Flujo Normal**|  1. El actor  pulsar el botón de Consultar productos para ver la lista de los productos <br> 2. El actor visualiza la disponibilidad del producto <br> 3. El actor busca el producto en el formulario de busqueda <br> 4. El sistema busca el prodcto en la tabla de producto <br> 5. Se comprueba la disponibildad del producto <br> 6. Si el producto esta disponible se le muestr al actor|
| **Flujo Alternativo** | 4B. El producto no esta disponible, por lo que se le muestra al actor un mensaje de la no disponibilidad del producto |
|**Postcondiciones**| |
|**Referencias**| UC-01, UC-09 |



| | |
| ----------- | :-----------: |
| **Identificador**: | UC-02 |
| **Nombre:** | IncorporarOferta |
| **Fecha:** | 30/09/2022 |
|  **Autor:** | Toderic Ioan Stefan |
|  **Descripcion:** | Boton opcional para incorporar una oferta   |
|  **Actores:** | Administrador |
|  **Precondiciones:** | El usuario debe estar logueado como administrador|
|  **Flujo normal:** | 1. El actor busca el producto en el formulario <br> 2. Si se le incorpora la oferta, el producto se vera modificado el precio y se guarda con oferta|
|  **Flujo alternativo:** | 2.B Si no se incorpora la oferta el producto se guarda sin oferta |
|  **Postcondiciones:** | Modificar el precio del producto |
| **Referencias**|UC-08|



| | |
| ----------- | :-----------: |
|  **Identificador:**| UC-04 |
|  **Nombre:** | FinalizarCompra |
|  **Fecha:** | 30/09/2022 |
|  **Autor:** | Guillermo Morales Caparros |
|  **Descripcion:**| Termina la compra y da informacion sobre la compra realizada |
|  **Actores:**| Comprador |
|  **Precondiciones:** | Debe existir el producto |
|  **Flujo normal:** | 1- El comprador pulsa el boton de finalizar|
| | 2- El sistema cierra la vision de compra|
| | 3- Se muestra una pestaña nueva con los productos comprados y su precio correspondiente|
|  **Flujo alternativo:** | Ninguno |
|  **Postcondiciones:** |  |


| |  |
| ---| :---: |
|  **ID**| UC-05|
|  **Nombre** | RealizarVenta |
|  **Fecha** | 13/10/2022 |
|  **Autor** | Luca Daniel Gavriloaie|
|  **Descripcion** | Permite realizar un venta |
|  **Actores** | Comprador, Vendedor |
|  **Precondiciones** | El comprador y el vendedor deben estar autenticados en el Sistema |
|  **Flujo Normal** | 1. El comprador elige el producto que desea comprar y lo anade al carrito de compra <br> 2. El comprador comienza el proceso de tramitación del pedido <br> 3. El vendedor busca el producto en el sistema <br> 4. El vendedor verifica la disponibilidad del producto <br> 5. El comprador y el vendedor se ponen de acuerdo en un precio <br> 6. El comprador y el vendedor finalizan el trámite del pedido |
|  **Flujo Alternativo** | 4A. Si el producto no está disponible, el vendedor recibe una notificación de la circunstancia y se lo notifica al comprador. El proceso termina <br> 4B. Los actores pueden consultar si lo desean el histórico de ventas del producto <br> 5A. Si no se llega a un acuerdo con respecto al precio, el proceso se cancela. |
| **Postcondiciones** | El stock del producto vendido disminuye y se actualiza el histórico de ventas del mismo |
| **Referencias** | UC-01, UC-10 |


| | |
| ----------- | :-----------: |
| **Identificador**: | UC-06 |
| **Nombre:** | EliminarProducto |
| **Fecha:** | 30/09/2022 |
|  **Autor:** | Guillermo Morales Caparros |
|  **Descripcion:** | Permite eliminar un producto  |
|  **Actores:** | Administrador |
|  **Precondiciones:** | Debe existir el producto |
|  **Flujo normal:** | 1- El actor pulsa el boton para eliminar el producto|
| | 2- Aparece un mensaje de "producto eliminado"|
| | 3- El administrador selecciona "aceptar" y vuelve la pantalla inicial|
|  **Flujo alternativo:** | Ninguno |
|  **Postcondiciones:** | El producto debe desaparecer |
| **Referencias**||

| |  |
| ---| :---: |
|  **ID**| UC-07|
|  **Nombre** | AvisarFinDeOferta |
|  **Fecha** | 13/10/2022 |
|  **Autor** | Luca Daniel Gavriloaie|
|  **Descripcion** | El proveedor avisará a los usuarios del sistema sobre el fin de una oferta |
|  **Actores** | Proveedor |
|  **Precondiciones** | El proveedor debe estar autenticado en el sistema |
|  **Flujo Normal** | 1. El proveedor comprueba el estado de la oferta <br> 2. Si la fecha del fin de la oferta está cerca, el proveedor emitirá un aviso para todos los usuarios en forma de notificación <br> 3. El proveedor eliminará la oferta |
|  **Flujo Alternativo** |  |
| **Postcondiciones** |  |
| **Referencias** |  |




#### **Supuesto 3: Compañía hotelera➡️**
En una compañía hotelera, el administrador y el comercial pueden consultar reservas. El comercial realiza ofertas y gestiona nuevas reservas. El administrador gestiona nuevas peticiones y también realiza ofertas. La realización de ofertas por parte del comercial conlleva un recálculo de precios. Además, dicha realización de ofertas conlleva opcionalmente el bloqueo temporal de una reserva. Los clientes, los administradores y los comerciales pueden consultar disponibilidades y visualizar ofertas. La consulta de disponibilidades y la consulta de reservas tienen la funcionalidad común de buscar elementos. Por su parte, la consulta de disponibilidades conlleva una funcionalidad que muestra un calendario.

![Supuesto 3: Compañía hotelera](/out/lab0/src/companiaHotelera/companiaHotelera.svg)


#### **Supuesto 4: Fotografía Online➡️**
En una aplicación de fotografía online, los clientes pueden visualizar las fotos, donde de forma excepcional se puede realizar una denuncia sobre la foto. Al denunciar una foto, se ha de introducir una explicación sobre la denuncia. Los clientes también pueden llevar a cabo consultas sobre las fotos, operación que es un caso particular de visualizar las fotos. Los controladores de fotos pueden indicar que una foto debe ser revisada. Esta funcionalidad es un caso general de la funcionalidad de denunciar foto. Además, los controladores también pueden editar la información de las fotos. En esta aplicación también participan usuarios de tipo vendedor. Los vendedores pueden escribir a los clientes para hacerles ofertas sobre los productos de la aplicación. De forma excepcional, al hacer una oferta pueden reducir el precio de un producto. Los vendedores también pueden buscar detalles en las fotos, operación que es un caso particular de visualizar fotos. Pero esa búsqueda conlleva la verificación de los datos introducidos. Por otro lado, los gestores de la aplicación pueden ver ofertas, bloquear ofertas, emitir facturas y editar facturas. La emisión de facturas requiere la participación de un software de facturación. El administrador de la tienda puede ver ofertas, emitir facturas, editar facturas, bloquear ofertas, crear usuarios y editar usuarios. Esta funcionalidad de ver ofertas también la pueden realizar los clientes. Editar usuarios tiene características en común con editar facturas. Crear usuarios conlleva el envío de un email en el que es necesario el uso de un gestor de correo.

![Supuesto 4: Fotografía Online](/out/lab0/src/fotografiaOnline/fotografiaOnline.svg)


#### **Supuesto 5: Gestión de Incidencias➡️**
En un sistema de gestión de incidencias, los técnicos y los operadores pueden dar de alta incidencias, para lo cual, de forma excepcional se enviará un correo (en esta operación participa un sistema de gestión de correo). Los técnicos también atienden llamadas telefónicas y realizan informes sobre las incidencias. Por su parte, los operadores atienden llamadas telefónicas, marcan incidencias como duplicadas y ordenan incidencias. La forma de atender llamadas de los técnicos y los operadores no es exactamente igual, pero tiene similitudes. De forma específica, cuando los técnicos atienden llamadas, comprueban datos de la incidencia en el sistema. Cuando los operadores atienden llamadas, introducen nuevos datos de la incidencia. Los administradores del sistema gestionan categorías de incidencias, consultan incidencias y ordenan incidencias. La ordenación por parte de los administradores conlleva la adición de un comentario. Los técnicos y los operadores también pueden consultar incidencias. La consulta de incidencias por parte técnicos, operadores y administradores puede conllevar, de forma excepcional, la edición de los datos de la incidencia. Los usuarios invitados también pueden consultar incidencias, pero sin la posible edición de los datos. Además, los invitados informan sobre posibles incidencias, se pueden registrar para ver notificaciones y pueden acceder a un listado del histórico de notificaciones. El informe de posibles incidencias conlleva el dar de alta la localización en un mapa, la incorporación de una explicación completa en formato textual y la subida de una foto.

![Supuesto 5: Gestión de Incidencias](../../out/lab0/src/gestionDeIncidencias/gestionDeIncidencias.svg)