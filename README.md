# DWES
Trabajo para la creación de una base para la programación del módulo Desarrollo Web en Entorno Servidor. 

## Resultados de aprendizaje principales

Según la programación didáctica de referencia y la normativa vigente, los resultados de aprendizaje (RA) del módulo son:

* Seleccionar arquitecturas y tecnologías de programación web en entorno servidor, analizando sus capacidades y características.

* Escribir sentencias ejecutables por un servidor web, integrando código en lenguajes de marcas.

* Escribir bloques de sentencias embebidos en lenguajes de marcas, utilizando estructuras de programación.

* Desarrollar aplicaciones web embebidas en lenguajes de marcas, incorporando funcionalidades según especificaciones.

* Desarrollar aplicaciones web separando el código de presentación de la lógica de negocio.

* Desarrollar aplicaciones de acceso a almacenes de datos, aplicando medidas de seguridad e integridad.

* Desarrollar servicios web, analizando su funcionamiento e implantando la estructura de sus componentes.

* Generar páginas web dinámicas utilizando tecnologías del servidor web que añadan código al lenguaje de marcas.

* Desarrollar aplicaciones web híbridas utilizando librerías de código y repositorios heterogéneos de información.

* Competencias y capacidades asociadas

## Secuenciación y Unidades de Trabajo con Jakarta EE y Django REST Framework

A continuación se presenta una propuesta de secuenciación de contenidos para el módulo "Desarrollo web en entorno servidor" en Formación Profesional de Aragón, adaptada para impartirse utilizando las tecnologías Jakarta EE (Java) y Django REST Framework (Python). Esta secuenciación cubre los resultados de aprendizaje establecidos y permite al alumnado adquirir competencias prácticas en ambos entornos, facilitando la comparación y el aprendizaje transversal.

### **1. Introducción a las arquitecturas web en entorno servidor**

- Conceptos de cliente-servidor, HTTP, REST y APIs.
- Diferencias y similitudes entre Jakarta EE y Django REST Framework.
- Instalación y configuración de entornos de desarrollo:
  - Eclipse/IntelliJ + WildFly/Payara para Jakarta EE[1].
  - Python, Django y Django REST Framework para Django[2][3].

### **2. Estructura básica de una aplicación web**

- Proyecto Java con Jakarta EE: estructura de carpetas, configuración con Maven, despliegue en servidor de aplicaciones[1].
- Proyecto Python con Django: estructura de carpetas, configuración de settings, migraciones y gestión de apps[2][3].
- Primeros endpoints: “Hola Mundo” en ambos entornos.

### **3. Desarrollo de la lógica de negocio y controladores**

- Servlets, controladores y recursos REST en Jakarta EE.
- Vistas, viewsets y routers en Django REST Framework[2][3].
- Implementación del patrón MVC en ambos frameworks[4][1].

### **4. Modelado y acceso a datos**

- Definición de modelos de datos:
  - JPA y entidades en Jakarta EE.
  - Modelos Django y migraciones.
- Acceso a bases de datos (PostgreSQL recomendado en ambos casos).
- Operaciones CRUD básicas:
  - Jakarta EE: JPA, DAOs, EJBs.
  - Django REST Framework: Serializers, ModelViewSets[5][2][3].

### **5. Seguridad y autenticación**

- Gestión de sesiones, autenticación y autorización:
  - Jakarta EE: dominios de seguridad, control de sesiones, uso de filtros y anotaciones de seguridad.
  - Django REST Framework: autenticación por Token/JWT, permisos y control de acceso[2].
- Buenas prácticas en la gestión de usuarios y roles.

### **6. Desarrollo de servicios web y APIs REST**

- Creación y consumo de servicios RESTful en Jakarta EE (JAX-RS)[4][1].
- Creación y consumo de APIs REST con Django REST Framework[5][6][2][3].
- Serialización y deserialización de datos (JSON).
- Documentación automática de APIs (Swagger/OpenAPI, DRF Browsable API).

### **7. Separación de lógica de negocio y presentación**

- Jakarta EE: uso de JSP, JSF o plantillas Thymeleaf para separar vistas y lógica.
- Django: separación entre views, templates y lógica de negocio.
- Integración de frontend básico para pruebas (HTML, JavaScript).

### **8. Generación dinámica de páginas y aplicaciones híbridas**

- Procesamiento en servidor y en cliente.
- Jakarta EE: generación dinámica con JSP/JSF y salida de datos en tablas[7].
- Django: generación dinámica de páginas y endpoints que interactúan con JavaScript y frameworks frontend.

### **9. Integración y reutilización de librerías y repositorios**

- Uso de librerías externas y gestión de dependencias:
  - Jakarta EE: Maven, integración de bibliotecas.
  - Django: pip, integración de paquetes y reutilización de apps.
- Consumo de APIs externas y trabajo con datos heterogéneos.

### **10. Pruebas, despliegue y documentación**

- Pruebas unitarias y funcionales en ambos entornos.
- Despliegue en servidores de producción (WildFly, Gunicorn, Docker).
- Documentación técnica y de usuario de las aplicaciones desarrolladas.
- Buenas prácticas de mantenimiento y actualización.

## Adaptación del módulo a trabajo por proyectos: Proyecto de una Asociación en Jakarta EE y Django REST Framework

El módulo "Desarrollo web en entorno servidor" se organizará en torno a la implementación de un proyecto realista: la gestión integral de una asociación. Este proyecto servirá como hilo conductor y se desarrollará de manera paralela en ambos frameworks, Jakarta EE y Django REST Framework, permitiendo al alumnado comparar enfoques, herramientas y buenas prácticas.

**Enfoque general del proyecto**
El proyecto de la asociación incluirá funcionalidades típicas como:

* Gestión de socios (altas, bajas, modificaciones, consulta)
* Gestión de actividades/eventos
* Gestión de cuotas y pagos
* Autenticación y autorización de usuarios (socios, administradores)
* Generación de informes y listados
* API REST para integración con frontend (por ejemplo, usando Vue.js o Nuxt.js)
* Seguridad y buenas prácticas (por ejemplo, uso de JWT para autenticación segura)

### Secuenciación de contenidos aplicada al proyecto
#### 1. Análisis y diseño del proyecto

Levantamiento de requisitos y modelado de datos de la asociación.

Diseño de la arquitectura de la aplicación en ambos frameworks.

#### 2. Configuración de entornos y creación de proyectos base

Creación y configuración del proyecto en Jakarta EE (Eclipse/IntelliJ + Maven + WildFly/Payara).

Creación y configuración del proyecto en Django REST Framework (gestión de variables de entorno, configuración de settings).

#### 3. Implementación de la gestión de usuarios y autenticación

Registro, login y gestión de sesiones.

Implementación de autenticación JWT en Django REST Framework.

Implementación de autenticación y control de acceso en Jakarta EE.

#### 4. Desarrollo de modelos y acceso a datos

Modelado de entidades: Socios, Actividades, Pagos.

Implementación de modelos y migraciones en Django.

Implementación de entidades JPA y DAOs en Jakarta EE.

#### 5. Desarrollo de la API REST

Creación de endpoints CRUD para socios, actividades y pagos en ambos frameworks.

Serialización y deserialización de datos (JSON).

Pruebas de los endpoints con herramientas como Postman.

#### 6. Seguridad y control de acceso

Definición de roles y permisos (socios, administradores).

Protección de rutas y recursos sensibles.

#### 7. Integración con frontend

Preparación de la API para ser consumida desde un frontend moderno (Vue.js con Nuxt.js, por ejemplo).

Pruebas de integración y documentación de la API.

#### 8. Generación de informes y listados

Endpoints para informes de pagos, listados de socios y actividades.

Exportación de datos (CSV, PDF).

#### 9. Pruebas, despliegue y documentación

Pruebas unitarias y funcionales.

Despliegue en servidores de pruebas y producción.

Documentación técnica y de usuario.

---

Esta secuenciación permite cubrir los resultados de aprendizaje del módulo, adaptando los contenidos a tecnologías actuales y demandadas como Jakarta EE y Django REST Framework, y asegurando la adquisición de competencias clave en desarrollo web en entorno servidor[8][7].

[1] https://danielme.com/2021/04/01/curso-jakarta-ee-la-primera-aplicacion-web/
[2] programming.java_web
[3] https://hektorprofe.github.io/academia/django/api-rest-framework/
[4] https://www.paradigmadigital.com/dev/introduccion-django-rest-framework/
[5] programming.python_web
[6] programming.django
[7] https://www.youtube.com/watch?v=E3NLddQ0dTM
[8] http://blog.enriqueoriol.com/2014/06/introduccion-django-rest-framework.html
[9] programming.api_development
[10] https://azulschool.net/courses/creacion-y-consumo-de-apis-con-django-rest-framework/
[11] https://www.iesjulioverne.es/wp-content/uploads/2025/01/Programaci%D0%B2n-Entorno-Servidor-2DAW_24_25.pdf
[12] programming.web_performance
[13] https://www.iesaguadulce.es/gestiona/datos/programaciones/FP_DAW_2/DWESE_89502229/2023_24/programacion_585219.pdf
[14] education.web_development
[15] https://www.youtube.com/watch?v=GE0Q8YNKNgs
[16] https://www.udemy.com/course/curso-jakartaee-java-ee-9-desde-cero-a-experto/
[17] https://www.apuntesdejava.com/search/label/jakarta%20ee
[18] https://blackhold.nusepas.com/2020/09/20/servidor-y-cliente-rest-django-rest-framework-requests/
[19] https://www.youtube.com/watch?v=KILuIyf91aA
[20] https://www.paraninfo.es/catalogo/9788428363877/uf1844---desarrollo-de-aplicaciones-web-en-el-entorno-servidor
[21] https://www.sitiolibre.com/curso/pdf/DWES01.pdf
[22] https://cursos.arquitecturajava.com/p/curso-jsf-java-server-faces-4-jakarta-faces
[23] http://www.iesaguadulce.es/gestiona/datos/programaciones/FP_DAW_2/DWESE_89502229/2020_21/programacion_110620.pdf
[24] https://developer.mozilla.org/es/docs/Learn_web_development/Extensions/Server-side/Django/development_environment
[25] https://iesruizgijon.es/images/departamentos/informatica/programaciones/DAW/prog_DAW-22-23_RG.pdf
[26] https://servidor.codeandcoke.com/apuntes:aplicaciones_web
