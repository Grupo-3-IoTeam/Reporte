# **CAPÍTULO VI: PRODUCT IMPLEMENTATION, VALIDATION & DEPLOYMENT**
## 6.1. Software Configuration Management
### 6.1.1. Software Development Environment Configuration
### 6.1.2. Source Code Management
### 6.1.3. Source Code Style Guide & Conventions
### 6.1.4. Software Deployment Configuration
## 6.2. Landing Page, Services & Applications Implementation
Esta sección resume el proceso de implementación, pruebas, documentación y despliegue del Landing Page, Web Services y las Aplicaciones Web y Móviles de ThirstySeed. Durante cada Sprint, se siguieron las mejores prácticas de desarrollo para garantizar la funcionalidad y calidad del producto.
### 6.2.1. Sprint 1
Durante el Sprint 1, se avanzó en la implementación de las funcionalidades planificadas, el equipo colaboró en la integración de los servicios y aplicaciones, realizando pruebas y documentando cada fase. Se incluyeron tareas como la planificación del sprint, la ejecución del desarrollo, la revisión de los avances y el ajuste de los entregables para asegurar un despliegue exitoso.
#### 6.2.1.1. Sprint Planning 1
<table border="1" style="width:100%; text-align: center;">
  <tr>
    <th colspan="4" style="text-align: center;"><strong>LANDING PAGE</strong></th>
  </tr>
  <tr>
    <th colspan="2" style="text-align: center;"><strong>Sprint #</strong></th>
    <th colspan="2" style="text-align: center;"><strong>Sprint 1</strong></th>
  </tr>
  <tr>
    <th colspan="4" style="text-align: center;"><strong>Sprint Planning Background</strong></th>
  </tr>
  <tr>
    <td><strong>Date</strong></td>
    <td colspan="3">2024/09/07</td>
  </tr>
  <tr>
    <td><strong>Time</strong></td>
    <td colspan="3">22:00</td>
  </tr>
  <tr>
    <td><strong>Location</strong></td>
    <td colspan="3">Lima, Peru - Meeting held via Discord</td>
  </tr>
  <tr>
    <td><strong>Prepared By</strong></td>
    <td colspan="3">Vargas Quispe, Manuel Alexis</td>
  </tr>
  <tr>
    <td><strong>Attendees (to planning meeting)</strong></td>
    <td colspan="3">
      Giakomo Rodolfo Causso Mariano<br>Kurt Matthews Puican Salas<br>Rafael Arturo Luyo Ramirez<br>Shayla Lussiné Choque Puma
    </td>
  </tr>
  <tr>
    <th colspan="4" style="text-align: center;"><strong>Sprint Goal & User Stories</strong></th>
  </tr>
  <tr>
    <td><strong>Sprint Goal</strong></td>
    <td colspan="3">Development and deployment of ThirstySeed's Landing Page</td>
  </tr>
  <tr>
    <td><strong>Sprint Velocity</strong></td>
    <td colspan="3">11</td>
  </tr>
  <tr>
    <td><strong>Sum of Story Points</strong></td>
    <td colspan="3">11 story points</td>
  </tr>
</table>




#### 6.2.1.2. Sprint Backlog 1

#### 6.2.1.3. Development Evidence for Sprint Review
<table border="1" cellspacing="0" cellpadding="5" style="width:100%; text-align: center; border-collapse: collapse;">
    <thead>
        <tr>
        <th colspan="6" style="text-align: center;"><strong>LANDING PAGE</strong></th>
        </tr>
        <tr>
            <th style="text-align: center;"><strong>Repository</strong></th>
            <th style="text-align: center;"><strong>Branch</strong></th>
            <th style="text-align: center;"><strong>Commit Id</strong></th>
            <th style="text-align: center;"><strong>Commit Message</strong></th>
            <th style="text-align: center;"><strong>Commit Message Body</strong></th>
            <th style="text-align: center;"><strong>Commited on (Date)</strong></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan="10"><a href="https://github.com/Grupo-3-IoTeam/ThirstySeed-Landing">https://github.com/Grupo-3-IoTeam/ThirstySeed-Landing</a></td>
            <td>Main</td>
            <td>70fe572</td>
            <td>feat: add new final version LandingPage</td>
            <td>Se publicó y editó la versión final del LandingPage (Ya desplegada)</td>
            <td>27/09/2024</td>
        </tr>
        <tr>
            <td>Developer</td>
            <td>601331e</td>
            <td>Update index.html</td>
            <td>Últimos cambios del LandingPage</td>
            <td>27/09/2024</td>
        </tr>
        <tr>
            <td>Feature/section-contact_us</td>
            <td>9ba5e7c</td>
            <td>feat: add file contact-us</td>
            <td>Se realizó la sección de contáctanos</td>
            <td>22/09/2024</td>
        </tr>
        <tr>
            <td>Feature/section-footer</td>
            <td>a9b1c3e</td>
            <td>feat: add file footer</td>
            <td>Se realizó la sección del pie de página</td>
            <td>22/09/2024</td>
        </tr>
        <tr>
            <td>Feature/section-gallery</td>
            <td>7455f96</td>
            <td>feat: add section gallery</td>
            <td>Se realizó la sección galería</td>
            <td>22/09/2024</td>
        </tr>
        <tr>
            <td>Feature/section-home</td>
            <td>459d30a</td>
            <td>feat: file home</td>
            <td>Se realizó la sección de inicio</td>
            <td>22/09/2024</td>
        </tr>
        <tr>
            <td>Feature/section-plans</td>
            <td>67fac89</td>
            <td>feat: add plans</td>
            <td>Se realizó la sección de planes de suscripción</td>
            <td>13/09/2024</td>
        </tr>
        <tr>
            <td>Feature/section-team</td>
            <td>f21e164</td>
            <td>feat: add file team</td>
            <td>Se realizó la sección del equipo</td>
            <td>22/09/2024</td>
        </tr>
        <tr>
            <td>Feature/section-testimonials</td>
            <td>c6027fd</td>
            <td>feat: add testimonials</td>
            <td>Se realizó la sección de testimonios de las personas que usaron la página</td>
            <td>13/09/2024</td>
        </tr>
        <tr>
            <td>Feature/section-toolbar</td>
            <td>14002c5</td>
            <td>feat: add file toolbar</td>
            <td>Se realizó la sección de toolbar</td>
            <td>22/09/2024</td>
        </tr>
    </tbody>
</table>


#### 6.2.1.4. Testing Suite Evidence for Sprint Review
Aquí se proporcionara información sobre las pruebas realizadas durante el sprint.Se detallaran las pruebas funcionales,de rendimiento que se han llevado a cabo para garantizar la calidad del software .Se incluiran los resultados de estas pruebas y cualquier correcion o mejora realizada.

## Landing Page
<p align="center">
    <img src="assets/Testing-Landing.png" alt="Imagen" style="width:100%"/>
</p>
<p align="center">
    <strong>Landing Page Testeo:</strong>
    <a href="https://pagespeed.web.dev/analysis/https-grupo-3-ioteam-github-io-ThirstySeed-Landing/foaeucaur9?hl=es-ES&form_factor=desktop" target="_blank">
        https://pagespeed.web.dev/analysis/https-grupo-3-ioteam-github-io-ThirstySeed-Landing/foaeucaur9?hl=es-ES&form_factor=desktop
    </a>
</p>

#### 6.2.1.5. Execution Evidence for Sprint Review
Esta sección se centrará en la ejecución de la aplicación durante el sprint. Se visualizará la navegación del Landing Page como la de la página web, de esta manera se destacaran las características y funcionalidades implementadas en la aplicación.
## Landing Page
<td><img src="assets/Evidence-Landing.png" alt="Imagen" style="width:100%"></td>
<p align="center">
    <strong>Landing Page Desplegado:</strong>
    <a href="https://grupo-3-ioteam.github.io/ThirstySeed-Landing/" target="_blank">
        https://grupo-3-ioteam.github.io/ThirstySeed-Landing/
    </a>
</p>

#### 6.2.1.6. Services Documentation Evidence for Sprint Review
#### 6.2.1.7. Software Deployment Evidence for Sprint Review
En este Sprint, nos enfocamos en el despliegue del producto ThirstySeed a través de GitHub para el deployment y la administración del repositorio. El proceso incluyó la creación de las cuentas y configuraciones necesarias para asegurar una integración eficiente entre el Landing Page, los Web Services y las Aplicaciones móviles.

<table border="1" style="width: 100%; text-align: center;">
    <tr>
        <th colspan="2" style="text-align: center;"><strong>LANDING PAGE</strong></th>
    </tr>
    <tr>
        <td style="text-align: left;">
            <strong>1. Creación de repositorios en GitHub:</strong> Se creó un repositorio dedicado para alojar el código de la Landing Page. Esto permitió la colaboración fluida y el control de versiones entre los miembros del equipo.
        </td>
    </tr>
    <tr>
        <td><img src="assets/Repo-Landing.png" alt="Imagen" style="width:100%"></td>
    </tr>
    <tr>
        <td style="text-align: left;">
            <strong>2. Despliegue en GitHub Pages:</strong> El <strong>Landing Page</strong> fue desplegado utilizando <strong>GitHub Pages</strong>, lo que facilitó la visualización pública de la web. Esta configuración incluyó la automatización del proceso para que cada vez que se hiciera un commit en la rama principal (main), el sitio se actualizara automáticamente.
        </td>
    </tr>
    <tr>
        <td><img src="assets/Pages-Landing.png" alt="Imagen" style="width:100%"></td>
    </tr>
</table>


<img src="assets/BARRA-SEPARADORA.png" alt="BARRA SEPARADORA" style="width:100%">



#### 6.2.1.8. Team Collaboration Insights during Sprint
<table border="1" style="width: 100%; text-align: center;">
    <tr>
        <th colspan="2" style="text-align: center;"><strong>LANDING PAGE</strong></th>
    </tr>
    <tr>
        <td colspan="2" style="text-align: justify;">
            En esta entrega, el objetivo principal fue la implementación de las funciones para la gestión y visualización en <strong>ThirstySeed</strong>. Para cumplir con este propósito, se utilizaron herramientas como <strong>GitHub</strong> (para el <em>deployment</em> y gestión del repositorio), <strong>Visual Studio Code</strong> como entorno de desarrollo, y lenguajes como <strong>HTML, CSS,</strong> y <strong>JavaScript</strong> para la construcción de la interfaz y funcionalidad. A continuación, se presentan los diagramas de flujo que detallan los <strong>commits</strong> realizados y las contribuciones de cada miembro del equipo en el desarrollo del proyecto.
        </td>
    </tr>
    <tr>
        <td colspan="2"><img src="assets/Pulse-Landing.png" alt="Imagen" style="width:100%"></td>
    </tr>
    <tr>
        <td colspan="2" style="text-align: justify;">
            En la imagen se evidencia el gráfico de barras de la cantidad de <strong>commits</strong> realizados por cada uno de los integrantes del equipo.
        </td>
    </tr>
    <tr>
        <td colspan="2"><img src="assets/Contributor-Landing.png" alt="Imagen" style="width:100%"></td>
    </tr>
    <tr>
        <td colspan="2" style="text-align: justify;">
            En esta imagen, se ofrece una representación visual de las fechas en las que se llevaron a cabo cambios en el repositorio de nuestro sprint (Enfocado al <strong>Landing Page</strong>), junto con la cantidad de modificaciones realizadas en cada uno de los <strong>commits</strong>. Esta representación gráfica es una herramienta valiosa para comprender la evolución temporal del proyecto y la intensidad del desarrollo a lo largo del tiempo.
        </td>
    </tr>
    <tr>
        <td colspan="2"><img src="assets/Traffic-Landing.png" alt="Imagen" style="width:100%"></td>
    </tr>
    <tr>
        <td colspan="2" style="text-align: justify;">
            Estos gráficos ofrecen una representación visual de las clonaciones registradas en nuestro repositorio, junto con la fecha en que cada una de estas acciones se llevó a cabo. Además, se presenta información sobre la cantidad de visitantes que ha tenido el repositorio de nuestro equipo a lo largo del tiempo.
        </td>
    </tr>
    <tr>
        <td colspan="2"><img src="assets/TeamColla-Landing.png" alt="Imagen" style="width:100%"></td>
    </tr>
</table>

<img src="assets/BARRA-SEPARADORA.png" alt="BARRA SEPARADORA" style="width:100%">