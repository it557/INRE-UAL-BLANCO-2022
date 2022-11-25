## ***Actividades***

---

### **Supuesto 1: Horarios➡️**
En una universidad, el personal del PDI, el personal del PAS y los estudiantes pueden consultar horarios. Por su parte, el personal del PAS puede modificar horarios y dar de alta estudiantes. El personal de PDI puede proponer cambios en los horarios y dar de alta estudiantes. La funcionalidad de dar de alta estudiantes del PAS realiza una verificación de los datos del estudiante. Sin embargo, la funcionalidad de dar de alta estudiantes del PDI, además de verificar los datos también permite de forma excepcional realizar la búsqueda en las listas de clase de sus asignaturas.

![Supuesto 1: Horarios](/out/lab0/src/horarios/horarios.svg)

<br>

>#### **Definición de requisitos de información**
| |  |
| ---| :--- |
|  **ID** | IR-01 |
| **Nombre** | Horario |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-07) Consultar horario <br> - (UC-01) Modificar horario <br> - (UC-03) Proponer cambios en los horarios|
| **Descripción** | El sistema deberá almacenar información correspondiente a los horarios de los estudiantes |
| **Datos específicos** | - Identificador del horario <br> - Nombre del horario <br> - Fecha de incorporación <br> - Fecha de validez <br> - Asignatura  |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-02 |
| **Nombre** | Estudiante |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-07) Consultar horario |
| **Descripción** | El sistema deberá almacenar información de los estudiantes |
| **Datos específicos** | - Identificador del estudiante <br> - Nombre del estudiante <br> - Fecha de incorporación <br> - Fecha de nacimiento <br> - DNI <br> - Correo electrónico |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-03 |
| **Nombre** | Lista de clase |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-06) Buscar estudiante en la lista de clase |
| **Descripción** | El sistema deberá almacenar información correspondiente a los listados de clase de los estudiantes |
| **Datos específicos** | - Identificador del listado <br> - Nombre del listado <br> - Fecha de incorporación <br> - Numero de estudiantes <br> - Asignatura a la que pertenece el listado |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-04 |
| **Nombre** | Asignatura |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-06) Buscar estudiante en la lista de clase |
| **Descripción** | El sistema deberá almacenar información correspondiente a los listados de clase de los estudiantes para cada asignatura |
| **Datos específicos** | - Identificador de la asignatura <br> - Nombre de la asignatura <br> - Fecha de incorporación <br> - Numero de estudiantes <br> - Profesor <br> - Curso |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-05 |
| **Nombre** |PAS|
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-01) Modificar horario  <br> - (UC-02) Dar de alta estudiantes <br> - (UC-04) Validar datos|
| **Descripción** | El sistema deberá almacenar la informacion de cada PAS |
| **Datos específicos** | - Identificador del PAS <br> - Nombre del PAS <br> - Fecha de contratacion <br> - Correo electrónico <br> - Número de teléfono |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-06 |
| **Nombre** |PDI|
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-03) Proponer cambios en los horarios <br> - (UC-02) Dar de alta estudiantes <br> - (UC-06) Buscar estudiantes en la lista de clase |
| **Descripción** | El sistema deberá almacenar la informacion de cada PDI |
| **Datos específicos** | - Identificador del PDI <br> - Nombre del PDI <br> - Fecha de contratación <br> - Correo electrónico <br> - Número de teléfono |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-07 |
| **Nombre** |Curso|
| **Versión** | Versión 1 (31/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-02) Dar de alta estudiantes |
| **Descripción** | El sistema deberá almacenar la informacion de los cursos de un determinado grado |
| **Datos específicos** | - Identificador del curso <br> - Coordinador del curso <br> - Identificador del grado al que pertenece el curso |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-08 |
| **Nombre** |Grado|
| **Versión** | Versión 1 (31/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - Todos los casos de uso |
| **Descripción** | El sistema deberá almacenar la informacion de los grados de una determinada institución universitaria |
| **Datos específicos** | - Identificador del grado <br> - Nombre del grado <br> - Rama a la que pertenece el grado <br> - Coordinador del grado <br> - Identificador de la universidad a la que pertenece el grado |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-09 |
| **Nombre** |Universidad|
| **Versión** | Versión 1 (31/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - Todos los casos de uso |
| **Descripción** | El sistema deberá almacenar la informacion de la universidad |
| **Datos específicos** | - Identificador de la universidad <br> - Nombre de la universidad <br> - Dirección <br> - Número de teléfono <br> - Correo electrónico <br> - Página web de la universidad |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||


#### **Diagrama entidad relacion**
<br>

![Supuesto 1: Horarios. Diagrama Entidad - Relación](/out/lab1/src/supuesto1E-R/supuesto1E-R.svg)

<br>

>#### **Definición de casos de uso**

|| |
|-|:-|
|**ID:**|UC-01|
|**Nombre:**|Modificar Horario|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PAS modificar el horario|
|**Actor:**|PAS|
|**Precondiciones:**|Pertenecer al PAS de esta institucion y estar autenticado en el sistema|
|**Flujo normal:**|1. El actor busca el horario que quiere modificar<br>2. El actor selecciona la asignatura correspondiente<br>3. El actor realiza la modificacion deseada en el horario<br>4. El sistema hace una verificacion automatica de esa modificacion<br>5. La modificacion es aprobada<br>6. Se guarda la modificacion realizada en la base de datos<br>7. Se manda un mensaje a todas las partes involucradas informandole del cambio de horario|
|**Flujo aternativo:**|5.2. La modificacion no es aceptada, por lo que se le vuelve a mandar a la pagina del horario informandole del motivo por la que no ha sido validada<br>6.2. La modificacion realizada no se guarda bien en la base de datos y manda un mensaje de error|
|**Postcondiciones:**|El horario ha de ser guardado o modificado|
|**Referencias:**|Ninguna|
||


|| |
|-|:-|
|**ID:**|UC-02|
|**Nombre:**|Dar de alta estudiantes|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PAS dar de alta a los estudiantes|
|**Actor:**|PAS|
|**Precondiciones:**|Pertenecer al PAS de esta institucion y estar autenticado en el sistema|
|**Flujo normal:**| 1. El actor accede al listado de estudiantes<br>2. El actor busca por DNI al estudiante que vamos a dar de alta<br>3. El actor manda una solicitud para dar de alta al estudiante<br>4. Se hace una valoracion automatica de esta solicitud y si no esta dentro de los parametros establecidos de esta verificacion se manda a un empleado para su verificacion<br>5. Se validan los datos propuestos <br> 6. Mediante una acción de confirmación, el actor envía al sistema los datos a ser validados <br> 7. El sistema comprueba que los datos de cada campo se adecúen a las restricciones del campo en cuestión en la base de datos <br> 8. El Sistema devuelve un mensaje de validación completada correctamente <br>9. Se aprueba el alta de este estudiante<br>10. Se cambia la informacion de este estudiante como dado de alta<br>11. Se le envia un correo al estudiante correspondiente para informarle |
|**Flujo aternativo:**|6.2. No se aprueba el alta del estudiante|
|**Postcondiciones:**|El estudiante se marca en la base de datos como dado de alta|
|**Referencias:**|UC-04, UC-05|
||

|| |
|-|:-|
|**ID:**|UC-03|
|**Nombre:**|Proponer cambios en los horarios|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PDI proponer cambios en los horarios|
|**Actor:**|PDI|
|**Precondiciones:**|Pertenecer al PDI de esta institucion|
|**Flujo normal:**|1. El actor busca el horario que quiere modificar<br>2. El actor selecciona la asignatura correspondiente<br>3. El actor propone la modificacion deseada del horario<br>4. Se hace una verificacion automatica de esa propuesta<br>5. La propuesta es validada<br>6. Se registra la propuesta realizada en la base de datos|
|**Flujo aternativo:**|5.2. La propuesta no es aprobada|
|**Postcondiciones:**|Ninguna|
|**Referencias:**|Ninguna|
||

|| |
|-|:-|
|**ID:**|UC-04|
|**Nombre:**|Validar datos|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PAS modificar el horario|
|**Actor:**|PAS|
|**Precondiciones:**|Pertenecer al PAS de esta institucion|
|**Flujo normal:**| 1. Mediante una acción de confirmación, el actor envía al sistema los datos a ser validados <br> 2. El sistema comprueba que los datos de cada campo se adecúen a las restricciones del campo en cuestión en la base de datos <br> 3. El Sistema devuelve un mensaje de validación completada correctamente |
|**Flujo aternativo:**|2A. En caso de que no se cumplan las restricciones en los datos de algún campo, el Sistema informa de los campos mal completados <br> 3A. Si los datos no se validan correctamente, el Sistema devuelve un mensaje de error |
|**Postcondiciones:**|El estudiante es dado de alta|
|**Referencias:**|UC-02|
||

|| |
|-|:-|
|**ID:**|UC-05|
|**Nombre:**|Dar de alta estudiantes (PDI)|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PDI <br> dar de alta a los estudiantes|
|**Actor:**|PDI|
|**Precondiciones:**|Pertenecer al PDI de esta institucion|
|**Flujo normal:**|1. Accedo al listado de estudiantes<br>2. Buscar al estudiante que vamos a dar de alta<br>3. Mandar solicitud para dar de alta al estudiante<br>4. Se hace una valoracion automatica de esta solicitud y si no esta dentro de los parametros establecidos de esta verificacion se manda a un empleado para su verificacion<br>5. Se validan los datos propuestos<br>6. Se aprueba el alta de este estudiante<br>7. Se cambia la informacion de este estudiante como dado de alta<br>8. Se le envia un correo al estudiante correspondiente para informarle |
|**Flujo aternativo:**|6.2. No se aprueba el alta del estudiante<br>9.2. Se busca al estudiante en las listas de clase para eliminar todos sus registros|
|**Postcondiciones:**|El estudiante se marca en la base de datos como dado de alta|
|**Referencias:**|UC-02, UC-06|
||

|| |
|-|:-|
|**ID:**|UC-06|
|**Nombre:**|Buscar estudiantes en la lista de clase|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PDI <br> buscar estudiantes en la lista de clase|
|**Actor:**|PDI|
|**Precondiciones:**|Pertenecer al PDI de esta institucion|
|**Flujo normal:**|1. Accedo al listado de estudiantes<br>2. Buscar al estudiante que vamos a dar de alta<br>3. Mandar solicitud para dar de alta al estudiante<br>4. Se hace una valoracion automatica de esta solicitud y si no esta dentro de los parametros establecidos de esta verificacion se manda a un empleado para su verificacion<br>5. Se validan los datos propuestos<br>6. Se aprueba el alta de este estudiante<br>7. Se cambia la informacion de este estudiante como dado de alta<br>8. Se le envia un correo al estudiante correspondiente para informarle |
|**Flujo aternativo:**|6.2. No se aprueba el alta del estudiante|
|**Postcondiciones:**|Ninguna|
|**Referencias:**|UC-05|
||

|| |
|-|:-|
|**ID:**|UC-07|
|**Nombre:**|Consultar Horario|
|**Fecha:**|30/09/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al actor PAS modificar el horario|
|**Actor:**|Estudiante, PDI, PAS|
|**Precondiciones:**|Ser un estudiante de esta institucion|
|**Flujo normal:**|1. Busco el horario que quiero consultar<br>2. Selecciono la asignatura correspondiente<br>3. Realizo la consulta deseada del horario<br>4. Se guarda el horario en la base de datos|
|**Flujo aternativo:**|Ninguno|
|**Postcondiciones:**|Ninguna|
|**Referencias:**|Ninguna|
||


### **Supuesto 2: Sistema de compras➡️**
En un sistema de compra, existen cuatro tipos de usuarios: comprador, vendedor, proveedor y administrador. Los compradores pueden agregar productos, consultar precios, finalizar la compra y consultar ofertas. Agregar productos implica marcar esos productos como bloqueados. Los vendedores también pueden consultar ofertas y consultar precios. Los proveedores pueden consultar precios, avisar de nuevos productos y consultar ofertas. Avisar de nuevos productos, de forma excepcional, realiza la incorporación de una oferta. Los proveedores también tienen una funcionalidad para avisar del fin de una oferta. Cuando se avisa del fin de una oferta, se ejecuta la funcionalidad de eliminar la oferta. Ambas funcionalidades de avisar del proveedor tienen en común que se encarga de enviar una notificación. Los administradores pueden consultar precios, consultar ofertas y eliminar productos. La funcionalidad de consultar precios incluye una funcionalidad de buscar productos que es similar a la funcionalidad de consultar productos de los compradores. Sin embargo, la funcionalidad de consultar productos añade una funcionalidad para verificar la disponibilidad. Para realizar una venta, un comprador y un vendedor participan de forma conjunta. En dicha operación, se lleva a cabo el acuerdo de un precio; excepcionalmente, durante la realización de la venta, se consultará el histórico de ventas.

![Supuerto 2: Sistema de Compras](/out/lab0/src/SistemaDeCompras/SistemaDeCompras.svg)

<br>

>#### **Definición de requisitos de información**
| |  |
| ---| :--- |
|  **ID** | IR-01 |
| **Nombre** | Producto |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-03) Consultar producto <br> - (UC-15) Buscar producto <br> - (UC-17) Agregar productos <br> - (UC-06) Eliminar producto <br> - (UC-09) Verificar disponibilidad <br> - (UC-18) Bloquear productos <br> - (UC-12) Consultar precio|
| **Descripción** | El sistema deberá almacenar información correspondiente a los productos del sistema de compras. En concreto: |
| **Datos específicos** | - Identificador del producto <br> - Nombre del producto <br> - Fecha de incorporación <br> - Stock disponible <br> - Precio <br> - En oferta (si o no) <br> - Fabricante <br> - Modelo <br> - Proveedor de dicho producto |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |

| |  |
| ---| :--- |
|  **ID** | IR-02 |
| **Nombre** | Oferta |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-02) Incorporar oferta <br> - (UC-07) Avisar de fin de oferta <br> - (UC-11) Consultar oferta <br> - (UC-13) Eliminar oferta |
| **Descripción** | El sistema deberá almacenar información correspondiente a las ofertas del sistema de compras. En concreto: |
| **Datos específicos** | - Identificador de la oferta <br> - Nombre de la oferta <br> - Fecha inicio <br> - Fecha fin <br> - Descuento aplicable <br> - Si está activa o no |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |

| |  |
| ---| :--- |
|  **ID** | IR-03 |
| **Nombre** | Venta |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-05) Realizar venta <br> - (UC-10) Acordar precio |
| **Descripción** | El sistema deberá almacenar información correspondiente a las ventas realizadas en el sistema de compras. En concreto: |
| **Datos específicos** | - Identificador del producto <br> - Comprador <br> - Vendedor  <br> - Fecha de la venta <br> - Precio de venta <br> - Unidades del producto compradas |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Incluimos el precio de venta en este requisito de información puesto que el comprador y el vendedor deben ponerse de acuerdo en el precio de la venta, de modo que los productos no tienen un precio asignado, sino que este se relaciona con la propia venta |

| |  |
| ---| :---|
|  **ID** | IR-04 |
| **Nombre** | Aviso |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-07) Avisar fin de oferta <br> - (UC-08) Avisar de nuevo producto <br> - (UC-14) Avisar (Proveedor) <br> - (UC-16) Enviar notificación |
| **Descripción** | El sistema deberá almacenar información correspondiente a los avisos realizados en el sistema de compras. En concreto: |
| **Datos específicos** | - Identificador del aviso <br> - Fecha del aviso <br> - Motivo de aviso <br> - Destinatarios <br> - Si fue notificado o no <br> - Proveedor que emitió el aviso (emisor) |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Pueden haber avisos sin notificar y avisos para los que se ha generado una notificación |

| |  |
| ---| :--- |
|  **ID** | IR-05 |
| **Nombre** | Notificaciones |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-07) Avisar fin de oferta <br> - (UC-14) Avisar (Proveedor) <br> - (UC-16) Enviar notificación |
| **Descripción** | El sistema deberá almacenar información correspondiente a las notificaciones enviadas en el sistema de compras. En concreto: |
| **Datos específicos** | - Identificador de la notificación <br> - Texto de la notificación <br> - Fecha de la notificación <br> - Aviso relacionado <br> - Destinatarios |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Las notificaciones solo podrán ser generadas por el Proveedor que emitió el aviso que se pretende notificar. Por ello las relacionamos con el aviso y no con el emisor, que se sobreentiende. |

| |  |
| ---| :--- |
|  **ID** | IR-06 |
| **Nombre** | Comprador |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Perez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-03) Consultar producto <br> - (UC-04) Finalizar compra <br> - (UC-05) Realizar venta <br> - (UC-09) Verificar disponibilidad <br> - (UC-10) Acordar precio <br> - (UC-01) Consultar historico |
| **Descripción** | El sistema deberá almacenar información correspondiente al comprador |
| **Datos específicos** | - Identificador del comprador <br> - Nombre del comprador <br> - Correo electrónico <br> - Número de teléfono |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |

| |  |
| ---| :--- |
|  **ID** | IR-07 |
| **Nombre** | Administrador |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Perez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-06) Eliminar producto <br> - (UC-11) Consultar oferta <br> - (UC-12) Consultar precio <br> - (UC-15) Buscar producto |
| **Descripción** | El sistema deberá almacenar información correspondiente al administrador |
| **Datos específicos** | - Identificador del administrador <br> - Nombre del administrador <br> - Correo electrónico <br> - Número de teléfono |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |

| |  |
| ---| :--- |
|  **ID** | IR-08 |
| **Nombre** | Vendedor |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Perez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-15) Realizar venta <br> - (UC-01) Consultar historico <br> - (UC-10) Acordar precio <br> - (UC-11) Consultar oferta <br> - (UC-12) Consultar precio <br> - (UC-15) Buscar producto  |
| **Descripción** | El sistema deberá almacenar información correspondiente al vendedor |
| **Datos específicos** | - Identificador del vendedor <br> - Nombre del vendedor <br> - Correo electrónico <br> - Número de teléfono |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |

| |  |
| ---| :--- |
|  **ID** | IR-09 |
| **Nombre** | Proveedor |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Perez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-07) Avisar fin de oferta <br>- (UC-08) Avisar de nuevo producto<br>- (UC-02) Incorporar oferta<br> - (UC-13) Eliminar oferta<br> - (UC-14) Avisar proveedor<br>- (UC-16) Enviar notificacion <br>- (UC-11) Consultar oferta<br> - (UC-12) Consultar precio<br>- (UC-15) Buscar producto  |
| **Descripción** | El sistema deberá almacenar información correspondiente al proveedor |
| **Datos específicos** | - Identificador del proveedor <br> - Nombre del proveedor <br> - Correo electrónico <br> - Número de teléfono |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |

| |  |
| ---| :--- |
|  **ID** | IR-10 |
| **Nombre** | Productos eliminados |
| **Versión** | Versión 1 (31/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-06) Eliminar producto |
| **Descripción** | El sistema deberá almacenar información correspondiente a los productos eliminados por el administrador |
| **Datos específicos** | - Identificador del administrador que realizó la eliminación <br> - Identificador del producto eliminado |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |

| |  |
| ---| :--- |
|  **ID** | IR-11 |
| **Nombre** | Cesta de la compra |
| **Versión** | Versión 1 (31/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-17) Agregar producto |
| **Descripción** | El sistema deberá almacenar información correspondiente a los productos agregados por el comprador en su cesta de la compra |
| **Datos específicos** | - Identificador del producto añadido a la cesta de la compra <br> - Identificador del comprador que lo añadió <br> - Unidades del producto añadidas a la cesta |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |

| |  |
| ---| :--- |
|  **ID** | IR-12 |
| **Nombre** | Productos ofertados |
| **Versión** | Versión 1 (01/11/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-02) Incorporar oferta <br> - (UC-07) Avisar fin de oferta <br> - (UC-11) Consultar oferta <br> - (UC-13) Eliminar oferta |
| **Descripción** | El sistema deberá almacenar información correspondiente a los productos ofertados |
| **Datos específicos** | - Identificador del producto en oferta <br> - Identificador de la oferta |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |

| |  |
| ---| :--- |
|  **ID** | IR-13 |
| **Nombre** | Productos bloqueados |
| **Versión** | Versión 1 (03/11/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-17) Agregar producto <br> - (UC-18) Bloquear producto |
| **Descripción** | El sistema deberá almacenar información correspondiente a los productos bloqueados o reservados |
| **Datos específicos** | - Identificador del comprador <br> - Identificador del producto bloqueado <br> - Unidades bloqueadas o reservadas del producto |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |



**Diagrama entidad relacion**
<br>

![Supuesto 2: Sistema de compras. Diagrama Entidad - Relación](/out/lab1/src/supuesto2E-R/supuesto2E-R.svg)

<br>

>#### **Definición de casos de uso**
| |  |
| ---| :--- |
|  **ID**| UC-01 |
|  **Nombre** | ConsultarHistorico |
|  **Fecha** | 18/10/2022 |
|  **Autor** | Toderic Ioan Stefan |
|  **Descripcion** | El actor comprador y vendedor pueden acceder a un historico de ventas realizadas  |
|  **Actores** | Comprador, Vendedor |
|  **Precondiciones** | Deben estar autentificado en el sistema como comprador o vendedor para obtener acceso al historico |
|  **Flujo Normal** | 1. El usuario accede a la sección de consultar historico <br> 2. Se abre el menu desplegable y el usuario selecciona un dia, hora <br> 3.Si todos los parametros introducidos son correctos se mostrara un documento pdf en una nueva pestaña indicando todos los productos vendidos en esa hora y dia seleccionada. |
|  **Flujo Alternativo** | 3A. Si algun párametro falla, se mostrará un mensaje de aviso en el campo erroneo indicando que no hay ventas realizadas ese dia o a esa hora y el sistema redirige al usuario al paso 3 para volver a introducir los parametros correctamente  |
| **Postcondiciones** |  |
| **Referencias** | UC-05 |


| | |
| ----------- | :----------- |
| **Identificador**: | UC-02 |
| **Nombre:** | IncorporarOferta |
| **Fecha:** | 30/09/2022 |
|  **Autor:** | Toderic Ioan Stefan |
|  **Descripcion:** | Boton opcional para incorporar una oferta   |
|  **Actores:** | Proveedor |
|  **Precondiciones:** | El usuario debe estar logueado como proveedor|
|  **Flujo normal:** | 1. El actor busca un producto en el formulario por su identificador <br> 2. El sistema muestra una lista de resultados <br> 3. El actor selecciona un producto <br> 4. El actor pulsa un botón para incorporarle una oferta al producto seleccionado <br> 5. El sistema muestra un listado de todas las ofertas <br> 6. El actor selecciona la oferta <br> 7. El sistema muestra una previsualización del producto ofertado con su nuevo precio <br> 8. Si el actor está de acuerdo, acepta y el producto se guarda con oferta |
|  **Flujo alternativo:** | 2A. Si el producto no se encuentra, se volverá a solicitar el identificador o se cancela el proceso <br> 5A. Si no hay ofertas activas, el proceso termina. <br> 8A. Si se rechaza la propuesta del producto ofertado, el producto se guarda sin oferta |
|  **Postcondiciones:** | Modificación del precio del producto |
| **Referencias**|UC-08|

| |  |
| ---| :--- |
| **ID**| UC-03 |
| **Nombre**| ConsultarProducto|
| **Fecha**| 07/10/2022 |
| **Autor**| Ioan Stefan Toderic |
| **Descripcion**| Permite consultar el historico de ventas  |
| **Actores**| Comprador |
| **Precondiciones**| El usuario debe estar logueado como comprador |
| **Flujo Normal**|  1. El usuario pulsa el botón de Consultar productos para ver la lista de los productos  <br>  2.El usuario introduce en la barra de busqueda del sistema un nombre del producto <br> 3.El sistema devuelve un listado con los productos con el nombre similar disponibles en el sistema <br>   4. El sistema busca el prodcto en la tabla de producto <br> 5.El usuario selecciona el producto al cual quiere comprobar si esta disponible <br> 6.Pulsa el boton de "Comprobar" <br> 7. El sistema busca en la base de datos el producto seleccionado y devuelve el producto en caso de que este disponible  <br> 8. Si el producto esta disponible se le muestra al actor<br>9. El actor visualiza la disponibilidad del producto |
| **Flujo Alternativo** | 2A.En caso de no existir un producto con el nombre indicado en la barra de busqueda el sistema cambiara el color de la barra de busqueda a rojo |
|**Postcondiciones**| |
|**Referencias**| UC-15, UC-09 |

| | |
| ----------- | :----------- |
|  **Identificador:**| UC-04 |
|  **Nombre:** | FinalizarCompra |
|  **Fecha:** | 30/09/2022 |
|  **Autor:** | Guillermo Morales Caparros |
|  **Descripcion:**| Termina la compra y da informacion sobre la compra realizada |
|  **Actores:**| Comprador |
|  **Precondiciones:** | El ususario debe estar logueado en el sistema como comprador |
|  **Flujo normal:** | 1.Una vez el usuario haya terminado de seleccionar los productos a comprar hace click en el boton "Comprar" <br> 2. El sistema cierra la vision de compra, le asigna una id al pedido <br> 3.El sistema envia el id a la base de datos y se lo asigna al comprador <br> 4.Se abre una pestaña en la cual el usuario elige el método de pago <br> 5.El usuario selecciona un método de pago y  realiza el pago <br> 6.El sistema comprueba que el pago se haya efectuado correctamente <br> 7.El sistema cambia la pestaña de pago <br> 3. Se muestra una pestaña nueva con los productos comprados y su precio correspondiente|
|  **Flujo alternativo:** | 6A.En caso de haber problema con la transación se le avisara al usuario de que el pago no ha sido posible de efecturar <br> 6B.Se abre la pestaña de elegir otro método de pago <br> 6C.En caso de que el usuario no quiera seguir comprando puede optar por darle al bóton "Cancelar" |
|  **Postcondiciones:** |  |
|**Referencias**|  |

| |  |
| ---| :--- |
|  **ID**| UC-05|
|  **Nombre** | RealizarVenta |
|  **Fecha** | 13/10/2022 |
|  **Autor** | Luca Daniel Gavriloaie|
|  **Descripcion** | Permite realizar un venta |
|  **Actores** | Comprador, Vendedor |
|  **Precondiciones** | El comprador y el vendedor deben estar autenticados en el Sistema |
|  **Flujo Normal** | 1. El comprador comienza el proceso de tramitación del pedido <br> 2. El vendedor busca el producto en el sistema <br> 3. El vendedor verifica la disponibilidad del producto <br> 4. El vendedor establece un precio y lo envia a la base de datos del sistema <br> 2.El sistema establece el precio a dicho producto <br> 5. El comprador recibe una notificacion con el precio ajustado por el vendedor y decide si comprarlo <br> 6. Si acepta el precio, hace click sobre el boton Acordar <br> 7. El Sistema abre una pestaña con un formulario para poder comprar dicho producto <br> 8. El comprador acepta y envia el formulario <br> 9. Se realiza una petición de precio acordado al sistema <br> 10. El comprador y el vendedor finalizan el trámite del pedido |
|  **Flujo Alternativo** | *3A*. Si el producto no está disponible, el vendedor recibe una notificación de la circunstancia y se lo notifica al comprador. El proceso termina <br> *3B*. Los actores pueden consultar si lo desean el histórico de ventas del producto <br>  - 3B1. El usuario accede a la sección de consultar historico <br> - 3B2 Se abre el menu desplegable y el usuario selecciona un dia, hora <br> - 3b3 Si todos los parametros introducidos son correctos se mostrara un documento pdf en una nueva pestaña indicando todos los productos vendidos en esa hora y dia seleccionada. <br> *6A*. Si no se llega a un acuerdo con respecto al precio, el proceso se cancela. |
| **Postcondiciones** | El stock del producto vendido disminuye y se actualiza el histórico de ventas del mismo |
| **Referencias** | UC-01, UC-10 |


| | |
| ----------- | :----------- |
| **Identificador**: | UC-06 |
| **Nombre:** | EliminarProducto |
| **Fecha:** | 30/09/2022 |
|  **Autor:** | Guillermo Morales Caparros |
|  **Descripcion:** | Permite eliminar un producto añadido en el carrito o lista de compra que ya se haya seleccionado previamente al darle al boton "Añadir" |
|  **Actores:** | Administrador |
|  **Precondiciones:** | El usuario debe estar logueado en el sistema como Administrador|
|  **Flujo normal:** | 1.El usuario accede a la lista de productos <br> 2. Selecciona un producto o varios  <br> 3.El sistema cambia el color de los productos seleccionados <br>4.Al seleccionar un producto aparece un icono de una papelera <br> 5.El usuario hace click en la papelera <br> 6.El sistema muestra un aviso "¿Seguro que desea eliminar estos productos?" <br> 7.El usuario decide pulsar "Si" <br> 8.Se cierra la pestaña y vuelve a llevarte a tu lista refrescandola con todos los productos actuales en ella |
|  **Flujo alternativo:** | 7A. El usuario decide pulsar "No" <br> 7B.El sistema no cierra la pestaña del aviso de "¿Seguro que desea eliminar estos productos?" <br> 7C.Muestra todos los productos seleccionados y brinda al usuario la opción de "Cancelar" donde no se hará nada y la lista quedará igual. |
|  **Postcondiciones:** | El producto o los productos seleccionados se eliminarán de la lista |
| **Referencias**||

| |  |
| ---| :--- |
|  **ID**| UC-07|
|  **Nombre** | AvisarFinDeOferta |
|  **Fecha** | 13/10/2022 |
|  **Autor** | Luca Daniel Gavriloaie|
|  **Descripcion** | El proveedor avisará a los usuarios del sistema sobre el fin de una oferta |
|  **Actores** | Proveedor |
|  **Precondiciones** | El proveedor debe estar autenticado en el sistema |
|  **Flujo Normal** | 1. El proveedor introduce el nombre de una oferta <br> 2. El sistema realiza la búsqueda de dicha oferta <br> 3. El proveedor selecciona y comprueba el estado de la oferta <br> 4. El proveedor pulsa crear un aviso <br> 5. El sistema lleva al proveedor a la interfaz de creación del aviso <br> 6. El proveedor debe configurar el aviso (información, fecha y hora, duración...) <br> 7. El proveedor crea el aviso <br> 8. El actor selecciona el aviso para ser notificado <br> 9. El actor solicita al sistema enviar una notificación <br> 10. El sistema consulta la información del aviso para generar la notificación a partir de dicha información <br> 11. El sistema envía la notificación <br> 12. El proveedor solicita al sistema el listado de ofertas activas <br> 13. El sistema muestra todas las ofertas <br> 14. El proveedor selecciona la oferta que desea eliminar <br> 15. El proveedor elimina la oferta |
|  **Flujo Alternativo** | 2A. Si el sistema no encuentra dicha oferta, se notificará sobre este resultado <br> 6A. Si la fecha y/o la hora seleccionadas son anteriores a la actual, el sistema dará error <br> 7A. El proveedor no podrá crear el aviso si no se han completado todos los campos del paso 6 <br>  |
| **Postcondiciones** | Creación de un nuevo aviso y su respectiva notificación en la base de datos. Eliminación de la oferta. |
| **Referencias** | UC-13, UC-14, UC-16 |

| |  |
| ---| :--- |
|  **ID**| UC-08|
|  **Nombre** | AvisarDeNuevoProducto |
|  **Fecha** | 14/10/2022 |
|  **Autor** | Luca Daniel Gavriloaie|
|  **Descripcion** | Permite avisar de la disponibilidad de un nuevo producto a los usuarios del sistema de compras |
|  **Actores** | Proveedor |
|  **Precondiciones** | El proveedor debe estar autenticado en el sistema |
|  **Flujo Normal** | 1. El proveedor busca el nuevo producto <br> 2. El proveedor marca el nuevo producto como disponible <br> 3. El proveedor emite un aviso para los usuarios del sistema de la disponibilidad del nuevo producto y de su precio |
|  **Flujo Alternativo** | 1A. Si el sistema no encuentra el producto, le notificará del error al actor <br> 3A. Opcionalmente, el proveedor podrá crear una oferta para el nuevo producto: <br> - 3A1. El actor busca el producto en el formulario por su identificador <br> - 3A2. El sistema muestra una lista de resultados <br> - 3A3. El actor selecciona el producto <br> - 3A4. El actor pulsa un botón para incorporarle una oferta al producto seleccionado <br> - 3A5. El sistema muestra un listado de todas las ofertas <br> - 3A6. El actor selecciona la oferta <br> - 3A7. El sistema muestra una previsualización del producto ofertado con su nuevo precio <br> - 3A8. Si el actor está de acuerdo, acepta y el producto se guarda con oferta |
| **Postcondiciones** | Creación de un nuevo aviso en la base de datos |
| **Referencias** | UC-02 |

| |  |
| ---| :--- |
|  **ID**| UC-09 |
|  **Nombre** | VerificarDisponibilidad |
|  **Fecha** | 18/10/2022 |
|  **Autor** | Ioan Stefan Toderic |
|  **Descripcion** | Permite comprobar si el producto esta disponible o no  |
|  **Actores** | Comprador |
|  **Precondiciones** | Debe estar logueado como un comprador y consultar el producto |
|  **Flujo Normal** | 1.El usuario selecciona el producto al cual quiere comprobar si esta disponible <br> 2.Pulsa el boton de "Comprobar" <br> 2. El sistema busca en la base de datos el producto seleccionado y devuelve el producto en caso de que este disponible |
|  **Flujo Alternativo** | 3A. Busca en la base de datos el producto seleccionado y devuelve un mensaje de "Producto indisponible" en caso de que no este indisponible |
| **Postcondiciones** |  |
| **Referencias** | UC-03 |

| |  |
| ---| :--- |
|  **ID**| UC-10 |
|  **Nombre** | AcordarPrecio |
|  **Fecha** | 14/10/2022 |
|  **Autor** | Toderic Ioan Stefan  |
|  **Descripcion** | El comprador y el vendedor se ponen de acuerdo en un precio común |
|  **Actores** | Comprador, Vendedor |
|  **Precondiciones** | Comprador y Vendedor deben estar autenticados en el sistema |
|  **Flujo Normal** | 1.El vendedor establece un precio y lo envia a la base de datos del sistema <br> 2.El sistema establece el precio a dicho producto <br> 3.El comprador recibe una notificacion con el precio ajustado por el vendedor y decide si comprarlo <br> 4.Si acepta el precio, hace click sobre el boton Acordar <br> 5.El Sistema abre una pestaña con un formulario para poder comprar dicho producto <br> 6.El comprador acepta y envia el formulario <br> 7.Se realiza una petición de precio acordado al sistema |
|  **Flujo Alternativo** | 4A. En caso que el comprador decida rechazar el precio propuesto por el vendedor, el sistema envia una petición al sistema "Precio denegado" |
| **Postcondiciones** |  |
| **Referencias** | UC-05 |


| | |
| ----------- | :----------- |
| **Identificador:** | UC-11 |
| **Nombre:** | ConsultarOferta |
| **Fecha:** | 07/10/2022 |
| **Autor:** | Guillermo Morales Caparros |
| **Descripcion:** | Debe mostrar una serie de datos relacionados con la oferta |
| **Actores:** | Comun, Administrador, Vendedor, Proveedor |
| **Precondiciones:** | El usuario debe estar registrado como alguno de los actores permitidos|
| **Flujo normal:** | 1. El usuario selecciona la opcion para consultar oferta de un producto seleccionado <br> 2.Se abre una pestana que muestra los datos de la oferta <br> 3. El usuario puede decidir si comprar el producto en oferta <br> 4.Si el usuario decide comprar el producto puede darle al boton de añadir producto a mi lista  |
| **Flujo alternativo:** | 3A.Si el usuario decide no comprar el producto con esa oferta, selecciona el botón "Cancelar" y el sistema cierra la pestaña de ofertas |
| **Postcondiciones:** ||
| **Referencias:** |  |

| |  |
| ---| :--- |
|  **ID**| UC-12 |
|  **Nombre** | ConsultarPrecio |
|  **Fecha** | 18/10/2022 |
|  **Autor** | Toderic Ioan Stefan |
|  **Descripcion** | El sistema muestra el precio del producto seleccionado por el actor |
|  **Actores** | Administrador, Vendedor, Proveedor |
|  **Precondiciones** | Debe de ser estar logueado en el sistema como un administrador, un vendedor o un proveedor  |
|  **Flujo Normal** | 1.El actor introduce en la barra de busqueda del sistema un nombre del producto <br> 2.El sistema devuelve un listado con los productos con el nombre similar disponibles en el sistema <br> 3.El sistema muestra los precios de cada producto buscado anteriormente |
|  **Flujo Alternativo** |  2A.En caso de no existir un producto con el nombre indicado en la barra de busqueda el sistema cambiara el color de la barra de busqueda a rojo |
| **Postcondiciones** |  |
| **Referencias** | UC-15 |

| |  |
| ---| :--- |
|  **ID**| UC-13|
|  **Nombre** | EliminarOferta |
|  **Fecha** | 14/10/2022 |
|  **Autor** | Luca Daniel Gavriloaie|
|  **Descripcion** | Permite eliminar la oferta del sistema de compras, actualizando el precio de los productos afectados por esta oferta |
|  **Actores** | Proveedor |
|  **Precondiciones** | El proveedor debe estar autenticado en el sistema |
|  **Flujo Normal** | 1. El proveedor solicita al sistema el listado de ofertas activas <br> 2. El sistema muestra todas las ofertas <br> 3. El proveedor selecciona la oferta que desea eliminar <br> 4. El proveedor elimina la oferta |
|  **Flujo Alternativo** | 4A. La oferta no se podrá eliminar sin haber avisado previamente de su finalización |
| **Postcondiciones** | Se actualiza el conjunto de ofertas activas y los productos afectados por la oferta eliminada vuelven a su precio anterior |
| **Referencias** | UC-07 |


|  |  |
| --- | :--- |
|  **ID**| UC-14 |
|  **Nombre** | AvisarProveedor |
|  **Fecha** | 18/10/2022 |
|  **Autor** | Luca Daniel Gavriloaie |
|  **Descripcion** | El proveedor podrá realizar avisos visibles en el sistema para determinados fines |
|  **Actores** | Proveedor |
|  **Precondiciones** | El proveedor debe estar autenticado en el sistema |
|  **Flujo Normal** | 1. El proveedor pulsa crear un aviso <br> 2. El sistema lleva al proveedor a la interfaz de creación del aviso <br> 3. El proveedor debe configurar el aviso (información, fecha y hora, duración...) <br> 4. El proveedor crea el aviso <br> 5. El actor selecciona el aviso para ser notificado <br> 6. El actor solicita al sistema enviar una notificación <br> 7. El sistema consulta la información del aviso para generar la notificación a partir de dicha información <br> 8. El sistema envía la notificación |
|  **Flujo Alternativo** | 3A. Si el proveedor pulsa enviar aviso sin completar la configuración necesaria, el sistema dará error y volverá a la vista de creación del aviso <br> 3B. Si la fecha y/o la hora seleccionadas son anteriores a la actual, el sistema dará error |
| **Postcondiciones** | Ninguna |
| **Referencias** | UC-07, UC-16 |

| |  |
| ---| :--- |
|  **ID**| UC-15 |
|  **Nombre** | BuscarProducto |
|  **Fecha** | 18/10/2022 |
|  **Autor** | Toderic Ioan Stefan  |
|  **Descripcion** | El comprador busca un producto en el sistema |
|  **Actores** | Comprador |
|  **Precondiciones** | El usuario debe estar logueado en el sistema como comprador |
|  **Flujo Normal** | 1.El actor introduce en la barra de busqueda del sistema un nombre del producto <br> 2.El sistema devuelve un listado con los productos con el nombre similar disponibles en el sistema |
|  **Flujo Alternativo** | 2A.En caso de no existir un producto con el nombre indicado en la barra de busqueda el sistema cambiara el color de la barra de busqueda a rojo |
| **Postcondiciones** |  |
| **Referencias** | UC-03, UC-12 |

| |  |
| ---| :--- |
| **ID**| UC-16 |
| **Nombre** | EnviarNotificacion |
| **Fecha** | 18/10/2022 |
| **Autor** | Luca Daniel Gavriloaie |
| **Descripcion** | Permite enviar una notificación a los usuarios del sistema |
| **Actores** | Proveedor |
| **Precondiciones** | El proveedor debe estar autenticado |
| **Flujo Normal** | 1. El actor selecciona el aviso para ser notificado <br> 2. El actor solicita al sistema enviar una notificación <br> 3. El sistema consulta la información del aviso para generar la notificación a partir de dicha información <br> 4. El sistema envía la notificación |
| **Flujo Alternativo** | 1A. Si no existe ningún aviso a notificar, el proceso termina |
| **Postcondiciones** | Ninguna |
| **Referencias** | UC-14 |

| |  |
| ---| :--- |
|  **ID**| UC-17 |
|  **Nombre** | Agregar productos |
|  **Fecha** | 18/10/2022 |
|  **Autor** | Luca Daniel Gavriloaie |
|  **Descripcion** | El comprador puede agregar productos a la cesta de compra |
|  **Actores** | Comprador |
|  **Precondiciones** | El comprador debe estar autenticado en el sistema |
|  **Flujo Normal** | 1. El comprador selecciona el producto deseado <br> 2. El comprador solicita al sistema agregar el producto a la cesta de compra pulsando un botón <br> 3. El sistema añade el producto a la cesta de compra del comprador <br> 4. El Comprador determina el número de unidades que desea bloquear o reservar <br> 5. El Comprador solicita al sistema bloquear ese número de unidades del producto <br> 6. El sistema comprueba que el número de unidades disponibles del producto se mayor al número de unidades que se desean bloquear o reservar <br> 7. En caso afirmativo, el Sistema marca tal número de unidades del producto como reservadas |
|  **Flujo Alternativo** | 2A. Si no hay stock del producto, el sistema devuelve un error |
| **Postcondiciones** | La lista con los productos en la cesta de la compra se actualiza |
| **Referencias** | UC-18 |

| |  |
| ---| :--- |
|  **ID**| UC-18 |
|  **Nombre** | Bloquear productos |
|  **Fecha** | 21/10/2022 |
|  **Autor** | Luca Daniel Gavriloaie |
|  **Descripcion** | Permite bloquear una unidad de un producto reservandola para un comprador |
|  **Actores** | Comprador |
|  **Precondiciones** | El Comprador debe estar autenticado en el sistema |
|  **Flujo Normal** | 1. El Comprador determina el número de unidades que desea bloquear o reservar <br> 2. El Comprador solicita al sistema bloquear ese número de unidades del producto <br> 3. El sistema comprueba que el número de unidades disponibles del producto se mayor al número de unidades que se desean bloquear o reservar <br> 4. En caso afirmativo, el Sistema marca tal número de unidades del producto como reservadas |
|  **Flujo Alternativo** | 3A. En caso contrario, todas las unidades están ya reservadas y se notificará de la circunstancia. |
| **Postcondiciones** | El producto se marca en la base de datos como bloqueado o reservado y se reduce el número de unidades reservables del producto |
| **Referencias** | UC-17 |


### **Supuesto 3: Compañía hotelera➡️**
En una compañía hotelera, el administrador y el comercial pueden consultar reservas. El comercial realiza ofertas y gestiona nuevas reservas. El administrador gestiona nuevas peticiones y también realiza ofertas. La realización de ofertas por parte del comercial conlleva un recálculo de precios. Además, dicha realización de ofertas conlleva opcionalmente el bloqueo temporal de una reserva. Los clientes, los administradores y los comerciales pueden consultar disponibilidades y visualizar ofertas. La consulta de disponibilidades y la consulta de reservas tienen la funcionalidad común de buscar elementos. Por su parte, la consulta de disponibilidades conlleva una funcionalidad que muestra un calendario.

![Supuesto 3: Compañía hotelera](/out/lab0/src/companiaHotelera/companiaHotelera.svg)

>#### **Definición de requisitos de información**
| |  |
| ---| :--- |
|  **ID** | IR-01 |
| **Nombre** | Reservas |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-05) Consultar reservas <br> - (UC-10) Gestionar nueva reserva  <br> - (UC-09) Bloquear temporalmente una reserva|
| **Descripción** | El sistema deberá almacenar información correspondiente a las reservas disponibles|
| **Datos específicos** | - Identificador de la reserva<br> - Nombre de la reserva <br> - Fecha de la reserva <br> - Duración de la reserva (en días) <br> - Precio de la reserva <br> - Habitación |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-02 |
| **Nombre** | Ofertas |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-07) Realizar oferta <br> - (UC-02) Visualizar oferta  <br> - (UC-09) Bloquear temporalmente una reserva|
| **Descripción** | El sistema deberá almacenar información correspondiente a las ofertas disponibles|
| **Datos específicos** | - Identificador de la oferta<br> - Nombre de la oferta <br> - Fecha de inicio <br> - Fecha de fin <br> - Precio de la oferta |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-03 |
| **Nombre** | Precio |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-12) Recalcular precio |
| **Descripción** | El sistema deberá almacenar información correspondiente a los precios de las ofertas disponibles|
| **Datos específicos** | - Valor del precio |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-04 |
| **Nombre** | Peticiones |
| **Versión** | Versión 1 (21/10/2022) |
| **Autores** | Daniel Pérez Escarcena |
| **Fuentes** |  |
| **Referencias** | - (UC-08) Gestionar peticion|
| **Descripción** | El sistema deberá almacenar información correspondiente a las peticiones que hacen los clientes|
| **Datos específicos** | - Identificador de la peticion<br> - Nombre de la peticion <br> - Fecha de incorporacion|
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-05 |
| **Nombre** | Cliente |
| **Versión** | Versión 1 (28/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-02) Visualizar ofertas <br> - (UC-03) Consultar disponibilidad |
| **Descripción** | El sistema deberá almacenar información correspondiente a los clientes |
| **Datos específicos** | - NIF <br> - Nombre <br> - Edad |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-06 |
| **Nombre** | Comercial |
| **Versión** | Versión 1 (28/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-10) Gestionar nueva reserva <br> - (UC-05) Consultar reservas |
| **Descripción** | El sistema deberá almacenar información correspondiente a los comerciales |
| **Datos específicos** | - NIF <br> - Nombre <br> - Edad <br> - Empresa |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-07 |
| **Nombre** | Administrador |
| **Versión** | Versión 1 (28/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC05) Consultar reservas <br> - (UC-07) Realizar oferta <br> - (UC-08) Gestionar petición |
| **Descripción** | El sistema deberá almacenar información correspondiente a los administradores |
| **Datos específicos** | - NIF <br> - Nombre <br> - Edad |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

| |  |
| ---| :--- |
|  **ID** | IR-08 |
| **Nombre** | Disponibilidades |
| **Versión** | Versión 1 (28/10/2022) |
| **Autores** | Luca Daniel Gavriloaie |
| **Fuentes** |  |
| **Referencias** | - (UC-03) Consultar disponibilidad <br> - (UC-06) Mostrar calendario |
| **Descripción** | El sistema deberá almacenar información correspondiente a las disponibilidades |
| **Datos específicos** | - Habitación <br> - Fecha |
| **Importancia** | Muy importante |
| **Estado** | Aceptado |
| **Comentarios** | Ninguno |
||

**Diagrama entidad relacion**
<br>



<br>

>#### **Definición de casos de uso**

|| |
|-|:--|
|**ID:**|UC-01|
|**Nombre:**|Consultar|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite a los actores realizar una consulta en el sistema de la compañía hotelera|
|**Actor:**|Cliente, Administrador, Comercial|
|**Precondiciones:**| Los actores deben estar autenticados en el sistema de la compañía hotelera |
|**Flujo normal:**|1- El actor solicita al sistema realizar una consulta <br> 2- El sistema le pide al actor introducir un parámetro de búsqueda <br> 3- El actor escribe en el buscador el nombre del elemento <br> 4- El sistema muestra todos los elementos que contengan la cadena introducida en el buscador |
|**Flujo aternativo:**|4A-Si no hay ningún elemento, se muestra un mensaje informativo y se vuelve a pedir al actor realizar la búsqueda (paso 3), o el actor puede terminar el proceso.|
|**Postcondiciones:**|Ninguna|
| **Referencias**|UC-03, UC-04, UC-05, UC-06|
||

|| |
|--|:--|
|**ID:**|UC-02|
|**Nombre:**|Visualizar ofertas|
|**Fecha:**|03/11/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite visualizar las ofertas del hotel|
|**Actores:**|Cliente, Comercial, Administrador|
|**Precondiciones:**| El actor debe estar autenticado en el sistema de la comañía hotelera |
|**Flujo normal:**| 1. El actor solicita al sistema visualizar las ofertas <br> 2. El sistema le pide al actor completar al menos un criterio de búsqueda (intervalo de tiempo, lugar, estrellas, número de personas) <br> 3. El sistema mostrará las ofertas encontradas para los criterios seleccionados <br> 4. El actor podrá seleccionar una oferta para ver detalles de la misma |
|**Flujo aternativo:**| 3A. Si no existen resultados, el sistema le pedirá al actor volver a seleccionar un criterio, o el actor podrá terminar el proceso. |
|**Postcondiciones:**|Ninguna|
| **Referencias**||
||

|| |
|-|:-|
|**ID:**|UC-03|
|**Nombre:**|Consultar disponibilidad|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al cliente ver si hay plazas disponibles|
|**Actor:**|Cliente, Administrador, Comercial|
|**Precondiciones:**|Ninguna|
|**Flujo normal:**|1-Clickar la opcion para mostrar las disponibilidades <br>2-El sistema muestra las distintas opciones disponibles|
|**Flujo aternativo:**|1-No queda ninguna opcion disponible, por lo que se muestra un mensaje informativo|
|**Postcondiciones:**|Ninguna|
| **Referencias**|UC-01|
||

|| |
|-|:--|
|**ID:**|UC-04|
|**Nombre:**|Buscar elemento|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al cliente buscar un elemento en concreto para agilizar busqueda|
|**Actor:**|Cliente, Administrador, Comercial|
|**Precondiciones:**|Ninguna|
|**Flujo normal:**|1- El cliente escribe en el buscador el nombre del elemento <br> 2- El sistema muestra todos los elementos que contengan la cadena introducida en el buscador|
|**Flujo aternativo:**|2A-Si no hay ningún elemento, se muestra un mensaje informativo y se vuelve a pedir al actor realizar la búsqueda, o el actor puede terminar el proceso.|
|**Postcondiciones:**|Ninguna|
| **Referencias**|UC-01|
||

|| |
|-|:-|
|**ID:**|UC-05|
|**Nombre:**|Consultar reservas|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al cliente ver si hay reservas realizadas a su nombre|
|**Actor:**|Cliente|
|**Precondiciones:**|El cliente debe estar registrado con su nombre de usuario o ID|
|**Flujo normal:**|1-Acceder al apartado de reservas<br>2-Seleccionar la opcion de mostrar reservas<br>3-El sistema muestra una tabla con las reservas realizadas|
|**Flujo aternativo:**|1-No hay ninguna reserva realizada, por lo que se muestra un mensaje informativo|
|**Postcondiciones:**|Ninguna|
| **Referencias**|UC-01|
||

|| |
|-|:-|
|**ID:**|UC-06|
|**Nombre:**|Mostrar calendario|
|**Fecha:**|18/10/2022|
|**Autor:**|Guillermo Morales|
|**Descripcion:**|Permite al cliente ver el calendario para consultar la disponibilidad|
|**Actor:**|Cliente|
|**Precondiciones:**|Ninguna|
|**Flujo normal:**|1-Al acceder a la consulta de disponibilidades se muestra el calendario|
|**Flujo aternativo:**|1-Si no hay disponibilidades no se muestra el calendario|
|**Postcondiciones:**|Ninguna|
| **Referencias**|UC-01, UC-03|
||

|| |
|-|:-|
|**ID:**|UC-07|
|**Nombre:**|Realizar ofertas|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al administrador ver si hay ofertas disponibles|
|**Actor:**|Administrador|
|**Precondiciones:**|El administrador debe estar registrado con su nombre de usuario o ID|
|**Flujo normal:**|1-Acceder a la web<br>2.Entra en el apartado de oferta<br>3.Filtra para encontrar los productos que estas buscando<br>4-Seleccionar la opcion de mostrar ofertas<br>5-El sistema muestra una tabla con las ofertas disponibles|
|**Flujo aternativo:**|1-No hay ninguna oferta disponible, por lo que se muestra un mensaje informativo|
|**Postcondiciones:**|Ninguna|
| **Referencias**||
||

|| |
|-|:-|
|**ID:**|UC-08|
|**Nombre:**|Gestionar peticion|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al administrador ver las peticiones realizadas|
|**Actor:**|Administrador|
|**Precondiciones:**|El administrador debe estar registrado con su nombre de usuario o ID|
|**Flujo normal:**|1-Acceder al apartado de peticiones<br>2-Seleccionar la opcion de mostrar peticiones<br>3-El sistema muestra una tabla con las peticiones realizadas|
|**Flujo aternativo:**|1-No hay ninguna peticion realizada, por lo que se muestra un mensaje informativo|
|**Postcondiciones:**|Ninguna|
| **Referencias**||
||

|| |
|-|:-|
|**ID:**|UC-09|
|**Nombre:**|Bloquear temporalmente una reserva|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al administrador bloquear una reserva temporalmente|
|**Actor:**|Administrador|
|**Precondiciones:**|El administrador debe estar registrado con su nombre de usuario o ID|
|**Flujo normal:**|1-Acceder al apartado de reservas <br> 2- Seleccionar la opcion de mostrar reservas <br> 3-El sistema muestra una tabla con las reservas actuales <br> 4-Selecciona la que quiere bloquear temporalmente|
|**Flujo aternativo:**|1-No hay ninguna reserva, por lo que se muestra un mensaje informativo|
|**Postcondiciones:**|Ninguna|
| **Referencias**|UC-11, UC-07|
||

|| |
|-|:-|
|**ID:**|UC-10|
|**Nombre:**|Gestionar nueva reserva|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al comercial gestionar una nueva reserva|
|**Actor:**|Comercial|
|**Precondiciones:**|El comercial debe estar registrado con su nombre de usuario o ID|
|**Flujo normal:**|1-Acceder al apartado de reservas <br> 2- Seleccionar la opcion de mostrar reservas <br> 3-El sistema muestra una tabla con las reservas actuales <br> 4-Selecciona la opcion de añadir una nueva reserva|
|**Flujo aternativo:**||
|**Postcondiciones:**|Ninguna|
| **Referencias**||
||

|| |
|-|:-|
|**ID:**|UC-11|
|**Nombre:**|Realizar oferta del comercial|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al administrador realizar una oferta|
|**Actor:**|Administrador|
|**Precondiciones:**|El administrador debe estar registrado con su nombre de usuario o ID|
|**Flujo normal:**|1-Acceder al apartado de ofertas<br>2-Seleccionar la opcion de mostrar ofertas<br>3-El sistema muestra una tabla con las ofertas disponibles<br>4-Realizar una nueva oferta|
|**Flujo aternativo:**||
|**Postcondiciones:**|Ninguna|
| **Referencias**|UC-07, UC-09, UC-12|
||

|| |
|-|:-|
|**ID:**|UC-12|
|**Nombre:**|Recalcular precio|
|**Fecha:**|07/10/2022|
|**Autor:**|Daniel Perez|
|**Descripcion:**|Permite al administrador modificar el precio que ofrece una oferta|
|**Actor:**|Administrador|
|**Precondiciones:**|El administrador debe estar registrado con su nombre de usuario o ID|
|**Flujo normal:**|1-Acceder al apartado de ofertas<br>2-Seleccionar la opcion de mostrar ofertas<br>3-El sistema muestra una tabla con las ofertas disponibles<br>4-Seleccionar una oferta concreta<br>5-Cambiar el precio de la oferta|
|**Flujo aternativo:**||
|**Postcondiciones:**|Ninguna|
| **Referencias**|UC-07, UC-09, UC-11|
||


### **Supuesto 4: Fotografía Online➡️**
En una aplicación de fotografía online, los clientes pueden visualizar las fotos, donde de forma excepcional se puede realizar una denuncia sobre la foto. Al denunciar una foto, se ha de introducir una explicación sobre la denuncia. Los clientes también pueden llevar a cabo consultas sobre las fotos, operación que es un caso particular de visualizar las fotos. Los controladores de fotos pueden indicar que una foto debe ser revisada. Esta funcionalidad es un caso general de la funcionalidad de denunciar foto. Además, los controladores también pueden editar la información de las fotos. En esta aplicación también participan usuarios de tipo vendedor. Los vendedores pueden escribir a los clientes para hacerles ofertas sobre los productos de la aplicación. De forma excepcional, al hacer una oferta pueden reducir el precio de un producto. Los vendedores también pueden buscar detalles en las fotos, operación que es un caso particular de visualizar fotos. Pero esa búsqueda conlleva la verificación de los datos introducidos. Por otro lado, los gestores de la aplicación pueden ver ofertas, bloquear ofertas, emitir facturas y editar facturas. La emisión de facturas requiere la participación de un software de facturación. El administrador de la tienda puede ver ofertas, emitir facturas, editar facturas, bloquear ofertas, crear usuarios y editar usuarios. Esta funcionalidad de ver ofertas también la pueden realizar los clientes. Editar usuarios tiene características en común con editar facturas. Crear usuarios conlleva el envío de un email en el que es necesario el uso de un gestor de correo.

![Supuesto 4: Fotografía Online](/out/lab0/src/fotografiaOnline/fotografiaOnline.svg)


### **Supuesto 5: Gestión de Incidencias➡️**
En un sistema de gestión de incidencias, los técnicos y los operadores pueden dar de alta incidencias, para lo cual, de forma excepcional se enviará un correo (en esta operación participa un sistema de gestión de correo). Los técnicos también atienden llamadas telefónicas y realizan informes sobre las incidencias. Por su parte, los operadores atienden llamadas telefónicas, marcan incidencias como duplicadas y ordenan incidencias. La forma de atender llamadas de los técnicos y los operadores no es exactamente igual, pero tiene similitudes. De forma específica, cuando los técnicos atienden llamadas, comprueban datos de la incidencia en el sistema. Cuando los operadores atienden llamadas, introducen nuevos datos de la incidencia. Los administradores del sistema gestionan categorías de incidencias, consultan incidencias y ordenan incidencias. La ordenación por parte de los administradores conlleva la adición de un comentario. Los técnicos y los operadores también pueden consultar incidencias. La consulta de incidencias por parte técnicos, operadores y administradores puede conllevar, de forma excepcional, la edición de los datos de la incidencia. Los usuarios invitados también pueden consultar incidencias, pero sin la posible edición de los datos. Además, los invitados informan sobre posibles incidencias, se pueden registrar para ver notificaciones y pueden acceder a un listado del histórico de notificaciones. El informe de posibles incidencias conlleva el dar de alta la localización en un mapa, la incorporación de una explicación completa en formato textual y la subida de una foto.

![Supuesto 5: Gestión de Incidencias](../../out/lab0/src/gestionDeIncidencias/gestionDeIncidencias.svg)