Ortega Salas Sandra, Martínez Infante Leslei Nevil
Ensayo de un Modelo Vista Controlador
Instituto Tecnológico de Tláhuac
Ingeniería en Sistemas Computacionales
Grupo: 8S2 Programación Web PHP con MVC
21-marzo, 2024



1.1 INDICE.

1.1 INDICE.	1
1.2 RESUMEN	2
1.3 INTRODUCCIÓN	2
1.3.1 DEFINICIÓN DE MODELO.	2
1.3.2 DEFINICIÓN DE VISTA.	3
1.3.3 DEFINICIÓN DE CONTROLADOR.	3
1.3.4 DEFINICIÓN DE PHP.	3
1.4 DESARROLLO	3
1.5 CONCLUSIONES	11
1.6 REFERENCIAS	11












1.2 RESUMEN

Dentro del proyecto, observaremos su elaboración por medio del Modelo-Vista-Controlador, en donde podemos visualizar como se va desarrollando, de tal manera que sea integrado dentro del mismo. Tomando en cuenta el código hecho en PHP, así mismo utilizando código HTML y el apoyo en diagramas, se va teniendo un margen del programa para que sea comprensible. 
En el desarrollo se debe tener una secuencia en los códigos y tener una congruencia de cómo se irá organizando en cada una de las carpetas que se van asignando conforme va funcionando cada parte de la estructura. 
Uno de los objetivos principales de este proyecto es conocer más sobre la estructura que se está tomando como referencia, especificar de manera clara el contexto que se va realizando cada una de las partes del código, generando así el Modelo-Vista-Controlador.
1.3 INTRODUCCIÓN 

El propósito del proyecto es encontrar una manera diferente para la venta de cosméticos, donde desarrollamos una aplicación web teniendo como base la estructura de Modelo-Vista-Controlador, esto con la finalidad de tener un control sobre el código, que, si a recomendaciones futuras se requiere realizar una modificación o insertar nuevas acciones, esto nos ayudará a realizarlo de manera entendible. 
	La importancia de este documento, está vinculado con el desarrollo de la aplicación web con la intención de darle formato en la estructura ya mencionada, siendo así que el presente escrito, denominado “Supershop cosmetic”, te será de ayuda para la realización de código dentro de un sistema Modelo-Vista-Controlador.
1.3.1 DEFINICIÓN DE MODELO.
El modelo es responsable de la lógica de datos de la aplicación, es independiente de la interfaz de usuario. Gestiona directamente los datos, garantiza su integridad y accesibilidad, la lógica y las reglas de aplicación. Si el estado de estos datos, el modelo generalmente debe notificar a la vista para que así pueda ser cambiado.
1.3.2 DEFINICIÓN DE VISTA.
La vista define como se deberán mostrar los datos de la aplicación, donde se proporciona la interfaz de usuario necesaria para interactuar con la aplicación. Dentro de esta, puede haber menús o botones, no maneja la entrada de usuario. Se comunica con el controlador, donde recibirá los datos para mostrar el modelo.
1.3.3 DEFINICIÓN DE CONTROLADOR.
El controlador contiene la lógica que actualiza el modelo y/o la vista en respuesta a las entradas de los usuarios de la aplicación, facilita las comunicaciones entre la aplicación actuando como la interfaz entre las capas, acepta entradas y las convierte en comandos para el modelo o vista.
1.3.4 DEFINICIÓN DE PHP.
Es un lenguaje de programación de código abierto, esto quiere decir que puede ser modificado por desarrolladores y se apta a diversos proyectos, se utiliza sobre todo en el entorno de desarrollo web, principalmente para el desarrollo de backend de una web, en el lado del servidor; sin embargo, tiene numerosas utilidades en el frontend, está diseñado para incrustarse en HTML. Una de las particularidades de PHP es que el código donde se integre se ejecutará del lado del servidor y sólo después se enviará al cliente.
1.4 DESARROLLO

Dentro del proyecto, podemos apreciar como principal diagrama, cada una de las partes que se van a presentar dentro de la estructura del programa:
 ![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/2d544884-b25a-4098-aaa7-e5c0cb586fb8)


Vista: es la parte de la estructura donde se muestra una interfaz que será para que el usuario pueda interactuar con la plataforma. 
En esta parte del proyecto realizamos una vista de manera que sea entendible para el usuario, donde utilizamos botones, áreas de texto, validación de datos. 
Como se muestra en el siguiente código, podemos visualizar como se realizó la interfaz de usuario donde tenemos un input de tipo texto, otro input de tipo password, dentro de este mismo código, observamos que se manda a llamar al controlador, y se utilizan diseños de CSS. 
![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/15f2d9cf-d21d-4eee-a4a8-24432cd3a613)

 
Como se a mencionado utilizamos diseños CSS que funcionan como:
.contenedor: que en su totalidad es el contorno donde se encuentra el login para ingresar a la aplicación web, teniendo una forma especial que se a integrado a este mismo. 
.contenedor form: que es la forma en que será presentado el login, en este caso se da el tamaño en pixeles.
.contenedor form input: el formato que llevará de igual manera el contenedor, en este caso se agrega que sea Cursiva y de igual manera se le da el tamaño en pixeles.
![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/0b5f407f-4d2a-4284-bda7-b99235809b16)

 
Después de generar la parte del código “Login” tenemos el siguiente diseño, que se puede visualizar de manera simple y entendible.
 
![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/2a39fa84-ec53-463f-9ea7-987cb5553578)





En el código siguiente podemos observar la realización del menú, donde tenemos la presentación de la aplicación web y por quienes a sido elaborada, teniendo en cuenta también el titulo de la página que ha sido denominado “supershop cosmetic”
 ![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/3e220349-81f6-403f-8b1e-1d76f5909831)

De está manera podemos encontrar nuestra vista de esta manera, agregando al código una serie de menú para entrar a las demás vistas. 

 ![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/c18b9134-d647-420d-b78b-fe6aaa41669a)

Modelo: donde se va a almacenar la llamada a la base de datos, permitiendo que se encuentre de igual manera los códigos relacionados a la base de datos. 
Para realizar la base de datos, debemos realizar un diagrama de bases de datos, el cuál va guiando al programador para realizar la base de datos. 
En este caso podemos visualizar las tablas de Usuario, la cual será utilizada para el login, Carrito está es utilizada para las compras que irá realizando el usuario. Prendas, en esta tabla se guardan los datos de cada uno de los productos que serán visualizados por el usuario, las Ventas las cuales también se van almacenando en nuestra base de datos, teniendo una segunda tabla, que recolecta el Detalle de venta donde se mantiene que es lo que compró el usuario.

 ![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/9ab7186a-70b1-4cf2-9133-47cea5bae822)

Dentro del siguiente lapso de código podemos apreciar como se manda a llamar la base de datos, donde se da la evaluación si el usuario y la contraseña son verdaderas y así mismo dejar ingresar al usuario a la siguiente parte de la vista. 
![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/85d5bef9-21f0-4ac4-96ff-9b6c3b7807be)

 
Aquí podemos observar la creación de la base de datos, la cual también es perteneciente al modelo.

 ![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/ef9024f9-2d6b-4265-9d04-fc1bb4a483d6)


Controlador: prácticamente este realiza la comunicación entre la base de datos y la vista, para que así el usuario pueda interactuar con la base de datos por medio de la vista que se le imparte.
En el controlador, como bien se ha mencionado tenemos que es la que interactúa entre la base de datos y la vista que será mostrada al usuario. Se da a conocer las siguientes líneas de código, donde se realiza la conexión de la base de datos.
$host = en esta parte de código, se agregará el host donde se encuentra la base de datos “localhost”.
$user = se ingresa el nombre del usuario de donde se extraerá en el caso de este código, es llamado “root”
$clave = en la clave, como su nombre lo indica se ingresa la contraseña del usuario, a veces este es denominado “$password” y en este caso podemos visualizar que se encuentran solas las comillas, esto es porque no se tiene contraseña en el usuario “”.
$bd = aquí tendrá que agregar el nombre de la base de datos en este código se tiene como “Leslei”.
$conexion = lo que realiza esta línea de código es que con los datos ya proporcionados se extrae la base de datos.
![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/115e5706-0abf-4237-8335-5773e2abe420)

 
Se puede mostrar en el siguiente código, como se manda a llamar cada una de las partes de inserción para los productos, y se comunica con modelProduct.php, con la línea de código: 
require_once "../model/modelProduct.php";
La cual después se llama a la Vista, y se esta manera sea visualizada, de la manera en que se pueda visualizar cada uno de los productos. Con esta línea de código pueden llamarse las distintas clases de cualquier carpeta, para que así nuestro Modelo-Vista-Controlador sea de manera más eficiente.
![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/2e230827-49b1-491c-a210-d1748b02fbe3)

 
Aquí se puede mostrar como con esta línea de código se puede integrar en la siguiente vista la base de datos para así poder agregar productos, ser eliminados e incluso agregar imágenes. 
 ![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/51139e53-5057-4b96-aa95-8ba0c613f7a2)

De esta manera, se va integrando nuestra carpeta CONTROLADOR, donde podemos encontrar login, delete, exit, mail, productos.
  
![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/012ea0dc-00f3-4fa4-acf7-80de5b708b52)
![image](https://github.com/LESLIEREPOSITORIO/Tiendaenlinea/assets/168056973/8f9462bf-2445-493d-a8aa-b8c07f9ff6c7)

 
1.5 CONCLUSIONES

En conclusión, el Modelo-Vista-Controlador es una estructura que se fundamenta en la elaboración de proyectos, y en este, podemos encontrar una organización de nuestros códigos de manera que sea entendible para futuras modificaciones, así como la generación de obtener una arquitectura más limpia, siendo el código más escalable y fácil de entender.
Generalmente esta estructura nos ayuda a clasificar la información, la lógica del sistema y la interfaz que se le es presentada al usuario, y dándole mayor capacidad al programador de poder modificar alguno de los componentes que se encuentran dentro de los códigos sin la necesidad de afectar los demás componentes.

1.6 REFERENCIAS

MVC - MDN Web Docs Glossary: Definitions of Web-related terms | MDN. (2023, 20 diciembre). MDN Web Docs. https://developer.mozilla.org/en-US/docs/Glossary/MVC
Wikipedia contributors. (2024b, marzo 16). Model–View–Controller. Wikipedia. https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller
Sheldon, R. (2023, 12 septiembre). model-view-controller (MVC). WhatIs. https://www.techtarget.com/whatis/definition/model-view-controller-MVC

