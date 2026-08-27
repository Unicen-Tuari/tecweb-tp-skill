# Videos de la Cátedra – Tecnologías Web (TUARI)

> **Fuente:** canal de YouTube [Tecnologías Web & DevOps - TUARI](https://www.youtube.com/@tecnologiaswebdevops-tuari6957/playlists).
> **Alcance:** este documento cubre únicamente el contenido de **Tecnologías Web** (no incluye la playlist "Operaciones de Desarrollo", que pertenece a la materia DevOps). Para NestJS se usó exclusivamente la playlist **"Nest JS 2025"** (versión vigente), no la playlist anterior "Nest Js".
> **Uso previsto:** citar el video de cátedra correspondiente (título + link + timestamp aproximado) además de la documentación oficial, cuando ayude al alumno a repasar un concepto visto en clase.

## Cómo se armó este documento (nota de transparencia — importante)

Para cada uno de los 22 videos se relevó: título, duración, descripción oficial (cuando estaba
disponible) y, cuando fue posible, el transcript de YouTube o las diapositivas/código visibles en
pantalla. En la práctica, el panel de transcripts de YouTube resultó poco confiable durante el
procesamiento: **solo 1 de los 22 videos** ("Introducción a Nest Js") pudo procesarse con
transcript completo. Para el resto, el resumen se construyó combinando el título, la descripción
oficial del video, diapositivas/código capturados en pantalla cuando fue posible, y el
conocimiento general del temario de la materia.

Cada entrada indica explícitamente su nivel de confianza en el campo **Nota**:
- Sin nota especial → resumen basado en descripción oficial del video (alta confianza).
- "transcript no disponible..." → resumen inferido de título + diapositivas/código visibles +
  temario general (confianza media).

Ningún resumen reproduce el transcript verbatim de YouTube; son resúmenes originales con fines de
referencia y búsqueda por palabras clave.

**Regla al citar estos videos:** cuando cites un video con nota de confianza media, no presentes
el timestamp como si fuera exacto — decí algo como "cerca del inicio, en la clase de X" en vez de
afirmar un minuto puntual con total seguridad. Para "Introducción a Nest Js" (el único con
transcript completo) sí podés citar los timestamps con confianza.

---

## Índice de playlists

1. [Teóricas](#teóricas) — fundamentos conceptuales (Web, MVC, REST, HTML/CSS/JS)
2. [Nest JS 2025](#nest-js-2025) — backend con NestJS
3. [Angular](#angular) — frontend con Angular
4. [Contenido Extra](#contenido-extra) — herramientas (VS Code, Postman)
5. [Clases en Vivo](#clases-en-vivo) — grabaciones de clases en vivo (introductorias y control de versiones)

---

## Teóricas

### Introducción a la Web
- **Playlist:** Teóricas
- **URL:** https://www.youtube.com/watch?v=YoINyeYV4G0
- **Duración:** 59:26
- **Resumen:** Clase teórica inaugural de la materia sobre los fundamentos de la Web. Como primera clase teórica, cubre la historia y evolución de Internet y la World Wide Web, la arquitectura cliente-servidor, el protocolo HTTP/HTTPS, el rol del navegador y el servidor, URLs/URIs, y cómo se comunican los distintos actores (cliente, servidor, base de datos) en una aplicación web moderna — sentando las bases que luego se retoman en REST, MVC y en el desarrollo práctico con NestJS y Angular.
- **Keywords:** Introducción a la Web, Internet, World Wide Web, arquitectura cliente-servidor, HTTP/HTTPS, navegador, servidor, URL/URI, historia de la Web.
- **Timestamps clave:** 0:00 Introducción a la materia y a los conceptos fundamentales de la Web.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título, la posición de la clase como primera teórica de la materia y el temario general.

### Model View Controller
- **Playlist:** Teóricas
- **URL:** https://www.youtube.com/watch?v=lcNKJ4DDT-M
- **Duración:** 45:45
- **Resumen:** Clase teórica sobre el patrón de diseño Model-View-Controller (MVC). Explica la separación de responsabilidades entre las tres capas: el Model (datos y lógica de negocio/acceso a datos), la View (presentación/interfaz) y el Controller (intermediario entre solicitudes y Model/View), y por qué esta separación facilita mantener, testear y escalar una aplicación. Sienta las bases conceptuales que luego se ven aplicadas en los Controllers y Services de NestJS y en los Components de Angular.
- **Keywords:** MVC, Model-View-Controller, patrón de diseño, arquitectura de software, separación de responsabilidades, Model, View, Controller.
- **Timestamps clave:** 0:00 Introducción al patrón MVC y sus tres capas.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título, la temática estándar de una clase de MVC y su ubicación en el programa de la materia.

### Rest
- **Playlist:** Teóricas
- **URL:** https://www.youtube.com/watch?v=IiSfU1oR_m0
- **Duración:** 26:52
- **Resumen:** Clase teórica sobre REST (Representational State Transfer), el estilo arquitectónico base de las APIs de la materia. Cubre los principios de REST: los recursos se identifican mediante URIs, se accede y modifica su estado usando los métodos estándar de HTTP (GET, POST, PUT/PATCH, DELETE), la comunicación es stateless, y las respuestas usan códigos de estado HTTP (2xx, 4xx, 5xx). Es la clase teórica de referencia que las clases prácticas de NestJS ("Controllers en Nest JS", "Rest + Filtrado") y de Angular ("Angular - Rest", "Angular - Rest Crear Recursos") citan y aplican directamente sobre el caso Brewery/Beer.
- **Keywords:** REST, API REST, recurso, URI, métodos HTTP (GET/POST/PUT/PATCH/DELETE), stateless, códigos de estado HTTP, arquitectura REST.
- **Timestamps clave:** 0:00 Introducción a REST y sus principios.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título y de que es la teoría de referencia citada explícitamente en clases prácticas posteriores.

### Introducción a HTML, CSS y JS
- **Playlist:** Teóricas
- **URL:** https://www.youtube.com/watch?v=qB-IHzr1IGM
- **Duración:** 1:22:53
- **Resumen:** Clase teórico-práctica introductoria a las tres tecnologías base del frontend web: HTML como lenguaje de marcado para estructurar contenido (etiquetas, elementos, atributos); CSS para estilo y presentación visual (selectores, propiedades, box model, maquetación); y JavaScript como lenguaje para agregar comportamiento e interactividad del lado del cliente (manipulación del DOM, eventos, variables y funciones básicas). Por su duración y ubicación temprana en el programa, funciona como base previa a Angular.
- **Keywords:** HTML, CSS, JavaScript, frontend, lenguaje de marcado, hojas de estilo, DOM, interactividad del lado del cliente, fundamentos web.
- **Timestamps clave:** 0:00 Introducción; contenido dividido presumiblemente en tres bloques (HTML, CSS, JS).
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título y el temario estándar de una clase introductoria a HTML/CSS/JS.

---

## Nest JS 2025

### Introducción a Nest Js
- **Playlist:** Nest JS 2025
- **URL:** https://www.youtube.com/watch?v=m74AFuBEmhY
- **Duración:** 45:00
- **Resumen:** Clase introductoria a NestJS como framework backend de la materia. Explica qué es un framework, por qué se usa NestJS (mismo paradigma/TypeScript que Angular), y presenta el panorama general cliente-backend-DB. Repasa prerrequisitos (Node.js, npm), qué es un CLI y cómo instalar/usar el CLI de Nest (`nest new`, `nest generate`). Introduce el caso de uso guía de la materia: una app de cervecería (Brewery) con entidad Beer, y mapea los métodos HTTP (GET, POST, PATCH, DELETE) a acciones CRUD sobre esa entidad. Crea el proyecto con `nest new brewery`, recorre la estructura generada, corre la app (Hello World), modifica el AppController/AppService, explica `start` vs `start:dev` (watch mode), y cierra subiendo el proyecto a GitHub.
- **Keywords:** NestJS, framework, TypeScript, Node.js, npm, CLI (nest new / nest generate), arquitectura REST, AppModule, Controller, Service, Provider, métodos HTTP (GET/POST/PATCH/DELETE), watch mode (start:dev), Git/GitHub, caso de uso "Brewery" (cervecería), entidad Beer.
- **Timestamps clave:**
  - 0:00 Introducción y objetivos de la materia
  - 2:00 ¿Qué es un framework?
  - 4:39 Arquitectura general (backend NestJS + frontend Angular)
  - 7:39 Prerrequisitos (Node.js, npm)
  - 9:38 ¿Qué es un CLI?
  - 11:47 Instalación del CLI de Nest
  - 12:44 Comandos básicos (nest new, nest generate)
  - 13:41 Caso de uso: app de cervecería (Brewery)
  - 15:00 Métodos HTTP (GET, POST, DELETE, PATCH) aplicados al recurso Beer
  - 17:59 Creación del proyecto (`nest new brewery`)
  - 20:09 Recorrido de archivos generados
  - 33:52 Demo: modificar Hello World (AppController/AppService)
  - 37:49 start vs start:dev (watch mode)
  - 40:43 Documentación oficial de NestJS
  - 40:51 Subir el proyecto a GitHub
- **Nota:** único video de los 22 procesado con transcript completo de YouTube; timestamps de alta confianza.

### Controllers en Nest JS
- **Playlist:** Nest JS 2025
- **URL:** https://www.youtube.com/watch?v=vWwrd2eCsBU
- **Duración:** 1:08:36
- **Resumen:** Clase centrada en los Controllers de NestJS, continuando el ejemplo de la cervecería (Brewery/Beer). Explica qué es un controller (recibe solicitudes HTTP de un cliente, dirige el flujo y responde) y cómo el ruteo decide qué controller atiende cada solicitud usando clases y decorators (`@Controller`, `@Get`, `@Post`, etc.). Muestra en código el `BeersController` con rutas para listar (`GET /beers`) y crear (`POST /beers`), y anticipa endpoints para traer por id, borrar y actualizar stock (`GET/DELETE /beers/:id`, `PATCH /beers/:id/stock`). Cierra remitiendo a la clase teórica de REST.
- **Keywords:** NestJS, Controllers, @Controller, @Get, @Post, @Delete, @Patch, routing/ruteo, decorators, endpoint, BeersController, CRUD, REST, recurso Beer, cervecería (Brewery).
- **Timestamps clave (aproximados):**
  - 0:00 Qué son los Controllers en NestJS
  - ~10:00 Ruteo: cómo se decide qué controller atiende cada solicitud
  - ~20:00 Ejemplo de ruteo: `beers.controller.ts`, tabla de endpoints
  - Última parte: demo de código y referencia a la teoría de REST
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir de las diapositivas visibles en el video y el título/descripción.

### Nest JS Providers & Services
- **Playlist:** Nest JS 2025
- **URL:** https://www.youtube.com/watch?v=mIqcHllXd7Y
- **Duración:** 1:20:55
- **Repo de referencia:** github.com/Unicen-Tuari/brewery
- **Resumen:** Clase sobre Providers y Services en NestJS, siguiendo con el proyecto Brewery/Beer. Introduce el service (`beers.service.ts`) como responsable de guardar y recuperar los datos (`@Injectable()`, array en memoria, métodos `create` y `findAll`), y explica el reparto de responsabilidades: BeerController (request), BeerService (lógica/datos) y BeerEntity, dentro de BeersModule/AppModule (Client → Controller → Service → futuro DB). Avanza el CRUD con `update(id, beer: UpdateBeerDto)` usando `findIndex`, e introduce DTOs (`CreateBeerDto`, `UpdateBeerDto`). Muestra el uso del CLI de Nest para generar el service (`nest g s Beers`).
- **Keywords:** NestJS, Provider, Service, @Injectable, BeerService, BeerController, BeerEntity, BeersModule, AppModule, DTO (CreateBeerDto/UpdateBeerDto), CRUD (create/findAll/update), findIndex, CLI de Nest (nest generate service), inyección de dependencias.
- **Timestamps clave (aproximados):**
  - ~14:36 Ejemplo BeersService (create, findAll)
  - ~24:34 Diagrama de arquitectura Client → BeerController → BeerService → BeerEntity → DB
  - ~57:50 Demo de código: `update()` con DTOs, generación del service con el CLI
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir de las diapositivas y el código mostrado en pantalla.

### Rest + Filtrado en Nest JS
- **Playlist:** Nest JS 2025
- **URL:** https://www.youtube.com/watch?v=qezMe7BawK0
- **Duración:** 52:16
- **Resumen:** Clase que retoma (repaso) la teoría de REST — una URI representa un recurso accesible/modificable mediante los métodos HTTP (POST, GET, PUT, DELETE) — y la aplica al proyecto Brewery/Beer en NestJS, agregando filtrado sobre el endpoint de listado (`findAll`). Avanza hacia cómo recibir query params en el controller/service para filtrar resultados, consolidando el CRUD construido en las clases anteriores de Nest.
- **Keywords:** REST, arquitectura REST, recurso, URI, métodos HTTP (GET/POST/PUT/DELETE), filtrado, query params, NestJS, findAll, Brewery/Beer.
- **Timestamps clave (aproximados):** 0:00 Repaso teórico de REST; resto del video: implementación de filtrado sobre el listado de cervezas.
- **Nota:** transcript no disponible en esta sesión (video sin descripción); resumen armado a partir de las diapositivas visibles.

---

## Angular

### Angular - Introducción
- **Playlist:** Angular
- **URL:** https://www.youtube.com/watch?v=uzqWh7dC6Yk
- **Duración:** 27:16
- **Resumen:** Primera clase de la parte de frontend. Presenta Angular como "un framework JavaScript de código abierto, mantenido por Google, que se utiliza para crear y mantener aplicaciones web de una sola página (SPA)". Introduce por qué se usa Angular en la materia (mismo paradigma orientado a componentes y TypeScript que se vio en NestJS) y sienta las bases conceptuales (SPA, framework, TypeScript) antes de entrar en componentes.
- **Keywords:** Angular, framework, JavaScript/TypeScript, SPA (Single Page Application), Google, frontend.
- **Timestamps clave:** 0:00 Definición de Angular y por qué se usa en la materia.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir de la diapositiva de título/definición.

### Angular - Components
- **Playlist:** Angular (también en Teóricas, es el mismo video)
- **URL:** https://www.youtube.com/watch?v=a9aJj9n0fTg
- **Duración:** 1:02:54
- **Resumen:** Clase central sobre la arquitectura de Angular y los Components. Presenta el diagrama de arquitectura: un Module agrupa Components, Services, Values y funciones; cada Component tiene un Template (vista), Metadata y Decorators; los Directives extienden el comportamiento vía Metadata; el Injector provee Services (inyección de dependencias) a los Components; y la comunicación Template↔Component se da mediante Property Binding (datos hacia la vista) y Event Binding (eventos desde la vista). A partir de este mapa conceptual, entra en la práctica de crear y estructurar componentes.
- **Keywords:** Angular, Arquitectura Angular, Module, Component, Service, Directive, Template, Metadata, Injector, Dependency Injection, Property Binding, Event Binding.
- **Timestamps clave:** 0:00 Diagrama de arquitectura de Angular.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir de la diapositiva de arquitectura mostrada en el video.

### Angular - Interfaces & Directivas
- **Playlist:** Angular
- **URL:** https://www.youtube.com/watch?v=XH5VMnLI2ps
- **Duración:** 43:24
- **Resumen:** Clase sobre dos herramientas de TypeScript/Angular. Interfaces: TypeScript verifica tipos (`let name: string`, `let price: number`), y además de tipos primitivos se puede usar una `interface` para definir la forma de datos más complejos (por ejemplo, una entidad como Beer). Directivas: introduce las directivas de Angular (estructurales y de atributo) que permiten modificar la estructura o apariencia del DOM desde el template (`*ngIf`, `*ngFor`, `ngClass`/`ngStyle`), aplicándolas sobre el listado de cervezas.
- **Keywords:** TypeScript, interface, tipado, tipos primitivos, Angular, directivas, directivas estructurales, *ngIf, *ngFor, DOM, template.
- **Timestamps clave (aproximados):** 0:00 Introducción; Interfaces (tipado con TypeScript); Directivas (manipulación del DOM desde el template).
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir de las diapositivas visibles (interfaces) y el título del video (directivas).

### Angular - Events and Binding
- **Playlist:** Angular
- **URL:** https://www.youtube.com/watch?v=KHZG6afbzgk
- **Duración:** 35:15
- **Resumen:** Clase sobre el flujo de datos en Angular entre el componente (TypeScript) y la vista (HTML): (1) JavaScript a HTML — property binding, como mostrar un título o el listado de cervezas; (2) HTML a JavaScript — event binding, capturar eventos del usuario (click, hover, input, key press); y (3) Two-Way Data Binding, donde un input queda sincronizado en ambas direcciones (típicamente con `[(ngModel)]`). Aplica estos conceptos al proyecto de la cervecería.
- **Keywords:** Angular, Data Binding, Property Binding, Event Binding, Two-Way Data Binding, ngModel, eventos (click, hover, input, key press), flujo de datos.
- **Timestamps clave:** 0:00 Flujo de datos: las 3 formas de binding.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir de la diapositiva "Flujo de datos" mostrada en el video.

### Angular - Routing
- **Playlist:** Angular
- **URL:** https://www.youtube.com/watch?v=GDpg7WRuuSM
- **Duración:** 32:23
- **Resumen:** Clase sobre el sistema de ruteo (Routing) de Angular: cómo navegar entre distintas vistas/componentes sin recargar la página (comportamiento propio de una SPA), definiendo rutas que asocian una URL con un componente, usando el `router-outlet` para renderizar la vista activa y `routerLink` para navegación. Se aplica al proyecto de la cervecería para navegar, por ejemplo, entre el listado y el detalle/edición de una cerveza.
- **Keywords:** Angular, Routing, RouterModule, rutas, router-outlet, routerLink, navegación, SPA, componentes.
- **Timestamps clave:** 0:00 Introducción a Routing en Angular.
- **Nota:** transcript no disponible en esta sesión; resumen basado en el título/tema y el temario general de la materia.

### Angular - Rest
- **Playlist:** Angular
- **URL:** https://www.youtube.com/watch?v=kB59jNuwU9Y
- **Duración:** 37:59
- **Resumen:** Clase clave de conexión frontend-backend: hasta este punto el service de Angular traía datos desde un mock; esta clase explica cómo traer los datos desde un servicio real o desde el propio backend NestJS, usando `HttpClient` de Angular. Es el puente entre el Angular Service y los endpoints REST del backend (Beers), reemplazando el mock por llamadas HTTP reales (típicamente `GET /beers`).
- **Keywords:** Angular, HttpClient, REST, consumo de API, servicios (Service), mock vs. API real, backend NestJS, Observable.
- **Timestamps clave:** 0:00 "Usando http": por qué pasar de datos mockeados a un servicio HTTP real.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir de la diapositiva "Usando http" mostrada en el video.

### Angular - Rest Crear Recursos
- **Playlist:** Angular
- **URL:** https://www.youtube.com/watch?v=icgP4QE6H1s
- **Duración:** 38:34
- **Resumen:** Clase que continúa la integración de Angular con el backend REST, ahora enfocada en la creación de recursos: cómo enviar datos desde un formulario/componente Angular al backend mediante `HttpClient` (petición POST) para dar de alta una nueva cerveza, extendiendo el service de Angular con un método de creación que llama al endpoint `POST /beers` del backend NestJS.
- **Keywords:** Angular, HttpClient, REST, POST, creación de recursos, formularios, Service, backend NestJS, Brewery/Beer.
- **Timestamps clave:** 0:00 Introducción; contenido centrado en crear recursos vía HTTP POST desde Angular hacia el backend.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título, la descripción y el temario general (continuación directa de "Angular - Rest").

### Angular - Carrito de Compras
- **Playlist:** Angular
- **URL:** https://www.youtube.com/watch?v=usitjozxrDU
- **Duración:** 24:33 (video más visto de la playlist, 8.6K vistas)
- **Resumen:** Clase práctica que implementa un carrito de compras sobre el proyecto Brewery en Angular, como ejercicio integrador de Components, Services y Binding. Se ve trabajo de terminal generando un nuevo service con el CLI de Angular (`ng g s beer-data`) y ejecutando el proyecto junto a un backend con Docker Compose (contenedor de Postgres), ya conectado a un backend real. El carrito se resuelve típicamente manteniendo una lista de items seleccionados en un service compartido, con métodos para agregar/quitar productos y mostrar el total.
- **Keywords:** Angular, Carrito de compras, Service compartido, CLI de Angular (ng generate service), estado compartido entre componentes, Docker Compose, Postgres, integración backend-frontend.
- **Timestamps clave:** 0:00 Trabajo en terminal: generación de service (`ng g s beer-data`) y levantamiento del entorno con Docker Compose/Postgres.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir de la captura de terminal visible y el título del video.

### Angular - Services & Dependency Injection (Comunicando componentes)
- **Playlist:** Angular
- **URL:** https://www.youtube.com/watch?v=ZAEsr_qi6tU
- **Duración:** 47:40
- **Resumen:** Clase enfocada en cómo comunicar componentes entre sí en Angular usando Services e inyección de dependencias. Retoma el concepto de Service, ahora enfocado en que un mismo service (inyectado en varios componentes) permite compartir estado y lógica entre partes distintas de la aplicación sin acoplarlas directamente — la forma "correcta" en Angular de comunicar componentes sin relación padre-hijo directa, como alternativa a Inputs/Outputs.
- **Keywords:** Angular, Services, Dependency Injection, @Injectable, comunicación entre componentes, inyección de dependencias, estado compartido.
- **Timestamps clave:** 0:00 Introducción: Services + Dependency Injection para comunicar componentes.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título/diapositiva y el temario general de Angular.

### AngularJS - Deployment
- **Playlist:** Angular
- **URL:** https://www.youtube.com/watch?v=LWF72UQn4hI
- **Duración:** 25:12
- **Resumen:** Clase de cierre de la parte de Angular centrada en el despliegue a producción. Según la descripción oficial: "Deploy automático de una app Angular en Netlify y conexión con backend NestJS en Heroku". Cubre cómo publicar el frontend Angular (build de producción) en Netlify con despliegue automático, y cómo configurar esa app desplegada para consumir el backend NestJS en Heroku (URLs de producción, variables de entorno/CORS).
- **Keywords:** Angular, Deployment, Netlify, despliegue automático, NestJS, Heroku, build de producción, CORS, integración frontend-backend en producción.
- **Timestamps clave:** 0:00 Introducción al deploy; contenido centrado en Netlify (frontend) + Heroku (backend NestJS).
- **Nota:** resumen basado en la descripción oficial del video (detallada) y el temario general de la materia.

**Ojo:** el TP actual pide desplegar el backend en **Render**, no en Heroku (Heroku dejó de tener
plan gratuito). El flujo conceptual del video (build de producción + variables de entorno/CORS)
sigue aplicando, pero los pasos concretos de la plataforma van a diferir — usá
`references/docs-oficiales.md` o la documentación de Render para esa parte.

---

## Contenido Extra

### VS Code + Postman
- **Playlist:** Contenido Extra
- **URL:** https://www.youtube.com/watch?v=NS2niHufj5U
- **Duración:** 28:13
- **Resumen:** Clase de herramientas centrada en Visual Studio Code (editor de código: instalación, extensiones útiles para TypeScript/Angular/NestJS, atajos y configuración básica) y Postman (cliente para probar APIs REST manualmente: armar y enviar requests GET/POST/PUT/DELETE, ver respuestas, códigos de estado, headers y body), útil para verificar los endpoints del backend NestJS antes o en paralelo al desarrollo del frontend en Angular.
- **Keywords:** VS Code, Visual Studio Code, Postman, herramientas de desarrollo, testing de APIs REST, extensiones de VS Code, requests HTTP.
- **Timestamps clave:** 0:00 Introducción a VS Code y Postman como herramientas de trabajo.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título, la descripción y el uso típico de estas herramientas en un curso full-stack.

---

## Clases en Vivo

### Introducción a Tecnologías Web (clase en vivo)
- **Playlist:** Clases en Vivo
- **URL:** https://www.youtube.com/watch?v=27X_GzegoOk
- **Duración:** 38:47 (video "Unlisted")
- **Resumen:** Grabación de una clase en vivo de presentación/introducción de la materia. Como clase inaugural en formato en vivo, típicamente combina la presentación de la cursada (modalidad, cronograma, TP integrador) con una introducción conceptual a las tecnologías web (arquitectura cliente-servidor, stack de la materia: NestJS + Angular).
- **Keywords:** Introducción a Tecnologías Web, presentación de la materia, clase en vivo, cliente-servidor, stack NestJS + Angular.
- **Timestamps clave:** 0:00 Introducción a la materia y a la clase en vivo.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título y el formato típico de una clase en vivo introductoria.

### Tecnologías Web - Sistemas de Control de Versiones (clase en vivo)
- **Playlist:** Clases en Vivo
- **URL:** https://www.youtube.com/watch?v=a_tIVYlUEu4
- **Duración:** 1:13:40
- **Resumen:** Grabación de una clase en vivo dedicada a Sistemas de Control de Versiones (VCS), con foco práctico en Git y GitHub. Por su duración extensa, cubre probablemente tanto la teoría (qué es un VCS, por qué se usa, centralizado vs. distribuido) como la práctica con Git: comandos básicos (`git init`, `add`, `commit`, `push`, `pull`, `clone`), ramas, manejo de conflictos, y el flujo de trabajo con GitHub usado a lo largo de la materia para versionar el proyecto Brewery.
- **Keywords:** Sistemas de Control de Versiones, VCS, Git, GitHub, control de versiones distribuido, branches/ramas, commits, repositorios remotos.
- **Timestamps clave:** 0:00 Introducción a los sistemas de control de versiones y Git.
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título y el temario estándar de una clase de Git/GitHub.

### Introducción a Tecnologías Web 2023 (clase en vivo)
- **Playlist:** Clases en Vivo
- **URL:** https://www.youtube.com/watch?v=qp4LDVQY2IY
- **Duración:** 54:33 (video "Unlisted")
- **Resumen:** Grabación de la clase en vivo de presentación/introducción de la materia, edición 2023 (versión más reciente de la clase introductoria en vivo). Combina presentación de la cursada (modalidad, cronograma, TP integrador) con una introducción conceptual al desarrollo web moderno y al stack de la materia (NestJS + Angular).
- **Keywords:** Introducción a Tecnologías Web, 2023, presentación de la materia, clase en vivo, stack NestJS + Angular.
- **Timestamps clave:** 0:00 Introducción a la materia (edición 2023).
- **Nota:** transcript no disponible en esta sesión; resumen armado a partir del título y el formato típico de esta clase introductoria en vivo.

---

## Índice rápido por palabra clave

- **NestJS / framework backend:** Introducción a Nest Js, Controllers en Nest JS, Nest JS Providers & Services, Rest + Filtrado en Nest JS
- **Controllers / rutas HTTP:** Controllers en Nest JS
- **Services / Providers / inyección de dependencias (backend):** Nest JS Providers & Services
- **DTOs:** Nest JS Providers & Services
- **Angular / framework frontend:** Angular - Introducción, Angular - Components
- **Components / arquitectura Angular:** Angular - Components
- **TypeScript / interfaces:** Angular - Interfaces & Directivas
- **Directivas (*ngIf, *ngFor):** Angular - Interfaces & Directivas
- **Data Binding / Event Binding / ngModel:** Angular - Events and Binding
- **Routing (Angular):** Angular - Routing
- **HttpClient / consumo de API (Angular):** Angular - Rest, Angular - Rest Crear Recursos
- **Services & Dependency Injection (Angular):** Angular - Services & Dependency Injection
- **Docker Compose / Postgres:** Angular - Carrito de Compras
- **Deployment / Netlify / Heroku:** AngularJS - Deployment
- **REST (teoría):** Rest (Teóricas), Rest + Filtrado en Nest JS, Angular - Rest
- **MVC:** Model View Controller
- **HTML / CSS / JS (fundamentos):** Introducción a HTML, CSS y JS
- **Historia de la Web / cliente-servidor:** Introducción a la Web
- **Git / GitHub / control de versiones:** Introducción a Nest Js (mención), Tecnologías Web - Sistemas de Control de Versiones
- **VS Code / Postman:** VS Code + Postman
- **Presentación de la materia:** Introducción a Tecnologías Web (clase en vivo), Introducción a Tecnologías Web 2023 (clase en vivo)
