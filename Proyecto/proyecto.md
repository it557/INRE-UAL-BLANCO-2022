

![Universidad de Almería](/Proyecto/Imagenes/05-Logotipo-Vertical.png)
# **Especificación de los requisitos del software**

<br>

### **Hoja de revision**

| Date            | Versión    | Descripción | Author |
|-------------------|-------------|---------------|--------------|
| 19/12/2022   | 2   |    Especificación de requisitos de sofrtare     |     Equipo Blanco    | 

<br> 

# **Contenidos**

**1. Introduccion**

**2. Necesidades del negocio**

    2.1. Objetivos del negocio

**3. Requisitos del sistema a desarrollar**

    3.1. Requisitos

    3.2. Casos de uso

         Lista de diagramas de casos de uso del modelo

         Diagramas de casos de uso

         Lista general de casos de uso  y actores del proyecto

         Detalle de los casos de uso

    3.3. Diagramas de clases asociados a los requisitos de información

<br><br>

# **1. Introducción**

En este documento se mostrará de forma textual los requisitos y las funcionalidades que deberán estar implementadas en el software a desarrollar.
Se podrá visualizar las tablas con los requisitos funcionales y los diagramas de casos de uso que servirán a los desarrolladores a elaborar el sistema con las especificaciones apropiadas.

# **2. Necesidades del negocio**

## ***2.1. Objetivos del negocio***
| OBJ1            | Portal    |
|-------------------|-------------|
| **Versión**  | 1.0   |
| **Descripción**   | Plataforma en la cual se podrá visualizar los distintos caminos en tiempo real , en la cual obtener la ruta, seleccionar el destino y origen,una sección en la cual se podrán ver las noticias y un foro.   |
| **Comentarios**   | Ninguno   |

| OBJ2            | Sistema de información    |
|-------------------|-------------|
| **Versión**  | 1.0   |
| **Descripción**   | Sistema integrado de información de la red de transporte público de todos los municipios de Gran Canaria que proporcione herramientas de análisis, consulta, localización y gestión, con el objeto de que el usuario del transporte público pueda consultar de forma dinámica la información del servicio permitiéndole conocer y programar con antelación su viaje.   |
| **Comentarios**   | Ninguno   |

| OBJ3            | Sistema de monitorización de la explotación del transporte    |
|-------------------|-------------|
| **Versión**  | 1.0   |
| **Descripción**   | El sistema debe de monitorizar en tiempo real el estado de la red de transporte público por carretera en la Isla de Gran Canaria en los siguientes aspectos:<br>- El cumplimiento de los servicios adjudicados a los operadores y considerados esenciales<br>- Servicios considerados como ampliaciones o mejoras prestados por parte de los operadores adjudicatarios<br>- La simulación de la situación real y su comprobación mediante el empleo de los sistemas de comunicaciones disponibles en los vehículos de los operadores |
| **Comentarios**   | Ninguno   |



# **3.Requisitos del sistema a desarrollar**

## ***3.1 Requisitos***

### ***3.1.1 Requisitos de Informacion***

| ID          | RI-1 | 
|-------------------|-------------|
|**Nombre**  | Lineas  |    
|**Versión**  | 1.0, 30/11/2022  |
|**Autor**  | David Hernández Carmona  |
|**Referencias**  |  RF-05, RF-06, RF-07 |
|**Descripción**  | Recorrido fijo de un transporte entre las paradas de comienzo y finalización del transporte  |
|**Datos Especificos**  | -Identificador de línea <br>-Descripción de la línea <br>-Parada de comienzo<br>-Parada de finalización<br>-El resto de paradas |
|**Importancia**  |  TBD |
|**Estado**  |  Obligatorio |
|**Comentarios**  |  Se almacenarán todas las líneas en tablas en la base de datos |


| ID          | RI-2 | 
|-------------------|-------------|
|**Nombre**  |  Paradas |    
|**Versión**  |  1.0, 30/11/2022 |
|**Autor**  |  David Hernández Carmona |
|**Referencias**  |  RF-05 |
|**Descripción**  |  Situación geográfica de la parada y otros datos |
|**Datos Especificos**  | Identificador de parada, descripción, dirección postal, código de municipio, coordenadas geográficas  |
|**Importancia**  |  TBD |
|**Estado**  | Obligatorio  |
|**Comentarios**  |  Se almacenarán todas las paradas en tablas en la base de datos |



| ID          | RI-3 | 
|-------------------|-------------|
|**Nombre**  |  Itinerarios de línea |    
|**Versión**  |  1.0, 30/11/2022 |
|**Autor**  |  David Hernández Carmona |
|**Referencias**  |  RF-07, RF-06, RF-05 |
|**Descripción**  | Recorrido que tiene que realizar el transporte  |
|**Datos Especificos**  | - Identificador de itinerario<br>- Tipo de Parada (inicial, final, etc.)<br>- Número de orden de la parada en la secuencia del itinerario<br>- Horas o frecuencias de paso planificada por cada parada|
|**Importancia**  | TBD  |
|**Estado**  |  Obligatorio |
|**Comentarios**  |  Hay itinerarios fijos asociados a las líneas y otros creados por el usuario en el momento de planificar el viaje |




| ID          | RI-4 | 
|-------------------|-------------|
|**Nombre**  |  Empresas |    
|**Versión**  | 1.0, 30/11/2022  |
|**Autor**  | David Hernández Carmona |
|**Referencias**  |  RF-06 |
|**Descripción**  | Las empresas encargadas de proporcionar los vehículos al sistema de transporte  |
|**Datos Especificos**  | - Identificador de empresa<br>- Nombre de la empresa <br>- Tipo de transporte <br> - Contacto |
|**Importancia**  |  TBD |
|**Estado**  | Obligatorio  |
|**Comentarios**  |  Ninguno |




| ID          | RI-5 | 
|-------------------|-------------|
|**Nombre**  |  Tarifas |    
|**Versión**  |  1.0, 30/11/2022 |
|**Autor**  | David Hernández Carmona |
|**Referencias**  | RF-06 |
|**Descripción**  | Precio de los tickets según itinerario  |
|**Datos Especificos**  |- Identificador de tarifa <br> - Precio<br> - Duración <br>- Líneas o itinerarios en los que es aplicada|
|**Importancia**  |  TBD |
|**Estado**  | Obligatorio  |
|**Comentarios**  |  En función de la empresa y el vehículo el precio de las tarifas variará |


| ID          | RI-6 | 
|-------------------|-------------|
|**Nombre**  | Administrador  |    
|**Versión**  | 1.0, 16/12/2022  |
|**Autor**  |  David Hernández Carmona |
|**Referencias**  | RF-09  |
|**Descripción**  |  Usuario que gestiona tanto los elementos de la web como los usuarios que intervienen en ella |
|**Datos Especificos**  |  - Identificador del administrador <br>- Correo Electronico<br>- Contraseña|
|**Importancia**  |  TBD |
|**Estado**  | Obligatorio  |
|**Comentarios**  |  Su logueo sería mediante una URL ‘especial’ con acceso limitado |

| ID          | RI-7 | 
|-------------------|-------------|
|**Nombre**  |  Usuario Registrado |    
|**Versión**  |  1.0, 16/12/2022 |
|**Autor**  |  David Hernández Carmona |
|**Referencias**  | RF-09  |
|**Descripción**  | Cualquier usuario que esté almacenado en la base de datos con su correo y contraseña  |
|**Datos Especificos**  | - Identificador de usuario<br>- Nombre y apellidos<br>- Dni <br>- Correo electrónico <br> - Contraseña|
|**Importancia**  |  TBD |
|**Estado**  |  Obligatorio |
|**Comentarios**  |  Ninguna |

| ID          | RI-8 | 
|-------------------|-------------|
|**Nombre**     | Administradores_Tarifas |    
|**Versión**  |  1.0, 16/12/2022 |
|**Autor**  | David Hernández Carmona |
|**Referencias**  |  RF-09 |
|**Descripción**  | Los administradores pueden modificar las tarifas si es necesario |
|**Datos Especificos**  | - Identificador del administrador<br> - Identificador de la tarifa modificada |
|**Importancia**  |  TBD |
|**Estado**  | Obligatorio  |
|**Comentarios**  |  Ninguno |

| ID          | RI-9 | 
|-------------------|-------------|
|**Nombre**  | Administradores_Paradas  |    
|**Versión**  | 1.0, 16/12/2022  |
|**Autor**  | David Hernández Carmona  |
|**Referencias**  |  RF-09, RF-05 |
|**Descripción**  | Los administradores pueden modificar las paradas si es necesario |
|**Datos Especificos**  | - Identificador de la parada<br>- Identificador del administrador|
|**Importancia**  |  TBD |
|**Estado**  | Obligatorio  |
|**Comentarios**  | Ninguno  |


| ID          | RI-10 | 
|-------------------|-------------|
|**Nombre**  | Administradores_Itinerarios  |    
|**Versión**  |  1.0, 16/12/2022 |
|**Autor**  |  David Hernández Carmona |
|**Referencias**  | RF-09,RF-07, RF-06, RF-05  |
|**Descripción**  | Los administradores pueden modificar los itinerarios si es necesario |
|**Datos Especificos**  | - Identificador del itinerario<br>- Identificador del administrador |
|**Importancia**  | TBD  |
|**Estado**  |  Obligatorio |
|**Comentarios**  | Ninguna  |



| ID          | RI-11 | 
|-------------------|-------------|
|**Nombre**  |  Administradores_Usuarios Registrados |    
|**Versión**  | 1.0, 16/12/2022  |
|**Autor**  | David Hernández Carmona  |
|**Referencias**  | RF-09  |
|**Descripción**  | Los administradores pueden modificar los usuarios registrados si es necesario  |
|**Datos Especificos**  | -Identificador del administrador <br>- Identificador  del usuario registrado |
|**Importancia**  |  TBD |
|**Estado**  |  Obligatorio |
|**Comentarios**  |  Ninguno |



| ID          | RI-12 | 
|-------------------|-------------|
|**Nombre**  |  Administradores_Líneas |    
|**Versión**  |  1.0, 16/12/2022 |
|**Autor**  | David Hernández Carmona |
|**Referencias**  |  RF-05, RF-06, RF-07, RF-09 |
|**Descripción**  | Los administradores pueden modificar las líneas si es necesario  |
|**Datos Especificos**  |  Identificador del administrador<br>-Identificador de la línea|
|**Importancia**  |  TBD |
|**Estado**  | Obligatorio  |
|**Comentarios**  |  Ninguno |



| ID          | RI-13 | 
|-------------------|-------------|
|**Nombre**  |  Itinerarios_Tarifa |    
|**Versión**  | 1.0, 16/12/2022  |
|**Autor**  | David Hernández Carmona  |
|**Referencias**  | RF-05, RF-06, RF-07  |
|**Descripción**  | El precio asociado a un itinerario calculado en base a los precios de las tarifas fijas  |
|**Datos Especificos**  | - Identificador de itinerario<br>- Identificador de la tarifa |
|**Importancia**  | TBD  |
|**Estado**  | Obligatorio  |
|**Comentarios**  | Ninguno  |



| ID          | RI-14 | 
|-------------------|-------------|
|**Nombre**  |  Itinerarios_Líneas |    
|**Versión**  |  1.0, 16/12/2022 |
|**Autor**  |  David Hernández Carmona |
|**Referencias**  | RF-05, RF-06, RF-07  |
|**Descripción**  |  Un itinerario puede englobar una o varias líneas en su recorrido |
|**Datos Especificos**  | - Identificador de la línea <br>- Identificador del itinerario|
|**Importancia**  |  TBD |
|**Estado**  |  Obligatorio |
|**Comentarios**  | Ninguno  |


| ID          | RI-15 | 
|-------------------|-------------|
|**Nombre**  | Líneas_Tarifa  |    
|**Versión**  |  1.0, 16/12/2022 |
|**Autor**  |  David Hernández Carmona |
|**Referencias**  |  RF-05, RF-06, RF-07 |
|**Descripción**  |  Cada línea tiene uno o varios precios asociados |
|**Datos Especificos**  | - Identificador de la línea<br>- Identificador de la tarifa
  |
|**Importancia**  |  TBD |
|**Estado**  |  Obligatorio |
|**Comentarios**  | Ninguno  |


| ID          | RI-16 | 
|-------------------|-------------|
|**Nombre**  |  Tarifa_Usuarios_Registrados |    
|**Versión**  | 1.0, 16/12/2022  |
|**Autor**  | David Hernández Carmona  |
|**Referencias**  |  RF-06, RF-09 |
|**Descripción**  |  Cada usuario debe pagar una tarifa ya sea para contratar el servicio de una línea o de un itinerario personalizado |
|**Datos Especificos**  | - Identificador de la tarifa <br> - Identificador del usuario  |
|**Importancia**  | TBD  |
|**Estado**  | Obligatorio  |
|**Comentarios**  | Ninguno  |


| ID          | RI-17 | 
|-------------------|-------------|
|**Nombre**  | Usuarios Registrados_Itinerarios  |    
|**Versión**  | 1.0, 16/12/2022  |
|**Autor**  | David Hernández Carmona  |
|**Referencias**  | RF-07, RF-06, RF-05, RF-09  |
|**Descripción**  | Cada usuario puede contratar un itinerario ya sea predeterminado (por una línea) o personalizado por el mismo usuario  |
|**Datos Especificos**  | - Identificador del usuario <br> - Identificador del itinerario <br> - Precio  |
|**Importancia**  | TBD  |
|**Estado**  | Obligatorio  |
|**Comentarios**  | Ninguno  |


| ID          | RI-18 | 
|-------------------|-------------|
|**Nombre**  | Tarjeta de transporte  |    
|**Versión**  | 1.0, 16/12/2022  |
|**Autor**  | David Hernández Carmona  |
|**Referencias**  | RF-12, RF-09  |
|**Descripción**  | Tarjeta asociada a un usuario registrado que almacena el número de viajes restantes.  |
|**Datos Especificos**  | - Identificador de la tarjeta <br> - Identificador del usuario <br> - Número de viajes disponibles  |
|**Importancia**  | TBD  |
|**Estado**  | Obligatorio  |
|**Comentarios**  | Ninguno  |


| ID          | RI-19 | 
|-------------------|-------------|
|**Nombre**  | Incidencias  |    
|**Versión**  | 1.0, 19/12/2022  |
|**Autor**  | Luca Daniel Gavriloaie  |
|**Referencias**  | RF-15, RF-09  |
|**Descripción**  | El sistema deberá almacenar información correspondiente a las incidencias que el administrador tenga que trasladar a la web.  |
|**Datos Especificos**  | - Identificador de la incidencia <br> - Identificador del administrador que la ha trasladado <br> - Nombre de la incidencia <br> - Fecha <br> - Lugar <br> - Línea <br> - Operador que la ha comunicado  |
|**Importancia**  | TBD  |
|**Estado**  | Obligatorio  |
|**Comentarios**  | Ninguno  |

<br>

### ***3.1.2 Requisitos Funcionales***
| RF-1            | Crear nuevas páginas    |
|-------------------|-------------|
| **Versión**  |  1.0 |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  | OBJ-1, OBJ-2  |
|**Requisitos asociados**  | RNF-1, RNF-2, RNF-4, RNF-5  |
|**Descripción**  | Permitir la ampliación de la Web si en algún momento posterior es necesario  |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  |  Esta función es necesaria para permitir el crecimiento de la plataforma |

| RF-2            | Modificar el diseño de la Web   |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  | OBJ-1, OBJ-2  |
|**Requisitos asociados**  | RNF-1,RNF-2, RNF-4, RNF-5  |
|**Descripción**  |  Permitir la modificación de la página Web de cualquier grupo contratado por la empresa para dicha función |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  |  Ninguno |

| RF-3            | Gestionar el contenido de la Web   |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  | OBJ-1, OBJ-2  |
|**Requisitos asociados**  |  RNF-1, RNF-4,RNF-5 |
|**Descripción**  |  Controlar el contenido que se publica en la Web |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  |  Ninguno |

| RF-4            | Realizar un seguimiento del portal    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  | OBJ-1, OBJ-2, OBJ-3  |
|**Requisitos asociados**  |  RNF-10 |
|**Descripción**  |  Monitorizar los viajes para adecuarlos al usuario |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-5            | Buscar contenido en la Web    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   | Daniel Perez Escarcena   |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  | OBJ-1, OBJ-2  |
|**Requisitos asociados**  | RI-1, RI-2,RNF-1,RNF-4, RNF-11  |
|**Descripción**  |  Navegar por la Web de forma más rápida |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-6            | Consultar de forma dinámica la información del servicio    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  | OBJ-1, OBJ-2, OBJ-3  |
|**Requisitos asociados**  | RI-1, RI2, RI-4,RI-5, RNF-1,RNF-8  |
|**Descripción**  |  Permite ver la información en tiempo real del viaje que estamos haciendo |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-7            | Ver itinerarios    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  |  OBJ-1, OBJ-2, OBJ-3 |
|**Requisitos asociados**  | RI-1, RNF-1  |
|**Descripción**  |  Permite ver todos los itinerarios disponibles al usuario |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-8            | Programar con antelación un viaje    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  | OBJ-1, OBJ-2, OBJ-3  |
|**Requisitos asociados**  | RNF-1,RNF-4  |
|**Descripción**  | Función que le permite al usuario reservar todos los traslados que necesita hacer para llegar a su destino a la vez  |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-9            | Iniciar sesión   |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |   Usuario administrador |
|**Objetivos asociados**  |  OBJ-1, OBJ-2 |
|**Requisitos asociados**  |  RI-7,RI-6,RNF-1,RNF-4, RNF-7 |
|**Descripción**  | Permite iniciar sesión en la aplicación a los usuarios  |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-10            | Calcular importe del itinerario a realizar    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  |  OBJ-1, OBJ-2, OBJ-3 |
|**Requisitos asociados**  | RNF-1  |
|**Descripción**  |  Después de planear el itinerario, te permite saber el costo total de todos los viajes que coges |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-11           | Enviar correo de confirmación de compra del itinerario    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   | Daniel Perez Escarcena   |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  | OBJ-1, OBJ-2 |
|**Requisitos asociados**  | RNF-7,RNF-12  |
|**Descripción**  | Una medida de seguridad para evitar fraudes y/o robos  |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-12           | Validar información introducida a la hora de hacer el pago    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Daniel Perez Escarcena  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  |  OBJ-1, OBJ-2 |
|**Requisitos asociados**  |  RNF-7,RNF-11,RNF-12,RI-18 |
|**Descripción**  |  Comprobar que la información introducida es real |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-13           | Pedir confirmación de compra en la aplicación antes de cobrar el pago a realizar    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   | Daniel Perez Escarcena   |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  |  OBJ-1, OBJ-2 |
|**Requisitos asociados**  | RNF-3, RNF-7, RNF-12  |
|**Descripción**  |  RNF-3, RNF-7, RNF-12 |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Ninguno  |

| RF-14            | Enviar código qr con información de la compra realizada    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   | Daniel Perez Escarcena   |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  |  OBJ-1, OBJ-2 |
|**Requisitos asociados**  |  RNF-3, RNF-7, RNF-12 |
|**Descripción**  |  Jutificante de la compra realizada |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  |  Seguro para confirmar que has realizado la compra |

| RF-15           | Mantenimiento y personal    |
|-------------------|-------------|
| **Versión**  | 1.0  |
| **Autores**   |  Toderic Ioan Stefan  |
| **Fuentes**   |  Usuario administrador  |
|**Objetivos asociados**  | OBJ-1, OBJ-2  |
|**Requisitos asociados**  |  RNF-6, RNF-9 |
|**Descripción**  | Proporcionar las herramientas para el mantenimiento del sistema  |
|**Importancia**  |  TBD |
|**Urgencia**  | Normal  |
|**Estado**  |  Obligatorio |
|**Estabilidad**  | Alta  |
|**Comentarios**  | Mantenimiento del sistema informático de la empresa  |


<br>

### ***3.1.3 Requisitos no Funcionales***
| RNF-1            | Tiempo de respuesta    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-01, RF-02, RF-03, RF-05, RF-06, RF-07, RF-08, RF-09, RF-10   |
| **Descripción**   | Tiempo de respuesta corto, baja  utilización de recursos, debe de ser accesible a todos los públicos, no tener un uso muy complejo.   |
| **Comentarios**   | Ninguno   |

| RNF-2            | Consistencia interna con la imagen corporativa de la AUTGC    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-01, RF-02   |
| **Descripción**   | El aspecto de la web debe ser similar con los colores, logo de la empresa   |
| **Comentarios**   | Ninguno   |

| RNF-3            | Compatibilidad y colaboración con el resto de sistemas informáticos de la AUT    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-13, RF-14   |
| **Descripción**   | Se deberán utilizar modelos, especificaciones, protocolos y herramientas compatibles con las otras herramientas de la AUTGC existentes en el momento de la adjudicación y preferentemente empleando modelos de datos de acuerdo con los estándares definidos por el CEN (Comité Europeo de Normalización).   |
| **Comentarios**   | Ninguno   |

| RNF-4            | Arquitectura modular y escalable    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-01, RF-02, RF-03, RF-05, RF-08, RF-09   |
| **Descripción**   | Se debe poder poner en marcha las distintas funcionalidades a medidas que vayan siendo comprobadas y válidas, permitiendo además las futuras ampliaciones que fuesen necesarias.  |
| **Comentarios**   | Ninguno   |

| RNF-5            | Multiplataforma    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-01, RF-02, RF-03   |
| **Descripción**   | Debe de ser multisistema , es decir ser capaz de acceder a la web desde todos los sistemas operativos y cualquier navegador existente en el mercado   |
| **Comentarios**   | Ninguno   |

| RNF-6            | Necesidad de contratación del personal    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-15   |
| **Descripción**   | Nosotros debemos de buscar y formar a la persona encargada de trasladar las información escrita por el conductor del autobús   |
| **Comentarios**   | Ninguno   |

| RNF-7            | Seguridad y protección de datos    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-09, RF-11, RF-12, RF-13, RF-14   |
| **Descripción**   | Se deberán incorporar mecanismos y medidas de seguridad (protocolos y servicios seguros, certificados, firma electrónica, etc.) con el objeto de garantizar la seguridad de las transacciones que se puedan realizar y para dar una imagen de seguridad y tecnología avanzada al sitio.   |
| **Comentarios**   | Ninguno   |

| RNF-8            | La visualización de las alarmas debe ser simultánea    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-06   |
| **Descripción**   | Deberán poderse manifestar mediante avisos acústicos, visuales, mensajes a móviles y cualesquiera otros mecanismos se considere conveniente   |
| **Comentarios**   | Ninguno   |

| RNF-9            | Contratación del personal para el mantenimiento del sistema    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-15   |
| **Descripción**   | Se deberá contratar un equipo de informáticos para realizar un mantenimiento al sistema   |
| **Comentarios**   | Ninguno   |

| RNF-10            | Posicionamiento WEB    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-04   |
| **Descripción**   | La página Web resultante deberá estar preparada para facilitar el posicionamiento natural en los principales buscadores de ámbito nacional e internacional para ello se deberán emplear las técnicas apropiadas.   |
| **Comentarios**   | Ninguno   |

| RNF-11            | Gestión de edición en otros idiomas    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-05   |
| **Descripción**   | La edición en español debe de ofrecer la posibilidad de clonar de forma sencilla la página para la traducción a otros de los idiomas contemplados en el sitio. Todas las ediciones en los distintos idiomas deberán tener las mismas funcionalidades y gestionarse del mismo modo.(Ingles, aleman, frances y español) |
| **Comentarios**   | Ninguno   |

| RNF-12            | Sistemas de pago y comercio electrónico    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-11, RF-12   |
| **Descripción**   | Se deberá contemplar todos los subsistemas, interfaces, desarrollos e implementaciones necesarias para permitir la recarga, consulta, y cualquier operación relativa al título único del transporte de Gran Canaria.   |
| **Comentarios**   | Ninguno   |


<br>

## **3.2 Casos de uso**

### ***Lista de diagramas de casos de uso del modelo***
Para identificar de manera más cómoda las funcionalidades del sistema, hemos realizado tres diagramas de casos de uso: uno que comprende las funcionalidades de los usuarios registrado y no registrado y el sistema, otro para el actor administrador y un último para el servicio externo de correo.


### ***Diagramas de casos de uso***<br>
- Sistema, Usuario registrado y Usuario no registrado.<br>
![Diagrama de casos de uso de los actores Sistema, Usuario registrado y Usuario no registrado](/Proyecto/src/DCU%20sistema%2C%20usuario%20registrado%20y%20usuario%20no%20registrado.svg)

- Administrador<br>
![Diagrama de casos de uso del actor Administrador](/Proyecto/src/DCU%20administrador.svg)

- Servicio de correo<br>
![Diagrama de casos de uso del actor externo Servicio de correo](/Proyecto/src/DCU%20servicio%20de%20correo.svg)

<br>

### ***Lista general de casos de uso  y actores del proyecto***
| ACT-01           | Usuario registrado    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-5, RF-6, RF-7, RF-8, RF-10, RF-12 |
| **Descripción**   | Conjunto de usuarios que interactúan con el sistema y que están registrados en el mismo, teniendo funcionalidades especiales como comprar un billete para un itinerario, después del inicio de sesión requerido, además de las funcionalidades básicas como buscar contenido o planificar una ruta, entre otras.   |
| **Comentarios**   | Ninguno   |

| ACT-02           | Usuario no registrado    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-5, RF-6, RF-7, RF-8, RF-9 |
| **Descripción**   | Este actor engloba a los usuarios que utilizan el sistema como invitados, disfrutando de las funcionalidades básicas, como buscar contenido o planificar una ruta, entre otras.   |
| **Comentarios**   | Ninguno   |

| ACT-03           | Administrador    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-1, RF-2, RF-3, RF-4, RF-5, RF-6, RF-7, RF-8, RF-9, RF-15 |
| **Descripción**   | El actor Administrador se refiere a aquel usuario del sistema cuyo objetivo principal es hacer seguimiento y gestionar el contenido y diseño del sistema, así como monitorizar el uso de la red de transporte.   |
| **Comentarios**   | Ninguno   |

| ACT-04           | Sistema    |
|-------------------|-------------|
| **Requisitos asociados**  | RF-1, RF-2, RF-3, RF-4, RF-5, RF-6, RF-7, RF-8, RF-9, RF-10, RF-11, RF-12, RF-13, RF-14, RF-15 |
| **Descripción**   | El actor Sistema se encarga del correcto funcionamiento de las partes monitorizadas del sistema   |
| **Comentarios**   | Ninguno   |

| ACT-05           | Servicio de correo |
|-------------------|-------------|
| **Requisitos asociados**  | RF-11, RF-14 |
| **Descripción**   | El actor Servicio de correo se encarga de mandar los mensajes que le informa el sistema al correo del usuario correspondiente.  |
| **Comentarios**   | Ninguno   |

### ***Detalle de los casos de uso***

| **ID**                | CU-01                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Calcular distancia entre paradas     |
| **Autor**             |    Toderic Ioan stefan     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El sistema es capaz de calcular la distancia entre dos paradas seleccionadas     |
| **Actores**           |    Sistema     |
| **Precondiciones**    |   Haber seleccionado dos paradas, independientemente de la forma (desde el mapa, en la planificación de itinerario, etc.)     |
| **Flujo Normal**      |    1. El sistema realiza un cálculo de la distancia entre las paradas seleccionadas teniendo en  cuenta la información geográfica del SI. <br> 2. El sistema devuelve un pop-up con la distancia en kilómetros. |
| **Flujo alternativo** |    Ninguno     |
| **Post Condiciones**  |    Ninguna     |
| **Referencias**       |    CU-07       |



| **ID**                | CU-02                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Ver instrucciones de itinerario     |
| **Autor**             |    Daniel Pérez Escarcena     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El usuario puede ver las distintas opciones que ofrece el itinerario que está visualizando en ese momento     |
| **Actores**           |    Usuario no registrado, Usuario registrado     |
| **Precondiciones**    |   Seleccionar el itinerario que quieres ver     |
| **Flujo Normal**      |    1. El usuario solicita al sistema instrucciones para llevar a cabo el itinerario pulsando un botón.<br>  2. El sistema muestra las instrucciones que debe seguir el usuario para cumplir con itinerario. |
| **Flujo alternativo** |    Ninguno     |
| **Post Condiciones**  |    Ninguna     |
| **Referencias**       |    CU-06       |



| **ID**                | CU-03                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Calcular tiempos de recorrido   |
| **Autor**             |    Toderic Ioan stefan     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El sistema es capaz de devolver la duración del viaje entre dos paradas seleccionadas     |
| **Actores**           |    Sistema     |
| **Precondiciones**    |   Haber seleccionado dos paradas     |
| **Flujo Normal**      |   1. El sistema evalúa las condiciones reales de tráfico y los factores influyentes consultando el sistema de información.<br>2. El sistema realiza un cálculo estimado del tiempo de recorrido teniendo en cuenta la información en tiempo real.<br>3. El sistema devuelve un pop-up con el tiempo estimado en minutos  y un pequeño resumen de la parada de origen y destino seleccionadas previamente. |
| **Flujo alternativo** |    Ninguno     |
| **Post Condiciones**  |    Ninguna     |
| **Referencias**       |    CU-07       |



| **ID**                | CU-04                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Realizar estadísticas     |
| **Autor**             |    Toderic Ioan stefan     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El sistema está programado para realizar periódicamente estadísticas, en la cual se podrá ver la mejor valoración entre todas las líneas, cuál de ellas está más concurrida…      |
| **Actores**           |    Sistema     |
| **Precondiciones**    |   Ninguna     |
| **Flujo Normal**      |   1. El sistema toma la información de la base de datos <br> 2. El sistema devuelve de forma gráfica las líneas más concurridas, las líneas con mejores valoraciones o cualquier otra estadística sobre el último periodo de tiempo. <br>3. El sistema pregunta al usuario si desea obtener las estadísticas como un informe descargable.|
| **Flujo alternativo** |    2A. Si existen aspectos sin medir, solo se mostrarán las estadísticas disponibles en ese momento.    |
| **Post Condiciones**  |    Ninguna     |
| **Referencias**       |    Ninguna     |



| **ID**                | CU-05                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Ajustar parámetros de búsqueda     |
| **Autor**             |    Daniel Pérez Escarcena     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El usuario escribe las condiciones que debe cumplir su ruta     |
| **Actores**           |    Usuario no registrado, Usuario registrado     |
| **Precondiciones**    |  El usuario debe haber accedido a la opción de planificar una ruta     |
| **Flujo Normal**      |    1. El usuario solicita al sistema ajustar los parámetros de búsqueda.<br> 2. El sistema solicita seleccionar un origen y un destino mostrándole una lista.<br> 3. El usuario proporciona al sistema dicha información.<br> 4. El sistema solicita indicar una fecha y una hora.<br> 5. El usuario introduce la fecha y la hora deseadas. <br>6.  El sistema solicita seleccionar un aspecto a potenciar en la planificación (menor duración, número de transbordos, el menor precio).<br>7.  El usuario indica el aspecto que quiere potenciar.<br> 8. El usuario guarda los parámetros configurados |
| **Flujo alternativo** |   Ninguno. El usuario puede dejar parámetros sin definir.     |
| **Post Condiciones**  |    Ninguna (los parámetros se guardan temporalmente solo para una planificación en particular, no se guardan en la base de datos)    |
| **Referencias**       |    CU-07       |




| **ID**                | CU-06                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Ver itinerario    |
| **Autor**             |    Daniel Pérez Escarcena     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El usuario puede ver el itinerario elegido     |
| **Actores**           |   Usuario no registrado, Usuario registrado     |
| **Precondiciones**    |   El usuario debe haber accedido a la opción de planificar una ruta.    |
| **Flujo Normal**      |    1. El usuario selecciona un itinerario.<br> 2. El sistema muestra información del itinerario.|
| **Flujo alternativo** |    2b. El usuario no encuentra ningun itinerario que se adecue a sus necesidades    |
| **Post Condiciones**  |    Ninguna    |
| **Referencias**       |    CU-07       |



| **ID**                | CU-07                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Planificar una ruta    |
| **Autor**             |    Daniel Pérez Escarcena     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El usuario puede planificar una ruta que se adecue a sus necesidades     |
| **Actores**           |   Usuario no registrado, Usuario registrado     |
| **Precondiciones**    |   Entrar en la sección de rutas    |
| **Flujo Normal**      | 1. El usuario solicita al sistema planificar un itinerario.<br> 2. El usuario solicita al sistema ajustar los parámetros de búsqueda.<br>3. El sistema solicita seleccionar un origen y un destino mostrándole una lista. <br> 4. El usuario proporciona al sistema dicha información. <br> 5. El sistema solicita indicar una fecha y una hora.<br> 6. El usuario introduce la fecha y la hora deseadas.<br>7. El sistema solicita seleccionar un aspecto a potenciar en la planificación (menor duración, número de transbordos, el menor precio).<br>8. El usuario indica el aspecto que quiere potenciar.<br>9. El usuario guarda los parámetros configurados<br>10. El usuario pulsa el botón para planificar la ruta descrita.<br>11. El sistema calcula el mejor itinerario para los filtros aplicados.<br>12. El sistema definirá los transbordos que se deben hacer comprobando cuál sería la mejor conexión entre las distintas líneas y medios de transporte disponibles.<br>13. El sistema muestra los transbordos que debe tomar para realizar el itinerario.<br>14. El sistema muestra una lista con los itinerarios que se adaptan a sus condiciones de búsqueda.<br>15. El usuario selecciona el itinerario deseado.<br>16. El sistema muestra información del itinerario.<br>17. El usuario solicita al sistema instrucciones para llevar a cabo el itinerario pulsando un botón.<br>18. El sistema muestra las instrucciones que debe seguir el usuario para cumplir con el itinerario.<br>19. El sistema evalúa las condiciones reales de tráfico y los factores influyentes consultando el sistema de información.<br>20. El sistema realiza un cálculo estimado del tiempo de recorrido teniendo en cuenta la información en tiempo real.<br>21. El sistema devuelve un pop-up con el tiempo estimado en minutos  y un pequeño resumen de la parada de origen y destino seleccionadas previamente.<br>22. El sistema realiza un cálculo de la distancia entre las paradas seleccionadas teniendo en cuenta la información geográfica del SI.<br>23. El sistema devuelve un pop-up con la distancia en kilómetros|
| **Flujo alternativo** |    12A. Si existe una línea con ese recorrido, le mostrará al usuario dicha línea y que no necesita realizar transbordos.<br>15A. El usuario no encuentra ningun itinerario que se adecue a sus necesidades  |
| **Post Condiciones**  |    Ninguna    |
| **Referencias**       |    Ninguna    |


| **ID**                | CU-08                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Definir Transbordos     |
| **Autor**             |    Daniel Pérez Escarcena     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |   El usuario puede ver los transbordos que debe tomar para llegar a la ruta deseada     |
| **Actores**           |    Usuario no registrado, Usuario registrado, Sistema     |
| **Precondiciones**    |   El usuario debe haber accedido a la opción de planificar una ruta (origen y destino seleccionados)  |
| **Flujo Normal**      |  1. El sistema definirá los transbordos que se deben hacer comprobando cuál sería la mejor conexión entre las distintas líneas y medios de transporte disponibles.<br> 2. El sistema muestra los transbordos que debe tomar para realizar el itinerario.|
| **Flujo alternativo** |    1A. Si existe una línea con ese recorrido, le mostrará al usuario dicha línea y que no necesita realizar transbordos.     |
| **Post Condiciones**  |   Ninguna   |
| **Referencias**       |   CU-07     |


| **ID**                | CU-09                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Identificar zonas no transitables     |
| **Autor**             |    Toderic Ioan stefan     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |   El sistema es capaz de identificar aquellos recorridos intransitables (Zonas de alto tráfico, zonas con un accidente)     |
| **Actores**           |    Sistema     |
| **Precondiciones**    |   Ninguna |
| **Flujo Normal**      |  1. El sistema toma información de la base de datos<br> 2. En base a la información de las incidencias recibidas y la información geográfica <br> 3.El sistema devuelve un resumen con las zonas intransitables|
| **Flujo alternativo** |    3A. El sistema no encuentra zonas intransitables<br> 3A.1. El sistema devuelve un mensaje en el cual se especifica que todas las zonas están disponibles |
| **Post Condiciones**  |   Ninguna   |
| **Referencias**       |   Ninguna   |


| **ID**                | CU-10                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Visualizar alarmas     |
| **Autor**             |    Daniel Pérez Escarcena     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |   El usuario puede ver las alarmas que informan todas las incidencias que han ocurrido |
| **Actores**           |    Usuario no registrado, Usuario registrado |
| **Precondiciones**    |   El usuario debe haber accedido a la aplicación |
| **Flujo Normal**      |  1. El usuario accede al panel de avisos. <br> 2. El sistema muestra las alarmas que los administradores han activado. <br> 3. El usuario clica en una alarma para poder obtener más información de ella <br> 4. El sistema ofrece información detallada sobre la alarma, como el asunto, la fecha y la descripción de la misma.|
| **Flujo alternativo** |    2b. No hay ninguna alarma disponible |
| **Post Condiciones**  |   Ninguna   |
| **Referencias**       |   Ninguna   |



| **ID** | CU-11 |
|--|--|
| **Nombre**            | Listar horarios y servicios |
| **Autor**             | Daniel Pérez Escarcena |
| **Fecha**             | 16/12/2022 |
| **Descripción**       | El usuario puede ver los horarios de los servicios disponibles |
| **Actores**           | Usuario no registrado, Usuario registrado |
| **Precondiciones**    | El usuario debe haber accedido a la aplicación |
| **Flujo Normal**      | 1. El usuario entra dentro de la aplicación<br> 2. El usuario entra en la opción de horarios <br> 3.El sistema muestra todos los horarios disponibles en ese momento <br> 4. El usuario busca el horario del servicio que va a utilizar <br> 5. Acceder al horario seleccionado |
| **Flujo alternativo** | 2b. No hay ninguna alarma disponible |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | Ninguna |


| **ID** | CU-12 |
|--|--|
| **Nombre**            | Ver sitios de interés |
| **Autor**             | Toderic Ioan Stefan |
| **Fecha**             | 16/12/2022 |
| **Descripción**       | El sistema tiene itinerarios que pasan por sitios de interés y estos se podrán ver |
| **Actores**           | Usuario no registrado, Usuario registrado |
| **Precondiciones**    | Ninguna |
| **Flujo Normal**      | 1. El usuario accede a la sección de sitios de interés <br> 2. El usuario selecciona un sitio entre todos los disponibles en el portal web <br> 3. El sistema le ofrece la posibilidad de ir <br> 4. El usuario aceptar e  ir <br> 5. El sistema abre una pestaña con el método de pago  <br> 6. El usuario introduce los datos pertinentes y envía el pago |
| **Flujo alternativo** | 4. A El usuario decide no aceptar y selecciona “no” |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | Ninguna |


| **ID** | CU-13 |
|--|--|
| **Nombre**            | Ver lineas |
| **Autor**             | Toderic Ioan Stefan  |
| **Fecha**             | 16/12/2022 |
| **Descripción**       | Le permite al usuario ver las líneas disponibles |
| **Actores**           | Usuario no registrado, Usuario registrado |
| **Precondiciones**    | El usuario debe haber accedido a la aplicación |
| **Flujo Normal**      | 1. El usuario selecciona el apartado donde se muestran las líneas disponibles <br> 2. El sistema muestra todas las líneas <br> 3. El usuarios selecciona una de las líneas disponibles <br>4. El sistema devuelve la información de la línea sin detalle |
| **Flujo alternativo** |  1.A El usuario hace click sobre en el botón ver más detalle de la línea <br> 1.A1 El sistema devuelve en una pestaña nueva toda la información     detallada de la línea seleccionada |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-14, CU-15, CU-16 |


| **ID** | CU-14 |
|--|--|
| **Nombre**            | Ver información de la línea |
| **Autor**             | Toderic Ioan Stefan |
| **Fecha**             | 16/12/2022 |
| **Descripción**       | Ofrece de manera detallada información sobre la línea seleccionada |
| **Actores**           | Usuario no registrado, Usuario registrado |
| **Precondiciones**    | El usuario debe haber accedido a la aplicación |
| **Flujo Normal**      |  1. El usuario hace click sobre en el botón ver más detalle de la línea <br> 2. El sistema devuelve en una pestaña nueva toda la información       detallada de la línea seleccionada
 |
| **Flujo alternativo** | Ninguna |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-13 |


| **ID** | CU-15 |
|--|--|
| **Nombre**            | Ver Posición de los transportes |
| **Autor**             | Toderic Ioan Stefan |
| **Fecha**             | 16/12/2022 |
| **Descripción**       | Ofrece la posibilidad de ver la posición del transporte de esa línea en tiempo real |
| **Actores**           | Usuario no registrado, Usuario registrado |
| **Precondiciones**    | Ninguna |
| **Flujo Normal**      | 1. El usuario hace clic sobre el botón de “Ver posición” <br> 2. El sistema dibuja en el mapa los medios transporte ofreciendo su ubicación en tiempo real |
| **Flujo alternativo** | Ninguno |
| **Post Condiciones**  | Ninguno |
| **Referencias**       | CU-13 |


| **ID** | CU-16 |
|--|--|
| **Nombre**            | Ver mapa |
| **Autor**             | Toderic Ioan Stefan |
| **Fecha**             | 16/12/2022 |
| **Descripción**       | Brinda toda la información del mapa con las líneas disponibles |
| **Actores**           | Usuario no registrado, Usuario registrado |
| **Precondiciones**    | El usuario debe haber accedido a la aplicación |
| **Flujo Normal**      | 1. El usuario entra en la sección de ver mapa <br> 2. El sistema ofrece la posibilidad de ver cartográficamente las líneas y las paradas con la posibilidad de ser seleccionadas (Opcionalmente) |
| **Flujo alternativo** | 2.A El usuario se desplaza por el mapa <br> 2.B El usuarios selecciona una de las líneas disponibles <br> - 2.B2 El sistema devuelve la información de la línea sin detalle <br> 2.C El usuario selecciona una de las líneas disponibles <br> - 2.C1 El sistema devuelve la información de la línea sin detalle |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-13, CU-17 |


| **ID** | CU-17 |
|--|--|
| **Nombre**            | Desplazarse por el mapa |
| **Autor**             | Toderic Ioan Stefan |
| **Fecha**             | 16/12/2022 |
| **Descripción**       | Ofrece la posibilidad de desplazarse por el mapa, haciendo zoom in, zoom out |
| **Actores**           | Usuario no registrado, Usuario registrado |
| **Precondiciones**    | Ninguna |
| **Flujo Normal**      | 1. El usuario se desplaza por el mapa |
| **Flujo alternativo** | Ninguno |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-16 |


| **ID** | CU-18 |
|--|--|
| **Nombre**            | Ver paradas |
| **Autor**             | Toderic Ioan Stefan |
| **Fecha**             | 16/12/2022 |
| **Descripción**       | Brinda toda la información acerca de las paradas |
| **Actores**           | Usuario no registrado, Usuario registrado |
| **Precondiciones**    | El usuario debe haber accedido a la aplicación |
| **Flujo Normal**      | 1. El usuario entra en la sección de paradas <br> 2. El sistema le ofrece la posibilidad de  ver las paradas en el mapa <br> 3. El usuario selecciona la opción de ver paradas dentro del mapa |
| **Flujo alternativo** | 2.A El sistema le ofrece la posibilidad de ver la informacion detallada de una parada |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-19 |


| **ID**                | CU-20                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Registrarse     |
| **Autor**             |    Luca Daniel Gavriloaie     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    Permite la realización del registro de un usuario en el sistema.     |
| **Actores**           |    Usuario no registrado     |
| **Precondiciones**    |   Acceder al portal web.   |
| **Flujo Normal**      |   1. El actor solicita al sistema registrarse en el mismo.<br>2.El sistema muestra la interfaz de registro y solicita la introducción de los datos de registro: nombre y apellidos, dni, correo electrónico y contraseña.<br>3.El usuario introduce los datos requeridos.<br>4.El sistema valida que los datos introducidos sean correctos.<br>5.El sistema registra en la base de datos al usuario.|
| **Flujo alternativo** |    4A. Si los datos introducidos son incorrectos, el sistema notifica al usuario del error.     |
| **Post Condiciones**  |    El sistema registra en la base de datos al usuario.     |
| **Referencias**       |   Ninguna       |

| **ID**                | CU-21                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Iniciar sesión     |
| **Autor**             |    Luca Daniel Gavriloaie     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    Permite el inicio de sesión de los usuarios registrados en el sistema.    |
| **Actores**           |    Usuario no registrado     |
| **Precondiciones**    |   El usuario debe estar registrado en el sistema.     |
| **Flujo Normal**      |   1.El actor solicita al sistema iniciar sesión.<br>2.El sistema solicita al usuario introducir las credenciales del inicio de sesión.<br>3.El usuario introduce las credenciales.<br>4.El sistema realiza la validación de dichas credenciales.<br>5.Si las credenciales son correctas, el sistema muestra al usuario la página de inicio. |
| **Flujo alternativo** |    5A. Si las credenciales son incorrectas, el sistema notificará al usuario del error y solicitará volver a introducir las credenciales.     |
| **Post Condiciones**  |    Ninguna     |
| **Referencias**       |    Ninguna      |

| **ID**                | CU-22                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Comprar billetes     |
| **Autor**             |    Luca Daniel Gavriloaie     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    Permite la compra de billetes para los itinerarios planificados.     |
| **Actores**           |    Usuario registrado     |
| **Precondiciones**    |   El usuario debe estar dado de alta en el sistema.     |
| **Flujo Normal**      |    1.El usuario planifica una ruta.<br>2.El sistema muestra el precio del billete para la ruta.<br>3.El usuario pulsa el botón de comprar un billete para el itinerario.<br>4.El sistema solicita seleccionar una forma de pago.<br>5.El usuario selecciona el método de pago deseado.<br>6.El sistema solicita realizar el pago.<br>7.El usuario realiza el pago confirmando el precio. |
| **Flujo alternativo** |    3A. Si algún medio de transporte del itinerario planificado está lleno, el sistema notifica al usuario y aborta el proceso de compra.     |
| **Post Condiciones**  |   El sistema guarda en la base de datos la compra realizada     |
| **Referencias**       |    Ninguna       |

| **ID**                | CU-23                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Consultar saldo de tarjeta    |
| **Autor**             |    Luca Daniel Gavriloaie     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    Permite consultar el saldo disponible en la tarjeta (título único de transporte).     |
| **Actores**           |    Usuario registrado     |
| **Precondiciones**    |   El usuario debe estar dado de alta en el sistema.|
| **Flujo Normal**      |   1.El usuario accede a la sección de su perfil.<br>2.El usuario solicita al sistema consultar el saldo de su tarjeta.<br>3.El sistema consulta en la base de datos la tarjeta del usuario y su saldo.<br>4.El sistema muestra información sobre el saldo de la tarjeta |
| **Flujo alternativo** |    2A. Si el usuario no tiene ninguna tarjeta registrada, el sistema notifica del error.     |
| **Post Condiciones**  |    Ninguna     |
| **Referencias**       |   Ninguna       |

| **ID**                | CU-24                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Valorar un itinerario     |
| **Autor**             |    Luca Daniel Gavriloaie     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    Permite la valoración de la experiencia del usuario con un itinerario. |
| **Actores**           |    Usuario registrado     |
| **Precondiciones**    |   El usuario debe estar dado de alta en el sistema y debe haber usado el servicio de transporte en ese itinerario. |
| **Flujo Normal**      |    1.El usuario busca el itinerario que ha seguido introduciendo los mismos parámetros que usó para planificarlo.<br>2.El sistema muestra el itinerario.<br>3.El usuario solicita al sistema valorar el itinerario pulsando un botón.<br>4.El sistema solicita el justificante de compra del itinerario.<br>5.El usuario proporciona el justificante de compra del itinerario.<br>6.El sistema solicita al usuario introducir una valoración por escrito y una puntuación numérica.<br>7.El usuario introduce la valoración y la puntuación y la envía. |
| **Flujo alternativo** |    Ninguno     |
| **Post Condiciones**  |    El sistema guarda la valoración del itinerario.     |
| **Referencias**       |    Ninguna       |

| **ID**                | CU-25                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Buscar contenido en el portal     |
| **Autor**             |    Guillermo Morales Caparros     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    Se muestra el contenido del portal de la página donde el usuario puede moverse libremente    |
| **Actores**           |    Usuario registrado y No registrado     |
| **Precondiciones**    |   El usuario debe haber accedido a la aplicación  |
| **Flujo Normal**      |    1.El usuario accede al apartado de busqueda de la aplicación<br>2.El usuario introduce lo que quiere buscar<br>3.El usuario añade filtros de búsqueda para acortar esta misma y que le de opciones más precisas con respecto a lo que busca<br>4.El sistema le muestra las coincidencias de su búsqueda |
| **Flujo alternativo** |   4A. No existen coincidencias con respecto a lo que busca     |
| **Post Condiciones**  |    Ninguna     |
| **Referencias**       |    Ninguna       |

| **ID**                | CU-26                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Ver calendario     |
| **Autor**             |    Guillermo Morales Caparrós     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    Se muestra el calendario en la fecha actual     |
| **Actores**           |    Usuario registrado y No registrado     |
| **Precondiciones**    |   El usuario debe acceder a la página Web    |
| **Flujo Normal**      |    1.El usuario entra en la opción de calendario<br>2.El sistema le muestra los diferentes tipos de calendarios de la Web (fiestas, itinerarios, etc)<br>3.El usuario elige un calendario en específico<br>4.El sistema le muestra por pantalla el calendario |
| **Flujo alternativo** |    Ninguno     |
| **Post Condiciones**  |    Ninguna     |
| **Referencias**       |    Ninguna       |

| **ID**                | CU-27                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |   Modificar contenido     |
| **Autor**             |   David Hernández Carmona     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El administrador puede modificar cualquier dato que se muestre en la web     |
| **Actores**           |    Usuario administrador     |
| **Precondiciones**    |   Que el usuario administrador esté previamente logueado |
| **Flujo Normal**      |    1.El administrador visualiza la web y sus contenidos<br>2.El administrador identifica un error o algún dato a corregir y lo selecciona<br>3.El administrador introduce en su lugar el dato que crea conveniente y lo almacena|
| **Flujo alternativo** |    2b. El administrador modifica el error seleccionado     |
| **Post Condiciones**  |   Las modificaciones se reflejan en la base de datos    |
| **Referencias**       |   UC-28      |

| **ID**                | CU-28                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Gestionar contenido de la Web     |
| **Autor**             |    Daniel Pérez Escarcena     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El administrador gestiona todo el contenido proporcionado en la web     |
| **Actores**           |   Usuario administrador     |
| **Precondiciones**    |  Que el usuario administrador esté previamente logueado    |
| **Flujo Normal**      |    1.El administrador visualiza la web y sus contenidos<br>2.El administrador identifica un error o algún dato a corregir y lo selecciona<br>3.El administrador introduce en su lugar el dato que crea conveniente y lo almacena |
| **Flujo alternativo** |    1b. El administrador crea una nueva sección dentro de la página Web<br>2b. El administrador modifica el error seleccionado<br>2c. El administrador elimina el contenido seleccionado dentro de la página Web |
| **Post Condiciones**  |    Las modificaciones se reflejan en la base de datos     |
| **Referencias**       |    Ninguna       |

| **ID**                | CU-29                                           |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Eliminar contenido     |
| **Autor**             |    Daniel Pérez Escarcena     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El administrador puede crear contenido en la Web     |
| **Actores**           |    Usuario administrador     |
| **Precondiciones**    |   Que el usuario administrador esté previamente logueado  |
| **Flujo Normal**      |    1.El administrador visualiza la web y sus contenidos<br>2.El administrador identifica un error o algún dato a corregir y lo selecciona<br>3.El administrador introduce en su lugar el dato que crea conveniente y lo almacena |
| **Flujo alternativo** |    2b. El administrador elimina el contenido seleccionado dentro de la página Web     |
| **Post Condiciones**  |   Las modificaciones se reflejan en la base de datos     |
| **Referencias**       |    CU-28       |

| **ID**                | CU-30                                          |
|-----------------------|-------------------------------------------------|
| **Nombre**            |    Crear contenido    |
| **Autor**             |    Daniel Pérez Escarcena     |
| **Fecha**             |    16/12/2022     |
| **Descripción**       |    El administrador puede crear contenido en la Web |
| **Actores**           |    Administrador     |
| **Precondiciones**    |   Que el usuario administrador esté previamente logueado     |
| **Flujo Normal**      | 1. El administrador visualiza la web y sus contenidos <br> 2. El administrador identifica un error o algún dato a corregir y lo selecciona <br> 3. El administrador introduce en su lugar el dato que crea conveniente y lo almacena   |
| **Flujo alternativo** |    1B. El administrador crea una nueva sección dentro de la página Web     |
| **Post Condiciones**  |    Las modificaciones se reflejan en la base de datos     |
| **Referencias**       |    CU-28       |

| **ID** | CU-31 |
|--|--|
| **Nombre**            | Avisar de Alarma |
| **Autor**             | Guillermo Morales Caparrós |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | Esta función habilita al administrador informar sobre una alarma |
| **Actores**           | Administrador |
| **Precondiciones**    | El administrador debe estar dado de alta en el sistema |
| **Flujo Normal**      | 1. El Administrador selecciona la opción de avisar <br> 2. Escribe un mensaje a modo de notificación <br> 3. En la web se muestra un icono de alarma <br> 4. Al colocar el ratón sobre el icono se muestra un cartelito con el mensaje que ha escrito el administrador |
| **Flujo alternativo** | Ninguno |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | Ninguna |

| **ID** | CU-32 |
|--|--|
| **Nombre**            | Trasladar incidencias a la Web |
| **Autor**             | Guillermo Morales Caparrós |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | Esta función la desempeña el administrador para informar sobre las incidencias que le transmiten los conductores de las guaguas |
| **Actores**           | Administrador |
| **Precondiciones**    | El administrador debe estar dado de alta en el sistema. Recibir la información a través de un papel físico (informe de los conductores). |
| **Flujo Normal**      | 1. El administrador solicita al sistema trasladar una incidencia a la web accediendo a la sección correspondiente para ello. <br> 2. El sistema solicita completar la información de la incidencia. <br> 3.El administrador introduce la información de la incidencia (nombre, fecha, lugar, línea, operador que la ha notificado). <br> 4. El administrador pulsa activar la incidencia en el sistema. <br> 5. El sistema hace visible la incidencia en la página web para el resto de usuarios. |
| **Flujo alternativo** | 4A. Si el administrador no ha introducido ninguna información, el sistema se lo pedirá mediante un aviso. <br> 4B. Si la información introducida es errónea, el administrador será notificado del error. |
| **Post Condiciones**  | El sistema guarda la incidencia en la base de datos. |
| **Referencias**       | Ninguna. |

| **ID** | CU-33 |
|--|--|
| **Nombre**            | Monitorizar estado de la red de transporte |
| **Autor**             | Guillermo Morales Caparrós |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | Se muestra por pantalla una serie de características actuales referentes al estado de la red de transportes junto con las cámaras. Si hay alguna línea bloqueada, si hay atrasos, si está correcto… |
| **Actores**           | Administrador |
| **Precondiciones**    | El administrador debe estar identificado |
| **Flujo Normal**      | 1. El administrador accede al mapa de la red de Transporte. <br> 2. El sistema le muestra en tiempo real los movimientos que realizan cada vehículo <br> 3. El administrador puede seleccionar un transporte en concreto para ver la informacion de este. <br> 4. El sistema muestra una pantalla donde estan los detalles del estado de la red por la que conduce. |
| **Flujo alternativo** | Ninguno |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-34, CU-35, CU-36 |

| **ID** | CU-34 |
|--|--|
| **Nombre**            | Visualizar video de las cámaras |
| **Autor**             | Guillermo Morales Caparrós |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | Se abre una pestaña en la que se pueden seleccionar los videos de las cámaras en tiempo real |
| **Actores**           | Administrador |
| **Precondiciones**    | El administrador debe estar identificado |
| **Flujo Normal**      | 1. El administrador accede al mapa de transportes en tiempo real. <br> 2. El sistema le muestra los transportes que están operativos en ese momento <br> 3. El administrador selecciona el transporte que quiere ver <br> 4. El sistema le muestra las cámaras en tiempo real de ese transporte |
| **Flujo alternativo** | Ninguno |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-33 |

| **ID** | CU-35 |
|--|--|
| **Nombre**            | Simular la situación real |
| **Autor**             | Guillermo Morales Caparrós |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | Se muestran las características actuales del medio de transporte |
| **Actores**           | Administrador |
| **Precondiciones**    | El administrador debe estar identificado |
| **Flujo Normal**      | 1. El administrador accede a la sección a la sección de simulación <br> 2. El administrador elige el transporte que quiere visualizar <br> 3. El sistema muestra la información en tiempo real del estado del transporte |
| **Flujo alternativo** | 2B. El sistema muestra un mensaje de que el transporte no está en uso en este momento |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-33 |

| **ID** | CU-36 |
|--|--|
| **Nombre**            | Comprobar cumplimiento de los servicios de los operadores |
| **Autor**             | Guillermo Morales Caparrós |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | El administrador podrá comprobar si los servicios de los operadores se cumplen correctamente. |
| **Actores**           | Administrador |
| **Precondiciones**    | El administrador debe estar identificado |
| **Flujo Normal**      | 1. Se muestran los servicios de los Operadores para su comprobación y correcto funcionamiento |
| **Flujo alternativo** | Ninguno |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-33 |

| **ID** | CU-37 |
|--|--|
| **Nombre**            | Modificar diseño de la Web |
| **Autor**             | Daniel Pérez Escarcena |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | El administrador modifica el diseño de la Web |
| **Actores**           | Administrador |
| **Precondiciones**    | El administrador debe estar identificado |
| **Flujo Normal**      | 1. El administrador accede a la configuración  de la página Web <br> 2. El administrador hace clic en la opción de modificar el diseño. <br> 3. El administrador carga la plantilla con la que se va a sustituir el diseño actual de la página Web. |
| **Flujo alternativo** | 3b. El sistema muestra un mensaje de error “este diseño no es compatible con la página” |
| **Post Condiciones**  | La página Web se ha cambiado correctamente con la plantilla seleccionada |
| **Referencias**       | Ninguna |

| **ID** | CU-38 |
|--|--|
| **Nombre**            | Ver la cartografía de la actividad de los operadores |
| **Autor**             | Daniel Pérez Escarcena |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | El administrador puede ver la actividad que han realizado los operadores dentro de la página Web |
| **Actores**           | Administrador |
| **Precondiciones**    | El usuario administrador está previamente logueado |
| **Flujo Normal**      | 1. El administrador accede a la actividad dentro de la página Web <br> 2. El administrador va a la opción de operadores <br> 3. El administrador ve la gráfica con la actividad realizada por los operadores <br> 4. El administrador ve los informes con las situaciones que ameritan ese informe |
| **Flujo alternativo** | 3b. Los operadores no realizaron actividad ese día por lo que la gráfica no aparece |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | Ninguna |

| **ID** | CU-39 |
|--|--|
| **Nombre**            | Registrar situaciones puntuales |
| **Autor**             | Daniel Pérez Escarcena |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | Registra situaciones que ocurren raramente dentro de la página Web |
| **Actores**           | Administrador |
| **Precondiciones**    | El usuario administrador está previamente logueado |
| **Flujo Normal**      | 1. El administrador accede a la actividad dentro de la página Web <br> 2. El administrador accede a la opción de las situaciones <br> 3. El administrador ve los informes con las situaciones que ameritan ese informe |
| **Flujo alternativo** | 3.b En caso de no haber situaciones, el sistema le muestra un mensaje “Sin incidencias” |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-38 |

| **ID** | CU-40 |
|--|--|
| **Nombre**            | Registrar periodos continuos de tiempo |
| **Autor**             | Daniel Pérez Escarcena |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | El administrador puede ver la actividad que han realizado los operadores durante un periodo de tiempo |
| **Actores**           | Administrador |
| **Precondiciones**    | El usuario administrador está previamente logueado como administrador |
| **Flujo Normal**      | 1. El administrador accede a la actividad dentro de la página Web <br> 2. El administrador va a la opción de operadores <br> 3. El administrador selecciona un rango de días para ver la gráfica con la actividad realizada por los operadores |
| **Flujo alternativo** | 3b. Los operadores no realizaron actividad en el plazo seleccionado por lo que la gráfica no aparece |
| **Post Condiciones**  | Ninguna |
| **Referencias**       | CU-38 |

| **ID** | CU-41 |
|--|--|
| **Nombre**            | Enviar factura de compra |
| **Autor**             | Daniel Pérez Escarcena |
| **Fecha**             | 15/12/2022 |
| **Descripción**       | El servicio de correo electrónico envía una factura con la información de la compra que acaba de realizar |
| **Actores**           | Servicio de correo electrónico |
| **Precondiciones**    | El usuario ha efectuado una compra |
| **Flujo Normal**      | 1. El correo electrónico visualiza la información del usuario <br> 2. El correo lee el correo electrónico del usuario <br> 3. El correo le envia la factura al correo del usuario |
| **Flujo alternativo** | 2b. El usuario no tiene puesto el correo electrónico por lo que la aplicación le pedirá que introduzca el correo <br> - 2b1.El correo vuelve a intentar enviar el mail |
| **Post Condiciones**  | El correo ha sido enviado |
| **Referencias**       | Ninguna |

## **3.3 Diagramas de clases asociados a los requisitos de información**

![Diagrama de clases asociados a los requisitos de información]()