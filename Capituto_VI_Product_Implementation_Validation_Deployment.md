## 6.1 Software Configuration Management
### 6.1.1.	Software Development Environment Configuration
En esta sección se describen cada uno de los productos software que empleamos en el proyecto. Es importante porque permite que los integrantes colaboren en el ciclo de vida del proyecto. El formato que tiene esta sección consiste en lo siguiente:  descripción del producto software y en la parte inferior una url de referencia.

**Project Management:**
Para el manejo del proyecto empleamos 2 herramientas. Por un lado, usamos Trello, para organizar nuestras actividades semanales ya sea por realizar, en proceso o finalizadas. Todo ello mediante notas de forma sencilla e intuitiva. Por otro lado, utilizamos Google Meet para las reuniones de equipo,  ya que es una aplicación web y resulta cómodo para todo el equipo. Ambas herramientas se despliegan en el navegador, son gratuitas y para su uso es necesario registrarse.

<ul>
    <li> Trello: <a>https://trello.com/</a>
    <li> Google Meet: <a>https://meet.google.com/</a> 
</ul>

**Product UX/UI Design:**
Respecto al diseño empleamos las siguientes 4 herramientas:
Utilizamos UXPressia en la creación de los User personas, el Customer journey map, Empathy map e Impact map porque cuenta con herramientas que nos facilitan el desarrollo de procesos de experiencia del usuario. Nos permite colaborar en equipo, es gratuito y para hacer uso del software necesitamos registrarnos. 
Para la creación de los wireframes, mockups y mobile applications prototyping se utilizó Figma. Figma es una herramienta de diseño colaborativo, para utilizarla debemos registrarnos en su plataforma.
Empleamos Lucidchart para el desarrollo de los wireflows, user flows y diagramas UML. En ella podemos crear diagramas y procesos secuenciales, funciona en el navegador y para usarla es necesario crear una cuenta.
Respecto al database design usamos Vertabelo, es una aplicación web con herramientas preparadas para el modelamiento profesional y que nos permite trabajar en equipo. Requerimos registrarnos para usarla y es gratuita.
<ul>
    <li> UXPressia: <a>https://uxpressia.com/</a>
    <li> Figma: <a>https://www.figma.com/</a> 
    <li> Lucidchart: <a>https://www.lucidchart.com/</a> 
    <li> Vertabelo: <a>https://www.vertabelo.com/</a>  
</ul>

**Software Development:**
<ul>
    <li> Landing Page:  Para la landing page empleamos los siguientes lenguajes, no es necesario instalar ninguno, ya que estos son interpretados por nuestro navegador.
    <li>HTML5: Es un lenguaje de marcado que nos permite construir la estructura de sitios web y aplicaciones más potentes que soportan multimedia.
    <li>CSS3: Con él ilustramos el aspecto, el estilo y el formato de nuestro landing page.
    <li>JavaScript: Es un lenguaje orientado a objetos, nos permite darle dinamismo a la página web.
</ul>

**Mobile Applications:**
Para la realización de nuestra aplicación móvil, utilizaremos los siguientes entornos de desarrollo.

<ul>
    <li>Kotlin: Es un lenguaje de programación moderno y orientado a objetos que se ejecuta en la Máquina Virtual de Java (JVM). Es el lenguaje de programación oficial para el desarrollo de aplicaciones de Android.<br>
    Enlace: <a>https://kotlinlang.org</a>
    <li>Jetpack Compose: Es el kit de herramientas moderno de Android para compilar IU nativas. Permite construir interfaces de usuario más fácilmente y de manera más eficiente.<br>
    Enlace: <a>https://developer.android.com/jetpack/compose?hl=es-419</a>
    <li>Flutter: Es un kit de desarrollo de software de código abierto creado por Google para crear aplicaciones móviles nativas para iOS y Android desde una sola base de código. Utiliza el lenguaje de programación Dart y cuenta con su propio conjunto de widgets personalizados y herramientas de desarrollo.<br>
    Enlace: <a>https://flutter.dev</a>
</ul>

**Software Testing:**
Según IBM (2022), “Las pruebas de software son el proceso de evaluar y verificar que un producto o aplicación de software hace lo que se supone que debe hacer”. Por ello, para las pruebas de testeo software, tanto de la landing page como de la aplicación web, se emplearon las herramientas de desarrollador de múltiples navegadores web como Google Chrome, Microsoft Edge, Brave y Mozilla Firefox. Estos navegadores son aplicaciones desktop y mobile gratuitos. En el caso de desktop podemos instalarlos desde sus sitios oficiales, en el caso de mobile, desde nuestra tienda de aplicaciones favorita.
<ul>
    <li>Google Chrome: <a>https://www.google.com/chrome/ </a>
    <li>Microsoft Edge: <a>https://www.microsoft.com/en-us/edge</a>
    <li>Brave: <a>https://brave.com/ </a>
    <li>Mozilla Firefox: <a>https://www.mozilla.org/en-US/firefox/browsers/</a>
</ul>

**Software Deployment:**
Landing Page: Para el despliegue de nuestra Landing Page utilizamos el servicio gratuito de GitHub Pages.
Github Pages: https://pages.github.com/  


### 6.1.2.	Source Code Management
La gestión y estructuración de las modificaciones se llevaron a cabo a través de GitHub. A continuación, se proporcionan los enlaces de la página de inicio y las pruebas de aceptación:
Landing Page: 
https://github.com/Innova-mind/Innova-mind.github.io

Acceptance Tests:

GitFlow:
Para el GitFlow seguimos lo establecido en “A successful Git branching model” de Vincent Driessen. Según su división podemos diferenciar 2 grupos de ramas.
<ul>
    <li>The main branches:<br>
    <strong>main:</strong> En esta rama almacenaremos las versiones lanzadas, las publicaciones oficiales de nuestro repositorio.<br>
    <strong>develop:</strong> Esta rama se utilizará como rama de integración para las “feature” branches. Una vez el “head” alcance un estado estable y el equipo lo considere listo para ser lanzado, se unirá a la rama release.
    <li>Supporting branches:<br>
    <strong>feature:</strong> En estas ramas trabajaremos las features que se unirán a la rama develop.<br>
    <strong>release:</strong> Esta rama la utilizaremos para preparar el lanzamiento de una nueva versión en la rama “main”. En ella podemos corregir pequeños bugs y preparar datos de la versión. Esta rama liberará la rama “develop” de estas preparaciones, evitando el retraso en el desarrollo mientras se prepara el lanzamiento.<br>
    <strong>feat:</strong> La utilizaremos cuando nuestra última versión en la rama “main” necesite un parche crítico que no puede esperar a un siguiente lanzamiento.
</ul>
En síntesis, tenemos la siguiente tabla:

|**Types of branches**|**May branch off**|**Must merge back into**|**Branch naming convention**|
| - | - | - | - |
|feature|develop|develop|anything except master, develop, release-\*, or hotfix-\*|
|release|develop|develop and master|release-\*|
|hotfix|master|develop and master|hotfix-\*|

Release Versioning Conventions:
Para el formato de versiones aplicamos “Semantic Versioning 2.0.0”. Se emplean X, Y y Z, las cuales representan números enteros positivos e incrementan de uno en uno:
(X.Y.Z)
En donde:
<ul>
    <li>X: Representa una versión mayor. Aquí se encuentran cambios en el API que NO son compatibles con las versiones anteriores. Empezando desde 0 para el desarrollo inicial y 1 cuando esté disponible al público para ser usado. Por convención Y y Z se reiniciarán a 0 cuando este incremente.
    <li>Y: Versión menor. Cambios que SI son compatibles con las versiones anteriores. Aquí incluiremos los commits desde las “release branches” cada vez que se agreguen nuevas funcionalidades. Por convención Z se reiniciará a 0 cuando este incremente.
    <li>Z: Parches y correcciones de errores menores. Aquí incluiremos los commits desde la “hotfix branch” que se unen al “master”.
    Semantic Versioning Specification: https://semver.org/
</ul>
A continuación un ejemplo para una HOTFIX BRANCH:

![HOTFIX BRANCH](/Resources/source-code-management/HOTFIX_BRANCH.png)

Commit Conventions:
El formato de nuestros commits sigue la estructura de los “Conventional Commits”  con el objetivo de proporcionar una lectura sencilla del historial de confirmaciones. Por ello seguimos el siguiente formato:
**< type >[optional scope]: < description >**
Donde:
<ul>
    <li>type: Especifica el tipo de cambio realizado, únicamente puede ser fix, feat o BREAKING CHANGE.
    <li>scope: Es el alcance que tiene nuestro commit.
    <li>description: Es un breve resumen de los cambios de código.
</ul>
Conventional Commits: https://www.conventionalcommits.org/

![Conventional Commits.](/Resources/source-code-management/commits.png)

### 6.1.3.	Source Code Style Guide & Conventions
Para el desarrollo de la parte de HTML se usará el HTML Style Guide and Coding que contiene las convenciones y la guía de estilos para este lenguaje. El nombre del archivo a crear como elemento será “index.html”. Además, se tienen como referencia a este sitio web, donde se especifica la forma correcta de escribir los códigos en html: https://www.w3schools.com/html/html5_syntax.asp  
Para el lenguaje CSS se utilizará el Google HTML/CSS Style Guide, ya que contiene las convenciones que se deben tener en cuenta al trabajar con dicho lenguaje. El elemento de archivo será nombrado como “styles.css”. Para guiarnos de las buenas prácticas accederemos mediante este enlace: https://google.github.io/styleguide/htmlcssguide.html  
Para el lenguaje JavaScript se usará JavaScript Coding Conventions debido a que se especifican las convenciones para tener en cuenta en este lenguaje. La nomenclatura del archivo creado tendrá el nombre “main.js”. Se puede acceder mediante este enlace: https://www.w3schools.com/js/js_conventions.asp  
Para el lenguaje Gherkin se usará las convenciones mencionadas en Make your Gherkin Specifications More Readable con el fin de utilizar buenas prácticas que nos permitan comprender mejor lo desarrollado. Los archivos creados tendrán la extensión “.feature”. Se puede conocer la forma de escribir en lenguaje Gerkhin mediante este enlace: https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/  
Para el desarrollo en Flutter se tiene como referencia las convenciones ya definidas en “Effective Dart: Style” y “Style guide for Flutter repo” definidas por el equipo de Flutter. Esto con el objetivo de mantener un formato entendible y que ayude en el mantenimiento del sistema. Se puede visualizar las convenciones en los siguientes enlaces: 
https://dart.dev/effective-dart/style
https://github.com/flutter/flutter/wiki/Style-guide-for-Flutter-repo    
Para el uso de Java Spring Boot en nuestra API se tendrá en cuenta el Good Coding Standards in Spring Boot
Spring Boot es un marco de alto rendimiento a nivel empresarial muy utilizado y muy popular. En el siguiente enlace se presentan algunas prácticas recomendadas y algunos consejos que puede utilizar para mejorar su aplicación Spring Boot y hacerla más eficiente. 
Se puede visualizar las convenciones en los siguientes enlaces: 
https://levelup.gitconnected.com/how-to-follow-good-coding-standards-in-spring-boot-a22dd735e3ec 

### 6.1.4.	Software Deployment Configuration
En esta sección abordaremos el proceso para desplegar nuestra Landing Page mediante el servicio gratuito de GitHub Pages. A continuación, describiremos los pasos necesarios para el desarrollo.

<ol>
    <li> Primero crearemos un apartado en nuestra organización.<br>
    <img src="/Resources/source-code-management/Software_Deployment_Configuration_1.png" />
    <li> Crearemos un nuevo repositorio para guardar los archivos de nuestra Landing Page
    <img src="/Resources/source-code-management/Software_Deployment_Configuration_2.png"/>
    <li> Procedemos a configurar el repositorio para el despliegue de la Landing Page, para ello necesitamos culminar el sprint 1.
</ol> 

## 6.2	Landing Page, Services & Applications Implementation
### 6.2.1. Sprint 1
#### 6.2.1.1.	Sprint Planning 1

<table><tr><th colspan="1" valign="top">Sprint #</th><th colspan="7" valign="top">1</th></tr>
<tr><td colspan="2" valign="top">User Story</td><td colspan="6" valign="top">Work-Item / Task</td></tr>
<tr><td colspan="1">Id</td><td colspan="1">Title</td><td colspan="1">Id</td><td colspan="1">Title</td><td colspan="1">Description</td><td colspan="1"><p>Estimation</p><p>(hours)</p><p></p></td><td colspan="1">Assigned To</td><td colspan="1"><p>Status</p><p>(To-do /In-</p><p>Process /</p><p>To-</p><p>Review /</p><p>Done)</p></td></tr>
<tr><td colspan="1" rowspan="2">HU23</td><td colspan="1" rowspan="2">Desplazarse fácilmente entre las secciones del landing page</td><td colspan="1">T14-01</td><td colspan="1">Secciones de landing page</td><td colspan="1">Desarrollo de las secciones empresas y clientes, about us, business, y planes y precios.</td><td colspan="1">4</td><td colspan="1">De la Mar Zurita</td><td colspan="1">Done</td></tr>
<tr><td colspan="1">T14-02</td><td colspan="1">Implementar barra de navegación</td><td colspan="1">Barra en la parte superior de la landing page con nombres de las secciones que la conforman</td><td colspan="1">2</td><td colspan="1">Abel Cierto</td><td colspan="1">Done</td></tr>
<tr><td colspan="1" rowspan="3">HU24</td><td colspan="1" rowspan="3">Visualizar los beneficios de los planes</td><td colspan="1">T15-01</td><td colspan="1">Estructura de la portada y el cuerpo</td><td colspan="1">Ubicación de los elementos en la sección correspondiente de la landing page</td><td colspan="1">2</td><td colspan="1">Fiorella Valencia</td><td colspan="1">Done</td></tr>
<tr><td colspan="1">T15-02</td><td colspan="1">Planes para conductores</td><td colspan="1">En esta sección se detallan los beneficios que tiene cada plan para los developers</td><td colspan="1">1</td><td colspan="1">De la mar Zurita</td><td colspan="1">Done</td></tr>
<tr><td colspan="1">T15-03</td><td colspan="1">Planes para empresas</td><td colspan="1">En esta sección se detallan los beneficios que tiene cada plan para las empresas</td><td colspan="1">1</td><td colspan="1">Michael Carrillo</td><td colspan="1">Done</td></tr>
<tr><td colspan="1" rowspan="2">HU25</td><td colspan="1" rowspan="2">Visualizar información sobre los desarrolladores de la app</td><td colspan="1">T16-01</td><td colspan="1">Sección en la landing page</td><td colspan="1">Diseñar y acoplar la sección en la landing page</td><td colspan="1">1</td><td colspan="1">Lennin Huama</td><td colspan="1">Done</td></tr>
<tr><td colspan="1">T16-03</td><td colspan="1">Perfiles de integrantes</td><td colspan="1">Agregar fotos de los integrantes de nuestra organización</td><td colspan="1">1</td><td colspan="1">Lennin Huaman</td><td colspan="1">Done</td></tr>
<tr><td colspan="1" rowspan="3">HU26</td><td colspan="1" rowspan="3">Sección de la landing page para los segmentos de usuarios </td><td colspan="1">T17-01</td><td colspan="1">Encabezado para cada segmento</td><td colspan="1">Imagen representativa en la parte superior según la sección developers o empresas</td><td colspan="1">1</td><td colspan="1">Fiorella Valencia</td><td colspan="1">Done</td></tr>
<tr><td colspan="1">T17-02</td><td colspan="1">Beneficios para los segmentos objetivos</td><td colspan="1">Ventajas que tiene la plataforma para clientes remitentes y empresas</td><td colspan="1">3</td><td colspan="1">Abel Cierto</td><td colspan="1">Done</td></tr>
<tr><td colspan="1">T17-03</td><td colspan="1">About us</td><td colspan="1">Sección que describe brevemente nuestras las características de nuestra organización</td><td colspan="1">1</td><td colspan="1">Abel Cierto</td><td colspan="1">Done</td></tr>
</table>

#### 6.2.1.2. Sprint Backlog 1: Desarrollo de landing page

#### 6.2.1.3. Development Evidence for Sprint Review

#### 6.2.1.4. Testing Suite Evidence for Sprint Review

#### 6.2.1.5. Execution Evidence for Sprint Review

#### 6.2.1.6. Services Documentation Evidence for Sprint Review

#### 6.2.1.7. Software Deployment Evidence for Sprint Review
Para la tb1 se desarrolló el landing page. Para ello, se realizó el despliegue de la landing page en Netlify. 
Luego de haber desplegado, el landing page se podrá acceder a través de un link proporcionado por Netlify.
![Landing Page Hero Section](/Resources/source-code-management/landing_page_1.png)
![Landing Page Company Section](/Resources/source-code-management/landing_page_2.png)
Link: https://6510f678a171f143f95de96d--vermillion-paprenjak-0251b7.netlify.app/ 

#### 6.2.1.8. Team Collaboration Insights during Sprint
Para el desarrollo de cada uno de los artefactos del informe se realizó reuniones por un grupo de Discord, en las cuales dividimos cada uno de los apartados de cada entrega para poder realizarlos con mayor facilidad. Posteriormente, realizado cada punto individualmente, nos reunimos para mostrar nuestros avances y pedir las opiniones de los demás integrantes. Asimismo, se creó una organización en teams para poder organizar las entregas e ir subiendo cada avance. Por otra parte, para la elaboración del landing page empleamos el sistema de control de versiones git y la plataforma de github. A continuación, se mestra el Network graph donde se puede evidenciar todos los commits realizados en nuestro repositorio:

![Network graph](/Resources/source-code-management/network_graph.png)