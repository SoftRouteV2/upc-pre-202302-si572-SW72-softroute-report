## **CAPÍTULO IV: SOLUTION SOFTWARE DESIGN ![Cuadro de texto](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.001.png)**






 ## **4.1**  **Strategic-Level Domain-Driven Design**
### **4.1.1** EventStorming
Para esta sección del proyecto se utilizó la técnica EventStorming para poder tener un mejor enfoque de los sistemas y procesos del negocio, con el fin de identificar eventos claves, modelar los procesos y establecer límites.

Enlace de mural: <https://app.mural.co/t/psyhelp9597/m/psyhelp9597/1693064503169/e9affcbf36c9b57c3f01d44b04523ec23ec7ecd3?sender=uf19e2134468e05a2ff112512>

**Step 1: Unstructured exploration**

![Imagen de la pantalla de un celular con letras
Descripción generada automáticamente con confianza media](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.002.png)

**Step 2: Timelines**

![Diagrama, Esquemático
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.003.png)

**Step 3: Pain points**

![Diagrama, Dibujo de ingeniería
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.004.png)


**Step 4: Pivotal points**

![Diagrama, Esquemático
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.005.png)


**Step 5: Commands

![Tabla
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.006.png)**

**Step 6: Policies**

![Imagen que contiene Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.007.png)

**Step 7 : Read models**

![Tabla
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.008.png)

**Step 8 : External system**

![Interfaz de usuario gráfica, Texto, Aplicación
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.009.png)

**Step 9 : Aggregates**

![Tabla
Descripción generada automáticamente con confianza media](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.010.png)

**Step 10 : Bounded Context**

![Interfaz de usuario gráfica, Aplicación, PowerPoint
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.011.png)

#### Candidate Context Discovery
![Interfaz de usuario gráfica, Aplicación, PowerPoint
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.012.png)
#### Domain Message Flows Modeling

![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.013.png)
#### Bounded Context Canvases
![Interfaz de usuario gráfica
Descripción generada automáticamente con confianza media](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.014.png)

![Interfaz de usuario gráfica
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.015.png)

![Interfaz de usuario gráfica
Descripción generada automáticamente con confianza media](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.016.png)

![Tabla
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.017.png)
### **4.1.2** Context Mapping
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.018.png)

### **4.1.3** Software Architecture
A continuación, se explicará sobre el modelo c4 de nuestra aplicación.
#### **4.1.3.1** Software Architecture System Landscape Diagram
El diagrama permite representar visualmente los sistemas y componentes que componen el sistema de software SoftRoute, lo que facilita la comprensión de la estructura general del sistema.

![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.019.png)

#### **4.1.3.2**  Software Architecture Context Level Diagramas
Permite comprender y comunicar cómo un sistema de software se relaciona con su entorno, sus interfaces con otros sistemas y los elementos clave que lo rodean.

![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.020.png)
#### **4.1.3.3**  Software Architecture Container Level Diagrams
Permite comprender y comunicar cómo un sistema de software se relaciona con su entorno, sus interfaces con otros sistemas y los elementos clave que lo rodean.

![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.021.png)
#### **4.1.3.4**  Software Architecture Deployment Diagrams
Muestra cómo los diferentes componentes de software, como aplicaciones, servidores, bases de datos y otros, se implementan en hardware físico, máquinas virtuales o entornos de ejecución.

![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.022.png)

## **4.2**  Tactical-Level Domain-Driven Design
### **4.2.1** Bounded Context: User
Dentro de este bounded context denominado USER, los usuarios tienen la capacidad de realizar registros y autenticarse en la aplicación, lo que les permite aprovechar plenamente todos los servicios proporcionados por SoftRute.
#### **4.2.1.1** Domain Layer
**Entities:** Para el contexto de User consideramos las siguientes entidades.

- **Company:** Esta entidad representa a las compañías o empresas que utilizan la aplicación. Cada instancia de la entidad "Company" tiene atributos como nombre de la compañía, RUC, información de contacto y otros datos. Las compañías pueden registrarse en la aplicación para acceder a los servicios ofrecidos por SoftRute.
- **Employee**: Esta entidad representa a los empleados de las compañías registradas en la aplicación. Cada instancia de esta entidad puede tener atributos como DNI y password. Los empleados pueden utilizar sus credenciales para autenticarse y acceder a las funcionalidades específicas proporcionadas por SoftRute.

**Methods**

- **addEmployee():** Este método permite agregar un nuevo empleado a la entidad Company. Al llamar a este método, se crea una instancia de Employee con los datos proporcionados (id, dni y contraseña), y se vincula al registro de la compañía. De esta manera, se puede llevar un registro completo de los empleados de la compañía en la aplicación.
- **deleteEmployee():** Con este método, es posible eliminar a un empleado existente de la entidad Company. Al proporcionar el identificador (id) del empleado a eliminar, se realiza la eliminación de manera efectiva, lo que garantiza una gestión actualizada de la lista de empleados en la compañía.
- **updateEmployee():** El método updateEmployee() permite actualizar los datos de un empleado específico de la entidad Company. Se pueden modificar aspectos como el DNI (documento de identidad) y la contraseña del empleado. Esta función es útil para mantener la información de los empleados actualizada sin necesidad de eliminar y volver a agregar.

**Value Objects:**

- **Phone**: Atributo que guarda el número de contacto de la compañía.
- **RUC:** Atributo que almacena el ruc de la compañía.

**Factories:**

- **EmployeeFactory:** Es el encargado de crear más empleados para una entidad de tipo Company.
#### **4.2.1.2** Interface Layer
**CompanyController:** Controlador que provee los REST API para la gestión del company.

**EmployeeController:** Controlador que provee los REST API para la gestión del Employee.
#### **4.2.1.3** Application Layer
**CompanyService:** Esta capa es el motor de la lógica de negocio relacionada con las compañías. Se encarga de administrar y orquestar operaciones que involucran a las compañías, como crear nuevas compañías o gestionar las existentes. Este servicio garantiza que todas las interacciones con las compañías sigan las reglas de negocio definidas.

**EmployeeService:** EmployeeService se enfoca en la lógica relacionada con los empleados dentro de nuestra aplicación. Es responsable de tareas como agregar, eliminar o actualizar empleados, gestionando así la información de manera precisa y segura. Este servicio asegura que las operaciones con empleados se realicen de manera coherente.
#### **4.2.1.4** Infrastructure Layer
**CompanyRepository:** La capa de infraestructura cuenta con CompanyRepository, que actúa como el puente entre nuestra aplicación y la base de datos. Este repositorio se encarga de almacenar y recuperar información de compañías de manera eficiente y confiable.

**EmployeeRepository:** Similar a CompanyRepository, EmployeeRepository se ocupa de la persistencia de datos relacionados con empleados. Permite que nuestra aplicación acceda, almacene y actualice información de empleados de manera eficaz, garantizando la integridad y disponibilidad de los datos.
#### **4.2.1.5** Bounded Context Software Architecture Component Level Diagrams
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.023.png)
#### **4.2.1.6** Bounded Context Software Architecture Code Level Diagrams.
##### Bounded Context Domain Layer Class Diagrams
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.024.png)

##### Bounded Context Database Design Diagram
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.025.png)


### **4.2.2**  Bounded Context: Shipment
Este "bounded context" se centra en la gestión integral de los envíos. Su objetivo principal es supervisar y coordinar todo el proceso de envío desde la recopilación de información sobre el paquete, su ruta planificada, la asignación de transportistas, hasta la entrega final al destinatario. Algunas funciones clave incluyen la gestión de datos de envío, coordinación logística y resolución de problemas relacionados con el transporte de paquetes.
#### **4.2.2.1** Domain Layer
**Entities:**

**Shipment:** Esta entidad representa un envío con atributos como identificación, descripción, cantidad, costo de envío, peso y fechas importantes como la de entrega, llegada y recepción, junto con un código de referencia.

**Sender:** La entidad Sender representa la información del remitente, con atributos como id, nombre completo y número de identificación (DNI).

**Receiver:** La entidad Receiver contiene detalles sobre el destinatario, incluyendo id, nombre completo y número de identificación (DNI).

**Methods:**

En esta capa de dominio, los métodos incluyen la gestión de envíos, como la actualización de datos de envío, el registro de llegada y entrega, así como la gestión de remitentes y destinatarios.

**Value Objects:**

Los objetos de valor en esta capa pueden ser utilizados para representar conceptos inmutables relacionados con los envíos, como fechas o valores calculados a partir de los atributos del envío.
#### **4.2.2.2** Interface Layer
**ShipmentController:** Este controlador se encarga de gestionar las solicitudes relacionadas con los envíos desde la interfaz de usuario o sistemas externos. Incluye operaciones como crear nuevos envíos, consultar el estado de los paquetes o actualizar la información de un envío.
#### **4.2.2.3** Application Layer
**ShipmentService:** El ShipmentService es fundamental para gestionar la lógica de negocio relacionada con los envíos. Incluye operaciones como registrar la llegada de un paquete, actualizar detalles de envío o calcular costos de envío en función de la distancia y el peso.

**SenderService:** Este servicio se encarga de administrar la información de los remitentes, permitiendo la creación y actualización de registros de remitentes.

**ReceiverService:** El ReceiverService gestiona la información de los destinatarios, permitiendo operaciones como el registro y actualización de detalles de destinatarios.
#### **4.2.2.3** Infrastructure Layer
**ShipmentRepository:** El ShipmentRepository es esencial para interactuar con la base de datos o sistema de almacenamiento de envíos. Se utiliza para almacenar, recuperar y actualizar información sobre envíos.

**SenderRepository:** Este repositorio se encarga de la persistencia de datos relacionados con los remitentes, permitiendo el almacenamiento y recuperación de información sobre los remitentes registrados.

**ReceiverRepository:** El ReceiverRepository tiene la misma función que el SenderRepository pero para la entidad de destinatarios, permitiendo el almacenamiento y recuperación de información sobre los destinatarios registrados.
#### **4.2.2.4** Bounded Context Software Architecture Component Level Diagrams
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.026.png)
#### **4.2.2.5** Bounded Context Software Architecture Code Level Diagrams.
##### Bounded Context Domain Layer Class Diagrams
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.027.png)

##### Bounded Context Database Design Diagram
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.028.png)

### **4.2.3** Bounded Context: Package Tracking
Este bounded context proporciona a los usuarios la capacidad de rastrear y monitorear sus paquetes en todo momento. Su objetivo principal es brindar visibilidad y transparencia en cuanto al estado y la ubicación de los paquetes. Algunas funciones clave incluyen la generación de números de seguimiento, notificaciones de estado, actualizaciones de ubicación en tiempo real y consultas de historial de seguimiento.
#### **4.2.3.1** Domain Layer
**Entities:**

**Tracking:** Esta entidad representa una instancia de seguimiento de paquetes y contiene atributos como un identificador único (id), latitud y longitud para proporcionar información sobre la ubicación actual del paquete.

**Destination:** La entidad Destination contiene información relacionada con el destino del paquete, incluyendo un identificador único (id), lugar de partida y lugar de llegada.

**Methods:**

En esta capa de dominio, los métodos incluyen operaciones relacionadas con el seguimiento de paquetes, como actualizar la ubicación, generar números de seguimiento y registrar información de destino.
#### **4.2.3.2** Interface Layer
**TrackingController:** Este controlador se encarga de gestionar las solicitudes relacionadas con el seguimiento de paquetes desde la interfaz de usuario o sistemas externos. Incluye operaciones para rastrear paquetes, recibir actualizaciones de estado y consultar historiales de seguimiento.
#### **4.2.3.3** Application Layer
**TrackingService:** El TrackingService es fundamental para gestionar la lógica de negocio relacionada con el seguimiento de paquetes. Incluye operaciones para actualizar la ubicación en tiempo real, generar números de seguimiento y notificar a los usuarios sobre el estado de sus paquetes.

**DestinationService:** Este servicio se encarga de gestionar la información de destino, permitiendo la creación y actualización de registros de destinos de paquetes.
#### **4.2.3.4** Infrastructure Layer
**TrackingRepository:** El TrackingRepository es esencial para interactuar con la base de datos o sistema de almacenamiento de información de seguimiento de paquetes. Se utiliza para almacenar, recuperar y actualizar la información de seguimiento de paquetes.

**DestinationRepository:** Este repositorio se encarga de la persistencia de datos relacionados con los destinos de paquetes, permitiendo el almacenamiento y recuperación de información sobre los destinos registrados.
#### **4.2.3.5** Bounded Context Software Architecture Component Level Diagrams
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.029.png)
#### **4.2.3.6** Bounded Context Software Architecture Code Level Diagrams.
##### Bounded Context Domain Layer Class Diagrams
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.030.png)

##### Bounded Context Database Design Diagram
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.031.png)

### **4.2.4** Bounded Context: Feedback
Este bounded context se enfoca en la recopilación y gestión de comentarios y opiniones de los usuarios sobre el servicio de envío y entrega. Su objetivo principal es recopilar y utilizar la retroalimentación para mejorar la calidad del servicio. Algunas funciones clave incluyen la recopilación de comentarios de los clientes y la gestión de quejas.
#### **4.2.4.1** Domain Layer
**Entities**

**Feedback:** Esta entidad representa la retroalimentación proporcionada por los clientes e incluye atributos como identificación única (id), fecha de retroalimentación, puntaje otorgado, descripción de los comentarios y una referencia a un envío relacionado (ShipmentId).

**Methods**

En esta capa de dominio, los métodos incluyen operaciones relacionadas con la gestión de la retroalimentación, como registrar nuevos comentarios, calcular puntuaciones promedio o asociar comentarios con envíos específicos.
#### **4.2.4.2** Interface Layer
**FeedbackController:** Este controlador es esencial para gestionar las solicitudes relacionadas con la retroalimentación de los clientes. Su responsabilidad incluye recibir y registrar comentarios de los clientes, así como manejar las quejas.
#### **4.2.4.3** Application Layer
**FeedbackService:** El FeedbackService desempeña un papel fundamental en la gestión de la retroalimentación. Sus funciones abarcan el registro y procesamiento de comentarios, el cálculo de puntuaciones promedio y la identificación de áreas de mejora basadas en la retroalimentación de los clientes.
#### **4.2.4.4** Infrastructure Layer
**FeedbackRepository:** El FeedbackRepository es esencial para interactuar con la base de datos o sistema de almacenamiento de comentarios y opiniones de los clientes. Se utiliza para almacenar, recuperar y actualizar la retroalimentación registrada.

**ShipmentRepository:** Este repositorio se encarga de la persistencia de datos relacionados con los envíos, ya que la retroalimentación puede estar vinculada a envíos específicos. Permite el almacenamiento y recuperación de información detallada sobre los envíos registrados.
#### **4.2.4.5** Bounded Context Software Architecture Component Level Diagrams
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.032.png)
#### **4.2.4.6** Bounded Context Software Architecture Code Level Diagrams.
##### Bounded Context Domain Layer Class Diagrams
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.033.png)

##### Bounded Context Database Design Diagram
![Diagrama
Descripción generada automáticamente](Resources/cap4/Aspose.Words.d16339ca-b224-4956-8a03-cc3770195cfb.034.png)

