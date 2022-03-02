# LaunchX_Semana1
Practicas realizadas en la primera semana de FrontEnd



## Caso: Abogabot 

Descripción: 

- Es un despacho de abogados que quiere ***automatizar las demandas de sus clientes***, esto lo harán a traves de una ***página web llenando un formulario***.
- Al momento de llenar el formulario se manda al ***proceso de pago*** para finalizar la transacción.
- Para dar seguimiento a su demanda, el cliente ***crea una cuenta en la plataforma*** y verá el ***seguimiento*** de cada una de las actualizaciones ***del proceso legal***.
- El ***administrador*** del sitio ***recibe la notificación de una nueva demanda*** y ***con los datos llenados del formulario se crea automaticamente el documento  legal en formato word para empezar el proceso***.
- El administrador ***recibe el pago*** y debe de ser capaz de verlo en un ***dashboard*** para ver la ***cantidad de ingresos*** recibidos.
- El administrador ***actualiza el proceso de la demanda*** y ***agrega comentarios en cada paso del proceso***.
- Al usuario le llegan ***correos de notificación*** para saber el avance de su proceso.
- La página debe de ser ***responsive*** para poderla ver desde el celular.
- La preferncia de ***colores del cliente es azul marino y blanco***, pero acepta propuestas.




- **Practicas**
	- Toma de requerimientos
      - Crea tu buyer persona
	- Publico objetivo
	- Crea tu primer Wireframe UX
	- Ahora el UI




## Requerimientos:

### Restricciones de diseño

- RD.1. El sistema será un sitio Web.
- RD.2. El sistema contará con 2 tipos de usuarios: administrador y cliente
- RD.3. El sistema web será responsivo 
- RD.4 Para el diseño deben de tenerse en consideración los colores: blanco y azul marino



## Requisitos funcionales
Conjunto de requisitos que reflejan las funciones que debe prestar el sistema. Se clasifican en las siguientes subsecciones:

### Requisitos funcionales nominales


#### FN.1. Inicio de sesión.
**Descripción:** El sistema permitirá el inicio de sesión de sus dos diferentes tipos de usuarios (administrador y cliente) mostrando contenido distinto según sea el caso.     
**Medible:** Cuando el usuario inicie sesión se mostrará contenido específico de acuerdo a su tipo de perfil.           
**Alcanzable:** El sistema realizara una consulta de la información del usuario y la contraseña a la base de datos, si los datos son correctos: el sistema comparara el tipo de usuario y mostrara las funciones pertenecientes.        
**Relevante:** El sistema podrá restringir o permitir el acceso de funciones del sistema según sea el usuario.              



#### FN.2. Gestión de Clientes.
**Descripción:** En este módulo el administrador podrá, registrar, ver, modificar o eliminar clientes, por otra parte, los clientes solamente podrán darse de alta desde el formulario de registro.   
**Medible:** El sistema permitirá ingresar los datos de un cliente nuevo por medio de un formulario, una vez guardado se registrará en la base de datos y aparecerá en una traba con los demás usuarios registrados, el administrador podrá seleccionar un usuario para modificar sus datos o para eliminarlo
**Alcanzable:** A través de la interfaz gráfica, el administrador podrá ingresar a módulo de clientes en el cual el sistema realizará una consulta para mostrar en una tabla todos los clientes registrados en la base de datos, además de la tabla el sistema muestra los campos correspondientes a el cliente que se seleccione de la tabla para así poder modificar el registro, poder agregar uno nuevo o eliminar con sus botones correspondientes.   
**Relevante:** El sistema será capaz de gestionar clientes y sus datos.                     



#### FN.3.  Gestión de Casos de Clientes.
**Descripción:** En este módulo el administrador podrá, registrar, ver, agregar comentarios o eliminar casos de clientes, además podrá descargar un documento Word con la información específica de cada caso, por otra parte, los clientes podrán dar de alta sus casos desde el formulario de registro y podrán ver el estado de su caso, cuando un cliente registre un caso nuevo el sistema mandara un correo al administrador para que este enterado que tiene un caso nuevo en que trabajar y cuando abogabot realice algún avance a algún caso, el sistema enviara un correo al cliente para notificarle del avance del caso .   
**Medible:** El sistema permitirá ingresar los datos de un caso nuevo por medio de un formulario, una vez guardado se registrará en la base de datos y aparecerá en una traba con los demás casos registrados, el administrador podrá seleccionar un caso y podrá agregar comentarios a lo largo del proceso del caso. 
**Alcanzable:** A través de la interfaz gráfica, el administrador podrá ingresar a módulo de casos en el cual el sistema realizará una consulta para mostrar en una tabla todos los casos registrados en la base de datos, además de la tabla el sistema muestra las opciones de eliminar y descargar los datos del caso en un documento de Word. Por su parte el cliente solamente podrá agregar sus casos a través de un formulario y visualizar sus casos por medio de un dashboard.
**Relevante:** El sistema será capaz de gestionar casos.                     



#### FN.4.  Gestión Pagos de Clientes.
**Descripción:** En este módulo el cliente podrá pagar por el proceso que lleva cada uno de sus casos, el administrador podrá verificar a que caso corresponde cada uno de los pagos y podrá ver la suma total de todos los pagos  
**Medible:** después de registrar su caso a través de un formulario, el cliente será llevado a otro formulario donde se procesará su pago para que abogabot lleve su caso.
**Alcanzable:**  a través de un formulario se pedirán los datos de pago a través de posibles múltiples plataformas: PayPal, Tarjeta de Crédito o Tarjeta de Débito, para hacer la transacción y pagar por el servició de llevar el caso ante la justicia
**Relevante:** El sistema será capaz de gestionar pagos.



### Requisitos funcionales no nominales
Requisitos para el funcionamiento del sistema en situaciones especiales o condiciones de error. Se etiquetan como FF.x, siendo x el número de requisito.


#### FF.1.Validacion de campos vacíos.
**Descripción:** El sistema no permitirá que el usuario omita el registro de datos obligatorios.   
**Medible:** Al querer realizar un registro, el usuario debería de ingresar todos los datos obligatorios.         
**Alcanzable:** Por medio de la validación de campos vacíos,  el sistema no permitirá realizar el registro de datos cuando el usuario no ingreso los datos obligatorios.
**Relevante:** El sistema será capaz de evitar un error de inconsistencia de datos incompletos en los registros de la base de datos.                       



#### FF.2.Error de inicio de sesión. 
**Descripción:** En caso de que se ingrese un usuario o una contraseña incorrecta, el sistema mostrara un mensaje de error. 
**Medible:** Al momento de ingresar un usuario o una contraseña que no esté registrada en el sistema, se mostrara un mensaje de error para que se registre el usuario o se corrijan los datos.
**Alcanzable:** Al momento de tratar de ingresar al sistema, se consultaran los datos de los campos usuario y contraseña en los registros de la base de datos, en caso de que estos no coincidan o no existan, el sistema mostrara un mensaje de error.
**Relevante:** El sistema restringirá el acceso a usuarios no registrados.                       



### Requisitos de interfaz
Conjunto de requisitos que definen las necesidades de la interacción del sistema con otros sistemas y usuarios. Se etiquetan como IN.x siendo x el número de requisito.

#### IN.1.   Uniformidad
**Descripción:** El sistema usa la misma paleta de colores que se usan en todos los sistemas de la empresa de abogabot. 
**Medible:** El sistema deberá de usar los colores característicos de la empresa, si existe una carga excesiva de colores que no forman parte de la empresa, el requisito se tomara como insatisfecho.
**Alcanzable:** Se usará como norma las mismas tipografías, el mismo tipo de botones y la misma paleta de colores para el diseño del sistema.
**Relevante:** El sistema contara con las mismas normas de diseño a lo largo de todas las interfaces.                       


## ANALISIS DE REQUISITOS Y REQUERIMIENTOS 

Especifique un diagrama de negocio que permita entender con claridad que parte del negocio se incluye o se modifica con la solución del requerimiento.
Se sugiere para esta tarea utilice diagramas BPM, diagramas de actividades, o diagramas ad hoc (boceto).


### Diagrama de Inicio de sesión 

<img alt="center" src="https://github.com/JairFraga/LaunchX_Semana1/blob/main/Requerimientos/inicio_sesion.png" width="700vw" />



### Diagrama de Gestión de clientes 

<img alt="center" src="https://github.com/JairFraga/LaunchX_Semana1/blob/main/Requerimientos/gestion_clientes.png" width="700vw" />


### Diagrama de Gestión de casos de clientes

<img alt="center" src="https://github.com/JairFraga/LaunchX_Semana1/blob/main/Requerimientos/Gestion_casos.png" width="700vw" />

### Diagrama de Gestión de pagos

<img alt="center" src="https://github.com/JairFraga/LaunchX_Semana1/blob/main/Requerimientos/Gestion_pagos.png" width="700vw" />



## FASE DE PLANEACIÓN Y GERENCIA DEL PROYECTO

### Diagrama de Gantt

<img alt="center" src="https://github.com/JairFraga/LaunchX_Semana1/blob/main/Requerimientos/gantt.png" width="700vw" />



