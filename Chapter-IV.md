# **CAPÍTULO IV: SOLUTION SOFTWARE DESIGN**
## 4.1. Strategic-Level Domain-Driven Design
### 4.1.1. EventStorming
![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.001.png)

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.002.png)

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.003.png)

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.004.png)

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.005.png)

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.006.png)

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.007.png)

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.008.png)

![](assets4/b9.png)

![](assets4/b10.png)

#### 4.1.1.1 Candidate Context Discovery
#### 4.1.1.2 Domain Message Flows Modeling
#### 4.1.1.3 Bounded Context Canvases

User:

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.009.png)

Inventory:

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.010.png)

Device:

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.011.png)

Notifications:

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.012.png)

Data Management:

![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.013.png)


### 4.1.2. Context Mapping
![](assets4/Aspose.Words.150ae8a6-bea6-4cd0-9a55-07688df6b288.014.png)
### 4.1.3. Software Architecture
#### 4.1.3.1. Software Architecture System Landscape Diagram
El diagrama de System Landscape muestra el ecosistema completo del sistema Thirsty Seed, incluyendo los actores externos y los sistemas con los que interactúa. Este diagrama ofrece una visión general de las relaciones clave entre los diferentes elementos de la plataforma.
![](assets4/structurizr-91625-SystemLandscape.png)

#### 4.1.3.2. Software Architecture Context Level Diagrams
Este diagrama contextualiza el sistema Thirsty Seed dentro de su entorno operativo, mostrando cómo interactúa con los actores principales, como el Productor Agrícola, el Proveedor de Riego, y el Técnico IoT, además de destacar los contenedores involucrados.
![](assets4/structurizr-91625-SystemContext-001.png)

#### 4.1.3.3. Software Architecture Container Level Diagrams
El diagrama de contenedores detalla los subsistemas clave del sistema Thirsty Seed, como la API, el servidor embebido, la aplicación web y la aplicación móvil. Muestra cómo se conectan e interactúan entre sí y con las bases de datos, proporcionando una visión técnica de la arquitectura del sistema.
![](assets4/structurizr-91625-Containers.png)

#### 4.1.3.4. Software Architecture Deployment Diagrams
Este diagrama de despliegue muestra cómo los diferentes componentes y contenedores del sistema Thirsty Seed se implementan en entornos físicos y virtuales, como servidores de borde, dispositivos IoT y servidores en la nube. Ilustra la estructura de despliegue necesaria para su operación.
![](assets4/despliegue.png)

## 4.2. Tactical-Level Domain-Driven Design

### 4.2.1 Bounded Context: Inventory

<table><tr><th colspan="2" valign="top">Nombre</th><th colspan="2" valign="top">Inventory </th><th valign="top"></th></tr>
<tr><td colspan="2" valign="top">Descripción</td><td colspan="2" valign="top">Representa la compra de productos</td><td valign="top"></td></tr>
<tr><td colspan="2" valign="top">Atributos</td><td colspan="2" valign="top">Relaciones</td><td rowspan="1" valign="top">Métodos   </td></tr>
<tr><td valign="top">Nombre </td><td valign="top">Tipo de Dato</td><td valign="top">Tipo</td><td valign="top">Clases/Enums</td></tr>
<tr><td valign="top">devicePurchaseId   </td><td valign="top">DevicePurchaseId</td><td valign="top">Composición</td><td valign="top">DevicePurchaseId   </td><td valign="top">purchase()  </td></tr>
<tr><td valign="top">userId   </td><td valign="top"><p>	   </p><p>UserId   </p><p></p></td><td valign="top">Composición</td><td valign="top">UserId</td><td valign="top">cancelPurchase ()  </td></tr>
<tr><td valign="top">title   </td><td valign="top">string   </td><td valign="top">Composición</td><td valign="top">Catalog   </td><td valign="top">track()   </td></tr>
<tr><td valign="top">description  </td><td valign="top">string</td><td valign="top">Composición</td><td valign="top">History </td><td valign="top"></td></tr>
<tr><td valign="top">date   </td><td valign="top">date</td><td valign="top"></td><td valign="top"></td><td valign="top"></td></tr>
<tr><td valign="top">catalog   </td><td valign="top">catalog</td><td valign="top"></td><td valign="top"></td><td valign="top"></td></tr>
<tr><td valign="top">history   </td><td valign="top">history</td><td valign="top"></td><td valign="top"></td><td valign="top"></td></tr>
</table>

|Nombre|Catalog|||
| :- | :- | :- | :- |
|Descripción|Representar el catálogo de productos|||
|Atributos|Relaciones|||
|` `Nombre|Tipo de Dato|||
|product|Product|Composición|Product|

|Nombre|Product|
| :- | :- |
|Descripción|Representar un producto|
|Atributos||
|Nombre|Tipo de Dato|
|description|String|

|Nombre|History|
| :- | :- |
|Descripción|Representar el historial de compras|
|Valores||
|LessThanTwoPurchase   ||
|MoreThanTwoPurchase   ||

|Nombre|UserId|
| :- | :- |
|Descripción|Representa el identificador del usuario  |
|Atributos||
|Nombre|Tipo de Dato|
|userId   |long   |




|Nombre|DevicePurchaseId |
| :- | :- |
|Descripción|Representar el identificador   de la compra |
|Atributos||
|Nombre|Tipo de Dato|
|devicePurchaseId   |long   |

#### 4.2.1.1. Domain Layer
Se identificó que la única clase central en el negocio es la clase **Device Purchase**, la cual representa la compra de productos como sensores o válvulas. Según las reglas de negocio, el productor agrícola tiene la posibilidad de solicitar una o más sensores o válvulas, según sea necesario para su situación particular.

**Entities**:

- **DevicePurchase (Aggregate)**: Representa la compra de una válvula o sensor.

**ValueObjects**:

- **UserId (Aggregate)**: Representa el identificador único del usuario.
- **DevicePurchaseId (Aggregate)**: Representa el identificador único de la compra.
- **Product**: Representa un sensor o una válvula.
- **Catalog (Aggregate)**: Representa el catálogo disponible.

**Enums**:

- **History (Aggregate)**: Representa el historial de compras.

**Factories**:

- **DevicePurchaseFactory**: Facilita la creación de órdenes de compra.

**Interfaces**:

- **IDevicePurchaseRepository:** Interfaz para la clase **DevicePurchaseRepository**, que ayuda a mantener un bajo nivel de acoplamiento.

|Nombre   |IDevicePurchaseRepository   |
| :- | :- |
|Descripción   |Permite la conexión con la base de datos  |
|Métodos||
|findAll()   ||
|findById()||
|findByUserId()||
|create()   ||
|update()  ||
|delete()   ||

- IDevicePurchaseServices: Interfaz de la clase DevicePurchaseService, ayuda a mantener un bajo acoplamiento

|Nombre   |IDevicePurchaseService|
| :- | :- |
|Descripción   |Declara las funciones que contiene las reglas de   negocio|
|Métodos||
|getAll()   ||
|getById() ||
|getByUserId() ||
|create()   ||
|delete()   ||
|purchase()   ||
|cancelPurchase ()   ||
|track()   ||

#### 4.2.1.2. Interface Layer
**Controllers** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|DataController |Maneja las solicitudes relacionadas con datos y reportes. |getDataRecords(request: DataRequest): Response, generateReport(request: ReportRequest): Response |

**Consumers** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|DataEventConsumer |Escucha y procesa eventos relacionados con datos. |consumeDataEvent(event: DataEvent): void |

![Shape]** 
#### 4.2.1.3. Application Layer
**Command Handlers** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|GenerateReportHandler |Maneja el comando para generar un reporte de análisis de datos. |handle(command: GenerateReportCommand): void |
|SaveDataRecordHandler |Maneja el comando para guardar un nuevo registro de datos. |handle(command: SaveDataRecordCommand): void |

**Event Handlers** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|DataRecordSavedEventHandler |Maneja eventos relacionados con la creación de registros de datos. |handle(event: DataRecordSavedEvent): void |

![Shape]** 

#### 4.2.1.4. Infrastructure Layer
**Repositories Implementations** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|DataRecordRepositoryImpl |Implementación concreta de DataRecordRepository para acceder a datos persistidos. |findByDateRange(dateRange: DateRange): List<DataRecord>, save(record: DataRecord): void, delete(recordId: String): void |
|AnalysisReportRepositoryImpl |Implementación concreta de AnalysisReportRepository para acceder a reportes persistidos. |findById(reportId: String): AnalysisReport, save(report: AnalysisReport): void |

**Messaging Systems** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|DataEventPublisher |Publica eventos relacionados con datos y reportes. |publish(event: DataEvent): void |

**External Services** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|ExternalAnalysisService |Servicio para interactuar con APIs externas para análisis avanzado. |performExternalAnalysis(data: List<DataRecord>): AnalysisReport, getExternalData(deviceId: String): List<DataRecord> |
**

#### 4.2.1.6. Bounded Context Software Architecture Component Level Diagrams
![](assets4/structurizr-91625-inventory_context_component_diagram.png)

#### 4.2.1.7. Bounded Context Software Architecture Code Level Diagrams
##### 4.2.1.7.1. Bounded Context Domain Layer Class Diagrams
Representa las clases y entidades que permiten la gestión de la asignación de dispositivos dentro del contexto de **Inventory**.

##### 4.2.1.7.2. Bounded Context Database Design Diagram
El diseño de la base de datos para este contexto gestiona las tablas necesarias para almacenar el estado del inventario y la información de los dispositivos asignados a los productores.

### 4.2.2. Bounded Context: Device Management
#### 4.2.2.1. Domain Layer
El dominio de **Device Management** se encarga de la configuración y monitoreo de los dispositivos IoT, incluyendo sensores y actuadores.

#### 4.2.2.2. Interface Layer
Expone interfaces API para configurar dispositivos IoT, recolectar datos de sensores y controlar los actuadores de riego.

#### 4.2.2.3. Application Layer
Incluye servicios como **Device Configuration Service** y **Actuator Control Service**, que manejan la lógica para configurar y controlar dispositivos.

#### 4.2.2.4. Infrastructure Layer
Utiliza un repositorio JPA para almacenar la configuración y estado de los dispositivos IoT.

#### 4.2.2.6. Bounded Context Software Architecture Component Level Diagrams
En el siguiente diagrama se desplieguen los componentes que implican este bounded en el API Application:
![](assets4/structurizr-91625-device_management_context_component_diagram.png)

Asimismo, se incluye el diagrama de componentes que comprende la configuración del Embedded Application:
![](assets4/structurizr-91625-embedded_application_component_diagram.png.png)

#### 4.2.2.7. Bounded Context Software Architecture Code Level Diagrams
##### 4.2.2.7.1. Bounded Context Domain Layer Class Diagrams
Representa las clases que manejan la configuración y el estado de los dispositivos IoT en el sistema.

##### 4.2.2.7.2. Bounded Context Database Design Diagram
El diagrama de diseño de la base de datos gestiona las tablas necesarias para la configuración y monitoreo de los dispositivos IoT.

---

### 4.2.3. Bounded Context: User Management
#### 4.2.3.1. Domain Layer
El contexto de **User Management** gestiona los usuarios, sus perfiles y roles dentro de la plataforma, proporcionando autenticación y autorización.

#### 4.2.3.2. Interface Layer
Existen interfaces API para manejar la autenticación de usuarios, la creación de perfiles y la asignación de roles.

#### 4.2.3.3. Application Layer
Incluye servicios como **User Service** y **Authentication Service**, responsables de la gestión de usuarios y la validación de autenticaciones.

#### 4.2.3.4. Infrastructure Layer
Los repositorios JPA permiten el almacenamiento de la información de los usuarios y sus perfiles.

#### 4.2.3.6. Bounded Context Software Architecture Component Level Diagrams
A continuación se presentan los diagrama de componentes que abarcan la gestión de usuarios, esto se gestiona en el API Application, aunque se reciben datos de los contenedores del web app y el mobile app.
![](assets4/structurizr-91625-user_context_component_diagram.png)

#### 4.2.3.7. Bounded Context Software Architecture Code Level Diagrams
##### 4.2.3.7.1. Bounded Context Domain Layer Class Diagrams
Representa las clases que gestionan los perfiles de usuarios, autenticación y autorización.

##### 4.2.3.7.2. Bounded Context Database Design Diagram
Este diseño gestiona las tablas que contienen los usuarios, sus roles y la información relacionada con su autenticación.

---

### 4.2.4. Bounded Context: Data Management
#### 4.2.4.1. Domain Layer
El dominio de **Data Management** se encarga de almacenar, analizar y reportar los datos recolectados de los dispositivos IoT.

#### 4.2.4.2. Interface Layer
Existen interfaces API que permiten acceder y gestionar los datos históricos de riego y humedad.

#### 4.2.4.3. Application Layer
Incluye servicios como **Data Analysis Service** y **Report Generation Handler** para analizar los datos y generar reportes.

#### 4.2.4.4. Infrastructure Layer
Los repositorios JPA permiten el almacenamiento y consulta de grandes volúmenes de datos históricos.

#### 4.2.4.6. Bounded Context Software Architecture Component Level Diagrams
Para el gestión de datos se han establecido los siguientes componentes, estos parten con el API Application:
![](assets4/structurizr-91625-data_management_context_component_diagram.png)

Una para la gestion de datos desde el edge server:
![](assets4/structurizr-91625-edge_server_component_diagram.png)

Por otro lado, para la presentación de estos datos se tiene lo siguiente de los componentes de la aplicación web:
![](assets4/structurizr-91625-web_application_component_diagram.png)

Y el siguiente para la aplicación movil:
![](assets4/structurizr-91625-mobile_application_component_diagram.png)


#### 4.2.4.7. Bounded Context Software Architecture Code Level Diagrams
##### 4.2.4.7.1. Bounded Context Domain Layer Class Diagrams
Representa las clases encargadas de almacenar, analizar y generar reportes basados en los datos de riego.

##### 4.2.4.7.2. Bounded Context Database Design Diagram
Este diseño de la base de datos gestiona las tablas de datos históricos de riego y análisis.

---

### 4.2.5. Bounded Context: Notification Management
#### 4.2.5.1. Domain Layer
El contexto de **Notification Management** maneja la generación y envío de notificaciones basadas en eventos de riego y datos analizados.

#### 4.2.5.2. Interface Layer
Proporciona una API para gestionar el envío de notificaciones a los usuarios a través de diferentes canales.

#### 4.2.5.3. Application Layer
Incluye servicios como **Notification Generation Handler** y **Notification Delivery Service** para generar y enviar notificaciones.

#### 4.2.5.4. Infrastructure Layer
Utiliza repositorios JPA para almacenar el historial de notificaciones.

**4.2.5. Bounded Context: Notification Management** 

**4.2.1.1. Domain Layer** 

**Entities** 

|**Class Name** |**Purpose** |**Attributes** |**Methods** |
| :- | :- | :- | :- |
|Notification |Representa una notificación que se envía a los usuarios. |notificationId: String, userId: String, message: String, status: String, timestamp: DateTime |markAsSent(): void, updateStatus(status: String): void |

**Value Objects** 

|**Class Name** |**Purpose** |**Attributes** |**Methods** |
| :- | :- | :- | :- |
|NotificationMessage |Define el contenido y formato de una notificación. |content: String, format: String |toString(): String |

**Aggregates** 

|**Class Name** |**Purpose** |**Root Entity** |**Methods** |
| :- | :- | :- | :- |
|NotificationAggregate |Agrega Notification y NotificationMessage para operaciones coherentes. |Notification |createNotification(userId: String, message: NotificationMessage): Notification, getNotification(notificationId: String): Notification |

**Domain Services** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|NotificationService |Proporciona lógica de negocio para la gestión y envío de notificaciones. |sendNotification(notification: Notification): void, getPendingNotifications(): List<Notification> |

**Repositories** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|NotificationRepository |Interfaz para acceder a notificaciones persistidas. |findById(notificationId: String): Notification, save(notification: Notification): void, delete(notificationId: String): void |

![Shape]** 

**4.2.5.2. Interface Layer** 

**Controllers** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|NotificationController |Maneja las solicitudes relacionadas con la creación y gestión de notificaciones. |createNotification(request: NotificationRequest): Response, getNotification(request: NotificationRequest): Response |

**Consumers** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|NotificationEventConsumer |Escucha y procesa eventos relacionados con el envío de notificaciones. |consumeNotificationEvent(event: NotificationEvent): void |
**


**4.2.5.3. Application Layer** 

**Command Handlers** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|CreateNotificationCommandHandler |Maneja el comando para crear una nueva notificación. |handle(command: CreateNotificationCommand): void |
|UpdateNotificationStatusHandler |Maneja el comando para actualizar el estado de una notificación. |handle(command: UpdateNotificationStatusCommand): void |

**Event Handlers** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|NotificationCreatedEventHandler |Maneja eventos relacionados con la creación de notificaciones. |handle(event: NotificationCreatedEvent): void |
**


**4.2.5.4. Infrastructure Layer** 

**Repositories Implementations** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|NotificationRepositoryImpl |Implementación concreta de NotificationRepository para acceder a notificaciones persistidas. |findById(notificationId: String): Notification, save(notification: Notification): void, delete(notificationId: String): void |

**Messaging Systems** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|NotificationEventPublisher |Publica eventos relacionados con la creación y envío de notificaciones. |publish(event: NotificationEvent): void |

**External Services** 

|**Class Name** |**Purpose** |**Methods** |
| :- | :- | :- |
|ExternalNotificationService |Servicio para interactuar con APIs externas para el envío de notificaciones. |sendNotificationToExternalService(notification: Notification): void, retrieveNotificationStatus(notificationId: String): String |
**

#### 4.2.5.6. Bounded Context Software Architecture Component Level Diagrams
![](assets4/structurizr-91625-notification_management_context_component_diagram.png)


#### 4.2.5.7. Bounded Context Software Architecture Code Level Diagrams
##### 4.2.5.7.1. Bounded Context Domain Layer Class Diagrams
Representa las clases que gestionan la lógica de generación y envío de notificaciones.

##### 4.2.5.7.2. Bounded Context Database Design Diagram
El diseño de la base de datos gestiona las tablas necesarias para almacenar el historial de notificaciones y los eventos que las generan.
