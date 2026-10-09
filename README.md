<div align="center">

<p align="center">
  <img src="assets/upc_logo.png" alt="logo" width="200"/>
</p>

<h3 align="center">
Universidad Peruana de Ciencias Aplicadas
</h3>

<h3 align="center">
Ingeniería de Software
<br><br>
1ASI0728 Arquitecturas de Software Emergentes
202620
<br><br>
NRC: 9046
<br><br>
Docente: Rojas Malasquez, Royer Edelwer
<br><br>
<strong>Informe de Trabajo Final</strong>  
<br><br>
Producto: Platter
<br><br>
Entrega: Segundo Hito - TP1 (Semana 7)
<br><br>
<br><br>
<strong>Integrantes</strong>  
<br><br>
Alvarado De La Cruz , Juan Carlos (U202216150) 
<br><br>
Duran Diaz, Antonio Rodrigo (U202215721)
<br><br>
Nakasone Gomes, Marco Antonio (U202210790)
<br><br>
Teves Samaniego, Joan Fernando (U202117303)
<br><br>
<br>

**Octubre - 2026**

</h3>
</div>

# Registro de Versiones del Informe

| Versión | Fecha | Autor(es) | Descripción de modificaciones |
| :---: | :---: | :--- | :--- |
| **1.0.0** | 19/09/2026 | Alvarado, Duran, Nakasone, Teves | Entrega inicial del Primer Hito (TB1). Incorporación de Carátula, Capítulo I (Startup Profile y Solution Profile con Lean UX), Capítulo II (Requirements Elicitation & Analysis con Needfinding y Lenguaje Ubicuo), Capítulo III (Requirements Specification con User Stories e Impact Mapping), Capítulo IV (Strategic-Level Software Design con ADD, DDD y C4 Model), Conclusiones iniciales, Bibliografía preliminar y sustento del Student Outcome ABET 3 para TB1. |
| **1.1.0** | 09/10/2026 | Alvarado, Duran, Nakasone, Teves | Entrega del Segundo Hito (TP1). Incorporación del Capítulo V (Tactical-Level Software Design con descomposición por capas, diagramas de componentes C4, diagramas de clases y diseño de base de datos para los cuatro Bounded Contexts) y Capítulo VI (Solution UX Design con guías de estilo visual, arquitectura de información, wireframes y mock-ups de Landing Page, y wireframes y diagramas de wireflow para aplicaciones móviles y WebAR). Actualización y avance de Conclusiones y Recomendaciones, ordenamiento formal de Bibliografía bajo estándar APA, y expansión acumulativa de la sección Student Outcome y Project Report Collaboration Insights para el hito TP1. |

# Project Report Collaboration Insights

El desarrollo y mantenimiento del presente informe técnico se gestiona de forma colaborativa y continua mediante un repositorio dedicado alojado en la organización oficial del equipo en GitHub:

- **Repositorio de Documentación (Reporte):** [https://github.com/upc-pre-1ASI0728-2620-9046-Platter/platter-report](https://github.com/upc-pre-1ASI0728-2620-9046-Platter/platter-report)
- **Repositorio de la Solución de Software:** [https://github.com/upc-pre-1ASI0728-2620-9046-Platter/platter](https://github.com/upc-pre-1ASI0728-2620-9046-Platter/platter)

### Metodología de Trabajo y Control de Versiones

Para asegurar la calidad técnica, la coherencia de notación y la trazabilidad del trabajo en equipo, se adoptó el flujo de trabajo GitFlow bajo los siguientes lineamientos:

1. **Estructura de Ramas:** La rama `main` custodia las versiones estables y formalmente auditadas correspondientes a cada hito evaluativo. La rama `develop` actúa como integradora de desarrollo del equipo. Cada capítulo y módulo de trabajo se desarrolló en ramas de características independientes (`feature/chapter-n` o `feature/tp1-final`).
2. **Convención de Commits:** Se aplicó la convención *Conventional Commits* (`docs:`, `feat:`, `refactor:`, `chore:`, `fix:`), garantizando un historial de cambios legible, granular y auditable.
3. **Revisión y Aprobación de Pull Requests:** La consolidación de artefactos hacia las ramas integradoras se ejecutó mediante Pull Requests revisados entre los integrantes, validando la sintaxis Markdown, la renderización de diagramas Mermaid y la integridad de los activos visuales alojados en el directorio `assets/`.

### Evidencias de Colaboración en GitHub

El equipo mantuvo una participación activa y equitativa en la redacción, diagramación y revisión de los artefactos del informe en ambas entregas (TB1 y TP1), registrando contribuciones continuas distribuidas entre todos los integrantes en las métricas de colaboración de GitHub:

- **Alvarado De La Cruz, Juan Carlos:** Liderazgo técnico en la especificación arquitectónica estratégica y táctica (Capítulos IV y V), estructuración de diagramas C4 y revisión de consistencia del modelo de dominio.
- **Duran Diaz, Antonio Rodrigo:** Elaboración de escenarios de atributos de calidad, especificación de persistencia de base de datos relacional y modelado de drivers arquitectónicos (Capítulos IV y V).
- **Nakasone Gomes, Marco Antonio:** Redacción del perfil de startup, antecedentes del sector, Lean UX, guías de estilo visual, arquitectura de información y diseño de interfaces comerciales y de usuario (Capítulos I y VI).
- **Teves Samaniego, Joan Fernando:** Especificación de requerimientos funcionales, historias de usuario Gherkin, diagramas de flujo de dominio y especificación de flujos de interacción de aplicaciones (Capítulos III y VI).

*(Las métricas consolidadas de frecuencia de código, commits y contribuyentes se encuentran auditables de manera transparente en la sección Insights del repositorio oficial).*

# Contenido

## Tabla de contenidos

- [Registro de versiones del informe](#registro-de-versiones-del-informe)
- [Project Report Collaboration Insights](#project-report-collaboration-insights)
- [Student Outcome](#student-outcome)
- [Capítulo I: Introducción](#capítulo-i-introducción)
  - [1.1. Startup Profile](#11-startup-profile)
    - [1.1.1. Descripción de la Startup](#111-descripción-de-la-startup)
    - [1.1.2. Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)
  - [1.2. Solution Profile](#12-solution-profile)
    - [1.2.1 Antecedentes y problemática](#121-antecedentes-y-problemática)
    - [1.2.2 Lean UX Process](#122-lean-ux-process)
  - [1.3. Segmentos objetivo](#13-segmentos-objetivo)
- [Capítulo II: Requirements Elicitation & Analysis](#capítulo-ii-requirements-elicitation--analysis)
  - [2.1. Competidores](#21-competidores)
  - [2.2. Entrevistas](#22-entrevistas)
  - [2.3. Needfinding](#23-needfinding)
  - [2.4. Big Picture EventStorming](#24-big-picture-eventstorming)
  - [2.5. Ubiquitous Language](#25-ubiquitous-language)
- [Capítulo III: Requirements Specification](#capítulo-iii-requirements-specification)
  - [3.1. To-Be Scenario Mapping](#31-to-be-scenario-mapping)
  - [3.2. User Stories](#32-user-stories)
  - [3.3. Impact Mapping](#33-impact-mapping)
  - [3.4. Product Backlog](#34-product-backlog)
- [Capítulo IV: Strategic-Level Software Design](#capítulo-iv-strategic-level-software-design)
  - [4.1. Strategic-Level Attribute-Driven Design](#41-strategic-level-attribute-driven-design)
  - [4.2. Strategic-Level Domain-Driven Design](#42-strategic-level-domain-driven-design)
  - [4.3. Software Architecture](#43-software-architecture)
- [Capítulo V: Tactical-Level Software Design](#capítulo-v-tactical-level-software-design)
  - [5.1. Bounded Context: Dish & Menu Catalog Management](#51-bounded-context-dish--menu-catalog-management)
  - [5.2. Bounded Context: AI Gastronomic Analysis](#52-bounded-context-ai-gastronomic-analysis)
  - [5.3. Bounded Context: AR Dining Experience](#53-bounded-context-ar-dining-experience)
  - [5.4. Bounded Context: Restaurant & Table Management](#54-bounded-context-restaurant--table-management)
- [Capítulo VI: Solution UX Design](#capítulo-vi-solution-ux-design)
  - [6.1. Style Guidelines](#61-style-guidelines)
    - [6.1.1. General Style Guidelines](#611-general-style-guidelines)
    - [6.1.2. Web, Mobile & Devices Style Guidelines](#612-web-mobile--devices-style-guidelines)
  - [6.2. Information Architecture](#62-information-architecture)
    - [6.2.1. Organization Systems](#621-organization-systems)
    - [6.2.2. Labeling Systems](#622-labeling-systems)
    - [6.2.3. Searching Systems](#623-searching-systems)
    - [6.2.4. SEO Tags, Meta Tags y ASO Elements](#624-seo-tags-meta-tags-y-aso-elements)
    - [6.2.5. Navigation Systems](#625-navigation-systems)
  - [6.3. Landing Page UI Design](#63-landing-page-ui-design)
    - [6.3.1. Landing Page Wireframe](#631-landing-page-wireframe)
    - [6.3.2. Landing Page Mock-up](#632-landing-page-mock-up)
  - [6.4. Applications UX/UI Design](#64-applications-uxui-design)
    - [6.4.1. Applications Wireframes](#641-applications-wireframes)
    - [6.4.2. Applications Wireflow Diagrams](#642-applications-wireflow-diagrams)
- [Conclusiones](#conclusiones)
- [Recomendaciones](#recomendaciones)
- [Bibliografía](#bibliografía)
- [Anexos](#anexos)

# Student Outcome

El curso contribuye al cumplimiento del Student Outcome ABET:

**ABET – EAC - Student Outcome 3**

**Criterio:** *Capacidad de comunicarse efectivamente con un rango de audiencias.*

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 3.

| Criterio específico | Acciones realizadas | Conclusiones |
| :--- | :--- | :--- |
| **Comunica oralmente sus ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerárquicos, en el marco del desarrollo de un proyecto en ingeniería.** | **Alvarado De La Cruz, Juan Carlos**<br>*TB1*<br>Expuse ante el equipo y en el video de sustentación los fundamentos de la descomposición estratégica bajo Domain-Driven Design (DDD), justificando la delimitación de Bounded Contexts y la implementación de una Capa Anticorrupción (ACL) para la integración con Google Gemini. Adapté el lenguaje técnico para comunicar claramente cómo la arquitectura soporta los requerimientos de negocio de restaurantes e inversionistas.<br>*TP1*<br>Sustenté ante el equipo y en las sesiones de revisión técnica las decisiones de diseño táctico para los Bounded Contexts de Catálogo y Análisis con IA, explicando con claridad la segregación en capas (Domain, Application, Infrastructure e Interfaces) y el uso de patrones de arquitectura hexagonal. Adapté la explicación técnica para justificar ante los evaluadores cómo el diseño por componentes desacopla los servicios y garantiza mantenibilidad a largo plazo.<br><br>**Duran Diaz, Antonio Rodrigo**<br>*TB1*<br>Participé activamente en las sesiones de discusión grupal y en la grabación del video de presentación de la entrega, explicando con objetividad los escenarios de atributos de calidad priorizados en Attribute-Driven Design (ADD) y cómo la infraestructura en la nube de AWS responde a las demandas de alta concurrencia en horas pico.<br>*TP1*<br>Presenté y argumenté de forma estructurada los diagramas de base de datos relacionales y el modelado de entidades de persistencia para los contextos de AR Dining Experience y Restaurant Management. Transmití con objetividad a los integrantes y docentes los criterios de normalización, llaves foráneas e índices seleccionados para asegurar tiempos de respuesta óptimos en consultas concurrentes.<br><br>**Nakasone Gomes, Marco Antonio**<br>*TB1*<br>Presenté oralmente en las reuniones de sincronización y en la exposición grabada los resultados del análisis de problemáticas del sector gastronómico y los supuestos de Lean UX, transmitiendo con claridad a perfiles tanto técnicos como de negocio el valor de la proyección en Realidad Aumentada sin fricción para el comensal.<br>*TP1*<br>Expuse en las reuniones de sincronización y preparación de la sustentación la propuesta integral de UX/UI, explicando con fundamentos el sistema de diseño (Material Design 3), las decisiones de la escala tipográfica y los contrastes cromáticos bajo WCAG 2.1 AA. Detallé con precisión el valor de negocio de los wireflows diseñados, demostrando cómo reducen la fricción cognitiva tanto para administradores de restaurante como para comensales.<br><br>**Teves Samaniego, Joan Fernando**<br>*TB1*<br>Expuse en el video grupal y en las reuniones técnicas los diagramas de interacción y flujo de mensajes mediante Domain Storytelling, describiendo detalladamente la secuencia técnica entre los clientes móviles, las APIs REST y los servicios en la nube de forma estructurada, fluida y comprensible para el equipo evaluador.<br>*TP1*<br>Expliqué oralmente en las sesiones de equipo la dinámica de navegación y los flujos de interacción entre pantallas de la aplicación móvil administrativa y el visor WebAR (WF-01 al WF-04). Articulé con claridad los escenarios alternativos de fallo (como latencia o indisponibilidad temporal de la IA) y su degradación elegante, facilitando la comprensión técnica de los flujos para perfiles de frontend y backend. | Durante el desarrollo del hito TB1, el equipo demostró capacidad para transmitir conceptos técnicos complejos de ingeniería de software a diversas audiencias. Se articularon con precisión técnica y pertinencia de negocio las decisiones de diseño estratégico, modelado de dominio y esquemas de infraestructura en la nube. A través de reuniones de retrospectiva internas y la sustentación en video, cada integrante adaptó su registro comunicativo para justificar de forma objetiva la viabilidad técnica y operativa de la solución ante evaluadores académicos y potenciales interesados del sector gastronómico.<br><br>Para el hito TP1, se consolidó la efectividad comunicativa oral al sustentar de manera integrada el diseño táctico por capas y la experiencia de usuario (UX/UI). Mediante reuniones técnicas de diseño y la preparación de la sustentación de hito, cada integrante demostró solvencia para defender alternativas arquitectónicas, justificar decisiones de persistencia relacional y argumentar elecciones de diseño visual frente a criterios de usabilidad, accesibilidad e impacto en el negocio gastronómico. |
| **Comunica en forma escrita ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerárquicos, en el marco del desarrollo de un proyecto en ingeniería.** | **Alvarado De La Cruz, Juan Carlos**<br>*TB1*<br>Redacté y consolidé los capítulos de diseño estratégico en Markdown, elaborando la especificación formal del Context Mapping y los diagramas C4 (Contexto, Contenedores y Despliegue). Cuidé la consistencia del lenguaje ubicuo del proyecto, documentando los contratos de integración y las decisiones arquitectónicas conforme al estándar de ingeniería solicitado.<br>*TP1*<br>Documenté formalmente en Markdown la especificación técnica de la arquitectura táctica de los Bounded Contexts Dish & Menu Catalog Management y AI Gastronomic Analysis, elaborando los diagramas C4 de nivel componente y los diagramas de clases del dominio. Mantuve una redacción rigurosa y libre de ambigüedades, asegurando la correspondencia exacta entre los contratos de dominio y el lenguaje ubicuo.<br><br>**Duran Diaz, Antonio Rodrigo**<br>*TB1*<br>Elaboré las especificaciones técnicas de los escenarios de calidad (Quality Attribute Scenarios) y el Backlog de Drivers Arquitectónicos, documentando de forma estructurada los requisitos de rendimiento, disponibilidad y escalabilidad, así como las tácticas arquitectónicas seleccionadas para mitigarlos.<br>*TP1*<br>Elaboré y documenté las especificaciones técnicas de persistencia del Capítulo V, diseñando los diagramas entidad-relación en Mermaid para cada Bounded Context y redactando las justificaciones técnicas de los esquemas relacionales, tipos de datos, llaves primarias e integridad referencial requerida por la solución.<br><br>**Nakasone Gomes, Marco Antonio**<br>*TB1*<br>Redacté la caracterización de la startup, la problemática del sector gastronómico, las declaraciones de problema de Lean UX, supuestos e hipótesis. Documenté los hallazgos en tablas y formatos estandarizados dentro del informe, facilitando la comprensión de los dolores del cliente tanto para perfiles de negocio como de desarrollo.<br>*TP1*<br>Redacté integralmente el Capítulo VI de Solution UX Design, documentando las guías de estilo generales (branding, tipografía, paleta accesible WCAG 2.1 AA y espaciados), la arquitectura de información (sistemas de organización, rotulado, búsqueda, navegación y metadatos SEO/ASO) y la justificación de los wireframes y mock-ups de la Landing Page comercial.<br><br>**Teves Samaniego, Joan Fernando**<br>*TB1*<br>Documenté la especificación formal de requerimientos mediante To-Be Scenario Mapping, User Stories bajo el formato Gherkin y los diagramas de secuencia de Domain Storytelling en Mermaid. Garanticé que la documentación escrita fuera rigurosa, no ambigua y completamente trazable con los objetivos del sistema.<br>*TP1*<br>Documenté las especificaciones de diseño UX de las aplicaciones (Platter Admin y Platter AR Viewer), elaborando las tablas de mapeo de pantallas hacia User Stories y la especificación detallada de los 4 diagramas de wireflow (happy path y flujos alternativos), asegurando trazabilidad directa con los requerimientos funcionales del Capítulo III. | La redacción colaborativa del informe técnico en GitHub bajo estándares de Markdown y conventional commits permitió consolidar un cuerpo documental riguroso, coherente y profesional. Se logró comunicar con claridad el análisis del problema, los modelos formales de dominio y las decisiones de arquitectura de software, empleando notaciones estándar (C4 Model, diagramas UML/secuencia y plantillas Lean UX). El producto escrito evidencia objetividad técnica y una estructura que satisface las exigencias metodológicas del curso y de la práctica profesional de la ingeniería de software.<br><br>En el hito TP1, esta capacidad escrita se fortaleció al integrar especificaciones formales de arquitectura de software a nivel táctico (diagramas de clases y esquemas de base de datos detallados) junto con especificaciones exhaustivas de diseño UX/UI (guías de estilo, metadatos SEO y flujos de pantallas vinculados a historias de usuario). La documentación escrita resultante mantiene uniformidad estilística, rigor técnico y plena trazabilidad metodológica, satisfaciendo los criterios de calidad académica y profesional exigidos por el estándar ABET. |

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

<div style="text-align: justify">
Platter es una startup dedicada al desarrollo de soluciones tecnológicas para el sector gastronómico, enfocada en cerrar la brecha entre lo que un comensal observa en la carta de un restaurante y lo que finalmente recibe en su mesa. La propuesta de valor de la startup se centra en permitir que los clientes de un restaurante visualicen, mediante Realidad Aumentada (AR), una representación tridimensional a escala real del plato que están por ordenar, directamente desde la cámara del navegador de su propio dispositivo móvil, sin necesidad de instalar una aplicación adicional.
 
La solución integra cuatro pilares tecnológicos que sustentan su propuesta de transformación digital para el sector: una aplicación móvil de gestión dirigida al restaurante, un componente de Realidad Extendida (WebAR) dirigido al comensal, un módulo de Inteligencia Artificial que analiza fotografías de los platos para autocompletar información gastronómica relevante (nombre, descripción, ingredientes, alérgenos y calorías estimadas), y una arquitectura de backend/BaaS que centraliza el registro de platos, los modelos tridimensionales asociados y los códigos QR que enlazan ambos mundos.
 
La misión de Platter es reducir la incertidumbre del comensal al momento de decidir su pedido y, con ello, mejorar la satisfacción del cliente y la eficiencia operativa de los restaurantes que adoptan la plataforma. La visión de la startup es convertirse en la herramienta de referencia para la digitalización de cartas gastronómicas en restaurantes pequeños y medianos de Perú y Latinoamérica, ampliando progresivamente sus capacidades hacia otros formatos de experiencia inmersiva para el sector food service.
 
Platter se posiciona como una alternativa accesible frente a soluciones de digitalización de menús que se limitan a listados de texto o fotografías estáticas, diferenciándose mediante la incorporación de Realidad Aumentada activada por un simple escaneo de código QR y la automatización del proceso de carga de información gastronómica mediante Inteligencia Artificial, lo que reduce la carga operativa que históricamente ha desincentivado a los restaurantes pequeños a mantener actualizada su carta digital.
 
</div>

### 1.1.2. Perfiles de integrantes del equipo

| Integrante | Descripción de Carrera | Conocimientos y Habilidades a aportar |
| --------------------------------| ----------------------| ------------------------------------ |
| ![Juan Carlos](./assets/foto-juan.jpeg) <br> Alvarado De La Cruz, Juan Carlos | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Soy estudiante de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Cuento con experiencia en el diseño arquitectónico de software bajo el C4 Model, modelado estratégico con Domain-Driven Design (DDD) y desarrollo backend con Spring Boot y bases de datos relacionales. En este proyecto mi meta es articular e implementar la comunicación desacoplada entre los Bounded Contexts, liderar las buenas prácticas de arquitectura y asegurar que cumplamos los estándares técnicos y plazos del equipo. |
| ![Antonio Rodrigo](./assets/foto-rodrigo.png) <br> Duran Diaz, Antonio Rodrigo | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Soy estudiante de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Me enfoco principalmente en el desarrollo de servicios backend y la gestión de infraestructura en la nube. Cuento con conocimientos en Java, SQL y diseño de APIs RESTful. Mi propósito en el equipo es implementar la lógica de negocio de los servicios centrales, asegurar la correcta persistencia y disponibilidad de los datos, y aportar activamente al cumplimiento de las metas en cada entrega. |
| ![Marco Antonio](./assets/foto-marco.png) <br> Nakasone Gomes, Marco Antonio | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Tengo 22 años y me encuentro cursando el noveno ciclo de la carrera de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Me caracterizo por mi capacidad para el trabajo colaborativo, la organización y el cumplimiento puntual de tareas. En este proyecto busco aportar en el diseño de interfaces web, la integración de servicios externos y la optimización de flujos de interacción, proponiendo soluciones prácticas que eleven la calidad de la solución. |
| ![Joan Fernando](./assets/foto-joan.jpeg) <br> Teves Samaniego, Joan Fernando | Ingeniería de Software <br>Universidad Peruana de Ciencias Aplicadas | Soy estudiante de Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Cuento con conocimientos en programación orientada a objetos, despliegue de aplicaciones en contenedores Docker y control de versiones con GitFlow. Mi objetivo en el proyecto es colaborar estrechamente en la construcción de endpoints resilientes, apoyar en la configuración de los entornos de despliegue y asegurar una integración fluida entre los módulos de software y las pruebas. |


## 1.2. Solution Profile

### 1.2.1 Antecedentes y problemática

<div style="text-align: justify">
El sector gastronómico peruano constituye uno de los ejes económicos más relevantes del país, tanto por su aporte a la generación de empleo como por su peso simbólico dentro de la identidad nacional. Este sector está compuesto mayoritariamente por micro y pequeños negocios: cerca del 99.9% de las empresas formales del rubro de restaurantes y afines en el Perú son micro y pequeñas empresas (Mype) (Produce, citado por Andina, 2020). Esta atomización del mercado implica que la mayoría de restaurantes no cuenta con presupuestos ni equipos de tecnología propios para digitalizar su operación, lo que limita su capacidad de adoptar herramientas modernas de interacción con el cliente.
 
El proceso de decisión de compra de un comensal se apoya casi exclusivamente en la carta del restaurante, ya sea física o digital, que en la gran mayoría de los casos se limita a texto descriptivo y, en el mejor de los casos, a una fotografía estática del plato. Esta representación bidimensional no logra comunicar con precisión el tamaño real de la porción, la disposición de los ingredientes ni la presentación final del plato, generando una brecha entre la expectativa que se forma el comensal y la realidad que recibe en su mesa. A nivel de comercio electrónico, esta misma brecha entre expectativa y producto recibido explica en gran medida las tasas de devolución de 20% a 30% que enfrentan categorías como indumentaria y mobiliario, donde el cliente no puede experimentar el producto antes de comprarlo (Ecosire, 2024).
 
La Realidad Aumentada ha demostrado ser una tecnología efectiva para cerrar esta brecha en otros sectores del retail: estudios reportados por Shopify indican que los compradores que utilizan visualización de productos en AR convierten entre 2 y 3 veces más que quienes no la utilizan, mientras que las tasas de devolución de productos con experiencias de visualización en AR disminuyen entre 25% y 40% (Ecosire, 2024; ARInsider, 2020). Sin embargo, esta tecnología ha sido adoptada principalmente por categorías como moda, mobiliario y belleza, y su aplicación específica al sector de servicios de alimentos —donde el "producto" es perecible, se prepara bajo pedido y no puede probarse físicamente antes de decidir— permanece prácticamente inexplorada en el mercado local.
 
Adicionalmente, el sector restaurantero peruano atraviesa un contexto de contracción reciente: se reporta que existen alrededor de 50,000 restaurantes menos en el país en comparación con el año 2019 (Gestión, 2024), lo que incrementa la presión competitiva sobre los negocios que permanecen activos y refuerza la necesidad de herramientas que les permitan diferenciarse y mejorar la experiencia que ofrecen a sus clientes sin incurrir en inversiones tecnológicas complejas o costosas.
 
</div>

### Problemática
 
<div style="text-align: justify">
Para comprender la necesidad del proyecto, se aplicó la técnica de las 5W's + 2H's:
 
### 5W's
 
### What (¿Cuál es el problema?):
 
Los comensales que visitan un restaurante o revisan su carta digital no cuentan con una forma confiable de anticipar cómo lucirá realmente el plato que están por ordenar, lo que genera indecisión al momento de elegir, expectativas no cumplidas al recibir el pedido y, en algunos casos, insatisfacción o devolución del plato.
 
Por su parte, los dueños y administradores de restaurantes no cuentan con herramientas accesibles para digitalizar su carta de forma atractiva y diferenciada, ni con procesos ágiles para mantener actualizada la información gastronómica (ingredientes, alérgenos, información nutricional) de cada plato, ya que su actualización manual demanda tiempo del que usualmente no disponen.
 
### When (¿Cuándo ocurre el problema?):
 
El problema del comensal ocurre en el momento exacto de decisión de compra, cuando revisa la carta física o digital del restaurante y debe elegir un plato basándose únicamente en una descripción textual o, en el mejor de los casos, en una fotografía que no refleja el tamaño real ni la disposición final del plato servido.
 
El problema del restaurante ocurre de forma recurrente cada vez que incorpora un plato nuevo a su carta o modifica uno existente, momento en el cual debe redactar manualmente la descripción, identificar ingredientes y alérgenos, y —si desea ofrecer una experiencia visual más rica— gestionar por separado la fotografía y cualquier material adicional, sin contar con herramientas que integren estos procesos.
 
### Where (¿Dónde ocurre el problema?):
 
En el punto de venta del restaurante, ya sea en el salón al momento de revisar la carta física, o en canales digitales (redes sociales, aplicaciones de delivery, página web) cuando el comensal explora el menú antes de decidir su pedido.
 
En el back-office del restaurante, donde el personal administrativo o los propios dueños gestionan manualmente la actualización de la carta, típicamente mediante documentos de texto, hojas de cálculo o publicaciones sueltas en redes sociales, sin un sistema centralizado que integre contenido visual enriquecido.
 
### Who (¿A quién o quiénes afecta el problema?):
 
- A los comensales, quienes enfrentan incertidumbre al momento de decidir su pedido y riesgo de recibir un plato que no coincide con lo que imaginaban, afectando su satisfacción con la experiencia del restaurante.
- A los dueños y administradores de restaurantes, especialmente de micro y pequeños negocios, quienes no cuentan con tiempo, presupuesto ni conocimiento técnico para digitalizar su carta con contenido visual enriquecido y mantenerla actualizada de forma ágil.
- De forma indirecta, al personal de sala (meseros), quienes deben invertir tiempo adicional explicando verbalmente el contenido y la presentación de los platos ante la falta de una referencia visual clara para el cliente.
### Why (¿Por qué sucede el problema?):
 
Porque la mayoría de restaurantes, especialmente los de menor tamaño, gestionan su carta de forma manual y con herramientas genéricas (documentos de texto, redes sociales, fotografías sueltas) que no están diseñadas para comunicar de forma inmersiva el contenido de un plato.
 
Al no existir una plataforma accesible que combine generación automática de contenido gastronómico con visualización en Realidad Aumentada, los restaurantes pequeños quedan al margen de una tecnología que en otros sectores del retail ya ha demostrado mejorar la conversión y reducir la insatisfacción del cliente.
 
### 2H's
 
### How (¿Cómo aparece el problema?):
 
Los restaurantes suelen publicar sus platos con descripciones breves y, en el mejor de los casos, una fotografía tomada sin estándares de calidad, careciendo de un proceso que les permita generar de forma rápida información gastronómica completa (ingredientes, alérgenos, calorías) y una representación tridimensional del plato para brindar mayor confianza al comensal.
 
Por su parte, los comensales dependen de su propia interpretación de un texto o una imagen plana para imaginar cómo lucirá el plato, lo que genera una desconexión entre expectativa y realidad que solo se resuelve —para bien o para mal— una vez que el plato llega a la mesa.
 
### How Much (¿Cuánto afecta el problema?):
 
El impacto es relevante tanto para el negocio como para la experiencia del cliente:
 
- Para los restaurantes, un comensal insatisfecho con la presentación o el tamaño del plato recibido representa un riesgo directo de reseñas negativas, menor probabilidad de recompra y pérdida de recomendaciones boca a boca, en un sector donde la reputación digital incide directamente en la afluencia de nuevos clientes.
- Para el sector en su conjunto, la falta de diferenciación digital entre restaurantes pequeños limita su capacidad de competir frente a cadenas más grandes que sí cuentan con presupuesto para marketing visual y experiencias digitales more elaboradas, en un contexto donde el número de restaurantes activos en el país ya se ha reducido significativamente en los últimos años (Gestión, 2024).
</div>

### 1.2.2 Lean UX Process.

#### 1.2.2.1. Lean UX Problem Statements.

<div style="text-align: justify">
El estado actual de la digitalización de cartas gastronómicas en restaurantes pequeños y medianos se ha centrado principalmente en descripciones textuales y fotografías estáticas, gestionadas de forma manual y desconectada entre el contenido informativo del plato y su representación visual. Esto genera indecisión y expectativas no cumplidas en los comensales, además de una carga operativa elevada para los restaurantes al momento de mantener su carta actualizada y atractiva.
 
Lo que los productos y servicios existentes no abordan es la necesidad de una solución accesible que permita a los restaurantes generar de forma ágil contenido gastronómico completo a partir de una simple fotografía, y que además ofrezca al comensal una experiencia de visualización inmersiva del plato a escala real, sin fricción de instalación y accesible desde cualquier smartphone mediante el escaneo de un código QR.
 
Nuestro producto, Platter, abordará esta brecha mediante una plataforma que combina una aplicación móvil de gestión para el restaurante, un módulo de Inteligencia Artificial que analiza la fotografía del plato para autocompletar nombre, descripción, ingredientes, alérgenos y calorías estimadas, un visor de Realidad Aumentada (WebAR) accesible mediante código QR que proyecta el plato en 3D a escala real sobre la mesa del comensal, y un backend que centraliza el registro de platos, modelos tridimensionales y códigos QR asociados.
 
Nuestro enfoque inicial será restaurantes pequeños y medianos en Lima, Perú, que buscan diferenciarse mediante una experiencia digital innovadora sin incurrir en costos elevados de desarrollo tecnológico propio, junto con sus comensales como usuarios finales de la experiencia de Realidad Aumentada.
 
Sabremos que tenemos éxito cuando veamos que al menos el 70% de los comensales que utilicen el visor WebAR reporten mayor confianza en su decisión de compra, y que los restaurantes que adopten la plataforma reduzcan en al menos 30% el tiempo que dedican a registrar y actualizar la información de cada plato en su carta.
 
</div>

#### 1.2.2.2. Lean UX Assumptions.

**Business Assumptions:**
 
1. Nuestros clientes (restaurantes) necesitan una forma más eficiente y atractiva de comunicar el contenido de sus platos a los comensales, sin depender de procesos manuales de redacción y fotografía.
2. Pensamos que estas necesidades pueden resolverse con una plataforma que combine una aplicación móvil de gestión, análisis de fotografías con Inteligencia Artificial y un visor de Realidad Aumentada accesible mediante código QR.
3. Nuestros clientes iniciales serán restaurantes pequeños y medianos en Lima, Perú, que buscan diferenciarse de su competencia mediante innovación en la experiencia del comensal.
4. El valor principal para los restaurantes será reducir el tiempo de gestión de su carta y diferenciarse visualmente frente a la competencia; para los comensales, será tomar decisiones de compra con mayor confianza y menor incertidumbre.
5. Captaremos clientes mediante demostraciones directas a dueños de restaurantes, alianzas con asociaciones gastronómicas y estrategias de marketing digital dirigidas al sector food service.
6. Generaremos ingresos con un modelo de suscripción mensual por restaurante, escalado según el número de platos registrados en la plataforma.
7. La competencia serán plataformas genéricas de menú digital y códigos QR estáticos, pero nos destacaremos por la incorporación de Realidad Aumentada y automatización mediante Inteligencia Artificial.
8. El mayor riesgo es la resistencia al cambio por parte de restaurantes con poca familiaridad tecnológica, que mitigaremos con un proceso de carga de platos simple, asistido por IA, y con soporte de onboarding personalizado.
9. Reconocemos que si los restaurantes no perciben un retorno claro sobre la inversión en la suscripción, el proyecto podría fracasar, por lo que validaremos su aceptación desde etapas tempranas mediante pilotos gratuitos.
**User Assumptions:**
 
1. Nuestros usuarios serán dueños y administradores de restaurantes, además de los comensales que visitan dichos restaurantes.
2. Nuestro producto encajará en el proceso diario de actualización de carta del restaurante y en el momento de decisión de compra del comensal previo a realizar su pedido.
3. Nuestro producto resolverá la incertidumbre del comensal sobre la presentación real de un plato y la carga operativa del restaurante al generar contenido gastronómico y visual para su carta.
4. Nuestro producto se usará de forma constante por parte del restaurante al incorporar nuevos platos a su carta, y de forma puntual por parte del comensal cada vez que visite el restaurante y escanee un código QR.
5. Las características más importantes serán la rapidez del análisis por Inteligencia Artificial, la fidelidad de la visualización en Realidad Aumentada y la facilidad para generar y compartir el código QR.
6. Nuestro producto deberá verse simple, confiable y no requerir instalación alguna para el comensal, y ser intuitivo para restaurantes con poca experiencia tecnológica previa.
**Business Outcome Assumptions:**
 
- Incrementar la diferenciación competitiva de los restaurantes que adoptan la plataforma frente a negocios que mantienen cartas tradicionales sin contenido visual enriquecido.
- Reducir el tiempo operativo que los restaurantes destinan a la redacción y actualización de la información de cada plato en su carta.
- Mejorar la satisfacción y confianza del comensal en su decisión de compra, reduciendo la brecha entre expectativa y producto recibido.
- Incrementar la recurrencia de visitas y la probabilidad de recomendación de los restaurantes que ofrecen la experiencia de Realidad Aumentada.
**User Outcome Assumptions:**
 
- Los restaurantes podrán registrar nuevos platos en su carta de forma más rápida, gracias al autocompletado de información mediante Inteligencia Artificial.
- Los comensales podrán visualizar el plato que están por ordenar en tamaño real sobre su propia mesa, reduciendo la incertidumbre al momento de decidir su pedido.
- La integración de información gastronómica automatizada (ingredientes, alérgenos, calorías) permitirá a los comensales con restricciones alimentarias tomar decisiones más informadas y seguras.
**Features:**
 
- Implementar un módulo de análisis de fotografías con Inteligencia Artificial (Gemini Vision) que autocomplete nombre, descripción, ingredientes, alérgenos y calorías estimadas del plato.
- Desarrollar un visor de Realidad Aumentada (WebAR) accesible mediante código QR, que proyecte el modelo 3D del plato a escala real sobre una superficie horizontal, sin necesidad de instalar una aplicación.
- Crear una aplicación móvil de gestión para el restaurante que permita registrar platos, asociar modelos 3D y generar códigos QR dinámicos.
- Incorporar un mecanismo de asignación automática de modelos 3D de muestra cuando el restaurante no cuente con un modelo propio del plato.

#### 1.2.2.3. Lean UX Hypothesis Statements.

Para la elaboración de los Hypothesis Statements, se empleó la plantilla recomendada por Lean UX:
 
We believe that [business outcome] will be achieved if [user] attains [benefit] with [feature].
 
#### Hipótesis 1
 
**Creemos que** la reducción del tiempo de gestión de la carta digital **se logrará si** los dueños y administradores de restaurantes **obtienen** información gastronómica completa de cada plato de forma automática **con** una funcionalidad de análisis de fotografías mediante Inteligencia Artificial.
 
#### Hipótesis 2
 
**Creemos que** el incremento en la confianza de los comensales al momento de decidir su pedido **se logrará si** los comensales **obtienen** una visualización realista del plato a escala real sobre su mesa **con** un visor de Realidad Aumentada (WebAR) accesible mediante código QR, sin necesidad de instalar una aplicación.
 
#### Hipótesis 3
 
**Creemos que** la diferenciación competitiva de los restaurantes que adoptan la plataforma **se logrará si** los dueños de restaurantes **obtienen** una carta digital enriquecida con Realidad Aumentada **con** un generador de códigos QR dinámico asociado a cada plato registrado.
 
#### Hipótesis 4
 
**Creemos que** la reducción de la insatisfacción por expectativas no cumplidas **se logrará si** los comensales **obtienen** información clara y anticipada sobre alérgenos e ingredientes del plato **con** una funcionalidad de detección automática de alérgenos basada en el análisis de la fotografía del plato.
 
#### Hipótesis 5
 
**Creemos que** el aumento en la adopción de la plataforma por restaurantes sin modelos 3D propios **se logrará si** los dueños de restaurantes **obtienen** una representación tridimensional del plato sin necesidad de contratar servicios de modelado 3D **con** una funcionalidad de asignación automática de modelos 3D de muestra basada en el análisis de la fotografía.
 
#### Hipótesis 6
 
**Creemos que** la mejora en la eficiencia del proceso de atención en sala **se logrará si** el personal de sala (meseros) **obtiene** una herramienta visual de apoyo para resolver dudas del comensal sobre el contenido y presentación del plato **con** la posibilidad de abrir el visor de Realidad Aumentada directamente desde la aplicación móvil de gestión durante la toma del pedido.

#### 1.2.2.4. Lean UX Canvas.

| **Business Problem** | **Solutions** | **Business Outcomes** |
|---|---|---|
| Los comensales no cuentan con una forma confiable de anticipar cómo lucirá el plato que están por ordenar, lo que genera indecisión y expectativas no cumplidas. <br> Los restaurantes, especialmente los pequeños y medianos, no cuentan con herramientas accesibles para generar contenido gastronómico completo ni para ofrecer una experiencia visual diferenciada en su carta, debido a procesos manuales que consumen tiempo y conocimiento técnico del que usualmente no disponen. | - Implementación de un módulo de análisis de fotografías con Inteligencia Artificial que autocomplete información gastronómica del plato.<br>- Desarrollo de un visor de Realidad Aumentada (WebAR) accesible por código QR, sin instalación, con proyección del modelo 3D a escala real.<br>- Aplicación móvil de gestión para que el restaurante registre platos, asocie modelos 3D y genere códigos QR dinámicos. | - Incremento en la confianza de los comensales al decidir su pedido.<br>- Reducción del tiempo operativo de los restaurantes para actualizar su carta.<br>- Mayor diferenciación competitiva frente a restaurantes con cartas tradicionales.<br>- Incremento en la recurrencia y recomendación de los restaurantes que adoptan la plataforma. |
 
| **Users and Customer** | | **User Outcomes & Benefits** |
|---|---|---|
| Dueños y administradores de restaurantes: registran platos en la aplicación móvil, cargan una fotografía y aprovechan el autocompletado con Inteligencia Artificial para generar descripción, ingredientes, alérgenos y calorías, además de generar el código QR asociado. <br> Comensales: escanean el código QR ubicado en la carta física o digital del restaurante y visualizan el plato en Realidad Aumentada, a escala real, sobre su propia mesa, directamente desde el navegador de su dispositivo móvil. | | - Los restaurantes podrán reducir el tiempo dedicado a la gestión de su carta gracias a la automatización con Inteligencia Artificial.<br>- Los comensales podrán tomar decisiones de compra más informadas y con mayor confianza al visualizar el plato antes de ordenarlo.<br>- Ambas partes mejorarán su experiencia de interacción, fortaleciendo la satisfacción del comensal y la reputación del restaurante. |
 
| **Hypotheses** | **What's the most important thing we need to learn first?** | **What's the least amount of work we need to do to learn the next most important thing?** |
|---|---|---|
| - Los restaurantes reducirán significativamente el tiempo dedicado a la gestión de su carta gracias al autocompletado de información mediante Inteligencia Artificial, lo que aumentará la probabilidad de adopción y uso continuo de la plataforma.<br>- Los comensales incrementarán su confianza en la decisión de compra al visualizar el plato en Realidad Aumentada antes de ordenarlo, lo que se traducirá en mayor satisfacción y menor tasa de reclamos por expectativas no cumplidas.<br>- Una plataforma que integre generación automática de contenido gastronómico, Realidad Aumentada y generación de códigos QR aportará valor tanto a restaurantes como a comensales, fortaleciendo la relación entre ambos y diferenciando a los restaurantes que la adopten. | Lo más importante que se necesita aprender primero es si los comensales realmente valoran la visualización del plato en Realidad Aumentada al punto de que influya en su decisión de compra o en su percepción de confianza hacia el restaurante. Validar esta percepción es crítico porque si los comensales no encuentran valor en la experiencia AR, el resto de funcionalidades (gestión con IA, generación de QR, panel administrativo) pierde relevancia como propuesta diferenciadora. | - Desarrollar un prototipo funcional del visor WebAR con un número reducido de platos de muestra y probarlo con comensales reales escaneando un código QR en un restaurante piloto.<br>- Crear un flujo mínimo de registro de plato con análisis de Inteligencia Artificial y medir si los dueños de restaurante perciben ahorro de tiempo frente a su proceso actual.<br>- Realizar una prueba comparativa simple entre una carta tradicional y una carta con Realidad Aumentada, midiendo percepción de confianza del comensal.<br>- MVP enfocado en el visor WebAR y el registro básico de platos para validar adopción temprana antes de desarrollar funcionalidades adicionales. |

## 1.3. Segmentos objetivo.

### Segmento 1: Dueños y administradores de restaurantes
 
- **Descripción:** Este segmento está conformado por propietarios y administradores de restaurantes pequeños y medianos, principalmente del rubro de comida criolla, pollerías, cevicherías y restaurantes de especialidades, que gestionan directamente el contenido de su carta gastronómica. Utilizan la aplicación móvil de Platter para registrar platos, cargar fotografías, revisar y ajustar la información sugerida por la Inteligencia Artificial, asociar modelos 3D y generar los códigos QR que se incorporan a su carta física o digital.
- **Sexo:** Masculino y femenino
- **Edades:** Adultos jóvenes (25-40 años) y adultos de mediana edad (41-55 años)
- **Nivel socioeconómico:** Principalmente clases B y C (media-alta y media)
- **Necesidades:** Diferenciarse de la competencia mediante una experiencia de carta más atractiva, reducir el tiempo dedicado a la redacción manual de la información de cada plato, y mejorar la satisfacción de sus comensales sin incurrir en inversiones tecnológicas complejas. Cerca del 99.9% de las empresas formales del sector Restaurantes y afines en el Perú son micro y pequeñas empresas (Produce, citado por Andina, 2020), lo que confirma que este segmento opera mayoritariamente con recursos y presupuestos tecnológicos limitados.
### Segmento 2: Comensales de restaurante
 
- **Descripción:** Este segmento está conformado por clientes que visitan un restaurante de forma presencial y utilizan su propio smartphone para escanear el código QR disponible en la carta, accediendo así al visor de Realidad Aumentada de Platter sin necesidad de instalar ninguna aplicación. Buscan tomar una decisión de compra más informada, visualizando el plato en 3D y a escala real antes de confirmar su pedido, y revisando la información de ingredientes y alérgenos autogenerada por la plataforma.
- **Sexo:** Masculino y femenino
- **Edades:** Jóvenes (18-30 años) y adultos jóvenes (31-45 años), segmento con alta familiaridad en el uso de smartphones y disposición a interactuar con experiencias digitales nuevas durante su consumo diario
- **Nivel socioeconómico:** Principalmente clases B y C (media-alta y media), consumidores habituales de restaurantes de comida casual y de especialidades en zonas urbanas
- **Necesidades:** Reducir la incertidumbre al momento de elegir un plato, contar con información confiable sobre ingredientes y alérgenos para quienes tienen restricciones alimentarias, y disfrutar de una experiencia de consumo más informada e interactiva. La adopción de Realidad Aumentada en procesos de decisión de compra ha demostrado mejorar la conversión entre 2 y 3 veces frente a la ausencia de visualización en AR en otros sectores del retail (Ecosire, 2024), lo que sustenta el valor potencial de esta experiencia también en el sector gastronómico.

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores.

<table border="1px">
    <thead>
        <th colspan="11">Competitive Analysis Landscape</th>
    </thead>
    <tbody>
        <tr>
            <td rowspan="2" colspan="2">¿Por qué llevar a
                cabo este análisis?</td>
        </tr>
        <tr>
            <td colspan="9">El objetivo de este análisis es comprender el funcionamiento, el enfoque de mercado y las características de los productos ofrecidos por competidores en el sector de digitalización de menús de restaurante y visualización de productos mediante Realidad Aumentada. Esto permitirá planificar estrategias que resalten las fortalezas de Platter y aprovechen las debilidades de las soluciones actuales en el mercado.</td>
        </tr>
        <tr>
            <tr>
                <td colspan="3"></td>
                <td colspan="2"><img src="/imagenes/Logo.png" style="width: 60px; height: auto;"><br>Platter</td>
                <td colspan="2"><img src="/imagenes/competidor-1.png" style="width: 60px; height: auto;"><br>ARmenu</td>
                <td colspan="2"><img src="/imagenes/competidor-2.png" style="width: 60px; height: auto;"><br>Menu3</td>
                <td colspan="2"><img src="/imagenes/competidor-3.png" style="width: 60px; height: auto;"><br>Onirix</td>
            </tr>
        </tr>
        <tr>
            <td rowspan="2" colspan="1">Perfil</td>
            <td colspan="2">Overview</td>
            <td colspan="2">Plataforma que digitaliza la carta de restaurantes combinando Inteligencia Artificial (Gemini Vision) y Realidad Aumentada. El restaurante registra un plato mediante una aplicación móvil, sube una fotografía y la IA autocompleta nombre, descripción, ingredientes, alérgenos y calorías; el modelo 3D se asigna automáticamente desde una biblioteca de muestra si el restaurante no cuenta con uno propio. El comensal accede al plato en Realidad Aumentada escaneando un código QR desde la cámara de su celular, sin instalar ninguna aplicación.</td>
            <td colspan="2">Plataforma británica que convierte fotografías de platos en modelos 3D fotorrealistas mediante fotogrametría (Apple Object Capture). El restaurante envía de 20 a 30 fotografías por plato y recibe, en 48 horas, un modelo 3D alojado en un CDN junto con un código QR imprimible que activa la visualización en WebAR desde el navegador del comensal, sin instalar aplicación.</td>
            <td colspan="2">Aplicación pionera de AR para menús, nacida como proyecto estudiantil en la Universidad de Illinois (EE. UU.). El comensal descarga una aplicación nativa (iOS/Android) y apunta la cámara hacia un marcador físico colocado en la mesa para visualizar el menú en 3D. Los modelos son generados por el propio equipo de Menu3 a partir de fotografías enviadas por el restaurante.</td>
            <td colspan="2">Plataforma española de WebAR de propósito general, con casos de uso en retail y restauración. Su caso más visible es la cadena La Tagliatella, que utiliza códigos QR individuales por plato para que el comensal visualice cada producto en Realidad Aumentada desde el navegador, sin instalar aplicación. Los modelos 3D son generados por el equipo de Onirix a solicitud del cliente.</td>
        </tr>
        <tr>
            <td colspan="2">Ventaja competitiva <br/> ¿Qué valor ofrece a los clientes?</td>
            <td colspan="2">Combina automatización con IA para reducir el tiempo y costo de registrar un plato (no requiere sesión fotográfica profesional ni fotogrametría), con una experiencia de Realidad Aumentada 100% libre de instalación para el comensal. Su valor adicional está en la generación automática de información de alérgenos y calorías, inexistente en los competidores analizados, y en un enfoque de mercado desatendido: restaurantes pequeños y medianos de Perú y Latinoamérica.</td>
            <td colspan="2">Su ventaja está en el fotorrealismo del modelo 3D obtenido por fotogrametría y en un tiempo de entrega rápido y predecible (48 horas). Aporta valor a restaurantes de gama media-alta que buscan una representación visual de máxima fidelidad de sus platos insignia.</td>
            <td colspan="2">Su ventaja fue ser de los primeros en demostrar que la Realidad Aumentada puede reducir la brecha entre expectativa y realidad en un plato. Aporta valor al dar una vista 3D rotable del menú completo dentro de una sola aplicación.</td>
            <td colspan="2">Su ventaja está en ser una plataforma de WebAR robusta y ya validada con cadenas de restauración de tamaño medio/grande, ofreciendo una implementación de Realidad Aumentada confiable sin necesidad de instalar aplicación.</td>
        </tr>
        <tr>
            <td rowspan="2" colspan="1">Perfil de Marketing</td>
            <td colspan="2">Mercado Objetivo</td>
            <td colspan="2">Dueños y administradores de restaurantes pequeños y medianos (pollerías, cevicherías, restaurantes de comida criolla y de especialidades) en Lima, Perú, en su fase inicial, con proyección de expansión a otras ciudades y países de Latinoamérica.</td>
            <td colspan="2">Restaurantes de gama media-alta en el Reino Unido, con especial tracción en cocinas premium o poco familiares para el comensal local (india, pakistaní, japonesa, alta cocina).</td>
            <td colspan="2">Restaurantes ubicados en un campus universitario en Champaign-Urbana, Illinois (EE. UU.), como mercado piloto; sin evidencia de expansión comercial posterior.</td>
            <td colspan="2">Cadenas de restauración medianas y grandes en España y Europa, dentro de una oferta más amplia de WebAR para retail.</td>
        </tr>
        <tr>
            <td colspan="2">Estrategia de Marketing</td>
            <td colspan="2">Demostraciones directas a dueños de restaurantes, alianzas con asociaciones gastronómicas peruanas, pilotos gratuitos con restaurantes seleccionados para generar casos de éxito medibles, y marketing digital dirigido al sector food service en redes sociales.</td>
            <td colspan="2">Venta directa basada en casos de éxito con métricas de conversión (2.4x de aumento en pedidos de platos destacados con AR) dirigida a restaurantes de gama alta dispuestos a pagar por plato.</td>
            <td colspan="2">Alianzas directas con restaurantes locales del campus (ej. restaurante Maize), cobertura de prensa universitaria y local, y participación en programas de aceleración universitaria (iVenture Accelerator).</td>
            <td colspan="2">Venta B2B a cadenas de restauración mediante casos de éxito documentados (La Tagliatella) y posicionamiento como proveedor tecnológico de WebAR para múltiples verticales de retail, no exclusivo de gastronomía.</td>
        </tr>
        <tr>
            <td rowspan="3" colspan="1">Perfil de Producto</td>
            <td colspan="2">Producto & Servicio</td>
            <td colspan="2">Aplicación móvil de gestión para el restaurante (registro de platos, autocompletado con IA, asociación de modelo 3D, generación de QR), visor WebAR (model-viewer sobre WebXR/AR Quick Look) y backend con base de datos para centralizar platos, modelos 3D y códigos QR.</td>
            <td colspan="2">Generación de modelos 3D fotorrealistas por fotogrametría, hosting del modelo en CDN, entrega de código QR imprimible y visor WebAR (AR Quick Look / Scene Viewer).</td>
            <td colspan="2">Aplicación móvil nativa con catálogo de platos en 3D/foto, activación de AR mediante marcador físico en mesa, y generación de modelos 3D a pedido del restaurante por el equipo de Menu3.</td>
            <td colspan="2">Plataforma WebAR de propósito general con generación de modelos 3D a pedido, códigos QR individuales por producto y panel de gestión de contenido.</td>
        </tr>
        <tr>
            <td colspan="2">Precio & Costos</td>
            <td colspan="2">Modelo de suscripción mensual por restaurante, escalable según el número de platos registrados, con un plan piloto inicial gratuito o de bajo costo para restaurantes pequeños, evitando el cobro por plato individual.</td>
            <td colspan="2">Desde £49 por plato, cobrado de forma individual por cada modelo 3D generado mediante fotogrametría.</td>
            <td colspan="2">Gratuito para el restaurante durante la fase piloto; sin modelo de precios comercial público conocido, limitado a un mercado universitario.</td>
            <td colspan="2">Precio no público; orientado a contratos B2B con cadenas medianas/grandes, lo que sugiere un costo de implementación superior al accesible para un restaurante independiente pequeño.</td>
        </tr>
        <tr>
            <td colspan="2">Canales de distribución (Web y/o Móvil)</td>
            <td colspan="2">Aplicación móvil (gestión del restaurante) y aplicación web/WebAR (experiencia del comensal, sin instalación)</td>
            <td colspan="2">Código QR impreso + aplicación web/WebAR (sin instalación para el comensal)</td>
            <td colspan="2">Aplicación móvil nativa (obligatoria para el comensal)</td>
            <td colspan="2">Código QR + aplicación web/WebAR (sin instalación para el comensal)</td>
        </tr>
        <tr>
            <td rowspan="5">Análisis SWOT</td>
            <td colspan="10">Realizado para Platter y para cada uno de los competidores identificados. Las fortalezas de Platter apoyan las oportunidades identificadas y sustentan su posible ventaja competitiva frente a los tres competidores analizados.</td>
        </tr>
        <tr>
            <td colspan="2">Fortalezas</td>
            <td colspan="2">Automatización con IA que reduce el costo y tiempo de registrar un plato; experiencia 100% sin instalación para el comensal; generación automática de alérgenos y calorías, inexistente en los competidores; enfoque en un mercado (Perú/Latinoamérica) sin competidores directos identificados; plataforma integrada de extremo a extremo (app + IA + AR + QR) que no depende de un equipo externo para cada actualización de carta.</td>
            <td colspan="2">Alto fotorrealismo del modelo 3D vía fotogrametría; tiempo de entrega predecible (48 horas); WebAR sin instalación ya validado comercialmente.</td>
            <td colspan="2">Pionero histórico en el espacio de AR para menús; validado con 24 restaurantes en un piloto real; catálogo completo de menú navegable en 3D dentro de una sola app.</td>
            <td colspan="2">Plataforma WebAR robusta y ya probada con clientes de cadena de restauración de tamaño medio/grande; experiencia sin instalación.</td>
        </tr>
        <tr>
            <td colspan="2">Debilidades</td>
            <td colspan="2">Marca nueva sin trayectoria ni casos de éxito documentados; la fidelidad del modelo 3D de muestra puede no coincidir exactamente con el plato real cuando el restaurante no sube un modelo propio; depende de la disponibilidad y estabilidad de una API externa de IA (Gemini) y de la compatibilidad AR del dispositivo del comensal.</td>
            <td colspan="2">Requiere que el restaurante realice una sesión fotográfica de 20 a 30 fotos por plato, lo que representa una carga operativa considerable; costo por plato (£49) poco accesible para restaurantes pequeños o medianos; no automatiza la generación de descripción, ingredientes, alérgenos ni calorías.</td>
            <td colspan="2">Exige la descarga de una aplicación nativa, generando fricción de adopción en el comensal; depende de un marcador físico en la mesa; quedó limitado a un piloto universitario sin evidencia de expansión comercial.</td>
            <td colspan="2">No está especializada exclusivamente en el rubro gastronómico, sino que atiende múltiples verticales de retail; no automatiza la generación de contenido gastronómico con IA; orientada a cadenas medianas/grandes, no a restaurantes independientes pequeños.</td>
        </tr>
        <tr>
            <td colspan="2">Oportunidades</td>
            <td colspan="2">Sector gastronómico peruano en recuperación que busca diferenciarse frente a la competencia; ausencia de competidores directos con enfoque en el mercado local; creciente familiaridad de los comensales con el escaneo de códigos QR desde la pandemia.</td>
            <td colspan="2">Expansión hacia mercados fuera del Reino Unido; crecimiento del segmento de restaurantes de alta cocina interesados en diferenciación digital.</td>
            <td colspan="2">Adoptar un modelo de WebAR sin aplicación para reducir la fricción que limitó su adopción; expandirse más allá del mercado universitario.</td>
            <td colspan="2">Ampliar su oferta con una vertical especializada en gastronomía; incorporar automatización de contenido con IA para atender también a restaurantes independientes.</td>
        </tr>
        <tr>
            <td colspan="2">Amenazas</td>
            <td colspan="2">Posible ingreso de competidores internacionales (ARmenu, Onirix) al mercado latinoamericano; resistencia al cambio tecnológico por parte de restaurantes tradicionales; cambios en el costo o disponibilidad de la API de Gemini Vision.</td>
            <td colspan="2">Aparición de soluciones basadas en IA (como Platter) que reduzcan drásticamente el costo y el tiempo de generación de modelos 3D frente a su proceso de fotogrametría manual.</td>
            <td colspan="2">Competidores con WebAR sin fricción (ARmenu, Onirix, Platter) capturan la preferencia del comensal final, que evita instalar aplicaciones para un solo restaurante.</td>
            <td colspan="2">Competidores especializados y más accesibles para el segmento de restaurantes pequeños y medianos (como Platter) le disputan ese nicho de mercado desatendido.</td>
        </tr>
    </tbody>
</table>

### 2.1.2 Estrategias y tácticas frente a competidores.

#### Estrategia de diferenciación por automatización con Inteligencia Artificial

Platter se diferenciará al ser, entre los competidores analizados, la única plataforma que automatiza tanto la generación de contenido gastronómico (descripción, ingredientes, alérgenos, calorías) como la asignación de un modelo 3D, sin exigir al restaurante una sesión fotográfica especializada como ARmenu ni depender de un equipo externo para modelar cada plato como Menu3 y Onirix.

**Tácticas:**
- Optimizar el flujo de análisis de fotografías con Gemini Vision para que el restaurante obtenga la ficha completa del plato en segundos, reduciendo la carga operativa que hoy enfrenta con procesos manuales o con competidores que exigen múltiples fotografías.
- Mantener y ampliar la biblioteca de modelos 3D de muestra emparejados automáticamente por categoría, para que ningún restaurante quede sin representación visual de un plato por no contar con un modelo 3D propio.
- Comunicar activamente la funcionalidad de detección de alérgenos y calorías como un diferenciador de seguridad alimentaria frente a competidores que no la ofrecen.

#### Estrategia de eliminación de fricción para el comensal

A diferencia de Menu3, que exige la descarga de una aplicación nativa y el uso de un marcador físico, Platter adoptará el mismo estándar sin fricción que ARmenu y Onirix: visualización en Realidad Aumentada activada directamente desde la cámara o el navegador del comensal mediante escaneo de un código QR.

**Tácticas:**
- Garantizar que el visor WebAR funcione de forma consistente tanto en Android (WebXR/Scene Viewer) como en iOS (AR Quick Look) desde un mismo código QR, sin pasos adicionales para el comensal.
- Evitar cualquier requerimiento de registro, descarga o cuenta de usuario para acceder a la experiencia AR desde el lado del comensal.

#### Estrategia de liderazgo en costos y accesibilidad para MYPE

Platter implementará un modelo de suscripción mensual accesible para restaurantes pequeños y medianos, evitando el cobro por plato individual de ARmenu (desde £49 por plato) y posicionándose como una alternativa viable para el segmento MYPE que domina el sector gastronómico peruano.

**Tácticas:**
- Ofrecer un plan piloto gratuito o de bajo costo a los primeros restaurantes adoptantes, a cambio de retroalimentación y casos de éxito documentados.
- Diseñar planes de suscripción escalables según el número de platos registrados, evitando cargos adicionales por generación de modelos 3D cuando se utiliza la biblioteca de muestra.

#### Estrategia de enfoque en el mercado peruano y latinoamericano

Ninguno de los competidores identificados (ARmenu en Reino Unido, Menu3 como piloto universitario en EE. UU., Onirix orientado a cadenas europeas) tiene presencia o enfoque específico en Perú o Latinoamérica. Platter aprovechará esta ausencia de competencia directa para posicionarse como la plataforma de referencia local antes de que un competidor internacional expanda su operación a la región.

**Tácticas:**
- Establecer alianzas con asociaciones gastronómicas peruanas para acelerar la adopción entre restaurantes pequeños y medianos.
- Priorizar el idioma, la moneda y los medios de pago locales, y adaptar la comunicación comercial a la identidad gastronómica peruana.
- Construir casos de éxito locales medibles (reducción de tiempo de gestión de carta, mejora en confianza de compra del comensal) para usarlos como evidencia frente a restaurantes indecisos.
## 2.2. Entrevistas.

### 2.2.1. Diseño de entrevistas.

El diseño de las entrevistas semiestructuradas tiene como propósito validar en el terreno empírico los puntos de dolor, las expectativas operativas y la disposición hacia la adopción tecnológica de la plataforma Platter en sus dos segmentos clave: administradores gastronómicos y comensales.

#### Segmento 1: Dueños y administradores de restaurantes

1. ¿Cuál es el proceso operativo que sigue actualmente en su restaurante para dar de alta un plato nuevo o actualizar precios, descripciones e ingredientes en su carta?
2. ¿Cuánto tiempo y recursos humanos demanda redactar manualmente la información detallada de cada plato (ingredientes, alérgenos y aporte calórico)?
3. ¿Con qué frecuencia el personal de salón debe resolver dudas o atender reclamos debido a que la porción o presentación servida difiere de lo que el comensal imaginó?
4. ¿Qué impacto económico o de reputación ha experimentado su establecimiento a causa de platos devueltos o insatisfacción por expectativas visuales no cumplidas?
5. ¿Cuáles han sido las principales barreras (costo, complejidad técnica, tiempo) que le han impedido incorporar fotografías profesionales continuas o modelos 3D en su carta?
6. Si una herramienta asistida por Inteligencia Artificial completara automáticamente el nombre, descripción, ingredientes, alérgenos y calorías a partir de una foto del plato, ¿cómo transformaría su dinámica operativa?
7. ¿Qué tan factible considera implementar códigos QR en mesa que permitan al comensal proyectar el plato en 3D sobre su mesa a escala real mediante Realidad Aumentada?
8. Ante la falta de modelos 3D propios de cada plato, ¿qué tan receptivo sería a utilizar modelos tridimensionales estándar de muestra asignados automáticamente por el sistema según la categoría gastronómica?

#### Segmento 2: Comensales de restaurante

1. Al acudir a un restaurante y revisar la carta física o digital, ¿en qué elementos visuales o textuales se basa para tomar su decisión de compra?
2. ¿Ha tenido experiencias donde el plato recibido fue notablemente distinto en volumen, estética o cantidad de ingredientes a lo que anticipó en la carta? ¿Cómo afectó esto su percepción del lugar?
3. ¿Qué relevancia tiene para usted conocer de forma clara e inmediata la presencia de alérgenos o restricciones nutricionales antes de ordenar?
4. ¿Cuánto tiempo suele demorar en elegir un plato debido a la incertidumbre sobre cómo lucirá en realidad?
5. ¿Qué fricciones encuentra habitualmente al interactuar con cartas mediante códigos QR (p. ej., descargas obligatorias de apps, lectura de PDFs pesados, interfaces lentas)?
6. ¿Qué valor representaría para usted proyectar el plato en 3D y a escala real sobre su propia mesa usando únicamente la cámara del celular y sin instalar ninguna aplicación?
7. ¿Tener una previsualización interactiva en Realidad Aumentada y el detalle de alérgenos incrementaría su confianza para solicitar platos nuevos o de mayor valor?
8. ¿Considera que la presencia de tecnología de Realidad Aumentada en mesa aumentaría su probabilidad de volver a visitar o recomendar el restaurante?

### 2.2.2. Registro de entrevistas.

* **Entrevista 1:**
  * Nombres: Carlos Mendoza Vidal
  * Segmento: Dueños y Administradores de Restaurantes (Propietario de restaurante criollo tradicional)
  * Edad: 42 años
  * Fecha: 12 de septiembre de 2026
  * Duración: 28 minutos

* **Entrevista 2:**
  * Nombres: Valeria Ramos Benavides
  * Segmento: Comensales de Restaurante
  * Edad: 26 años
  * Fecha: 14 de septiembre de 2026
  * Duración: 22 minutos
  
<img src="./assets/Entrevista 1.png">

### 2.2.3. Análisis de entrevistas.

El análisis cualitativo estructurado de las respuestas obtenidas permitió sintetizar los siguientes hallazgos:

* **Patrones de comportamiento identificados:**
  * Los administradores gastronómicos recurren a soluciones ofimáticas básicas (Word, Excel) e intermediarios de diseño gráfico informal para actualizar cartas impresas o archivos PDF, con ciclos de actualización lentos y desconectados del inventario real.
  * Los comensales presentan una conducta de verificación cruzada: ante descripciones escuetas, buscan fotos en redes sociales del restaurante o interrogan al personal de sala para contrastar porciones y apariencia.
  * Existe un hábito consolidado en el escaneo de códigos QR, pero condicionado estrictamente a que no demande instalar software adicional ni consuma tiempos prolongados de carga.

* **Puntos de dolor críticos (Pains):**
  * *Administradores:* Sobrecarga de tiempo administrativo al redactar fichas técnicas de platos, desconocimiento de cómo declarar alérgenos formalmente y frustración por el costo inaccesible de servicios de modelado 3D o fotografía publicitaria periódica.
  * *Comensales:* Incertidumbre volumétrica y estética (brecha entre expectativa y realidad), sensación de lentitud al ordenar por falta de referencias visuales confiables y riesgo latente de salud para personas con alergias alimentarias.

* **Recepción y disposición hacia la tecnología propuesta:**
  * El procesamiento multimodal con Inteligencia Artificial (Gemini Vision) fue recibido por los administradores como un catalizador de eficiencia, reduciendo drásticamente la barrera de entrada al ingreso de platos.
  * La adopción de WebAR fue ampliamente validada por los comensales, destacando que proyectar el plato a escala real sobre la mesa disipa la desconfianza de compra y aporta un componente lúdico e innovador sin fricción de descarga.

* **Conclusión y validación de hipótesis:**
  Los resultados validan plenamente las hipótesis del Lean UX Canvas. La reducción de la brecha de expectativa visual mediante WebAR responde directamente al núcleo del problema del comensal, mientras que la automatización del catálogo asistida por IA elimina la fricción operativa del restaurante, confirmando la viabilidad y pertinencia del modelo arquitectónico de Platter.

---

## 2.3. Needfinding.

### 2.3.1. User Personas.

Los User Personas representan arquetipos construidos a partir de los patrones conductuales, motivaciones y limitaciones identificados durante la investigación cualitativa. El primer arquetipo consolida la perspectiva del gestor de una micro o pequeña empresa gastronómica que busca modernizar su servicio y reducir fricciones operativas sin elevar sus costos fijos. El segundo arquetipo refleja al comensal urbano habitual que valora la transparencia en el servicio, busca optimizar su tiempo de decisión y prioriza experiencias inmersivas respaldadas por información nutricional confiable.

UserPersona 1 
<img src="./assets/Carlos Mendoza Vidal.png">

UserPersona 2 
<img src="./assets/Valeria Ramos Benavides.png">

### 2.3.2. User Task Matrix.

| Tareas | Segmento 1: Dueños y Administradores | Segmento 2: Comensales | Frecuencia | Importancia |
| :--- | :--- | :--- | :--- | :--- |
| Registrar nuevo plato cargando una fotografía | Alta | No aplica | Semanal / Quincenal | Alta |
| Autocompletar y verificar datos gastronómicos (alérgenos, calorías) con IA | Alta | No aplica | Semanal / Quincenal | Alta |
| Asignar o vincular modelo 3D al plato del catálogo | Media | No aplica | Ocasional | Media |
| Generar e imprimir código QR dinámico para mesas | Media | No aplica | Ocasional | Alta |
| Monitorear métricas de visualización y platos más consultados | Media | No aplica | Mensual | Media |
| Escanear código QR desde la mesa del restaurante | No aplica | Alta | Por visita | Alta |
| Proyectar y visualizar plato en WebAR a escala real sobre la mesa | No aplica | Alta | Por visita | Alta |
| Consultar detalle de ingredientes, alérgenos y aporte calórico | No aplica | Alta | Por visita | Alta |
| Solicitar aclaraciones verbales al mesero sobre el plato | Baja | Media | Por visita | Baja |
| Tomar la decisión y ordenar el pedido final en mesa | No aplica | Alta | Por visita | Alta |

#### Análisis de Tareas

* **Tareas con mayor frecuencia e importancia:**
  En el Segmento 1, las tareas más críticas y recurrentes son el registro fotográfico del plato y la verificación asistida por IA de la información gastronómica, ya que alimentan la base de datos de la carta. En el Segmento 2, las tareas dominantes son el escaneo del código QR dinámico, la proyección tridimensional en WebAR a escala real y la consulta inmediata de alérgenos, determinantes en el momento de la compra.

* **Principales diferencias:**
  El Segmento 1 realiza tareas asincrónicas de back-office, centradas en la gobernanza del catálogo, configuración visual y control de contenido. Por el contrario, el Segmento 2 ejecuta tareas sincrónicas en el front-stage (salón del restaurante), con un ciclo de interacción efímero de alta demanda de inmediatez y rendimiento visual.

* **Principales similitudes:**
  Ambos segmentos convergen en la necesidad de coherencia y exactitud del contenido gastronómico. El código QR dinámico actúa como el punto de integración operacional mutuo: el administrador lo genera y distribuye, mientras que el comensal lo consume como punto de partida de su interacción.

* **Enfoque de los segmentos:**
  El Segmento 1 está enfocado en la productividad, el ahorro de tiempo en gestión de contenidos y la diferenciación competitiva frente a otras opciones gastronómicas. El Segmento 2 está enfocado en la certidumbre visual, la seguridad alimentaria (control riguroso de alérgenos) y una experiencia de usuario rápida y sin barreras técnicas.

### 2.3.3. Empathy Mapping.

El Mapa de Empatía sintetiza el entorno sensorial y emocional de ambos actores clave, identificando lo que dicen, hacen, piensan y sienten en su contexto operativo o de consumo regular, permitiendo una comprensión holística de sus dolores y aspiraciones.

#### Mapa de Empatía - Segmento 1: Dueños y Administradores de Restaurantes
<img src="./assets/Empathy map1.png">

#### Mapa de Empatía - Segmento 2: Comensales de Restaurante
<img src="./assets/Empathy map2.png">

### 2.3.4. As-is Scenario Mapping.

El mapeo de escenarios actuales ("As-is") documenta el flujo cronológico de interacciones, fricciones y estados emocionales por los que atraviesan los usuarios en el sistema actual sin la intervención de Platter.

Para el administrador, el flujo inicia con la concepción manual de cartas impresas o archivos PDF, atravesando por la dificultad de calcular información nutricional y la frustración por costos elevados de diseño publicitario, culminando en cartas estáticas difíciles de mantener al día.

Para el comensal, el escenario actual abarca desde la llegada a la mesa, la lectura de cartas basadas en descripciones ambiguas o fotografías planas desactualizadas, la constante consulta verbal al personal de salón y la decepción final cuando el plato recibido no cumple las expectativas visuales ni de porción deseadas.

#### As-is Scenario Mapping - Segmento 1: Dueños y Administradores de Restaurantes
<img src="./assets/Customer journey map1.png">

#### As-is Scenario Mapping - Segmento 2: Comensales de Restaurante
<img src="./assets/Customer journey map2.png">

## 2.4. Big Picture EventStorming.
<img src="./assets/fase_1_backoffice.png">
<img src="./assets/fase_2_frontstage.png">

## 2.5. Ubiquitous Language.

| Term (English) | Término (Español) | Definition (Definición en español) |
| :--- | :--- | :--- |
| **Dish Profile** | Perfil del Plato | Entidad fundamental del dominio que encapsula la información descriptiva, comercial, nutricional y los activos 3D de un ítem del menú. |
| **Computer Vision Extraction** | Extracción por Visión Computacional | Proceso automatizado en el cual un modelo multimodal de IA analiza la imagen de un plato para inferir ingredientes, alérgenos y aporte calórico. |
| **Allergen Tagging** | Etiquetado de Alérgenos | Clasificación explícita y normalizada de sustancias potencialmente reactivas (gluten, mariscos, frutos secos) detectadas o asociadas al plato. |
| **WebAR Viewer** | Visor WebAR | Interfaz web que procesa y renderiza elementos en Realidad Aumentada desde el navegador móvil del comensal sin instalación de aplicaciones nativas. |
| **Dynamic QR Code** | Código QR Dinámico | Código bidimensional que redirecciona a un URI configurable, permitiendo actualizar la referencia del plato o carta sin alterar el código físico impreso. |
| **Real-scale 3D Projection** | Proyección 3D a Escala Real | Renderizado volumétrico tridimensional anclado en el espacio físico que replica con exactitud las proporciones y dimensiones métricas del plato servido. |
| **Surface Tracking** | Detección de Superficie | Técnica de visión espacial del dispositivo móvil encargada de identificar planos horizontales (mesas) para situar y estabilizar el modelo tridimensional. |
| **Sample 3D Model** | Modelo 3D de Muestra | Representación tridimensional genérica provista por el sistema asignada automáticamente a un plato cuando el restaurante no posee un activo 3D propio. |
| **Menu Catalog** | Catálogo de Carta | Agregado que agrupa, categoriza y gobierna la totalidad de perfiles de platos pertenecientes a una sede o restaurante en particular. |
| **Restaurant Manager** | Administrador del Restaurante | Rol de usuario que gestiona el ciclo de vida de los platos, administra el catálogo y supervisa la configuración visual y operativa de su carta. |
| **Diner** | Comensal | Actor final que escanea el identificador en mesa para interactuar con la carta digitalizada y examinar los platos en Realidad Aumentada. |
| **Nutritional Estimation** | Estimación Nutricional | Cálculo aproximado del valor calórico y macronutrientes inferido a partir de la identificación volumétrica y visual de los ingredientes por IA. |
| **Visual Expectation Gap** | Brecha de Expectativa Visual | Discrepancia entre la representación mental que el comensal elabora a partir del texto o foto plana y el plato físico servido en su mesa. |
| **Dish Onboarding** | Alta de Plato | Flujo operativo mediante el cual el administrador carga la imagen inicial, valida las sugerencias de la IA y publica el ítem en la carta visible. |
| **Bounded Context** | Contexto Delimitado | Frontera arquitectónica explícita en DDD dentro de la cual un submodelo de dominio particular (p. ej., Gestión de Menú, Experiencia WebAR) tiene significado unívoco. |

# Capítulo III: Requirements Specification

Esta sección permite especificar los requisitos de los productos digitales que conforman la plataforma **Platter**, a partir del análisis riguroso de la información obtenida en los capítulos precedentes (Problem Statement, Lean UX Canvas y Needfinding de los segmentos objetivo). En este capítulo se detallan: el To-Be Scenario Mapping que proyecta la experiencia ideal de interacción para cada segmento; el catálogo consolidado de Epics y User Stories con criterios de aceptación estructurados en formato formal Gherkin; el Impact Mapping que alinea estratégicamente las capacidades de software con las metas de negocio de la startup; y el Product Backlog priorizado estrictamente en función del valor generado para el negocio y el usuario final.

## 3.1. To-Be Scenario Mapping.

El To-Be Scenario Mapping describe la secuencia de interacción ideal que experimentan los usuarios objetivo al utilizar la solución tecnológica propuesta, proyectando las fases del recorrido y detallando las dimensiones de comportamiento (*Doing*), cognición (*Thinking*) y emoción (*Feeling*) para cada segmento.

### Segmento 1 - Carlos Mendoza

| Phases | Captura del plato | Análisis y autocompletado con IA | Asignación 3D y generación QR | Monitoreo en salón |
| :--- | :--- | :--- | :--- | :--- |
| **Doing** | Ingresa a la app móvil de Platter y toma una fotografía directa del plato preparado en cocina. | Carga la foto y revisa la descripción, ingredientes, alérgenos y calorías sugeridas por la IA. Ajusta detalles y confirma. | Vincula un modelo 3D a escala real desde el catálogo y genera los códigos QR de las mesas listos para imprimir. | Coloca los códigos QR en las mesas e ingresa al panel administrativo para observar las visualizaciones AR en tiempo real. |
| **Thinking** | "No necesito un fotógrafo profesional, una foto clara con mi celular es suficiente". "El proceso es rápido y sencillo". | "La IA redactó una descripción atractiva y detectó los alérgenos al instante". "Ahorro horas de redacción manual". | "El modelo 3D coincide con las dimensiones de nuestro plato real". "Tengo los QR listos sin pagar diseño extra". | "Mis clientes exploran la carta antes de pedir". "Puedo saber qué platos llaman más la atención en tiempo real". |
| **Feeling** | Tranquilidad y confianza. | Asombro y alivio. | Seguridad y profesionalismo. | Satisfacción y control. |

### Segmento 2 - Valeria Ramos

| Phases | Llegada y escaneo de QR | Exploración de la carta | Proyección en Realidad Aumentada | Decisión y pedido |
| :--- | :--- | :--- | :--- | :--- |
| **Doing** | Se sienta en la mesa, abre la cámara de su smartphone y escanea el código QR ubicado en el soporte físico. | Navega por las categorías de la carta digital en su navegador móvil y revisa los platos con fotos y descripciones claras. | Selecciona "Ver en mi mesa", enfoca la superficie del mantel y visualiza el plato en 3D a tamaño real interactuando con su entorno. | Verifica que no contenga alérgenos que le afecten, confirma su elección y realiza su pedido al mozo con total certeza. |
| **Thinking** | "Qué práctico que no tenga que descargar ninguna aplicación pesada solo para almorzar". | "La carta carga rápido y muestra ingredientes detallados". "Puedo ver qué opciones se adaptan a mi dieta". | "¡Se ve a tamaño real sobre mi mesa!". "Ahora sé con certeza qué tan generosa es la porción antes de pedir". | "Tengo total confianza en lo que voy a comer y el plato superó mis dudas sobre su tamaño". |
| **Feeling** | Comodidad y tranquilidad. | Curiosidad e interés. | Asombro y seguridad. | Satisfacción y valoración. |

---

## 3.2. User Stories.

Para formalizar los requisitos funcionales y técnicos de los productos digitales de Platter (Landing Page estática, Aplicación Web/Móvil Administrativa, Visor WebAR para Comensales y Servicios Backend RESTful), el equipo definió un catálogo consolidado de **22 User Stories** articuladas en **7 Epics**. 

Las historias cumplen con las siguientes normas metodológicas:
* **Formato estándar de usuario:** Redactadas desde la perspectiva de los roles involucrados: *Visitante* (para el sitio estático/Landing Page), *Dueño de restaurante / Administrador*, *Comensal* y *Developer* (para las historias técnicas de arquitectura e integración).
* **Criterios de Aceptación Gherkin (`Given - When - Then`):** Redactados en tiempo presente, tercera persona, sin referencias acopladas a detalles visuales de la interfaz de usuario (evitando mencionar colores, botones específicos o coordenadas) y plenamente comprobables mediante pruebas funcionales y de integración.
* **Trazabilidad:** Cada historia está asociada a su Epic correspondiente.

| Epic / User Story ID | Título | Descripción | Criterios de Aceptación | Relacionado con (Epic ID) |
| :--- | :--- | :--- | :--- | :--- |
| **EP01** | Landing Page & Adquisición de Clientes | Como visitante interesado en soluciones gastronómicas, deseo explorar un sitio web informativo para conocer la propuesta de valor, los beneficios económicos y los planes de Platter. | - El sitio web estático presenta información clara y responsiva dirigida a restaurantes y comensales.<br>- Incluye secciones de beneficios, retorno de inversión (ROI), demostración interactiva, planes comerciales y formulario de contacto. | - |
| **EP02** | Catálogo Gastronómico & Análisis con IA | Como dueño de restaurante, deseo registrar mis platos mediante fotografías y procesamiento con Inteligencia Artificial para automatizar la creación de fichas técnicas de mi carta sin esfuerzo manual. | - Permite cargar fotografías de platos desde el dispositivo móvil.<br>- Genera descripción gastronómica, ingredientes, alérgenos y estimación calórica con IA.<br>- Permite asociar modelos 3D a escala real y habilitar o deshabilitar platos en tiempo real. | - |
| **EP03** | Generación & Administración de Códigos QR | Como dueño de restaurante, deseo generar y descargar códigos QR asociados a las mesas de mi salón para que mis clientes accedan directamente a la carta en Realidad Aumentada. | - Genera identificadores únicos por mesa y por restaurante.<br>- Proporciona plantillas descargables de alta resolución listas para imprimir y exhibir en mesas físicas. | - |
| **EP04** | Experiencia WebAR para Comensales | Como comensal en el restaurante, deseo visualizar los platos en Realidad Aumentada sobre mi mesa a tamaño real directamente desde el navegador web para tomar una decisión informada de compra sin instalar aplicaciones. | - Permite abrir la carta mediante escaneo de código QR sin autenticación.<br>- Renderiza modelos 3D fotorrealistas a escala 1:1 mediante estándares WebXR / Quick Look.<br>- Permite rotar y comparar el tamaño del plato respecto a la vajilla física. | - |
| **EP05** | Información Nutricional & Alérgenos | Como comensal con restricciones alimentarias, deseo consultar el detalle de ingredientes, calorías y alérgenos de cada plato para consumir alimentos seguros según mi perfil de salud. | - Presenta lista clara de alérgenos certificados por la ficha del plato.<br>- Permite filtrar la carta descartando platos con alérgenos no tolerados por el comensal.<br>- Muestra advertencias de ingredientes sensibles de manera visible y accesible. | - |
| **EP06** | Panel Administrativo & Suscripciones MYPE | Como dueño de restaurante, deseo consultar métricas de interacción con mi carta y gestionar mi plan de suscripción mensual para optimizar la rentabilidad de mi establecimiento. | - Proporciona analítica de platos más visualizados en AR y mesas con mayor interacción.<br>- Permite seleccionar y gestionar planes de suscripción mensual mediante pasarela de pagos. | - |
| **EP07** | Arquitectura Backend & Asset Pipeline (Technical Epics) | Como Developer, deseo disponer de servicios RESTful desacoplados y pipelines de procesamiento para asegurar alta disponibilidad, inferencia de IA y entrega eficiente de modelos 3D ligeros. | - Expone endpoints modulares en Spring Boot bajo arquitectura limpia.<br>- Gestiona compresión y despacho en caché de modelos GLB/USDZ con tiempos de respuesta reducidos. | - |
| **US01** | Visualización de Propuesta de Valor y Demostrador WebAR | Como visitante del sitio web estático, deseo experimentar una demostración interactiva de Realidad Aumentada desde mi dispositivo para comprobar la efectividad de la carta 3D antes de registrar mi negocio. | **Scenario 1: Demostración exitosa desde móvil**<br>**Given** que el visitante navega en la sección principal de la Landing Page desde un dispositivo móvil compatible con WebAR,<br>**When** selecciona la opción de prueba interactiva de un plato de muestra,<br>**Then** el navegador activa la vista de Realidad Aumentada y proyecta el plato gastronómico tridimensional a escala real sobre su entorno.<br><br>**Scenario 2: Demostración desde navegador de escritorio**<br>**Given** que el visitante ingresa a la Landing Page desde una computadora de escritorio,<br>**When** consulta el área de demostración interactiva,<br>**Then** el sistema presenta un visor 3D interactivo navegable con cursor y un código QR en pantalla para escanearlo y probar la experiencia en el smartphone. | EP01 |
| **US02** | Sección de Beneficios, Métricas de Retorno (ROI) y Casos de Uso | Como visitante del segmento dueño de restaurante, deseo revisar estadísticas del impacto de la Realidad Aumentada en ventas y testimonios de restaurantes piloto para fundamentar mi decisión de afiliación. | **Scenario 1: Consulta de indicadores de rentabilidad**<br>**Given** que el visitante navega en la sección de beneficios de la Landing Page,<br>**When** explora los datos comparativos de conversión y reducción de tiempos de gestión,<br>**Then** visualiza métricas documentadas sobre incremento de ticket promedio (2x a 3x en conversión AR) y reducción de tiempos de actualización de carta.<br><br>**Scenario 2: Navegación de casos de uso**<br>**Given** que el visitante revisa los ejemplos por tipo de cocina (criolla, marina, especialidades),<br>**When** selecciona un caso de uso específico,<br>**Then** se despliegan detalles de cómo la solución resuelve la exhibición de porciones para dicho giro gastronómico. | EP01 |
| **US03** | Consulta de Planes de Suscripción y Calculadora MYPE | Como visitante del segmento dueño de restaurante, deseo consultar los planes tarifarios y calcular el costo según el número de mesas de mi local para evaluar la asequibilidad de la inversión. | **Scenario 1: Visualización transparente de planes**<br>**Given** que el visitante accede a la sección de precios de la Landing Page,<br>**When** revisa las alternativas de suscripción mensual,<br>**Then** se detallan los límites de platos, soporte de IA, generación de códigos QR y acceso a la biblioteca de modelos 3D sin cobros ocultos por plato.<br><br>**Scenario 2: Cálculo estimado de inversión**<br>**Given** que el visitante ingresa el número de platos y mesas de su establecimiento en la calculadora de la página,<br>**When** solicita el cálculo estimado,<br>**Then** el sistema recomienda el plan óptimo y resalta el ahorro frente al modelado fotogramétrico tradicional. | EP01 |
| **US04** | Formulario de Solicitud de Piloto Gratuito | Como visitante del segmento dueño de restaurante, deseo enviar mis datos de contacto y nombre de mi local comercial para solicitar una prueba piloto gratuita de 14 días con mi carta. | **Scenario 1: Envío exitoso de solicitud**<br>**Given** que el visitante completa el formulario con nombre del restaurante, correo corporativo, teléfono y número de mesas válidos,<br>**When** envía la solicitud de afiliación,<br>**Then** el sistema registra los datos en la base de prospectos y muestra un mensaje de confirmación notificando que recibirá su acceso en menos de 24 horas.<br><br>**Scenario 2: Validación de datos incompletos**<br>**Given** que el visitante omite ingresar un correo o teléfono con formato válido,<br>**When** intenta remitir el formulario,<br>**Then** el sistema no procesa el envío y destaca los campos requeridos con mensajes de subsanación claros. | EP01 |
| **US05** | Carga Fotográfica de Plato para Análisis Automatizado | Como dueño de restaurante, deseo cargar una fotografía de un plato recién preparado desde la cámara o galería de mi móvil para iniciar el proceso de digitalización con Inteligencia Artificial. | **Scenario 1: Carga de fotografía válida**<br>**Given** que el administrador tiene una sesión activa en la aplicación y selecciona la opción de registrar plato,<br>**When** captura o adjunta una fotografía en formato JPEG o PNG con peso menor a 10 MB,<br>**Then** la imagen se procesa satisfactoriamente y se almacena en el repositorio de activos digitales para su análisis posterior.<br><br>**Scenario 2: Formato o tamaño no soportado**<br>**Given** que el usuario intenta subir un archivo con extensión no admitida o peso superior a 10 MB,<br>**When** ejecuta la acción de carga,<br>**Then** el sistema rechaza el archivo y emite una notificación indicando los límites permitidos de formato y peso. | EP02 |
| **US06** | Sugerencia Inteligente de Descripción y Categoría con IA | Como dueño de restaurante, deseo que la plataforma analice la imagen del plato mediante Inteligencia Artificial multimodal para obtener una descripción comercial atractiva y su categoría sugerida en segundos. | **Scenario 1: Inferencia exitosa de descripción**<br>**Given** que una fotografía gastronómica válida ha sido cargada al sistema,<br>**When** se invoca el motor de análisis multimodal de Gemini Vision,<br>**Then** el sistema retorna una propuesta de nombre comercial, categoría sugerida y descripción sensorial de entre 40 y 70 palabras adaptada a la gastronomía local.<br><br>**Scenario 2: Fotografía difusa o no gastronómica**<br>**Given** que el usuario subió una imagen con baja iluminación o sin elementos gastronómicos discernibles,<br>**When** el motor de IA procesa la imagen y obtiene un nivel de confianza menor al umbral mínimo,<br>**Then** el sistema solicita amablemente al usuario una nueva toma más clara o la opción de completar los datos de forma manual. | EP02 |
| **US07** | Detección Automática de Ingredientes Clave y Alérgenos | Como dueño de restaurante, deseo que el sistema identifique los ingredientes principales y marque alérgenos normados a partir de la foto del plato para cumplir con las regulaciones de seguridad alimentaria. | **Scenario 1: Detección y clasificación de alérgenos comunes**<br>**Given** que la imagen del plato contiene elementos como mariscos, maní, lácteos, huevo o trigo,<br>**When** finaliza el análisis de ingredientes con IA,<br>**Then** el sistema preselecciona las etiquetas de alérgenos correspondientes en la ficha del plato y lista los ingredientes principales reconocidos.<br><br>**Scenario 2: Sin alérgenos evidentes**<br>**Given** que el plato corresponde a una preparación libre de alérgenos principales,<br>**When** concluye el análisis,<br>**Then** el sistema presenta la lista de ingredientes limpia y deja las casillas de alérgenos desmarcadas para validación del administrador. | EP02 |
| **US08** | Estimación Calórica y Ficha Nutricional Automatizada | Como dueño de restaurante, deseo contar con una estimación aproximada del rango calórico y macronutrientes del plato para ofrecer información nutricional transparente a mis comensales. | **Scenario 1: Cálculo estimado de calorías**<br>**Given** que se han identificado los ingredientes y la porción típica del plato analizado,<br>**When** el sistema calcula los parámetros nutricionales sugeridos,<br>**Then** se despliega un rango calórico estimado (ej. 450 - 550 kcal) y advertencias informativas de que se trata de una estimación nutricional orientativa.<br><br>**Scenario 2: Ajuste de porción**<br>**Given** que el plato tiene una presentación personal o familiar grande,<br>**When** el usuario modifica la escala de porción en la ficha,<br>**Then** el sistema recalcula proporcionalmente el rango calórico sugerido. | EP02 |
| **US09** | Validación y Ajuste Manual de Ficha Gastronómica | Como dueño de restaurante, deseo revisar, editar y confirmar los textos, ingredientes y alérgenos sugeridos por la IA antes de que el plato sea visible en la carta digital. | **Scenario 1: Aprobación con modificaciones**<br>**Given** que la IA sugirió la ficha técnica del plato,<br>**When** el administrador corrige un ingrediente particular y pulsa confirmar publicación,<br>**Then** los datos editados reemplazan la sugerencia automática y el plato queda registrado oficialmente en el catálogo del restaurante.<br><br>**Scenario 2: Cancelación de registro**<br>**Given** que el usuario decide no continuar con el alta del plato analizado,<br>**When** cancela la operación antes de guardar,<br>**Then** el borrador temporal se descarta y el catálogo se mantiene sin alteraciones. | EP02 |
| **US10** | Asignación de Modelo 3D a Escala Real desde Biblioteca | Como dueño de restaurante, deseo vincular un modelo 3D fotorrealista a escala 1:1 desde la biblioteca gastronómica predeterminada de Platter para que el plato disponga de visualización en Realidad Aumentada sin costo adicional de modelado. | **Scenario 1: Asociación automática por categoría**<br>**Given** que el plato registrado pertenece a una categoría con modelos estándar disponibles (ej. cebiche, lomo saltado, hamburguesa artesanal),<br>**When** el sistema clasifica el plato,<br>**Then** vincula por defecto el modelo 3D optimizado (GLB/USDZ) configurado con dimensiones físicas exactas en metros.<br><br>**Scenario 2: Selección manual alternativa**<br>**Given** que el usuario desea asignar una representación 3D diferente a la sugerida,<br>**When** navega por la galería de modelos gastronómicos y escoge un activo alternativo,<br>**Then** la asociación se actualiza y la vista previa 3D refleja el nuevo modelo elegido. | EP02 |
| **US11** | Generación de Códigos QR con Identificador de Mesa | Como dueño de restaurante, deseo generar códigos QR individuales asociados a cada una de las mesas de mi restaurante para que los comensales accedan de manera contextualizada a la carta digital. | **Scenario 1: Generación masiva por rango de mesas**<br>**Given** que el administrador ingresa la cantidad de mesas de su salón (ej. Mesas 1 a 20),<br>**When** solicita la generación de códigos QR,<br>**Then** el sistema genera identificadores criptográficos únicos vinculados al restaurante y al número de mesa correspondiente, dejándolos listos para consulta y descarga.<br><br>**Scenario 2: Incorporación de una nueva mesa**<br>**Given** que el local amplía su capacidad con una mesa adicional,<br>**When** el administrador añade la mesa identificada como "Terraza 01",<br>**Then** se genera de forma instantánea el QR respectivo sin alterar los códigos de las mesas previamente existentes. | EP03 |
| **US12** | Descarga de Plantilla de QR en Alta Calidad para Impresión | Como dueño de restaurante, deseo descargar los códigos QR en un formato gráfico listo para imprenta con el logotipo y nombre de mi negocio para colocarlos en soportes físicos de mesa. | **Scenario 1: Descarga en PDF vectorizado / PNG HD**<br>**Given** que los códigos QR de las mesas han sido generados,<br>**When** el usuario selecciona descargar la plantilla de mesas seleccionadas en formato imprimible,<br>**Then** el sistema descarga un archivo estructurado en alta resolución apto para impresión con instrucciones de escaneo para el comensal.<br><br>**Scenario 2: Personalización con marca del restaurante**<br>**Given** que el restaurante tiene configurado su nombre comercial y logotipo en su perfil,<br>**When** se genera la plantilla descargable,<br>**Then** el arte gráfico incorpora dichos distintivos de marca de forma armonizada sobre el código QR. | EP03 |
| **US13** | Acceso Inmediato a Carta Digital sin Registro ni App | Como comensal en la mesa del restaurante, deseo acceder a la carta digital interactiva inmediatamente al escanear el código QR con mi teléfono móvil sin tener que crear cuentas ni instalar aplicaciones. | **Scenario 1: Escaneo y carga exitosa en navegador**<br>**Given** que el comensal escanea el código QR de su mesa mediante la aplicación de cámara de su smartphone (iOS o Android),<br>**When** se abre la URL en el navegador móvil predeterminado,<br>**Then** la carta del restaurante carga en menos de 2 segundos, mostrando el número de mesa identificada y las categorías del menú sin solicitar autenticación previa.<br><br>**Scenario 2: Acceso a mesa no configurada o inactiva**<br>**Given** que un comensal escanea un código QR deshabilitado o con identificador inválido,<br>**When** el navegador intenta resolver la dirección web,<br>**Then** el sistema muestra una pantalla amigable indicando que la mesa no está activa y ofreciendo visualizar el menú general del restaurante. | EP04 |
| **US14** | Proyección del Plato en Realidad Aumentada (WebAR) a Escala 1:1 | Como comensal, deseo proyectar el modelo 3D del plato sobre la superficie de mi mesa con dimensiones reales a escala 1:1 para evaluar su presentación y tamaño antes de solicitarlo. | **Scenario 1: Activación de Realidad Aumentada en Android (WebXR / Scene Viewer)**<br>**Given** que el comensal navega en la carta desde un dispositivo Android compatible con ARCore,<br>**When** selecciona "Ver en Realidad Aumentada" en la ficha de un plato,<br>**Then** el navegador ejecuta el visor nativo sin aplicaciones intermedias, detecta la superficie horizontal de la mesa y ubica el modelo 3D fotorrealista a escala 1:1.<br><br>**Scenario 2: Activación de Realidad Aumentada en iOS (AR Quick Look)**<br>**Given** que el comensal utiliza un dispositivo iPhone o iPad compatible con ARKit,<br>**When** activa la visualización en AR,<br>**Then** iOS despliega el visor AR Quick Look en formato USDZ permitiendo interactuar con el modelo y rotarlo 360 grados sobre el mantel.<br><br>**Scenario 3: Dispositivo móvil sin compatibilidad AR**<br>**Given** que el smartphone del comensal no posee soporte de hardware para Realidad Aumentada,<br>**When** intenta ingresar a la experiencia AR,<br>**Then** el sistema activa automáticamente un visor 3D interactivo en pantalla donde puede rotar y hacer zoom sobre el plato en 360°. | EP04 |
| **US15** | Filtrado de Platos por Alérgenos y Preferencias Dietarias | Como comensal con requerimientos dietarios o alergias alimentarias, deseo filtrar los platos de la carta excluyendo alérgenos específicos para encontrar opciones seguras para mi consumo. | **Scenario 1: Aplicación de filtros de seguridad alimentaria**<br>**Given** que el comensal ingresa a la carta digital de su mesa,<br>**When** marca los filtros de exclusión (ej. "Sin Gluten" y "Sin Mariscos"),<br>**Then** la lista de platos se actualiza dinámicamente mostrando únicamente las preparaciones certificadas libres de dichos alérgenos.<br><br>**Scenario 2: Búsqueda sin resultados disponibles**<br>**Given** que la combinación de filtros seleccionada por el comensal no coincide con ningún plato del menú,<br>**When** se aplican las restricciones,<br>**Then** el sistema informa que no hay platos disponibles bajo ese criterio estricto y sugiere consultar al personal del restaurante sobre adaptaciones de cocina. | EP05 |
| **US16** | Comparación Visual de Dimensiones del Plato en Mesa | Como comensal, deseo mover, rotar e inspeccionar la proyección 3D del plato junto a cubiertos o vasos reales sobre mi mesa para constatar su volumen y porción real. | **Scenario 1: Manipulación de gestos táctiles en AR**<br>**Given** que el modelo 3D se encuentra proyectado en la mesa en modo Realidad Aumentada,<br>**When** el comensal realiza gestos táctiles de rotación con sus dedos sobre la pantalla,<br>**Then** el modelo gira sobre su eje vertical manteniendo estrictamente su escala métrica calibrada en relación con el entorno real.<br><br>**Scenario 2: Bloqueo de escalado para fidelidad de porción**<br>**Given** que el comensal intenta agrandar el plato con gesto de pellizco en modo AR,<br>**When** interactúa con el modelo,<br>**Then** el sistema restringe el cambio de tamaño libre y emite un mensaje indicando que el plato se mantiene en escala física 1:1 para garantizar la fidelidad de la porción servida. | EP04 |
| **US17** | Consulta de Ingredientes y Advertencias de Contaminación Cruzada | Como comensal alérgico, deseo acceder a la ficha informativa detallada del plato para revisar posibles trazas de ingredientes y notas de advertencia de cocina. | **Scenario 1: Despliegue de ficha de ingredientes**<br>**Given** que el comensal visualiza la ficha de un plato en la carta digital,<br>**When** expande la sección de información de alérgenos e ingredientes,<br>**Then** se despliegan las etiquetas destacadas con iconos representativos de cada alérgeno y la advertencia sobre buenas prácticas de manipulación del restaurante.<br><br>**Scenario 2: Certificación de plato vegetariano/vegano**<br>**Given** que un plato cuenta con certificación vegana en su registro,<br>**When** el comensal inspecciona la ficha,<br>**Then** se muestra el distintivo correspondiente y el desglose de sustitutos de origen vegetal utilizados. | EP05 |
| **US18** | Actualización de Disponibilidad de Platos en Tiempo Real | Como dueño de restaurante, deseo marcar platos como "Agotado" con un solo toque desde mi panel para que los comensales no intenten ordenar preparaciones que ya no están disponibles en cocina. | **Scenario 1: Desactivación inmediata por quiebre de stock**<br>**Given** que el administrador identifica que se agotaron los insumos de un plato en el turno,<br>**When** desmarca la disponibilidad del plato en su panel administrativo,<br>**Then** de forma inmediata y reactiva la carta digital y el visor AR ocultan el botón de pedido o marcan el plato como "Agotado por hoy" para todos los comensales conectados.<br><br>**Scenario 2: Reactivación de plato disponible**<br>**Given** que cocina prepara una nueva tanda del plato previamente agotado,<br>**When** el administrador activa nuevamente la casilla de disponibilidad,<br>**Then** el plato vuelve a mostrarse activo en las cartas digitales de todas las mesas al instante. | EP02 |
| **US19** | Panel de Analítica de Interacciones AR y Platos Populares | Como dueño de restaurante, deseo visualizar métricas de escaneos de QR y visualizaciones AR por plato para identificar qué preparaciones despiertan mayor interés entre mis comensales. | **Scenario 1: Consulta de métricas semanales**<br>**Given** que el administrador ingresa al módulo de reportes de su cuenta,<br>**When** selecciona el periodo de los últimos 7 días,<br>**Then** el sistema presenta un ranking gráfico con los platos más explorados en AR, el promedio de permanencia en la carta y la mesa con mayor actividad.<br><br>**Scenario 2: Descarga de reporte consolidado**<br>**Given** que el restaurante requiere cruzar datos con su sistema de ventas de caja,<br>**When** solicita la exportación de interacciones,<br>**Then** el sistema genera y descarga un resumen en formato CSV con las marcas de tiempo y tipos de interacción por plato. | EP06 |
| **US20** | Gestión de Suscripción Mensual y Métodos de Pago | Como dueño de restaurante, deseo gestionar mi plan de suscripción mensual y registrar mi tarjeta de crédito/débito para mantener activo el servicio de Platter sin interrupciones. | **Scenario 1: Renovación automática de membresía**<br>**Given** que el restaurante se encuentra suscrito a un plan mensual vigente con método de pago registrado,<br>**When** llega la fecha de corte mensual,<br>**Then** la pasarela procesa el cargo del abono recurrente, emite el comprobante de pago digital correspondiente y mantiene la cuenta en estado activo.<br><br>**Scenario 2: Notificación por cobro declinado**<br>**Given** que la tarjeta del cliente no cuenta con fondos suficientes en la fecha de corte,<br>**When** la pasarela reporta el fallo de cobro,<br>**Then** el sistema envía un correo de alerta y otorga un periodo de gracia de 72 horas manteniendo el servicio activo mientras el usuario actualiza sus datos de facturación. | EP06 |
| **US21** | Inferencia Multimodal RESTful con Gemini Vision (Technical Story) | Como Developer, deseo disponer de un servicio RESTful en Spring Boot que reciba la imagen binaria del plato y se comunique con la API de Google Gemini para retornar la metadata estructurada en JSON. | **Scenario 1: Inferencia procesada exitosamente**<br>**Given** que el cliente envía una petición `POST` al endpoint `/api/v1/dishes/analyze` con un archivo de imagen válido en multipart/form-data y token JWT autorizado,<br>**When** el servicio procesa la solicitud con la API externa de IA en menos de 3.5 segundos,<br>**Then** la API responde con código HTTP `200 OK` y un cuerpo JSON con los campos `suggestedName`, `description`, `category`, `ingredients` (array), `allergens` (array) y `estimatedCalories` (rango min-max).<br><br>**Scenario 2: Excedido tiempo de respuesta o fallo de API de IA**<br>**Given** que la API externa experimenta latencia o falta de disponibilidad temporal,<br>**When** la petición excede el tiempo límite de timeout configurado (5000 ms),<br>**Then** el microservicio aplica el patrón Circuit Breaker, responde con código HTTP `503 Service Unavailable` y devuelve una estructura de error estandarizada indicando la opción de reintento. | EP07 |
| **US22** | Despacho y Caché de Activos 3D Optimizados (Technical Story) | Como Developer, deseo implementar un endpoint optimizado para servir modelos 3D (GLB/USDZ) con compresión Draco y cabeceras de caché HTTP agresivas para garantizar cargas WebAR en menos de 1.5 segundos en redes móviles. | **Scenario 1: Petición de activo con compresión y caché activa**<br>**Given** que el visor WebAR solicita un activo 3D mediante petición `GET` a `/api/v1/assets/models/{modelId}.glb`,<br>**When** el servidor resuelve el archivo optimizado desde el almacenamiento de objetos,<br>**Then** responde con código HTTP `200 OK`, cabecera `Content-Type: model/gltf-binary`, cabecera `Cache-Control: public, max-age=31536000, immutable` y tamaño comprimido inferior a 3.0 MB.<br><br>**Scenario 2: Validación de caché no modificada (ETag / If-None-Match)**<br>**Given** que el navegador del comensal ya posee una copia local del modelo y envía una cabecera `If-None-Match` con el ETag correspondiente,<br>**When** el servidor comprueba que el activo no ha variado,<br>**Then** responde inmediatamente con código HTTP `304 Not Modified` sin reenviar el cuerpo binario, minimizando el consumo de datos móviles del comensal. | EP07 |

---

## 3.3. Impact Mapping.

A continuación, se presenta el Impact Mapping de Platter, una representación estratégica elaborada en la herramienta **UXPressia** que alinea los objetivos de negocio (Business Goals) con los usuarios clave (Personas), los cambios de comportamiento que esperamos provocar (Impacts) y las características del producto que construiremos (Deliverables), vinculándolos directamente con nuestras User Stories.

![Impact Mapping](./assets/impact-mapping.png)

*(Nota: En la herramienta UXPressia se ha construido el diagrama completo en donde se observa:*

* **Business Goal:** Lograr que el 75% de los comensales en mesas piloto visualicen al menos un plato en Realidad Aumentada y afiliar a 50 restaurantes en los primeros 3 meses.
* **Personas:** Dueño / Administrador de Restaurante, Comensal en Mesa.
* **Impacts:** "Digitalizar la carta en minutos usando fotos y autocompletado con IA", "Equipar mesas con códigos QR listos para imprimir", "Ver platos en 3D sobre la mesa a escala 1:1 sin descargar apps", "Revisar ingredientes y alérgenos antes de ordenar".
* **Deliverables:** Autocompletado con Gemini Vision, Generador de códigos QR para mesas, Visor WebAR sin instalación, Filtro de alérgenos y ficha de ingredientes).


---

## 3.4. Product Backlog.

El **Product Backlog** de Platter consolida y prioriza todas las User Stories del sistema utilizando la técnica ágil de estimación relativa en **Story Points** fundamentada en la secuencia modificada de Fibonacci (**1, 2, 3, 5, 8**). 

El orden del backlog está estrictamente determinado por el **Valor de Negocio**: la Landing Page (adquisición de prospectos tempranos) y el núcleo funcional mínimo viable (MVP compuesto por la captura con IA y el visor WebAR sin fricción) se posicionan en los primeros lugares del backlog para permitir validaciones de mercado tempranas desde el Sprint 1. Las tareas de configuración de pagos o analítica avanzada se reservan para etapas posteriores una vez validada la propuesta central.

| # Orden | User Story Id | Título | Descripción | Story Points (1 / 2 / 3 / 5 / 8) |
| :---: | :---: | :--- | :--- | :---: |
| **1** | **US01** | Visualización de Propuesta de Valor y Demostrador WebAR | Como visitante del sitio web estático, deseo experimentar una demostración interactiva de Realidad Aumentada desde mi dispositivo para comprobar la efectividad de la carta 3D antes de registrar mi negocio. | **5** |
| **2** | **US04** | Formulario de Solicitud de Piloto Gratuito | Como visitante del segmento dueño de restaurante, deseo enviar mis datos de contacto y nombre de mi local comercial para solicitar una prueba piloto gratuita de 14 días con mi carta. | **2** |
| **3** | **US02** | Sección de Beneficios, Métricas de Retorno (ROI) y Casos de Uso | Como visitante del segmento dueño de restaurante, deseo revisar estadísticas del impacto de la Realidad Aumentada en ventas y testimonios de restaurantes piloto para fundamentar mi decisión de afiliación. | **2** |
| **4** | **US03** | Consulta de Planes de Suscripción y Calculadora MYPE | Como visitante del segmento dueño de restaurante, deseo consultar los planes tarifarios y calcular el costo según el número de mesas de mi local para evaluar la asequibilidad de la inversión. | **3** |
| **5** | **US13** | Acceso Inmediato a Carta Digital sin Registro ni App | Como comensal en la mesa del restaurante, deseo acceder a la carta digital interactiva inmediatamente al escanear el código QR con mi teléfono móvil sin tener que crear cuentas ni instalar aplicaciones. | **3** |
| **6** | **US14** | Proyección del Plato en Realidad Aumentada (WebAR) a Escala 1:1 | Como comensal, deseo proyectar el modelo 3D del plato sobre la superficie de mi mesa con dimensiones reales a escala 1:1 para evaluar su presentación y tamaño antes de solicitarlo. | **8** |
| **7** | **US05** | Carga Fotográfica de Plato para Análisis Automatizado | Como dueño de restaurante, deseo cargar una fotografía de un plato recién preparado desde la cámara o galería de mi móvil para iniciar el proceso de digitalización con Inteligencia Artificial. | **3** |
| **8** | **US06** | Sugerencia Inteligente de Descripción y Categoría con IA | Como dueño de restaurante, deseo que la plataforma analice la imagen del plato mediante Inteligencia Artificial multimodal para obtener una descripción comercial atractiva y su categoría sugerida en segundos. | **5** |
| **9** | **US07** | Detección Automática de Ingredientes Clave y Alérgenos | Como dueño de restaurante, deseo que el sistema identifique los ingredientes principales y marque alérgenos normados a partir de la foto del plato para cumplir con las regulaciones de seguridad alimentaria. | **5** |
| **10** | **US10** | Asignación de Modelo 3D a Escala Real desde Biblioteca | Como dueño de restaurante, deseo vincular un modelo 3D fotorrealista a escala 1:1 desde la biblioteca gastronómica predeterminada de Platter para que el plato disponga de visualización en Realidad Aumentada sin costo adicional de modelado. | **3** |
| **11** | **US11** | Generación de Códigos QR con Identificador de Mesa | Como dueño de restaurante, deseo generar códigos QR individuales asociados a cada una de las mesas de mi restaurante para que los comensales accedan de manera contextualizada a la carta digital. | **3** |
| **12** | **US12** | Descarga de Plantilla de QR en Alta Calidad para Impresión | Como dueño de restaurante, deseo descargar los códigos QR en un formato gráfico listo para imprenta con el logotipo y nombre de mi negocio para colocarlos en soportes físicos de mesa. | **2** |
| **13** | **US09** | Validación y Ajuste Manual de Ficha Gastronómica | Como dueño de restaurante, deseo revisar, editar y confirmar los textos, ingredientes y alérgenos sugeridos por la IA antes de que el plato sea visible en la carta digital. | **3** |
| **14** | **US16** | Comparación Visual de Dimensiones del Plato en Mesa | Como comensal, deseo mover, rotar e inspeccionar la proyección 3D del plato junto a cubiertos o vasos reales sobre mi mesa para constatar su volumen y porción real. | **3** |
| **15** | **US15** | Filtrado de Platos por Alérgenos y Preferencias Dietarias | Como comensal con requerimientos dietarios o alergias alimentarias, deseo filtrar los platos de la carta excluyendo alérgenos específicos para encontrar opciones seguras para mi consumo. | **3** |
| **16** | **US17** | Consulta de Ingredientes y Advertencias de Contaminación Cruzada | Como comensal alérgico, deseo acceder a la ficha informativa detallada del plato para revisar posibles trazas de ingredientes y notas de advertencia de cocina. | **2** |
| **17** | **US08** | Estimación Calórica y Ficha Nutricional Automatizada | Como dueño de restaurante, deseo contar con una estimación aproximada del rango calórico y macronutrientes del plato para ofrecer información nutricional transparente a mis comensales. | **3** |
| **18** | **US18** | Actualización de Disponibilidad de Platos en Tiempo Real | Como dueño de restaurante, deseo marcar platos como "Agotado" con un solo toque desde mi panel para que los comensales no intenten ordenar preparaciones que ya no están disponibles en cocina. | **2** |
| **19** | **US21** | Inferencia Multimodal RESTful con Gemini Vision (Technical Story) | Como Developer, deseo disponer de un servicio RESTful en Spring Boot que reciba la imagen binaria del plato y se comunique con la API de Google Gemini para retornar la metadata estructurada en JSON. | **8** |
| **20** | **US22** | Despacho y Caché de Activos 3D Optimizados (Technical Story) | Como Developer, deseo implementar un endpoint optimizado para servir modelos 3D (GLB/USDZ) con compresión Draco y cabeceras de caché HTTP agresivas para garantizar cargas WebAR en menos de 1.5 segundos en redes móviles. | **5** |
| **21** | **US19** | Panel de Analítica de Interacciones AR y Platos Populares | Como dueño de restaurante, deseo visualizar métricas de escaneos de QR y visualizaciones AR por plato para identificar qué preparaciones despiertan mayor interés entre mis comensales. | **5** |
| **22** | **US20** | Gestión de Suscripción Mensual y Métodos de Pago | Como dueño de restaurante, deseo gestionar mi plan de suscripción mensual y registrar mi tarjeta de crédito/débito para mantener activo el servicio de Platter sin interrupciones. | **5** |

El backlog completo ha sido registrado y organizado en la herramienta de gestión ágil Jira Software del equipo:
* **Enlace público al Product Backlog en Jira:** [https://marcoanakasone-1789856155139.atlassian.net/jira/software/projects/SCRUM/boards/1/backlog](https://marcoanakasone-1789856155139.atlassian.net/jira/software/projects/SCRUM/boards/1/backlog)



# Capítulo IV: Strategic-Level Software Design

## 4.1. Strategic-Level Attribute-Driven Design.

### 4.1.1. Design Purpose

El propósito del diseño arquitectónico para **Platter** consiste en establecer la estructura estratégica, táctica y operativa de una plataforma SaaS concebida para revolucionar la digitalización de cartas gastronómicas en el segmento de micro y pequeñas empresas (MYPE) y brindar una experiencia inmersiva sin fricción a los comensales en salón mediante Realidad Aumentada (WebAR) e Inteligencia Artificial multimodal.

La problemática diagnosticada en los capítulos precedentes evidencia que la mayoría de los restaurantes MYPE carecen de recursos técnicos y financieros para implementar cartas interactivas tridimensionales: los métodos actuales basados en cartas físicas o documentos PDF accesibles mediante códigos QR estándar resultan estáticos, tediosos de actualizar y fallan en comunicar la volumetría real, ingredientes críticos y alérgenos de los platos. Por otro lado, las soluciones de Realidad Aumentada pioneras en el mercado internacional demandan procesos de fotogrametría manual con costos prohibitivos (superiores a £49 por plato) y exigen que el comensal descargue aplicaciones móviles nativas pesadas en su teléfono personal, generando una severa fricción que desalienta su uso en mesa.

Frente a esta brecha, el diseño de software de Platter satisface las necesidades de negocio y de los segmentos objetivo a través de los siguientes pilares de arquitectura:
1. **Digitalización Automatizada e Inteligente:** Un pipeline de procesamiento en el backend que consume la API de **Google Gemini Vision** para transformar una simple fotografía tomada con un smartphone en una ficha gastronómica estructurada (nombre comercial, descripción sensorial, desglose de ingredientes, detección de alérgenos normados y cálculo calórico estimado) en un tiempo inferior a 3.5 segundos.
2. **Biblioteca Gastronómica 3D Normalizada:** Un catálogo centralizado de modelos tridimensionales fotorrealistas optimizados en formatos estándar (GLB y USDZ) calibrados a escala métrica 1:1, eliminando la barrera económica del modelado individual para restaurantes pequeños.
3. **Acceso WebAR sin Descargas ni Registro:** Una arquitectura de consumo público sin estado que permite a cualquier comensal escanear un código QR en mesa y proyectar de manera instantánea el plato en Realidad Aumentada mediante estándares web nativos (**WebXR Device API** para Android y **AR Quick Look** para iOS), prescindiendo totalmente de autenticación y de descargas de aplicaciones en tiendas de apps.
4. **Arquitectura Limpia y Modular en Spring Boot:** Un núcleo de servicios RESTful desacoplados, resilientes y de alta disponibilidad construidos sobre Java 21, siguiendo los principios de Domain-Driven Design (DDD) y garantizando escalabilidad elástica ante la concurrencia propia de los horarios pico de salón.

---

### 4.1.2. Attribute-Driven Design Inputs.

El proceso de diseño arquitectónico se fundamenta en la metodología **Attribute-Driven Design (ADD 3.0)** desarrollada por el *Software Engineering Institute (SEI)*. ADD es un enfoque sistemático basado en atributos de calidad que guía la toma de decisiones mediante iteraciones sucesivas, donde las estructuras y patrones arquitectónicos se eligen con el propósito explícito de satisfacer los requerimientos funcionales críticos, los atributos de calidad priorizados y las restricciones de entorno y negocio.

A continuación, se documentan los tres insumos esenciales que alimentan el proceso de diseño arquitectónico de Platter: la Funcionalidad Primaria (Primary Functionality), los Escenarios de Atributos de Calidad (Quality Attribute Scenarios) y las Restricciones del Sistema (Constraints).

#### 4.1.2.1. Primary Functionality (Primary User Stories).

En concordancia con las pautas del método ADD, no todos los requerimientos funcionales poseen la misma relevancia para la arquitectura. En esta sección se seleccionan aquellas Historias de Usuario del Product Backlog que introducen los mayores desafíos estructurales, determinan la asignación de responsabilidades entre capas y contenedores, o imponen integraciones críticas con sistemas externos de procesamiento en la nube e inferencia de Inteligencia Artificial.

| Epic / User Story ID | Título | Descripción | Criterios de Aceptación | Relacionado con (Epic ID) |
| :--- | :--- | :--- | :--- | :--- |
| **US06** | Sugerencia Inteligente de Descripción y Categoría con IA | Como dueño de restaurante, deseo que la plataforma analice la imagen del plato mediante Inteligencia Artificial multimodal para obtener una descripción comercial atractiva y su categoría sugerida en segundos. | **Scenario 1: Inferencia exitosa de descripción**<br>**Given** que una fotografía gastronómica válida ha sido cargada al sistema,<br>**When** se invoca el motor de análisis multimodal de Gemini Vision,<br>**Then** el sistema retorna una propuesta de nombre comercial, categoría sugerida y descripción sensorial de entre 40 y 70 palabras adaptada a la gastronomía local.<br><br>**Scenario 2: Fotografía difusa o no gastronómica**<br>**Given** que el usuario subió una imagen con baja iluminación o sin elementos gastronómicos discernibles,<br>**When** el motor de IA procesa la imagen y obtiene un nivel de confianza menor al umbral mínimo,<br>**Then** el sistema solicita amablemente al usuario una nueva toma más clara o la opción de completar los datos de forma manual. | EP02 |
| **US10** | Asignación de Modelo 3D a Escala Real desde Biblioteca | Como dueño de restaurante, deseo vincular un modelo 3D fotorrealista a escala 1:1 desde la biblioteca gastronómica predeterminada de Platter para que el plato disponga de visualización en Realidad Aumentada sin costo adicional de modelado. | **Scenario 1: Asociación automática por categoría**<br>**Given** que el plato registrado pertenece a una categoría con modelos estándar disponibles (ej. cebiche, lomo saltado, hamburguesa artesanal),<br>**When** el sistema clasifica el plato,<br>**Then** vincula por defecto el modelo 3D optimizado (GLB/USDZ) configurado con dimensiones físicas exactas en metros.<br><br>**Scenario 2: Selección manual alternativa**<br>**Given** que el usuario desea asignar una representación 3D diferente a la sugerida,<br>**When** navega por la galería de modelos gastronómicos y escoge un activo alternativo,<br>**Then** la asociación se actualiza y la vista previa 3D refleja el nuevo modelo elegido. | EP02 |
| **US11** | Generación de Códigos QR con Identificador de Mesa | Como dueño de restaurante, deseo generar códigos QR individuales asociados a cada una de las mesas de mi restaurante para que los comensales accedan de manera contextualizada a la carta digital. | **Scenario 1: Generación masiva por rango de mesas**<br>**Given** que el administrador ingresa la cantidad de mesas de su salón (ej. Mesas 1 a 20),<br>**When** solicita la generación de códigos QR,<br>**Then** el sistema genera identificadores criptográficos únicos vinculados al restaurante y al número de mesa correspondiente, dejándolos listos para consulta y descarga.<br><br>**Scenario 2: Incorporación de una nueva mesa**<br>**Given** que el local amplía su capacidad con una mesa adicional,<br>**When** el administrador añade la mesa identificada como "Terraza 01",<br>**Then** se genera de forma instantánea el QR respectivo sin alterar los códigos de las mesas previamente existentes. | EP03 |
| **US13** | Acceso Inmediato a Carta Digital sin Registro ni App | Como comensal en la mesa del restaurante, deseo acceder a la carta digital interactiva inmediatamente al escanear el código QR con mi teléfono móvil sin tener que crear cuentas ni instalar aplicaciones. | **Scenario 1: Escaneo y carga exitosa en navegador**<br>**Given** que el comensal escanea el código QR de su mesa mediante la aplicación de cámara de su smartphone (iOS o Android),<br>**When** se abre la URL en el navegador móvil predeterminado,<br>**Then** la carta del restaurante carga en menos de 2 segundos, mostrando el número de mesa identificada y las categorías del menú sin solicitar autenticación previa.<br><br>**Scenario 2: Acceso a mesa no configurada o inactiva**<br>**Given** que un comensal escanea un código QR deshabilitado o con identificador inválido,<br>**When** el navegador intenta resolver la dirección web,<br>**Then** el sistema muestra una pantalla amigable indicando que la mesa no está activa y ofreciendo visualizar el menú general del restaurante. | EP04 |
| **US14** | Proyección del Plato en Realidad Aumentada (WebAR) a Escala 1:1 | Como comensal, deseo proyectar el modelo 3D del plato sobre la superficie de mi mesa con dimensiones reales a escala 1:1 para evaluar su presentación y tamaño antes de solicitarlo. | **Scenario 1: Activación de Realidad Aumentada en Android (WebXR / Scene Viewer)**<br>**Given** que el comensal navega en la carta desde un dispositivo Android compatible con ARCore,<br>**When** selecciona "Ver en Realidad Aumentada" en la ficha de un plato,<br>**Then** el navegador ejecuta el visor nativo sin aplicaciones intermedias, detecta la superficie horizontal de la mesa y ubica el modelo 3D fotorrealista a escala 1:1.<br><br>**Scenario 2: Activación de Realidad Aumentada en iOS (AR Quick Look)**<br>**Given** que el comensal utiliza un dispositivo iPhone o iPad compatible con ARKit,<br>**When** activa la visualización en AR,<br>**Then** iOS despliega el visor AR Quick Look en formato USDZ permitiendo interactuar con el modelo y rotarlo 360 grados sobre el mantel.<br><br>**Scenario 3: Dispositivo móvil sin compatibilidad AR**<br>**Given** que el smartphone del comensal no posee soporte de hardware para Realidad Aumentada,<br>**When** intenta ingresar a la experiencia AR,<br>**Then** el sistema activa automáticamente un visor 3D interactivo en pantalla donde puede rotar y hacer zoom sobre el plato en 360°. | EP04 |
| **US21** | Inferencia Multimodal RESTful con Gemini Vision (Technical Story) | Como Developer, deseo disponer de un servicio RESTful en Spring Boot que reciba la imagen binaria del plato y se comunique con la API de Google Gemini para retornar la metadata estructurada en JSON. | **Scenario 1: Inferencia procesada exitosamente**<br>**Given** que el cliente envía una petición `POST` al endpoint `/api/v1/dishes/analyze` con un archivo de imagen válido en multipart/form-data y token JWT autorizado,<br>**When** el servicio procesa la solicitud con la API externa de IA en menos de 3.5 segundos,<br>**Then** la API responde con código HTTP `200 OK` y un cuerpo JSON con los campos `suggestedName`, `description`, `category`, `ingredients` (array), `allergens` (array) y `estimatedCalories` (rango min-max).<br><br>**Scenario 2: Excedido tiempo de respuesta o fallo de API de IA**<br>**Given** que la API externa experimenta latencia o falta de disponibilidad temporal,<br>**When** la petición excede el tiempo límite de timeout configurado (5000 ms),<br>**Then** el microservicio aplica el patrón Circuit Breaker, responde con código HTTP `503 Service Unavailable` y devuelve una estructura de error estandarizada indicando la opción de reintento. | EP07 |
| **US22** | Despacho y Caché de Activos 3D Optimizados (Technical Story) | Como Developer, deseo implementar un endpoint optimizado para servir modelos 3D (GLB/USDZ) con compresión Draco y cabeceras de caché HTTP agresivas para garantizar cargas WebAR en menos de 1.5 segundos en redes móviles. | **Scenario 1: Petición de activo con compresión y caché activa**<br>**Given** que el visor WebAR solicita un activo 3D mediante petición `GET` a `/api/v1/assets/models/{modelId}.glb`,<br>**When** el servidor resuelve el archivo optimizado desde el almacenamiento de objetos,<br>**Then** responde con código HTTP `200 OK`, cabecera `Content-Type: model/gltf-binary`, cabecera `Cache-Control: public, max-age=31536000, immutable` y tamaño comprimido inferior a 3.0 MB.<br><br>**Scenario 2: Validación de caché no modificada (ETag / If-None-Match)**<br>**Given** que el navegador del comensal ya posee una copia local del modelo y envía una cabecera `If-None-Match` con el ETag correspondiente,<br>**When** el servidor comprueba que el activo no ha variado,<br>**Then** responde inmediatamente con código HTTP `304 Not Modified` sin reenviar el cuerpo binario, minimizando el consumo de datos móviles del comensal. | EP07 |

#### 4.1.2.2. Quality Attributes Scenarios.

Los atributos de calidad representan los requerimientos no funcionales que determinan el éxito operativo, la experiencia del usuario y la robustez del sistema. Para Platter, se han formulado los siguientes escenarios iniciales de calidad que actúan como inputs del proceso de diseño:

1. **Rendimiento y Latencia (Performance):**
   * *Escenario QA-01 (Despacho WebAR):* Cuando un comensal escanea el código QR de una mesa en condiciones normales de red móvil 4G (latencia promedio de 50 ms), el sistema debe descargar el modelo tridimensional comprimido (GLB/USDZ < 3.0 MB) y activar la proyección WebAR sobre la mesa en menos de **1.5 segundos**.
   * *Escenario QA-02 (Inferencia de IA):* Cuando el administrador del restaurante envía una fotografía de un plato desde la app móvil, el servicio de backend debe coordinar la inferencia multimodal con la API de Google Gemini y devolver la ficha técnica estructurada en menos de **3.5 segundos** en el 95% de los casos.
2. **Disponibilidad y Tolerancia a Fallos (Availability & Fault Tolerance):**
   * *Escenario QA-03 (Degradación elegante ante fallos de IA):* Si la API externa de Google Gemini experimenta una caída de servicio o una latencia superior a 5000 ms, el sistema debe abrir el circuito (Circuit Breaker) en menos de 100 ms, responder con código HTTP 503 controlado y permitir que el usuario continúe registrando el plato de manera manual sin bloquear la aplicación móvil ni afectar las operaciones en salón.
   * *Escenario QA-04 (Alta disponibilidad en salón):* El servicio de consulta de cartas por QR y visualización WebAR debe mantener una disponibilidad anual mínima del **99.5%** durante el horario de atención gastronómica (11:00 a 23:00 horas).
3. **Usabilidad y Accesibilidad (Usability):**
   * *Escenario QA-05 (Zero-Friction Access):* Un comensal debe ser capaz de acceder a la carta digital interactiva y activar la visualización 3D en su mesa realizando un máximo de **2 toques** en su pantalla tras el escaneo del código QR físico, sin pantallas intermedias de inicio de sesión, consentimiento de cookies invasivo ni redirección a tiendas de aplicaciones.
4. **Escalabilidad (Scalability):**
   * *Escenario QA-06 (Concurrencia en hora pico):* Durante los horarios pico de almuerzo (13:00 - 15:30) y cena (20:00 - 22:30), el backend debe soportar una carga sostenida de hasta **500 peticiones concurrentes por segundo** de consulta de carta y descarga de metadatos sin que el tiempo de respuesta del servidor exceda los 250 ms.
5. **Seguridad (Security):**
   * *Escenario QA-07 (Control de acceso y protección de activos):* Las operaciones de administración y carga de fotos deben estar estrictamente autenticadas mediante tokens JWT con expiración configurable (1 hora) y algoritmos HMAC-SHA256, mientras que los enlaces de almacenamiento para subida de fotos deben utilizar URLs prefirmadas (Pre-signed URLs) con validez no mayor a 5 minutos.

#### 4.1.2.3. Constraints.

Las restricciones de diseño representan decisiones prefijadas impuestas por el contexto académico, tecnológico y de mercado que acotan el espacio de soluciones posibles:

* **CON-01 (Backend Framework):** El backend de servicios debe desarrollarse utilizando el framework **Spring Boot** sobre la versión **Java 21 LTS**, aplicando patrones de arquitectura limpia y exponiendo interfaces de comunicación estrictamente basadas en **APIs RESTful** con serialización JSON.
* **CON-02 (Estándar WebAR sin Aplicación):** La experiencia de Realidad Aumentada para el comensal debe ejecutarse exclusivamente en el navegador web móvil mediante estándares abiertos (**WebXR Device API / Scene Viewer** para dispositivos Android y **AR Quick Look** sobre Safari para dispositivos iOS), quedando prohibido exigir la instalación de paquetes APK/IPA nativos en el dispositivo del comensal.
* **CON-03 (Aplicación Móvil de Gestión):** La aplicación de gestión operativa para el dueño y administrador de restaurante debe construirse en **Flutter** (Dart), asegurando una experiencia nativa homogénea y acceso directo a la cámara fotográfica del dispositivo tanto en Android (versión 10+) como en iOS (versión 14+).
* **CON-04 (Persistencia y Almacenamiento de Archivos):** La persistencia transaccional de catálogos, restaurantes, mesas y suscripciones debe gestionarse en un motor relacional **PostgreSQL**, mientras que los activos binarios voluminosos (fotografías gastronómicas y modelos 3D en formatos `.glb` y `.usdz`) deben alojarse en un servicio de almacenamiento de objetos en la nube (**Cloud Object Storage**, compatible con Amazon S3 o Google Cloud Storage).
* **CON-05 (Motor de Inferencia de Inteligencia Artificial):** El servicio de análisis gastronómico automatizado debe integrarse con los modelos multimodales **Google Gemini 1.5 Flash / Pro** a través de su API oficial en la nube, optimizando el consumo de cuota y costos por token.
* **CON-06 (Perfil Económico y Técnico MYPE):** La solución está dirigida al mercado gastronómico peruano de micro y pequeñas empresas. Por ende, los costos operativos de infraestructura en la nube deben mantenerse en niveles mínimos (tier gratuito o infraestructura ligera serverless/paas) para viabilizar planes de suscripción mensuales asequibles (entre S/ 49 y S/ 129 al mes).

---

### 4.1.3. Architectural Drivers Backlog.

El **Architectural Drivers Backlog** consolida y prioriza todos los factores determinantes de la arquitectura identificados durante el proceso de diseño con ADD: los Requerimientos Funcionales Primarios (FD), los Atributos de Calidad (QA) y las Restricciones Técnicas (CON). 

El backlog se encuentra ordenado de acuerdo con su nivel de criticidad combinada, posicionando en los primeros lugares aquellos drivers que poseen simultáneamente **Alta Importancia para los Stakeholders (High)** y un **Alto Impacto en la Complejidad Técnica Arquitectónica (High)**.

| Driver ID | Título de Driver | Descripción | Importancia para Stakeholders (High, Medium, Low) | Impacto en Architecture Technical Complexity (High, Medium, Low) |
| :---: | :--- | :--- | :---: | :---: |
| **DRV-01** | Despacho ultrarrápido de modelos 3D WebAR (QA-01) | La descarga y renderizado de modelos 3D en mesa debe realizarse en < 1.5 s sobre redes 4G mediante compresión Draco y caché CDN. | **High** | **High** |
| **DRV-02** | Inferencia resiliente con IA Multimodal (QA-02 / US21) | El análisis de fotos con Gemini Vision debe responder en < 3.5 s e implementar Circuit Breaker ante indisponibilidad externa. | **High** | **High** |
| **DRV-03** | Experiencia WebAR sin instalación (CON-02 / US14) | El comensal debe visualizar platos en escala 1:1 en su mesa directamente desde el navegador (WebXR / Quick Look) sin instalar apps. | **High** | **High** |
| **DRV-04** | Acceso público sin fricción a la carta (QA-05 / US13) | Apertura de carta digital en mesa en < 2 segundos y con máximo 2 toques tras escanear el QR físico, sin requerir login ni registro. | **High** | **Medium** |
| **DRV-05** | Digitalización automatizada de platos (FD-01 / US06) | Generación automática de nombre, descripción sensorial, ingredientes y alérgenos a partir de una foto del plato. | **High** | **High** |
| **DRV-06** | Biblioteca de modelos 3D normalizados 1:1 (FD-02 / US10) | Catálogo precargado de modelos tridimensionales fotorrealistas calibrados a escala física real para evitar costos de modelado a la MYPE. | **High** | **Medium** |
| **DRV-07** | Generación de códigos QR por mesa (FD-03 / US11) | Emisión de identificadores criptográficos únicos y plantillas vectorizadas imprimibles para contextualizar mesas físicas. | **High** | **Medium** |
| **DRV-08** | Filtrado estricto de seguridad alimentaria (FD-04 / US15) | Exclusión inmediata de platos con alérgenos no tolerados según normativas alimentarias y notas de advertencia de cocina. | **High** | **Medium** |
| **DRV-09** | Backend RESTful en Spring Boot Java 21 (CON-01) | Implementación de microservicios o módulos desacoplados bajo arquitectura limpia con Java 21 LTS y contratos RESTful JSON. | **High** | **Medium** |
| **DRV-10** | Alta disponibilidad en salón (QA-04) | Disponibilidad operativa mínima del 99.5% durante el horario de atención gastronómica (11:00 a 23:00 hrs). | **High** | **High** |
| **DRV-11** | Escalabilidad elástica en horas pico (QA-06) | Capacidad para procesar hasta 500 peticiones concurrentes/segundo en horas de almuerzo y cena sin degradar latencia. | **Medium** | **High** |
| **DRV-12** | Seguridad y control de acceso JWT (QA-07) | Autenticación stateless para administradores y aislamiento de datos por restaurante (multi-tenancy a nivel lógico). | **High** | **Medium** |
| **DRV-13** | Almacenamiento híbrido PostgreSQL y Cloud Storage (CON-04) | Datos relacionales en PostgreSQL y archivos binarios pesados (GLB, USDZ, JPG) en Object Storage distribuido. | **Medium** | **Medium** |
| **DRV-14** | Operación económica y asequible para MYPE (CON-06) | Mantenimiento de costos mensuales de infraestructura reducidos para sustentar planes comerciales de bajo costo. | **High** | **Medium** |

---

### 4.1.4. Architectural Design Decisions.

Para dar respuesta a los drivers priorizados, el equipo técnico llevó a cabo un proceso estructurado siguiendo las etapas del **Quality Attribute Workshop (QAW)**. Durante este taller se evaluaron múltiples tácticas y patrones de diseño arquitectónico alternativos, ponderando sus ventajas (*Pros*), desventajas (*Cons*) y compensaciones (*Trade-offs*).

A continuación, se presenta la matriz comparativa **Candidate Pattern Evaluation Matrix** que sintetiza las evaluaciones y fundamenta las decisiones adoptadas:

| Driver ID | Título de Driver | Patrón / Táctica Candidata 1 | Patrón / Táctica Candidata 2 | Patrón / Táctica Candidata 3 | Decisión Arquitectónica Adoptada |
| :---: | :--- | :--- | :--- | :--- | :--- |
| **DRV-01** | Despacho de modelos 3D WebAR | **Despacho directo desde Base de Datos (BLOBs):**<br>• *Pro:* Todo centralizado en una única BD.<br>• *Con:* Degrada catastróficamente la memoria y ancho de banda de la BD relacional con archivos de 2 a 5 MB. | **Almacenamiento de Objetos (S3) con CDN Edge Caching y Compresión Draco:**<br>• *Pro:* Descarga distribuida a nivel geográfico con latencia < 300 ms, cabeceras `Cache-Control: immutable` y reducción del 60% de peso.<br>• *Con:* Requiere configuración de CDN y pipeline de optimización de malla. | **Renderizado remoto en servidor (Pixel Streaming):**<br>• *Pro:* Dispositivos de baja gama no procesan 3D localmente.<br>• *Con:* Costos exorbitantes de servidores GPU en la nube e inviable para comensales en redes móviles peruanas. | **Se adopta el Patrón 2 (Object Storage + CDN + Draco):** Garantiza la latencia < 1.5 s (QA-01), reduce drásticamente el consumo de datos móviles y descarga por completo a la base de datos relacional. |
| **DRV-02** | Inferencia resiliente con IA Multimodal | **Llamada REST Síncrona Bloqueante:**<br>• *Pro:* Implementación trivial y directa.<br>• *Con:* Cualquier lentitud o indisponibilidad de la API de Google bloquea los hilos de Tomcat en Spring Boot y tumba el backend. | **Llamada Síncrona con Circuit Breaker y Timeout (Resilience4j):**<br>• *Pro:* Aísla las fallas externas, corta peticiones si la latencia supera los 5000 ms y activa un fallback a carga manual controlada.<br>• *Con:* Agrega complejidad de configuración de umbrales en el microservicio. | **Arquitectura Asíncrona basada en Eventos (Kafka / RabbitMQ):**<br>• *Pro:* Desacoplamiento total y reintentos automáticos desacoplados.<br>• *Con:* Sobrediseño y complejidad innecesaria para un flujo interactivo donde el dueño espera la respuesta en pantalla. | **Se adopta el Patrón 2 (REST + Circuit Breaker / Fallback):** Protege la disponibilidad del sistema (QA-03) y ofrece una degradación elegante sin sobrecargar la infraestructura con brokers pesados. |
| **DRV-03 / DRV-04** | Experiencia de consumo en mesa | **Aplicación Móvil Nativa obligatoria (Android/iOS):**<br>• *Pro:* Acceso completo a APIs nativas de ARCore y ARKit de alto desempeño.<br>• *Con:* Fricción de instalación inaceptable: el 80% de comensales desiste si tiene que descargar 80 MB para ver una carta. | **WebAR sin instalación (WebXR Device API + Apple AR Quick Look):**<br>• *Pro:* Fricción cero; se activa con 1 toque en el navegador móvil al escanear el QR físico; estándar universal en Android e iOS.<br>• *Con:* Limitaciones de sombreado avanzado frente a motores gráficos nativos. | **Visualización 2D tradicional mediante PDF estático:**<br>• *Pro:* Muy económica y común.<br>• *Con:* No ofrece diferenciación, no muestra el tamaño real del plato (1:1) y perpetúa la incertidumbre del comensal. | **Se adopta el Patrón 2 (WebAR sin instalación):** Cumple con la regla de oro de eliminación de fricción para comensales (QA-05 / CON-02) maximizando la tasa de visualización en mesa. |
| **DRV-09 / DRV-11** | Estilo Arquitectural General | **Monolito Tradicional Acoplado:**<br>• *Pro:* Rápido de arrancar en etapas iniciales.<br>• *Con:* Fuerte acoplamiento entre el módulo de catálogos y el de cobros; escalado rígido que desperdicia recursos en horas valle. | **Monolito Modular con Separación Limpia por Bounded Contexts:**<br>• *Pro:* Despliegue unificado y económico para MYPE (CON-06); límites estrictos de dominio basados en DDD; migración sencilla a microservicios.<br>• *Con:* Requiere rigurosidad en los límites de paquetes e interfaces de dominio. | **Microservicios Distribuidos en Kubernetes:**<br>• *Pro:* Escalado independiente extremo por contenedor.<br>• *Con:* Costo prohibitivo de infraestructura para una fase inicial (CON-06), sobrecarga de red y complejidad operativa desproporcionada. | **Se adopta el Patrón 2 (Monolito Modular / Arquitectura Limpia en Spring Boot):** Equilibrio óptimo entre mantenibilidad estratégica (DDD), bajo costo operativo para MYPE y preparación para desacoplamiento futuro. |

---

### 4.1.5. Quality Attribute Scenario Refinements.

A continuación, se documentan las especificaciones formalmente refinadas según el estándar del SEI para los escenarios de atributos de calidad de mayor prioridad arquitectónica:

**Scenario Refinement for Scenario 1 (Rendimiento en Despacho de Activos 3D WebAR)

| Elemento | Descripción Detallada |
| :--- | :--- |
| **Scenario(s):** | **QA-01 (Despacho de activos 3D WebAR en menos de 1.5 segundos sobre redes móviles)** |
| **Business Goals:** | Incrementar la tasa de conversión en salón logrando que al menos el 75% de comensales proyecten el plato en su mesa sin abandonar la experiencia por tiempos de carga lentos. |
| **Relevant Quality Attributes:** | Latencia, Rendimiento (Performance), Eficiencia de Ancho de Banda. |
| **Stimulus:** | Petición HTTP GET solicitando la descarga del modelo tridimensional (`.glb` o `.usdz`) y su metadata de calibración métrica al momento de presionar "Ver en mi mesa". |
| **Stimulus Source:** | Navegador web móvil del comensal (Chrome en Android o Safari en iOS). |
| **Environment:** | Operación normal en salón de restaurante con red móvil de datos 4G (latencia promedio ~50 ms, ancho de banda ~15-25 Mbps) en horas pico de almuerzo. |
| **Artifact (if Known):** | Componente de entrega de activos (CDN Edge Cache + Cloud Object Storage Bucket) y Visor WebAR (WebXR Device API / model-viewer). |
| **Response:** | El sistema resuelve el archivo binario pre-optimizado con compresión Draco (< 3.0 MB), aplica la caché del navegador (`Cache-Control: public, max-age=31536000, immutable`), inicializa el contexto WebXR y proyecta el plato en Realidad Aumentada a escala 1:1. |
| **Response Measure:** | Tiempo total transcurrido desde el toque del botón hasta la aparición del plato en AR inferior a **1.5 segundos**; tamaño transferido por la red menor a 3.0 MB. |
| **Questions:** | ¿Cómo afecta la calidad de cobertura en interiores de locales rústicos o subterráneos? |
| **Issues:** | Se debe asegurar una vista 3D interactiva orbital en pantalla como fallback si el acelerómetro o la cámara del dispositivo móvil no responden a tiempo. |

---

**Scenario Refinement for Scenario 2 (Disponibilidad y Resiliencia en Inferencia con IA)

| Elemento | Descripción Detallada |
| :--- | :--- |
| **Scenario(s):** | **QA-03 (Degradación elegante y protección por Circuit Breaker ante fallos de la API externa de IA)** |
| **Business Goals:** | Evitar la pérdida de productividad del dueño de restaurante durante el registro de nuevos platos, garantizando la continuidad operativa incluso si los servicios de Google Cloud presentan incidencias. |
| **Relevant Quality Attributes:** | Disponibilidad (Availability), Tolerancia a Fallos (Fault Tolerance), Robustez. |
| **Stimulus:** | Solicitud POST de análisis de fotografía gastronómica enviada desde la app móvil del restaurante. |
| **Stimulus Source:** | Administrador o dueño del restaurante registrando un plato en cocina mediante la app Flutter. |
| **Environment:** | Petición procesada en condiciones donde la API de Google Gemini Vision experimenta alta latencia (> 5000 ms), throttling por cuota o indisponibilidad temporal (HTTP 500 / 503). |
| **Artifact (if Known):** | Microservicio de Backend Spring Boot (`AI Analysis Service`), cliente REST con Resilience4j Circuit Breaker. |
| **Response:** | El Circuit Breaker detecta el fallo o timeout de 5000 ms, interrumpe la espera para evitar el consumo de hilos del servidor, emite una respuesta JSON estructurada informando el estado del servicio externo y habilita inmediatamente el formulario con los campos vacíos para que el usuario ingrese la descripción manualmente. |
| **Response Measure:** | Tiempo de corte y retorno de respuesta al cliente móvil inferior a **100 ms** tras cumplirse el umbral de timeout; 0 hilos de ejecución bloqueados en el pool de Tomcat. |
| **Questions:** | ¿Con qué frecuencia debe verificarse si la API externa se ha recuperado (estado Half-Open)? |
| **Issues:** | Configurar una ventana deslizante de 10 peticiones con un umbral de apertura del circuito al 50% de tasa de fallos y un periodo de espera de 30 segundos en estado Open. |

---

**Scenario Refinement for Scenario 3 (Escalabilidad y Concurrencia en Salón)

| Elemento | Descripción Detallada |
| :--- | :--- |
| **Scenario(s):** | **QA-06 (Concurrencia masiva de consultas de cartas digitales en horarios pico de almuerzo y cena)** |
| **Business Goals:** | Garantizar una experiencia de consulta fluida y simultánea en decenas de restaurantes afiliados sin saturación del backend ni costos exorbitantes de servidor. |
| **Relevant Quality Attributes:** | Escalabilidad (Scalability), Concurrencia, Rendimiento. |
| **Stimulus:** | Oleada repentina de peticiones HTTP GET simultáneas para resolver URLs de códigos QR, cargar categorías de carta y consultar disponibilidad de platos. |
| **Stimulus Source:** | Múltiples comensales (hasta 500 usuarios concurrentes) escaneando códigos QR de mesa en diferentes restaurantes afiliados. |
| **Environment:** | Horario estelar de servicio de restaurante en día festivo o fin de semana (13:30 - 15:00 hrs). |
| **Artifact (if Known):** | API Gateway, Módulo de Catálogo en Spring Boot, Capa de Caché en Memoria (Redis) y Base de Datos PostgreSQL. |
| **Response:** | El sistema atiende el 90% de las consultas de lectura de catálogo y mesas resolviéndolas directamente desde la caché en memoria distribuida (Redis) sin tocar el disco de PostgreSQL, manteniendo conexiones abiertas mediante HTTP Keep-Alive. |
| **Response Measure:** | Latencia de respuesta en el percentil 95 ($P_{95}$) menor a **250 ms**; tasa de errores HTTP 5xx igual a 0.0%; CPU del servidor de aplicaciones por debajo del 70%. |
| **Questions:** | ¿Cuál es la estrategia de invalidación de caché cuando un restaurante agota un plato? |
| **Issues:** | Implementar invalidación reactiva de claves de caché por restaurante/mesa mediante eventos del dominio al momento de actualizar la disponibilidad de un plato. |

---

## 4.2. Strategic-Level Domain-Driven Design.

Para estructurar la complejidad inherente al modelo de negocio de Platter, el equipo adoptó la perspectiva estratégica del diseño guiado por el dominio (**Domain-Driven Design - DDD**). Este enfoque permite descomponer el espacio del problema en modelos conceptuales con límites semánticos estrictos denominados **Bounded Contexts** (Contextos Delimitados), garantizando que cada término del Lenguaje Ubicuo posea un significado unívoco y que los equipos de desarrollo puedan evolucionar componentes de software de manera autónoma y altamente cohesiva.

A continuación, se detalla el proceso sistemático seguido para el modelado estratégico: EventStorming colaborativo, descubrimiento de contextos candidatos, modelado de flujos de mensajes mediante Domain Storytelling, diseño de Bounded Context Canvases y la construcción del mapa de relaciones estratégicas (Context Mapping).

---

### 4.2.1. EventStorming.

El equipo llevó a cabo una sesión de **EventStorming** con una duración de 90 minutos en un tablero virtual interactivo (**Miro**). El objetivo de este taller radicó en plasmar de forma rápida y holística todos los eventos significativos que ocurren en el dominio del negocio gastronómico interactivo de Platter, mapeando la secuencia cronológica de sucesos desde que un restaurante se afilia hasta que un comensal disfruta de la proyección de un plato en su mesa.

Durante la sesión se empleó la notación estandarizada por colores:
* **Domain Events (Post-its Naranjas):** Eventos de negocio en tiempo pasado que representan hechos inmutables ocurridos en el sistema (ej. `DishPhotoUploaded`, `DishAnalyzedByAI`, `QRCodeScanned`).
* **Commands / Triggers (Post-its Azules):** Acciones o decisiones intencionales disparadas por los actores humanos o por el propio sistema (ej. `UploadDishPhoto`, `GenerateTableQR`, `ProjectARModel`).
* **Actors / Users (Post-its Amarillos pequeños):** Los roles que interactúan con el dominio: *Dueño de Restaurante*, *Comensal en Mesa*, *Developer / Sistema*.
* **Aggregates / Entities (Post-its Amarillos grandes):** Conjuntos de entidades de negocio que mantienen consistencia transaccional (ej. `Dish`, `RestaurantTable`, `MenuCatalog`, `ARSession`).
* **Read Models / Views (Post-its Verdes):** Modelos de consulta diseñados para optimizar la visualización de datos en interfaces de usuario (ej. `PublicMenuView`, `AllergenSafetySheet`, `TableInteractionMetrics`).
* **Policies / Business Rules (Post-its Lilas):** Reglas reactivas o condiciones del tipo *"Cuando ocurre X, entonces ejecutar Y"* (ej. *Cuando un plato se marca como agotado, ocultar inmediatamente el botón de proyección AR en todas las mesas*).

A continuación, se representa el flujo conceptual resultante de la sesión de EventStorming en formato secuencial interactivo:

```mermaid
flowchart LR
    subgraph S1["Fase 1: Onboarding y Registro"]
        E1(["RestaurantRegistered"]) --> E2(["SubscriptionPlanSelected"])
        E2 --> E3(["PaymentProcessed"])
        E3 --> E4(["TablesConfigured"])
        E4 --> E5(["QRCodesGenerated"])
    end

    subgraph S2["Fase 2: Digitalización con IA"]
        E6(["DishPhotoCaptured"]) --> E7(["PhotoUploadedToStorage"])
        E7 --> E8(["AIAnalysisRequested"])
        E8 --> E9(["GastronomicDataInferred"])
        E9 --> E10(["AllergensIdentified"])
        E10 --> E11(["3DModelAssociated"])
        E11 --> E12(["DishDraftApproved"])
        E12 --> E13(["DishPublishedToMenu"])
    end

    subgraph S3["Fase 3: Experiencia WebAR en Salón"]
        E14(["TableQRCodeScanned"]) --> E15(["SessionContextResolved"])
        E15 --> E16(["DigitalMenuRendered"])
        E16 --> E17(["AllergenFilterApplied"])
        E17 --> E18(["ARProjectionRequested"])
        E18 --> E19(["Model3DDownloaded"])
        E19 --> E20(["DishRenderedInAR1to1"])
        E20 --> E21(["InteractionLogged"])
    end

    S1 ==> S2 ==> S3
```


---

### 4.2.2. Candidate Context Discovery.

A partir de los eventos del dominio identificados en el EventStorming, el equipo aplicó técnicas sistemáticas de particionamiento estratégico para descubrir los **Bounded Contexts candidatos**:

1. **Técnica *Start-with-Value*:** Se aislaron las partes que constituyen la propuesta de valor diferencial e insustituible de Platter (el núcleo generador de ventaja competitiva). Esto permitió delinear de inmediato el **AI Gastronomic Analysis Context** (el motor de enriquecimiento automático con Gemini Vision) y el **AR Dining Experience Context** (la entrega inmersiva sin fricción para comensales).
2. **Técnica *Look-for-Pivotal-Events*:** Se identificaron aquellos eventos clave que marcan transiciones tajantes de responsabilidad y cambios de ciclo de vida en el negocio:
   * El evento `DishPhotoUploaded` transfiere la responsabilidad de la aplicación móvil de gestión hacia el procesador de Inteligencia Artificial.
   * El evento `DishPublishedToMenu` transfiere el plato desde el taller de edición privada hacia el catálogo público activo.
   * El evento `TableQRCodeScanned` marca la entrada de un comensal anónimo al entorno contextualizado de consumo en salón.
   * El evento `SubscriptionExpired` suspende los privilegios de visualización AR en mesa.

Como resultado de este análisis, se descubrieron y consolidaron **5 Bounded Contexts Candidatos**:

```mermaid
graph TD
    subgraph CoreDomain["Core Domain (Diferenciación de Negocio)"]
        BC1["<b>Dish & Menu Catalog Management Context</b><br>Gestión de cartas, categorías, platos y disponibilidad"]
        BC2["<b>AI Gastronomic Analysis Context</b><br>Inferencia multimodal con Gemini Vision y detección de alérgenos"]
        BC3["<b>AR Dining Experience Context</b><br>Despacho de carta WebAR, visor 3D escala 1:1 e interactividad"]
    end

    subgraph SupportingDomain["Supporting Domain (Soporte Especializado)"]
        BC4["<b>Restaurant & Table Management Context</b><br>Gestión de locales, mesas, generación y renderizado de códigos QR"]
    end

    subgraph GenericDomain["Generic Subdomain (Servicios Reutilizables)"]
        BC5["<b>Subscription & Billing Context</b><br>Planes MYPE, pasarela de cobros recurrentes y control de membresía"]
    end

    BC4 -. "Provee mesas y QR" .-> BC3
    BC2 -. "Suministra metadata enriquecida" .-> BC1
    BC1 -. "Publica platos disponibles" .-> BC3
    BC5 -. "Regula límites operativos" .-> BC4
```


---

### 4.2.3. Domain Message Flows Modeling.

Para verificar cómo colaboran los Bounded Contexts descubiertos ante situaciones reales del negocio, se aplicó la técnica visual de **Domain Storytelling**. Esta metodología permite ilustrar la interacción dinámica entre actores humanos, sistemas de software y objetos de trabajo (mensajes, imágenes, contratos JSON y activos 3D).

A continuación, se modelan los dos escenarios operacionales más críticos de Platter:

**Historia 1:** Flujo de Digitalización y Publicación de Plato con IA

* **Actores:** Dueño / Administrador del Restaurante (Actor humano), App de Gestión (Móvil), Contexto de Análisis de IA, Contexto de Catálogo Gastronómico y Bucket de Objetos.
* **Secuencia de Pasos:**
  1. El Dueño de Restaurante toma la foto del plato recién servido desde la App de Gestión.
  2. La App de Gestión envía el binario de la imagen al servicio de backend mediante petición HTTP Multipart.
  3. El Contexto de Catálogo almacena la imagen en el Bucket de Objetos y emite la orden de análisis al Contexto de IA.
  4. El Contexto de Análisis de IA invoca el motor multimodal de Gemini Vision a través de un Anti-Corruption Layer (ACL).
  5. La IA procesa la imagen y retorna la sugerencia estructurada: nombre comercial, descripción gastronómica, ingredientes identificados, alérgenos normados y calorías estimadas.
  6. El Contexto de Catálogo asocia automáticamente un modelo 3D fotorrealista predeterminado según la categoría asignada.
  7. El Dueño de Restaurante revisa la ficha técnica en su pantalla, realiza modificaciones si lo considera necesario y pulsa "Publicar Plato".
  8. El Contexto de Catálogo emite el evento de dominio `DishPublishedToMenu`, dejando el plato activo para visualización en salón.

```mermaid
sequenceDiagram
    autonumber
    actor Owner as Dueno de Restaurante
    participant App as App Movil (Flutter)
    participant Catalog as Dish & Menu Catalog BC
    participant AI as AI Gastronomic Analysis BC
    participant Gemini as Google Gemini Vision API

    Owner->>App: Captura foto del plato en cocina
    App->>Catalog: POST /api/v1/dishes (Imagen + Metadata inicial)
    Catalog->>AI: Solicitar analisis multimodal de imagen
    AI->>Gemini: POST /v1beta/models/gemini-1.5-flash:generateContent
    Gemini-->>AI: Respuesta JSON (Texto, Ingredientes, Alergenos, Calorias)
    AI-->>Catalog: Metadata gastronomica normalizada
    Note over Catalog: Asociar Modelo 3D predeterminado de la biblioteca
    Catalog-->>App: Ficha tecnica completa en estado Borrador
    Owner->>App: Valida datos y confirma publicacion
    App->>Catalog: PUT /api/v1/dishes/{id}/publish
    Catalog-->>App: Plato oficialmente publicado en la carta
```

---

**Historia 2:** Flujo de Consulta y Proyección WebAR en Mesa por el Comensal

* **Actores:** Comensal en Mesa (Actor humano), Cámara del Smartphone, WebAR Client (Navegador), Contexto de Restaurantes y Mesas, Contexto de Catálogo, CDN / Object Storage.
* **Secuencia de Pasos:**
  1. El Comensal apunta la cámara de su teléfono móvil hacia el código QR ubicado en el soporte físico de su mesa.
  2. El navegador web resuelve la URL contextualizada (`https://platter.menu/r/{restId}/t/{tableId}`).
  3. El Contexto de Restaurantes y Mesas valida la vigencia de la mesa y retorna el identificador del restaurante activo.
  4. El WebAR Client solicita el catálogo vigente al Contexto de Catálogo.
  5. El Comensal navega entre las categorías y selecciona "Ver en Realidad Aumentada" en su plato preferido.
  6. El navegador descarga el activo tridimensional optimizado (`.glb` o `.usdz` < 3.0 MB) directamente desde el CDN Edge Cache.
  7. El motor WebXR detecta la superficie plana de la mesa y proyecta el modelo fotorrealista a escala 1:1, permitiendo al comensal constatar la porción real antes de ordenar al mesero.

```mermaid
sequenceDiagram
    autonumber
    actor Comensal as Comensal en Mesa
    participant Cam as Cámara Smartphone
    participant WebAR as WebAR Client (Browser)
    participant TableBC as Restaurant & Table BC
    participant CatalogBC as Dish & Menu Catalog BC
    participant CDN as CDN / Object Storage

    Comensal->>Cam: Escanea código QR físico en mesa
    Cam->>WebAR: Abre URL contextualizada de la mesa
    WebAR->>TableBC: GET /api/v1/tables/resolve?token={token}
    TableBC-->>WebAR: Mesa válida (Mesa 4, Restaurante El Criollo)
    WebAR->>CatalogBC: GET /api/v1/restaurants/{id}/menu
    CatalogBC-->>WebAR: Catálogo de platos activos con alérgenos
    Comensal->>WebAR: Selecciona plato y pulsa "Ver en mi mesa"
    WebAR->>CDN: GET /assets/models/lomo-saltado.glb
    CDN-->>WebAR: Retorna archivo 3D comprimido con Draco
    WebAR->>Comensal: Proyecta plato en WebAR a escala métrica 1:1 sobre mantel
```

---

### 4.2.4. Bounded Context Canvases.

A continuación, se documenta el diseño sistemático de los **Bounded Context Canvases** para los contextos arquitectónicos clave de Platter, aplicando la estructura formal recomendada por la comunidad internacional de DDD:

**Canvas 1:** Dish & Menu Catalog Management Bounded Context

| Sección del Canvas | Detalle y Especificación Técnica |
| :--- | :--- |
| **Context Overview** | • **Nombre:** Dish & Menu Catalog Management Context<br>• **Propósito:** Administrar el ciclo de vida del catálogo gastronómico, categorías, disponibilidad en tiempo real, vinculación de modelos 3D y fichas técnicas de seguridad alimentaria.<br>• **Clasificación Estratégica:** **Core Domain** (Generador central de valor del producto). |
| **Business Rules & Policies** | 1. Un plato no puede publicarse si carece de nombre, categoría y precio base asignado.<br>2. Si un plato es marcado como "Agotado por hoy", su visibilidad en el visor WebAR se deshabilita de inmediato para todas las mesas.<br>3. Todo plato debe tener al menos una fotografía de referencia y un modelo 3D vinculado (sea propio o asignado desde la biblioteca de muestra).<br>4. La lista de alérgenos debe ser explícita: si un plato no contiene alérgenos reconocidos, debe declararse como libre de alérgenos certificados. |
| **Ubiquitous Language** | • **Dish (Plato):** Entidad fundamental que representa una preparación culinaria con descripción sensorial, precio y modelo 3D.<br>• **MenuCatalog (Catálogo):** Agregado que agrupa los platos activos organizados por categorías para un restaurante.<br>• **Allergen (Alérgeno):** Sustancia de presencia obligatoria en la ficha según normas de salud (gluten, mariscos, frutos secos, lácteos, etc.).<br>• **DracoModelAsset:** Activo tridimensional comprimido para renderizado web eficiente. |
| **Inbound Capabilities** | • `CreateDishDraft(restaurantId, photoUrl)`<br>• `EnrichDishData(dishId, suggestedMetadata)`<br>• `UpdateDishAvailability(dishId, isAvailable)`<br>• `Assign3DModelAsset(dishId, modelId)`<br>• `PublishDish(dishId)` |
| **Outbound Capabilities** | • `GetActiveMenuCatalog(restaurantId): MenuCatalogView`<br>• `GetDishDetail(dishId): DishDetailView` |
| **Dependencies** | • **Recibe datos de:** AI Gastronomic Analysis Context (para autocompletado de descripciones y alérgenos).<br>• **Sirve datos a:** AR Dining Experience Context (para alimentar la carta pública de los comensales). |

---

**Canvas 2:** AI Gastronomic Analysis Bounded Context

| Sección del Canvas | Detalle y Especificación Técnica |
| :--- | :--- |
| **Context Overview** | • **Nombre:** AI Gastronomic Analysis Context<br>• **Propósito:** Orquestar el análisis multimodal automatizado de fotografías gastronómicas mediante Inteligencia Artificial, abstrayendo al resto del sistema de la complejidad de prompts y contratos de la API externa de Google Gemini.<br>• **Clasificación Estratégica:** **Core Domain** (Diferenciador competitivo de alta eficiencia para restaurantes MYPE). |
| **Business Rules & Policies** | 1. La imagen enviada debe ser en formato JPEG o PNG y no superar los 10 MB de tamaño.<br>2. Las peticiones a la API externa de IA deben tener un tiempo de espera máximo (timeout) de 5000 ms.<br>3. Si el nivel de confianza visual del plato es bajo, el servicio debe emitir una advertencia sugiriendo validación manual.<br>4. Los textos sensoriales autogenerados deben mantener un tono apetitoso, formal y adaptado al léxico culinario regional. |
| **Ubiquitous Language** | • **ImagePayload:** Archivo binario optimizado enviado para inferencia visual.<br>• **PromptTemplate:** Estructura de instrucciones de ingeniería de contexto enviada a Gemini Vision solicitando schema JSON estricto.<br>• **NutritionalEstimate:** Rango calórico y macronutrientes inferidos a partir de los ingredientes detectados.<br>• **CircuitBreakerState:** Estado de salud del enlace hacia el servicio externo de IA (Closed, Open, Half-Open). |
| **Inbound Capabilities** | • `AnalyzeGastronomicImage(imageBytes): InferredGastronomicMetadata` |
| **Outbound Capabilities** | • Emisión de eventos: `GastronomicInferenceCompleted`, `GastronomicInferenceFailed`. |
| **Dependencies** | • **Consume de:** API externa de Google Gemini 1.5 Flash / Pro a través de un Anti-Corruption Layer (ACL).<br>• **Responde a:** Dish & Menu Catalog Management Context. |

---

**Canvas 3:** AR Dining Experience Bounded Context

| Sección del Canvas | Detalle y Especificación Técnica |
| :--- | :--- |
| **Context Overview** | • **Nombre:** AR Dining Experience Context<br>• **Propósito:** Proporcionar la experiencia de navegación de carta y visualización 3D en mesa sin autenticación para los comensales, optimizando la entrega de modelos tridimensionales y el filtrado por seguridad alimentaria.<br>• **Clasificación Estratégica:** **Core Domain** (El canal de interacción directa con el consumidor final). |
| **Business Rules & Policies** | 1. El acceso debe ser anónimo y contextualizado exclusivamente por el token criptográfico de la mesa física escaneada.<br>2. El renderizado en Realidad Aumentada debe bloquear el escalado libre para garantizar que el modelo se proyecte a escala métrica real 1:1.<br>3. Los filtros por alérgenos tienen precedencia absoluta en la vista: si un plato contiene un alérgeno marcado como excluido, se oculta de la carta.<br>4. Se registran métricas anónimas de interacción (platos proyectados, tiempo en vista 3D) para analítica de negocio. |
| **Ubiquitous Language** | • **DiningSession:** Sesión efímera de navegación en salón iniciada tras el escaneo de un código QR de mesa.<br>• **ScaleLock:** Restricción matemática de la escena WebXR para forzar la relación de aspecto y dimensiones físicas del plato real.<br>• **AllergenFilter:** Criterio estricto de exclusión dietaria aplicado a la lista de platos.<br>• **ModelViewerSession:** Instancia del motor WebXR o Quick Look ejecutándose en el navegador del teléfono. |
| **Inbound Capabilities** | • `InitializeDiningSession(tableToken)`<br>• `FilterDishesByDietaryRestrictions(sessionToken, allergenList)`<br>• `LogARProjectionEvent(dishId, tableToken, durationSeconds)` |
| **Outbound Capabilities** | • `Stream3DModel(modelId, format): BinaryStream` (optimizado con compresión Draco y cabeceras de caché). |
| **Dependencies** | • **Consulta datos de:** Restaurant & Table Management Context (valida mesa) y Dish & Menu Catalog Management Context (obtiene catálogo). |

---

**Canvas 4:** Restaurant & Table Management Bounded Context

| Sección del Canvas | Detalle y Especificación Técnica |
| :--- | :--- |
| **Context Overview** | • **Nombre:** Restaurant & Table Management Context<br>• **Propósito:** Gestionar la información institucional de los establecimientos gastronómicos, la configuración física de salones y mesas, y la emisión de códigos QR seguros listos para imprenta.<br>• **Clasificación Estratégica:** **Supporting Domain** (Soporta la operación física de los restaurantes). |
| **Business Rules & Policies** | 1. Cada código QR generado debe incorporar un identificador criptográfico único no secuencial para evitar ataques de enumeración de mesas.<br>2. Una mesa puede habilitarse o deshabilitarse temporalmente en el panel (ej. mesa en mantenimiento).<br>3. Las plantillas de códigos QR deben generarse en formatos vectorizados de alta resolución (PDF / PNG HD) incorporando el logotipo del restaurante. |
| **Ubiquitous Language** | • **RestaurantProfile:** Datos fiscales, nombre comercial, dirección física y logotipo del establecimiento.<br>• **DiningTable:** Entidad que representa una mesa física identificada en el salón (ej. "Mesa 1", "Terraza 05").<br>• **TableSecureToken:** Hash criptográfico único asignado al código QR impreso en el soporte de mesa.<br>• **PrintableQRTemplate:** Plantilla gráfica vectorizada formateada para exhibición física. |
| **Inbound Capabilities** | • `RegisterRestaurantProfile(data)`<br>• `ConfigureTablesBatch(restaurantId, startNumber, endNumber)`<br>• `GeneratePrintableQRPDF(restaurantId, tableIds)` |
| **Outbound Capabilities** | • `ResolveTableToken(token): ValidatedTableContext` |
| **Dependencies** | • **Regulado por:** Subscription & Billing Context (valida límites de mesas según el plan contratado). |

---

### 4.2.5. Context Mapping.

El **Context Map** (Mapa de Contextos) formaliza las relaciones estructurales, dependencias organizacionales y patrones de integración entre los diferentes Bounded Contexts de Platter. 

Durante el proceso de diseño, el equipo debatió decisiones estratégicas clave respondiendo a las preguntas de análisis arquitectónico recomendadas por la metodología:
* *¿Qué pasaría si el análisis de IA estuviese dentro del contexto de catálogo?* Generaría un fuerte acoplamiento tecnológico: cualquier cambio en el SDK o en la estructura de prompts de Google Gemini contaminaría el modelo de entidades del catálogo de platos. Por ello, se decidió aislar la IA en su propio Bounded Context.
* *¿Por qué utilizar un Anti-Corruption Layer (ACL)?* La API de Google Gemini es un servicio externo gobernado por un tercero que utiliza sus propias estructuras de datos (`Content`, `Part`, `Candidate`). El patrón **ACL** traduce los esquemas de Google hacia el lenguaje ubicuo interno de Platter, blindando la arquitectura ante roturas de contrato externas.
* *¿Qué relación existe entre Catálogo y la Experiencia WebAR?* La relación es **Upstream / Downstream ($U 
ightarrow D$)** donde el Catálogo actúa como proveedor de servicios mediante un contrato formal **Open Host Service / Published Language (OHS / PL)** basado en endpoints RESTful con esquemas JSON documentados en OpenAPI 3.0.
* *¿Cómo se relaciona la gestión de mesas con las suscripciones?* Existe una relación **Customer / Supplier ($C/S$)** donde el contexto de Suscripciones es Upstream y condiciona las capacidades del contexto de Mesas (ej. no permitir emitir más de 15 mesas si el restaurante cuenta con el plan Básico).

A continuación, se presenta la especificación formal del mapa de relaciones entre los contextos:

```mermaid
flowchart TD
    classDef core fill:#dbeafe,stroke:#1d4ed8,stroke-width:2px,color:#1e3a8a;
    classDef supp fill:#dcfce7,stroke:#15803d,stroke-width:2px,color:#14532d;
    classDef gen fill:#fef9c3,stroke:#a16207,stroke-width:2px,color:#713f12;
    classDef ext fill:#fee2e2,stroke:#b91c1c,stroke-width:2px,color:#7f1d1d;

    Gemini["<b>Google Gemini Vision API</b><br>[External System]"]:::ext
    AI["<b>AI Gastronomic Analysis Context</b><br>[Core Domain]"]:::core
    Catalog["<b>Dish & Menu Catalog Context</b><br>[Core Domain]"]:::core
    AR["<b>AR Dining Experience Context</b><br>[Core Domain]"]:::core
    Table["<b>Restaurant & Table Management Context</b><br>[Supporting Domain]"]:::supp
    Billing["<b>Subscription & Billing Context</b><br>[Generic Subdomain]"]:::gen

    Gemini -->|"[U] Public API / [D] ACL"| AI
    AI -->|"[U] Supplier / [D] Customer"| Catalog
    Catalog -->|"[U] OHS/PL / [D] Consumer"| AR
    Table -->|"[U] Provider / [D] Resolver"| AR
    Billing -->|"[U] Limits / [D] Conformist"| Table
    Billing -->|"[U] Limits / [D] Policy"| Catalog
```

**Patrones de Integración Aplicados:**
1. **Gemini API $
ightarrow$ AI Gastronomic Analysis Context:** Patrón **Anti-Corruption Layer (ACL)**. La clase adaptadora interna `GeminiApiClientAdapter` encapsula la serialización JSON de Google y expone únicamente interfaces del dominio (`GastronomicInferenceService`).
2. **AI Gastronomic Analysis $
ightarrow$ Dish & Menu Catalog:** Patrón **Customer / Supplier (C/S)**. El equipo de Catálogo establece los requerimientos de metadata que el servicio de IA debe abastecer.
3. **Dish & Menu Catalog $
ightarrow$ AR Dining Experience:** Patrón **Open Host Service / Published Language (OHS / PL)**. La API de consulta pública expone recursos REST estandarizados consumidos de forma desacoplada por la WebApp del comensal.
4. **Restaurant & Table Management $
ightarrow$ AR Dining Experience:** Patrón **Upstream / Downstream (U/D)**. La aplicación web del comensal consulta al servicio de mesas para validar criptográficamente el token del QR antes de renderizar la carta.
5. **Subscription & Billing $
ightarrow$ Restaurant / Catalog:** Patrón **Upstream / Downstream (U/D)** con políticas de límite de recursos (cuota de platos y número máximo de mesas activas).


---

## 4.3. Software Architecture.

La arquitectura de software de Platter ha sido diseñada y modelada siguiendo el estándar del **C4 Model** concebido por Simon Brown. Este modelo organiza la descripción arquitectónica en múltiples niveles de abstracción visual progresiva para comunicar con claridad la solución técnica a diferentes audiencias (desde directores de negocio hasta desarrolladores de software).

A continuación, se presentan los diagramas arquitectónicos en sus cuatro dimensiones: el Paisaje General del Sistema (System Landscape), el Diagrama de Contexto del Sistema (Context Level), el Diagrama de Contenedores de Software (Container Level) y el Diagrama de Despliegue en Infraestructura Cloud (Deployment Diagram).

---

### 4.3.1. Software Architecture System Landscape Diagram.

El **System Landscape Diagram** proporciona una panorámica global del ecosistema tecnológico en el que coexiste Platter, mostrando a todos los usuarios humanos, el sistema de software principal y los diversos sistemas externos y proveedores en la nube con los que se comunica.

```mermaid
graph TB
    subgraph Users["Usuarios de la Plataforma"]
        Owner["<b>Dueño / Administrador de Restaurante</b><br>[Person]<br>Registra platos con fotos, genera códigos QR de mesa y gestiona su suscripción."]
        Diner["<b>Comensal en Salón</b><br>[Person]<br>Escanea el QR en mesa, explora la carta digital y visualiza platos en WebAR 1:1."]
        PlatformAdmin["<b>Administrador de Platter</b><br>[Person]<br>Monitorea la salud global, métricas de negocio y biblioteca base de modelos 3D."]
    end

    subgraph PlatterSystem["Plataforma Platter"]
        Platter["<b>Platter SaaS Platform</b><br>[Software System]<br>Permite la digitalización automatizada de cartas con IA y entrega experiencias gastronómicas interactivas en Realidad Aumentada."]
    end

    subgraph ExternalSystems["Sistemas Externos y Servicios Cloud"]
        GeminiAPI["<b>Google Gemini Vision API</b><br>[External System]<br>Servicio de inferencia de IA multimodal que extrae nombres, descripciones sensoriales, alérgenos y calorías."]
        CloudStorage["<b>Cloud Object Storage & CDN</b><br>[External System (AWS S3 / Cloudflare)]<br>Almacena y distribuye con baja latencia fotografías gastronómicas y modelos 3D optimizados (.glb/.usdz)."]
        PaymentGateway["<b>Pasarela de Pagos</b><br>[External System (MercadoPago / Stripe)]<br>Procesa los cobros de suscripción mensual de los restaurantes afiliados."]
        EmailService["<b>Servicio Transaccional de Correo</b><br>[External System (SendGrid)]<br>Envía notificaciones de bienvenida, facturación y reportes de desempeño."]
    end

    Owner -->|Gestiona platos y mesas vía HTTPS| Platter
    Diner -->|Consulta carta y WebAR vía HTTPS/WebXR| Platter
    PlatformAdmin -->|Supervisa sistema vía Dashboard| Platter

    Platter -->|Envía fotos para inferencia visual vía HTTPS/REST| GeminiAPI
    Platter -->|Sube y recupera activos 3D vía S3 API / CDN| CloudStorage
    Platter -->|Procesa suscripciones recurrentes vía HTTPS| PaymentGateway
    Platter -->|Emite comprobantes y alertas vía SMTP/REST| EmailService
```

**Descripción de Componentes e Interacciones:**
* **Platter SaaS Platform:** Núcleo de software responsable de gobernar las identidades, catálogos gastronómicos, resolución de mesas y orquestación de experiencias WebAR.
* **Google Gemini Vision API:** Motor externo de inteligencia artificial que procesa imágenes en tiempo real y extrae la metadata estructurada requerida por la ficha técnica del plato.
* **Cloud Object Storage & CDN:** Infraestructura distribuida que aloja los modelos 3D binarios comprimidos y los entrega directamente a los navegadores móviles de los comensales en menos de 1.5 segundos.
* **Pasarela de Pagos (MercadoPago / Stripe):** Administra los cobros automáticos de suscripción de los restaurantes afiliados según el plan seleccionado.


---

### 4.3.2. Software Architecture Context Level Diagrams.

El **System Context Diagram (C4 Nivel 1)** coloca al sistema de software **Platter** en el centro de atención, definiendo con precisión las fronteras del sistema, sus responsabilidades primordiales y cómo interactúa bidireccionalmente con cada actor y sistema adyacente.

```mermaid
C4Context
    title System Context Diagram - Platter Platform (C4 Level 1)

    Person(restaurantAdmin, "Administrador de Restaurante", "Gestiona la carta, modelos 3D de platos, configuración de mesas y suscripciones.")
    Person(diner, "Comensal", "Escanea códigos QR en mesa para visualizar platos interactivos en Realidad Aumentada (WebAR).")

    Enterprise_Boundary(b0, "Platter Ecosystem") {
        System(platterSystem, "Platter Software System", "Provee la gestión de cartas digitales, proyección WebAR, análisis asistido por IA y administración de salones.")
    }

    System_Ext(geminiAPI, "Google Gemini Vision API", "Motor externo multimodal para análisis y extracción de información de platos e insumos.")
    System_Ext(stripeGateway, "Payment Gateway (Stripe)", "Procesa pagos recurrentes y facturación de suscripciones SaaS.")
    System_Ext(cloudStorage, "Cloud Object Storage", "Repositorio de almacenamiento para texturas y modelos 3D (.glb/.gltf).")

    Rel(restaurantAdmin, platterSystem, "Administra locales, platos y mesas usando", "HTTPS/Web")
    Rel(diner, platterSystem, "Escanea QR y visualiza platillos en", "HTTPS/Mobile Web Browser")
    Rel(platterSystem, geminiAPI, "Envía imágenes de platillos y consultas con", "REST/JSON / HTTPS")
    Rel(platterSystem, stripeGateway, "Gestiona suscripciones y cobros con", "REST/Webhooks")
    Rel(platterSystem, cloudStorage, "Sube y descarga assets 3D optimizados mediante", "HTTPS / S3 API")
```

**Explicación del Diagrama de Contexto:**
* **Fronteras del Sistema:** Platter asume la responsabilidad integral del ciclo de vida gastronómico (desde la captura fotográfica hasta la proyección WebAR). No asume la gestión contable de pedidos de cocina (POS tradicional), sino que se integra como un amplificador visual de venta y seguridad alimentaria en mesa.
* **Interacción Comensal:** El comensal no necesita crearse una cuenta ni autenticarse; su interacción con Platter es puramente anónima y transaccional, contextualizada por el identificador de mesa inyectado por el código QR.
* **Interacción Dueño de Restaurante:** El dueño de restaurante interactúa mediante un canal autenticado con tokens JWT seguros para gestionar el catálogo y monitorear las métricas de interacción de sus comensales.


---

### 4.3.3. Software Architecture Container Level Diagrams.

El **Container Diagram (C4 Nivel 2)** descompone el sistema Platter en sus unidades ejecutables independientes (**Contenedores de Software**), detallando las tecnologías elegidas, las responsabilidades de cada contenedor y los protocolos de comunicación interna y externa.

```mermaid
C4Container
    title Container Diagram - Platter Solution (C4 Level 2)

    Person(restaurantAdmin, "Administrador de Restaurante", "Usuario gestor del restaurante")
    Person(diner, "Comensal", "Cliente en mesa física")

    Container_Boundary(c1, "Platter Platform") {
        Container(adminWeb, "Restaurant Admin Web App", "Vue.js / TypeScript, SPA", "Interfaz web para gestión de menús, códigos QR de mesas y panel de suscripción.")
        Container(arWeb, "AR Dining Web Client", "Three.js / WebXR, PWA", "Cliente web ligero optimizado para navegadores móviles que renderiza platos 3D sin descargas.")
        
        Container(apiGateway, "API Gateway / Reverse Proxy", "Nginx / CloudFront", "Ruta peticiones, aplica rate limiting, balanceo de carga y terminación SSL.")
        
        Container(backendService, "Platter Core REST API", "Spring Boot / ASP.NET Core", "Implementa los Bounded Contexts, la lógica del dominio, control de tokens de mesa y reglas de negocio.")

        ContainerDb(relationalDb, "Relational Database", "PostgreSQL", "Almacena perfiles de restaurantes, configuraciones de mesa, usuarios, cartas y registros de facturación.")
        ContainerDb(cacheDb, "In-Memory Cache", "Redis", "Caché de catálogos frecuentes y control de sesiones activas de mesas.")
    }

    System_Ext(geminiAPI, "Google Gemini Vision API", "Servicio externo de IA multimodal.")
    System_Ext(cloudStorage, "AWS S3 Bucket", "Almacén de modelos 3D (.glb, .usdz) y logos vectoriales.")
    System_Ext(stripeGateway, "Stripe API", "Servicio de pasarela de pagos.")

    Rel(restaurantAdmin, adminWeb, "Accede a", "HTTPS")
    Rel(diner, arWeb, "Interactúa con la experiencia AR en", "HTTPS / WebXR")

    Rel(adminWeb, apiGateway, "Consume servicios vía", "JSON/HTTPS")
    Rel(arWeb, apiGateway, "Consume catálogo y resuelve tokens vía", "JSON/HTTPS")

    Rel(apiGateway, backendService, "Enruta tráfico a", "HTTP/REST")

    Rel(backendService, relationalDb, "Lectura y persistencia con", "JPA / JDBC / TCP")
    Rel(backendService, cacheDb, "Consulta y escribe caché con", "Redis Protocol")
    Rel(backendService, geminiAPI, "Solicita inferencia gastronómica a", "HTTPS/REST")
    Rel(backendService, stripeGateway, "Procesa checkout y webhooks con", "HTTPS/REST")
    Rel(backendService, cloudStorage, "Genera URLs presignadas y gestiona modelos en", "AWS SDK / HTTPS")
    Rel(arWeb, cloudStorage, "Descarga modelos 3D directamente desde", "HTTPS / CDN")
```

**Responsabilidades Técnicas de los Contenedores:**
1. **Landing Page Web App:** Aplicación web estática optimizada para SEO (Next.js / HTML5) desplegada en un CDN edge, diseñada para la adquisición de clientes y demostración interactiva.
2. **Restaurant Admin Mobile App (Flutter):** Aplicación multiplataforma (Android e iOS) instalada por el personal de cocina y administración del restaurante, que proporciona acceso directo a la cámara para la digitalización instantánea de platos.
3. **WebAR Dining Web App:** Single Page Application extremadamente ligera (< 150 KB de bundle inicial) construida con Web Components y el componente `@google/model-viewer`. Se ejecuta en el navegador Safari o Chrome del comensal y se comunica con la GPU del smartphone vía WebXR Device API para proyectar el plato en 3D.
4. **API Gateway (Spring Cloud Gateway / NGINX):** Punto único de entrada para todas las aplicaciones clientes. Aplica reglas de rate limiting, valida tokens JWT antes de alcanzar los servicios de backend y maneja CORS y cabeceras de seguridad.
5. **Platter Core Backend Service (Spring Boot 3.3 / Java 21):** Servicio central que implementa la arquitectura limpia organizada por Bounded Contexts (Catálogo, Mesas, Suscripciones).
6. **AI Ingestion & Analysis Service:** Servicio especializado que implementa el Anti-Corruption Layer y los patrones de resiliencia (Resilience4j Circuit Breaker y Retry) para interactuar de forma segura con la API de Google Gemini Vision.
7. **PostgreSQL 16:** Almacenamiento relacional de datos persistentes con integridad referencial estricta y aislamiento lógico multitenant por restaurante.
8. **Redis Distributed Cache:** Almacenamiento en memoria volátil de alto desempeño que retiene en memoria los menús activos de los restaurantes, reduciendo en más del 85% las consultas directas a la base de datos relacional durante horas pico.
9. **Cloud Object Storage (S3) & CDN:** Repositorio distribuido de archivos binarios estáticos (modelos GLB/USDZ con compresión Draco y fotos JPEG).

---

### 4.3.4. Software Architecture Deployment Diagrams.

El **Deployment Diagram** describe la topología física y lógica de la infraestructura en la nube donde se instancian, ejecutan y escalan los contenedores de software de Platter, detallando los entornos de ejecución, zonas de disponibilidad, balanceadores de carga y esquemas de distribución de contenido.

La infraestructura ha sido diseñada sobre la nube pública de **Amazon Web Services (AWS)** aprovechando servicios gestionados para garantizar alta disponibilidad (99.5%), escalabilidad automática y costos operativos contenidos:

```mermaid
flowchart TD
    classDef client fill:#e0f2fe,stroke:#0284c7,stroke-width:2px,color:#0369a1;
    classDef edge fill:#fef3c7,stroke:#d97706,stroke-width:2px,color:#92400e;
    classDef compute fill:#ede9fe,stroke:#7c3aed,stroke-width:2px,color:#5b21b6;
    classDef data fill:#dcfce7,stroke:#16a34a,stroke-width:2px,color:#166534;
    classDef ext fill:#fee2e2,stroke:#dc2626,stroke-width:2px,color:#991b1b;

    subgraph UserDevices ["Dispositivos de Usuario"]
        BrowserAdmin["<b>Navegador Web / PWA</b><br>Admin Portal (Vue.js)"]:::client
        BrowserDiner["<b>Navegador Móvil</b><br>WebAR Viewer (WebXR / Three.js)"]:::client
    end

    subgraph AWSCloud ["Amazon Web Services (AWS) - Región us-east-1"]
        
        subgraph EdgeTier ["Edge Tier & Content Delivery"]
            CloudFront["<b>Amazon CloudFront (CDN)</b><br>Distribución global y caché periférica"]:::edge
            S3Storage["<b>Amazon S3 Bucket</b><br>Assets web estáticos y modelos 3D (.glb)"]:::edge
        end

        subgraph VPC ["Amazon Virtual Private Cloud (VPC) - 10.0.0.0/16"]
            
            subgraph PublicSubnet ["Public Subnet (Multi-AZ)"]
                ALB["<b>Application Load Balancer (ALB)</b><br>Terminación SSL y enrutamiento"]:::compute
            end

            subgraph PrivateAppSubnet ["Private App Subnet (Multi-AZ)"]
                ECSCluster["<b>Amazon ECS Cluster (AWS Fargate)</b><br>Tareas Docker de Spring Boot (API REST)"]:::compute
            end

            subgraph PrivateDataSubnet ["Private Data Subnet (Multi-AZ)"]
                RDS["<b>Amazon RDS PostgreSQL 16</b><br>Primary DB & Multi-AZ Standby"]:::data
                ElastiCache["<b>Amazon ElastiCache (Redis)</b><br>Caché distribuida de cartas y sesiones"]:::data
            end
        end
    end

    subgraph ExternalServices ["Servicios Externos"]
        GeminiAPI["<b>Google Gemini Vision API</b><br>Inferencia multimodal"]:::ext
        StripeAPI["<b>Stripe API</b><br>Cobro de suscripciones"]:::ext
    end

    %% Conexiones
    BrowserAdmin -->|HTTPS / 443| CloudFront
    BrowserDiner -->|HTTPS / 443| CloudFront
    CloudFront -->|Origin Fetch| S3Storage

    BrowserAdmin -->|HTTPS / REST| ALB
    BrowserDiner -->|HTTPS / REST| ALB

    ALB -->|HTTP / 8080| ECSCluster

    ECSCluster -->|TCP / 5432| RDS
    ECSCluster -->|TCP / 6379| ElastiCache
    ECSCluster -->|Presigned URLs / S3 API| S3Storage
    ECSCluster -->|HTTPS / Inferencia IA| GeminiAPI
    ECSCluster -->|HTTPS / Webhooks| StripeAPI
```

**Aspectos Relevantes de la Infraestructura de Despliegue:**
1. **Red de Distribución Edge (CloudFront / Cloudflare):** Todos los activos estáticos y modelos 3D son cacheados en servidores periféricos (Edge Locations) distribuidos en Latinoamérica, logrando tiempos de descarga de modelos 3D inferiores a 500 ms directamente desde la caché local sin sobrecargar los servidores de aplicaciones.
2. **Virtual Private Cloud (VPC) Segura:** Los contenedores de backend y la base de datos se encuentran alojados en subredes privadas (*Private Subnets*) sin acceso directo desde internet público. Solo el Application Load Balancer (ALB) reside en la subred pública para canalizar las solicitudes externas.
3. **Contenedores Autogestionados (AWS ECS Fargate):** Los microservicios de Spring Boot se empaquetan en imágenes Docker ultraligeras basadas en Alpine Linux / Eclipse Temurin JDK 21. Fargate escala automáticamente el número de tareas (tasks) de 1 a 4 instancias ante picos de concurrencia en horarios de comida.
4. **Base de Datos Gestionada (Amazon RDS Multi-AZ):** Despliegue de PostgreSQL 16 con replicación automática entre zonas de disponibilidad, asegurando respaldo continuo y recuperación ante desastres sin pérdida de datos.
5. **Gestión Segura de Secretos y Roles IAM:** La comunicación con Amazon S3 se autoriza mediante roles IAM asimilados a las tareas de ECS, sin necesidad de quemar credenciales ni llaves de acceso en el código fuente.



# Capítulo V: Tactical-Level Software Design

## 5.1. Bounded Context: Dish & Menu Catalog Management

### 5.1.1. Domain Layer
La capa de dominio encapsula las reglas de negocio, invariantes y entidades fundamentales del catálogo gastronómico, manteniéndose completamente desacoplada de frameworks web, librerías ORM e infraestructura externa.

* **`Dish` (Aggregate Root / Entity):** Representa un plato ofrecido en el restaurante y gobierna su ciclo de vida, precio, información nutricional y disponibilidad.
  * *Atributos:* `id: DishId`, `restaurantId: RestaurantId`, `name: String`, `description: String`, `price: Money`, `category: DishCategory`, `status: DishStatus`, `ingredients: List<Ingredient>`, `allergens: Set<Allergen>`, `nutritionalInfo: NutritionalInfo`, `model3DRef: Model3DReference`, `photoUrl: String`, `createdAt: Instant`.
  * *Métodos:* `updateDetails(name: String, description: String, price: Money): void`, `assignModel3D(modelId: String, scaleFactor: Double): void`, `markAsOutOfStock(): void`, `markAsAvailable(): void`, `publish(): void`, `addAllergen(allergen: Allergen): void`.
* **`DishId` (Value Object):** Identificador unívoco e inmutable del plato basado en UUID v4.
* **`RestaurantId` (Value Object):** Identificador unívoco del restaurante propietario del plato.
* **`Money` (Value Object):** Modela el importe monetario compuesto por `amount: BigDecimal` y `currency: Currency` (PEN). Valida que el monto no sea negativo ni nulo.
* **`Allergen` (Value Object / Enum):** Clasificación estandarizada de sustancias reactivas según directrices sanitarias: `GLUTEN`, `CRUSTACEANS`, `EGGS`, `FISH`, `PEANUTS`, `SOYBEANS`, `MILK`, `NUTS`, `CELERY`, `MUSTARD`, `SESAME`, `SULPHITES`.
* **`NutritionalInfo` (Value Object):** Encapsula el rango estimado de energía y macronutrientes: `minCalories: Integer`, `maxCalories: Integer`, `proteinGrams: Double`, `carbsGrams: Double`, `fatGrams: Double`.
* **`Model3DReference` (Value Object):** Enlace hacia el activo tridimensional optimizado: `modelId: String`, `storageKey: String`, `scaleFactor: Double`, `isStandardSample: Boolean`.
* **`DishCategory` (Enum):** Clasificación del menú: `ENTREE`, `MAIN_COURSE`, `BEVERAGE`, `DESSERT`, `SPECIAL`.
* **`DishStatus` (Enum):** Estados de ciclo de vida del plato: `DRAFT`, `PUBLISHED`, `OUT_OF_STOCK`, `ARCHIVED`.
* **`DishRepository` (Domain Interface):** Puerto del dominio que abstrae las operaciones de persistencia del agregado: `save(dish: Dish): Dish`, `findById(id: DishId): Optional<Dish>`, `findByRestaurantId(restaurantId: RestaurantId): List<Dish>`.
* **`DishPublishedEvent` (Domain Event):** Evento emitido al momento en que un plato es validado y publicado oficialmente en la carta, utilizado para la invalidación de cachés y la sincronización con el visor WebAR.

### 5.1.2. Interface Layer
Expone las capacidades del contexto hacia clientes HTTP/REST mediante controladores Spring MVC conformes con el estándar OpenAPI 3.0.

* **`DishCommandController`:** Controlador REST administrativo que expone endpoints de mutación asegurados mediante tokens JWT:
  * `POST /api/v1/dishes`: Registra un nuevo borrador de plato.
  * `PUT /api/v1/dishes/{id}`: Actualiza los detalles y datos gastronómicos del plato.
  * `PATCH /api/v1/dishes/{id}/availability`: Modifica la disponibilidad en tiempo real (disponible / agotado).
  * `POST /api/v1/dishes/{id}/publish`: Cambia el estado a publicado tras validación.
* **`DishQueryController`:** Controlador REST público que expone endpoints de solo lectura optimizados para comensales en salón:
  * `GET /api/v1/restaurants/{restaurantId}/dishes/active`: Retorna el catálogo activo de platos para la carta digital.
  * `GET /api/v1/dishes/{id}`: Retorna el detalle completo de un plato específico con su activo 3D.
* **`DishDtoMapper`:** Componente encargado de realizar la conversión bidireccional entre entidades de dominio y objetos de transferencia de datos (`CreateDishRequestDto`, `DishResponseDto`, `MenuCatalogViewDto`).

### 5.1.3. Application Layer
Orquesta los casos de uso del catálogo, transformando los comandos de entrada en invocaciones sobre los agregados y gestionando las transacciones de negocio.

* **`CreateDishDraftCommandHandler`:** Procesa la solicitud inicial de registro del plato a partir de una fotografía, creando la entidad en estado `DRAFT`.
* **`EnrichDishWithAIDataCommandHandler`:** Toma los metadatos gastronómicos inferidos (nombre, descripción, alérgenos y calorías) provistos por el contexto de IA y los asocia al plato en borrador.
* **`PublishDishCommandHandler`:** Valida las reglas de publicación (existencia de precio y modelo 3D vinculado), pasa el estado a `PUBLISHED` y dispara el evento de dominio `DishPublishedEvent`.
* **`UpdateDishAvailabilityCommandHandler`:** Conmuta la disponibilidad del plato y ejecuta la invalidación inmediata de claves asociadas en la caché distribuida.
* **`GetActiveMenuQueryHandler`:** Recupera la lista de platos activos para un local, consultando prioritariamente la capa de caché distribuida antes de consultar la persistencia relacional.

### 5.1.4. Infrastructure Layer
Implementa los puertos definidos por el dominio y la persistencia física en PostgreSQL 16 a través de Spring Data JPA, además del control de caché en Redis.

* **`JpaDishRepositoryAdapter`:** Implementación concreta del puerto `DishRepository` que traduce las llamadas de dominio a operaciones de Spring Data JPA utilizando `DishJpaEntity`.
* **`SpringDataDishJpaRepository`:** Interfaz de Spring Data que extiende de `JpaRepository<DishJpaEntity, UUID>`.
* **`DishRedisCacheService`:** Administrador de caché que serializa y recupera proyecciones JSON de cartas activas en Redis, con un TTL de 24 horas y purga reactiva por restaurante.
* **`S3ModelAssetStorageService`:** Componente de infraestructura que se comunica con Amazon S3 para resolver las rutas y pre-firmar accesos a modelos tridimensionales `.glb` y `.usdz`.

### 5.1.6. Bounded Context Software Architecture Component Level Diagrams

```mermaid
C4Component
    title Component Diagram - Dish & Menu Catalog Management Context

    Container_Boundary(catalog_bc, "Dish & Menu Catalog Context (Spring Boot)") {
        Component(command_ctrl, "DishCommandController", "Spring REST Controller", "Expone endpoints administrativos de creación, edición y publicación con JWT.")
        Component(query_ctrl, "DishQueryController", "Spring REST Controller", "Expone catálogo activo y detalle de platos para el cliente WebAR.")
        Component(cmd_handler, "DishCommandHandlerService", "Spring Service (Application)", "Orquesta casos de uso de negocio y coordina transacciones del agregado.")
        Component(query_handler, "CatalogQueryHandlerService", "Spring Service (Application)", "Resuelve consultas de catálogo optimizadas apoyándose en Redis.")
        Component(domain_model, "Dish Aggregate Root", "Java Domain Model", "Encapsula reglas de negocio, alérgenos, precios y estados.")
        Component(repo_adapter, "JpaDishRepositoryAdapter", "Spring Component (Infrastructure)", "Implementa DishRepository persistiendo en PostgreSQL.")
        Component(cache_service, "DishRedisCacheService", "Spring Component (Infrastructure)", "Administra caché de catálogos y revocaciones reactivas.")
    }

    ContainerDb(postgres, "PostgreSQL 16", "Relational Database", "Tablas dishes, dish_allergens, dish_ingredients.")
    ContainerDb(redis, "Redis Cache", "In-Memory DB", "Almacena JSON de cartas activas por restaurante.")

    Rel(command_ctrl, cmd_handler, "Invoca comandos", "Java Call")
    Rel(query_ctrl, query_handler, "Invoca queries", "Java Call")
    Rel(cmd_handler, domain_model, "Aplica reglas de negocio", "Domain Call")
    Rel(cmd_handler, repo_adapter, "Persiste agregado", "Java Interface")
    Rel(cmd_handler, cache_service, "Invalida caché al mutar", "Java Call")
    Rel(query_handler, cache_service, "Consulta primero", "Redis Protocol")
    Rel(query_handler, repo_adapter, "Fallback si miss", "Java Interface")
    Rel(repo_adapter, postgres, "Lee/Escribe vía JPA", "JDBC/SQL")
    Rel(cache_service, redis, "Guarda claves con TTL", "TCP/RESP")
```

### 5.1.7. Bounded Context Software Architecture Code Level Diagrams

#### 5.1.7.1. Bounded Context Domain Layer Class Diagrams

```mermaid
classDiagram
    class Dish {
        -DishId id
        -RestaurantId restaurantId
        -String name
        -String description
        -Money price
        -DishCategory category
        -DishStatus status
        -List~Ingredient~ ingredients
        -Set~Allergen~ allergens
        -NutritionalInfo nutritionalInfo
        -Model3DReference model3DRef
        -String photoUrl
        -Instant createdAt
        +updateDetails(name: String, desc: String, price: Money) void
        +assignModel3D(modelId: String, scale: Double) void
        +markAsOutOfStock() void
        +markAsAvailable() void
        +publish() void
        +addAllergen(allergen: Allergen) void
    }

    class DishId {
        -UUID value
        +getValue() UUID
    }

    class RestaurantId {
        -UUID value
        +getValue() UUID
    }

    class Money {
        -BigDecimal amount
        -String currency
        +getAmount() BigDecimal
    }

    class NutritionalInfo {
        -Integer minCalories
        -Integer maxCalories
        -Double proteinGrams
        -Double carbsGrams
        -Double fatGrams
    }

    class Model3DReference {
        -String modelId
        -String storageKey
        -Double scaleFactor
        -Boolean isStandardSample
    }

    class Allergen {
        <<enumeration>>
        GLUTEN
        CRUSTACEANS
        EGGS
        FISH
        PEANUTS
        SOYBEANS
        MILK
        NUTS
    }

    class DishStatus {
        <<enumeration>>
        DRAFT
        PUBLISHED
        OUT_OF_STOCK
        ARCHIVED
    }

    class DishRepository {
        <<interface>>
        +save(dish: Dish) Dish
        +findById(id: DishId) Optional~Dish~
        +findByRestaurantId(restaurantId: RestaurantId) List~Dish~
    }

    Dish *-- DishId
    Dish *-- RestaurantId
    Dish *-- Money
    Dish *-- NutritionalInfo
    Dish *-- Model3DReference
    Dish --> DishStatus
    Dish o-- Allergen
    DishRepository ..> Dish : administra
```
### 5.1.7.2. Bounded Context Database Design Diagram

```mermaid
erDiagram
    DISHES ||--o{ DISH_ALLERGENS : "contiene"
    DISHES ||--o{ DISH_INGREDIENTS : "compuesto por"

    DISHES {
        uuid id PK
        uuid restaurant_id
        varchar name
        text description
        numeric price_amount
        varchar price_currency
        varchar category
        varchar status
        int min_calories
        int max_calories
        numeric protein_grams
        numeric carbs_grams
        numeric fat_grams
        varchar model3d_id
        varchar model3d_storage_key
        numeric model3d_scale_factor
        boolean is_standard_sample
        varchar photo_url
        timestamp created_at
        timestamp updated_at
    }

    DISH_ALLERGENS {
        uuid id PK
        uuid dish_id FK
        varchar allergen_name
    }

    DISH_INGREDIENTS {
        uuid id PK
        uuid dish_id FK
        varchar name
        boolean is_highlighted
    }
```
## 5.2. Bounded Context: AI Gastronomic Analysis

En esta sección se especifica el diseño táctico del motor de inferencia y extracción gastronómica automatizada con Inteligencia Artificial multimodal, aislando la complejidad de Google Gemini mediante una Capa Anticorrupción (ACL) y protegiendo el backend con patrones de resiliencia.

### 5.2.1. Domain Layer
Modela el núcleo de extracción de conocimiento culinario a partir de imágenes fotográficas, manteniéndose agnóstico de formatos externos y dependencias de la nube.

* **`GastronomicAnalysisRequest` (Aggregate Root / Entity):** Representa la transacción de análisis visual solicitada por un restaurante.
  * *Atributos:* `requestId: UUID`, `restaurantId: UUID`, `imageHash: String`, `executionStatus: AnalysisStatus`, `inferredMetadata: InferredMetadata`, `createdAt: Instant`.
  * *Métodos:* `completeAnalysis(metadata: InferredMetadata): void`, `failAnalysis(reason: String): void`, `markFallbackTriggered(): void`.
* **`InferredMetadata` (Value Object):** Encapsula los atributos gastronómicos inferidos por el modelo multimodal: `suggestedName: String`, `sensoryDescription: String`, `suggestedCategory: String`, `identifiedIngredients: List<String>`, `detectedAllergens: Set<String>`, `estimatedCaloriesRange: String`, `confidenceScore: Double`.
* **`AnalysisStatus` (Enum):** Estados del flujo de procesamiento: `PENDING`, `COMPLETED`, `FAILED`, `FALLBACK_TRIGGERED`.
* **`GastronomicInferenceService` (Domain Interface):** Puerto del dominio que declara la capacidad de inferencia visual: `analyzeDishImage(imageBytes: byte[], mimeType: String): InferredMetadata`.
* **`GastronomicInferenceCompletedEvent` (Domain Event):** Evento emitido cuando los datos estructurados son generados exitosamente.

### 5.2.2. Interface Layer
Expone el punto de entrada para que las aplicaciones cliente envíen fotografías para procesamiento inteligente.

* **`AIGastronomicAnalysisController`:** Expone el endpoint `POST /api/v1/dishes/analyze` que recibe la fotografía del plato en `multipart/form-data`. Responde con código `200 OK` y el JSON estructurado, o `503 Service Unavailable` controlado vía Circuit Breaker ante fallos externos.
* **`AnalysisRequestValidator`:** Valida que el archivo binario cumpla con extensiones válidas (JPEG, PNG) y no exceda el límite de tamaño de 10 MB antes de su procesamiento.

### 5.2.3. Application Layer
Gestiona el caso de uso de análisis gastronómico, controlando el flujo entre la validación de entrada y la llamada al servicio de dominio.

* **`AnalyzeDishImageCommandHandler`:** Recibe los bytes de la imagen, genera el hash de control, invoca el puerto `GastronomicInferenceService` y retorna la respuesta normalizada `GastronomicAnalysisResponseDto`.
* **`GastronomicAnalysisResponseDto`:** Objeto de transferencia que transporta los nombres, descripciones, lista de ingredientes, alérgenos normalizados y estimación calórica hacia la aplicación de administración.

### 5.2.4. Infrastructure Layer
Implementa los adaptadores técnicos y de integración hacia la API de Google Gemini Vision.

* **`GeminiApiClientAdapter` (Anti-Corruption Layer - ACL):** Implementación de `GastronomicInferenceService`. Traduce las estructuras internas al contrato de Google Gemini (`gemini-1.5-flash`), inyectando el system prompt gastronómico y configurando el `responseSchema` en JSON estricto.
* **`GeminiResilienceWrapper`:** Aspecto configurado con Resilience4j que aplica un **Circuit Breaker** (umbral de 5000 ms y 50% de fallas en ventanas de 10 peticiones) y fallback ordenado a carga manual para proteger los hilos del servidor.

### 5.2.6. Bounded Context Software Architecture Component Level Diagrams

```mermaid
C4Component
    title Component Diagram - AI Gastronomic Analysis Context

    Container_Boundary(ai_bc, "AI Gastronomic Analysis Context (Spring Boot)") {
        Component(ai_ctrl, "AIGastronomicAnalysisController", "Spring REST Controller", "Recibe multipart/form-data de la imagen y autentica la solicitud.")
        Component(ai_app_service, "AnalyzeDishImageCommandHandler", "Spring Service (Application)", "Valida formato de imagen y gestiona la ejecución del análisis.")
        Component(acl_adapter, "GeminiApiClientAdapter (ACL)", "Spring Component (Infrastructure)", "Traduce estructuras internas a llamadas Gemini Vision con Schema JSON.")
        Component(resilience_cb, "Resilience4j CircuitBreaker", "Resilience4j Aspect", "Corta llamadas si latencia > 5000ms o fallas > 50%.")
        Component(gemini_client, "GoogleGeminiRestClient", "Spring HTTP Interface", "Cliente HTTP que despacha peticiones a Google Cloud.")
    }

    System_Ext(gemini_api, "Google Gemini Vision API", "Motor externo multimodal LLM.")

    Rel(ai_ctrl, ai_app_service, "Pasa imagen en bytes", "Java Call")
    Rel(ai_app_service, resilience_cb, "Ejecuta con protección", "Java Call")
    Rel(resilience_cb, acl_adapter, "Ejecuta si circuito Closed", "Java Call")
    Rel(acl_adapter, gemini_client, "Serializa prompt JSON", "HTTP Client")
    Rel(gemini_client, gemini_api, "POST generateContent", "HTTPS / JSON")
```
### 5.2.7. Bounded Context Software Architecture Code Level Diagrams
#### 5.2.7.1. Bounded Context Domain Layer Class Diagrams
```mermaid
classDiagram
    class GastronomicAnalysisRequest {
        -UUID requestId
        -UUID restaurantId
        -String imageHash
        -AnalysisStatus executionStatus
        -InferredMetadata inferredMetadata
        -Instant createdAt
        +completeAnalysis(metadata: InferredMetadata) void
        +failAnalysis(reason: String) void
        +markFallbackTriggered() void
    }

    class InferredMetadata {
        -String suggestedName
        -String sensoryDescription
        -String suggestedCategory
        -List~String~ identifiedIngredients
        -Set~String~ detectedAllergens
        -String estimatedCaloriesRange
        -Double confidenceScore
        +getSuggestedName() String
        +getDetectedAllergens() Set~String~
    }

    class AnalysisStatus {
        <<enumeration>>
        PENDING
        COMPLETED
        FAILED
        FALLBACK_TRIGGERED
    }

    class GastronomicInferenceService {
        <<interface>>
        +analyzeDishImage(imageBytes: byte[], mimeType: String) InferredMetadata
    }

    GastronomicAnalysisRequest *-- InferredMetadata
    GastronomicAnalysisRequest --> AnalysisStatus
    GastronomicInferenceService ..> InferredMetadata : produce
```
#### 5.2.7.2. Bounded Context Database Design Diagram

```mermaid
erDiagram
    AI_ANALYSIS_AUDIT_LOGS {
        uuid request_id PK
        uuid restaurant_id
        varchar image_hash
        varchar execution_status
        text prompt_tokens_used
        text completion_tokens_used
        numeric response_time_ms
        jsonb inferred_payload
        varchar error_reason
        timestamp executed_at
    }
```

## 5.3. Bounded Context: AR Dining Experience

En esta sección se especifica el diseño táctico del contexto de experiencia de consumo interactivo en mesa (Front-Stage), orientado a garantizar el acceso inmediato del comensal sin descargas ni credenciales, el renderizado de modelos tridimensionales a escala métrica real 1:1 y el filtrado estricto por seguridad alimentaria.

### 5.3.1. Domain Layer
Modela el ciclo de vida efímero de la sesión de mesa del comensal, la gobernanza de filtros de alérgenos y las restricciones de escala métrica para la proyección volumétrica.

* **`DiningSession` (Aggregate Root / Entity):** Representa la sesión temporal y anónima de un comensal en el salón físico.
  * *Atributos:* `sessionToken: UUID`, `restaurantId: UUID`, `tableId: UUID`, `activeAllergenFilters: Set<String>`, `startedAt: Instant`, `lastInteractionAt: Instant`.
  * *Métodos:* `applyAllergenFilter(allergens: Set<String>): void`, `clearFilters(): void`, `isDishSafe(dishAllergens: Set<String>): Boolean`, `touchSession(): void`.
* **`ARModelAsset` (Entity / Read Model):** Representa la metadata del activo tridimensional calibrado para su proyección en el espacio físico.
  * *Atributos:* `modelId: String`, `format: ModelFormat`, `scaleFactor: Double`, `dracoCompressed: Boolean`, `cdnDownloadUrl: String`.
  * *Métodos:* `isMetricScaleCalibrated(): Boolean`.
* **`ModelFormat` (Enum):** Formatos de archivo para Realidad Aumentada móvil: `GLB` (WebXR Device API / Scene Viewer para Android) y `USDZ` (AR Quick Look para iOS).
* **`ScaleConstraint` (Value Object):** Restricción matemática inmutable que bloquea la escala libre del visor WebAR para asegurar fidelidad volumétrica física 1:1 frente al tamaño del plato real.
* **`DiningSessionRepository` (Domain Interface):** Puerto para la gestión de sesiones efímeras: `save(session: DiningSession): DiningSession`, `findByToken(token: UUID): Optional<DiningSession>`.

### 5.3.2. Interface Layer
Expone los servicios de navegación y consumo público para los comensales, optimizados para clientes web ligeros móviles (PWA).

* **`DiningSessionController`:** Expone endpoints públicos sin autenticación contextualizados por el identificador de mesa:
  * `POST /api/v1/dining/session`: Inicia una sesión efímera a partir del token de mesa física.
  * `GET /api/v1/dining/session/{token}/catalog`: Retorna la carta filtrada según las preferencias activas del comensal.
  * `POST /api/v1/dining/session/{token}/filters`: Actualiza los alérgenos a excluir de la vista.
* **`ARModelDeliveryController`:** Controlador REST especializado en la entrega de activos 3D (`GET /api/v1/assets/models/{modelId}`), configurando cabeceras agresivas de caché (`Cache-Control: public, max-age=31536000, immutable`) y validación ETag para minimizar el consumo de datos móviles.

### 5.3.3. Application Layer
Coordina los flujos de interacción del comensal, el filtrado dinámico de ítems y la resolución de rutas de descarga de activos volumétricos.

* **`StartDiningSessionCommandHandler`:** Valida la vigencia del token de mesa y crea una nueva instancia de `DiningSession` persistida en memoria.
* **`FilterCatalogByAllergensQueryHandler`:** Toma los filtros dietarios solicitados y purga en memoria cualquier preparación culinaria que declare alérgenos restringidos por el comensal.
* **`GetARModelDownloadUrlQueryHandler`:** Resuelve la dirección URL óptima en el CDN de Amazon CloudFront para despachar el archivo binario (`.glb` / `.usdz`) en menos de 1.5 segundos.
* **`LogARInteractionCommandHandler`:** Registra de forma asíncrona la telemetría de interacción con el modelo 3D para la analítica de negocio del restaurante.

### 5.3.4. Infrastructure Layer
Implementa los adaptadores de almacenamiento volátil y entrega perimetral distribuida para maximizar el rendimiento.

* **`RedisDiningSessionRepository`:** Implementación concreta de `DiningSessionRepository` que almacena los estados de sesión en Redis con un TTL de 3 horas, liberando automáticamente memoria al expirar la visita.
* **`CloudFrontUrlSignerService`:** Genera y valida las rutas perimetrales de distribución en Amazon CloudFront para el despacho de activos pesados cacheados cerca al dispositivo móvil.

### 5.3.6. Bounded Context Software Architecture Component Level Diagrams

```mermaid
C4Component
    title Component Diagram - AR Dining Experience Context

    Container_Boundary(ar_bc, "AR Dining Experience Context (Spring Boot)") {
        Component(dining_ctrl, "DiningSessionController", "Spring REST Controller", "Expone APIs anónimas de sesión de mesa y consulta de carta con filtros.")
        Component(asset_ctrl, "ARModelDeliveryController", "Spring REST Controller", "Gestiona redirección y entrega con cabeceras de caché agresivas.")
        Component(session_service, "DiningSessionAppService", "Spring Service (Application)", "Gobierna ciclo de vida de la sesión efímera y filtrado por alérgenos.")
        Component(domain_session, "DiningSession Aggregate", "Java Domain Model", "Aplica reglas de seguridad alimentaria y bloqueo de escala 1:1.")
        Component(redis_session_repo, "RedisSessionRepositoryAdapter", "Spring Component (Infrastructure)", "Guarda sesiones en Redis con TTL de 3 horas.")
    }

    Container(web_client, "AR Dining Web Client", "Three.js / WebXR", "Renderiza modelos 3D en el navegador móvil.")
    ContainerDb(redis, "Redis Cache", "In-Memory DB", "Almacena DiningSessions activas.")
    Container(cdn, "Amazon CloudFront CDN", "Edge Storage", "Despacha binarios GLB/USDZ comprimidos con Draco.")

    Rel(web_client, dining_ctrl, "POST /session con token de mesa", "JSON/HTTPS")
    Rel(web_client, asset_ctrl, "GET /assets/models/{id}", "HTTPS")
    Rel(dining_ctrl, session_service, "Coordina sesión", "Java Call")
    Rel(session_service, domain_session, "Evalúa filtros", "Domain Call")
    Rel(session_service, redis_session_repo, "Persiste sesión efímera", "Java Interface")
    Rel(redis_session_repo, redis, "Escribe sesión con TTL", "TCP/RESP")
    Rel(asset_ctrl, cdn, "Redirige a URL Edge o despacha caché", "HTTP 302/ETag")
    Rel(web_client, cdn, "Descarga modelo binario < 3MB", "HTTPS")
```
### 5.3.7. Bounded Context Software Architecture Code Level Diagrams
#### 5.3.7.1. Bounded Context Domain Layer Class Diagrams
```mermaid
classDiagram
    class DiningSession {
        -UUID sessionToken
        -UUID restaurantId
        -UUID tableId
        -Set~String~ activeAllergenFilters
        -Instant startedAt
        -Instant lastInteractionAt
        +applyAllergenFilter(allergens: Set~String~) void
        +clearFilters() void
        +isDishSafe(dishAllergens: Set~String~) Boolean
        +touchSession() void
    }

    class ARModelAsset {
        -String modelId
        -ModelFormat format
        -Double scaleFactor
        -Boolean dracoCompressed
        -String cdnDownloadUrl
        +isMetricScaleCalibrated() Boolean
    }

    class ModelFormat {
        <<enumeration>>
        GLB
        USDZ
    }

    class ScaleConstraint {
        -Double fixedScale
        -Boolean allowFreeScaling
        +validateScaleIntegrity() Boolean
    }

    class DiningSessionRepository {
        <<interface>>
        +save(session: DiningSession) DiningSession
        +findByToken(token: UUID) Optional~DiningSession~
    }

    DiningSession ..> ARModelAsset : proyecta
    DiningSession *-- ScaleConstraint
    ARModelAsset --> ModelFormat
    DiningSessionRepository ..> DiningSession : gestiona
```
#### 5.3.7.2. Bounded Context Database Design Diagram
```mermaid
erDiagram
    AR_INTERACTION_METRICS {
        uuid id PK
        uuid restaurant_id
        uuid table_id
        uuid dish_id
        varchar model_id
        varchar device_platform
        int view_duration_seconds
        timestamp interacted_at
    }
```
## 5.4. Bounded Context: Restaurant & Table Management

En esta sección se especifica el diseño táctico del subdominio de soporte encargado de la administración institucional de los restaurantes, la parametrización física del salón y las mesas, y la emisión de identificadores criptográficos contextualizados para la generación de plantillas de códigos QR físicos de alta definición.

### 5.4.1. Domain Layer
Modela el perfil operativo del establecimiento gastronómico, la configuración espacial de mesas y la unicidad criptográfica de los identificadores de mesa.

* **`Restaurant` (Aggregate Root / Entity):** Representa el establecimiento afiliado a la plataforma Platter.
  * *Atributos:* `id: RestaurantId`, `name: String`, `commercialName: String`, `slug: String`, `logoUrl: String`, `isActive: Boolean`, `tables: List<DiningTable>`, `createdAt: Instant`.
  * *Métodos:* `addTable(tableIdentifier: String): DiningTable`, `disableTable(tableId: TableId): void`, `enableTable(tableId: TableId): void`, `getTableByToken(token: String): Optional<DiningTable>`, `updateProfile(commercialName: String, logoUrl: String): void`.
* **`DiningTable` (Entity):** Entidad subordinada que representa una mesa física del salón.
  * *Atributos:* `id: TableId`, `restaurantId: RestaurantId`, `tableIdentifier: String` (ej. "Mesa 12", "Terraza 03"), `secureToken: TableSecureToken`, `isAvailable: Boolean`, `createdAt: Instant`.
  * *Métodos:* `regenerateSecureToken(): void`, `markAsUnavailable(): void`, `markAsAvailable(): void`.
* **`RestaurantId`, `TableId` (Value Objects):** Identificadores unívocos basados en UUID v4.
* **`TableSecureToken` (Value Object):** Hash criptográfico aleatorio no correlativo de 32 caracteres alfanuméricos que protege el acceso a la mesa contra ataques de barrido o enumeración secuencial.
* **`TableRepository` (Domain Interface):** Puerto de persistencia que declara las operaciones del dominio: `save(restaurant: Restaurant): Restaurant`, `findById(id: RestaurantId): Optional<Restaurant>`, `findByTableSecureToken(token: String): Optional<DiningTable>`.
* **`TableBatchCreatedEvent` (Domain Event):** Evento emitido tras la configuración exitosa de un conjunto de mesas, habilitando la generación asíncrona de artes vectoriales.

### 5.4.2. Interface Layer
Expone los endpoints administrativos de parametrización del local y la resolución pública de los códigos QR leídos por los dispositivos móviles.

* **`RestaurantTableAdminController`:** Controlador REST administrativo asegurado con JWT:
  * `POST /api/v1/restaurants/{id}/tables/batch`: Registra rangos de mesas en bloque.
  * `GET /api/v1/restaurants/{id}/tables`: Consulta la relación de mesas registradas y sus tokens.
  * `GET /api/v1/restaurants/{id}/tables/pdf`: Descarga la plantilla PDF vectorizada lista para imprimir.
* **`TablePublicResolverController`:** Controlador REST público que procesa el escaneo del código QR:
  * `GET /api/v1/tables/resolve?token={token}`: Valida la existencia del token seguro y devuelve el contexto del restaurante y número de mesa para arrancar la sesión WebAR.

### 5.4.3. Application Layer
Orquesta los casos de uso administrativos de estructuración de salones y la emisión de documentos imprimibles.

* **`ConfigureTablesBatchCommandHandler`:** Genera las instancias de `DiningTable` dentro del agregado `Restaurant`, garantizando la asignación de tokens no repetidos y persistiendo la transacción.
* **`ResolveTableTokenQueryHandler`:** Consulta el puerto de persistencia mediante el hash recibido y valida si la mesa y el local se encuentran habilitados para el servicio.
* **`GeneratePrintableQRPdfCommandHandler`:** Recupera la lista de mesas, obtiene los datos gráficos institucionales del local y delega la construcción del archivo imprimible hacia la capa de infraestructura.

### 5.4.4. Infrastructure Layer
Implementa los adaptadores de base de datos relacional y el motor de dibujo vectorial de códigos QR.

* **`JpaRestaurantRepositoryAdapter`:** Implementación concreta del puerto `TableRepository` mediante Spring Data JPA (`SpringDataRestaurantJpaRepository`), mapeando las entidades relacionales `RestaurantJpaEntity` y `DiningTableJpaEntity`.
* **`PdfQrGeneratorService`:** Servicio de infraestructura que combina la librería de renderizado matricial ZXing con el procesador PDF OpenPDF para compilar un documento en alta resolución con el logo del restaurante, las instrucciones de escaneo y el código QR por cada mesa.

### 5.4.6. Bounded Context Software Architecture Component Level Diagrams

```mermaid
C4Component
    title Component Diagram - Restaurant & Table Management Context

    Container_Boundary(table_bc, "Restaurant & Table Context (Spring Boot)") {
        Component(table_admin_ctrl, "RestaurantTableAdminController", "Spring REST Controller", "Administra creación de mesas y descarga de plantillas PDF.")
        Component(table_resolver_ctrl, "TablePublicResolverController", "Spring REST Controller", "Resuelve criptográficamente el token del QR escaneado en mesa.")
        Component(table_service, "TableManagementAppService", "Spring Service (Application)", "Genera identificadores y orquesta la emisión masiva.")
        Component(domain_table, "Restaurant & Table Entities", "Java Domain Model", "Garantiza unicidad de tokens y consistencia de mesas.")
        Component(jpa_table_repo, "JpaRestaurantRepositoryAdapter", "Spring Component (Infrastructure)", "Persiste locales y mesas en PostgreSQL.")
        Component(pdf_qr_svc, "PdfQrGeneratorService", "Spring Component (Infrastructure)", "Genera PDF vectorizado con QR y logotipo del local.")
    }

    ContainerDb(postgres, "PostgreSQL 16", "Relational DB", "Tablas restaurants y dining_tables.")

    Rel(table_admin_ctrl, table_service, "Gestiona mesas", "Java Call")
    Rel(table_resolver_ctrl, table_service, "Resuelve token", "Java Call")
    Rel(table_service, domain_table, "Aplica reglas", "Domain Call")
    Rel(table_service, jpa_table_repo, "Persiste entidades", "Java Interface")
    Rel(table_service, pdf_qr_svc, "Compila PDF de mesa", "Java Call")
    Rel(jpa_table_repo, postgres, "Lee/Escribe en base de datos", "JDBC/SQL")
```

### 5.4.7. Bounded Context Software Architecture Code Level Diagrams
#### 5.4.7.1. Bounded Context Domain Layer Class Diagrams
```mermaid
classDiagram
    class Restaurant {
        -RestaurantId id
        -String name
        -String commercialName
        -String slug
        -String logoUrl
        -Boolean isActive
        -List~DiningTable~ tables
        -Instant createdAt
        +addTable(tableIdentifier: String) DiningTable
        +disableTable(tableId: TableId) void
        +enableTable(tableId: TableId) void
        +getTableByToken(token: String) Optional~DiningTable~
        +updateProfile(commercialName: String, logoUrl: String) void
    }

    class DiningTable {
        -TableId id
        -RestaurantId restaurantId
        -String tableIdentifier
        -TableSecureToken secureToken
        -Boolean isAvailable
        -Instant createdAt
        +regenerateSecureToken() void
        +markAsUnavailable() void
        +markAsAvailable() void
    }

    class RestaurantId {
        -UUID value
        +getValue() UUID
    }

    class TableId {
        -UUID value
        +getValue() UUID
    }

    class TableSecureToken {
        -String tokenHash
        +getTokenHash() String
    }

    class TableRepository {
        <<interface>>
        +save(restaurant: Restaurant) Restaurant
        +findById(id: RestaurantId) Optional~Restaurant~
        +findByTableSecureToken(token: String) Optional~DiningTable~
    }

    Restaurant "1" *-- "0..*" DiningTable : compone
    Restaurant *-- RestaurantId
    DiningTable *-- TableId
    DiningTable *-- TableSecureToken
    TableRepository ..> Restaurant : persiste
```

#### 5.4.7.2. Bounded Context Database Design Diagram

```mermaid
erDiagram
    RESTAURANTS ||--o{ DINING_TABLES : "posee"

    RESTAURANTS {
        uuid id PK
        varchar name
        varchar commercial_name
        varchar slug UK
        varchar logo_url
        boolean is_active
        timestamp created_at
    }

    DINING_TABLES {
        uuid id PK
        uuid restaurant_id FK
        varchar table_identifier
        varchar secure_token UK
        boolean is_available
        timestamp created_at
    }
```


# Capítulo VI: Solution UX Design

En el presente capítulo se aborda la definición formal de la propuesta de diseño de experiencia de usuario (UX) e interfaz de usuario (UI) para el ecosistema digital de **Platter**, integrando de manera sinérgica la **Landing Page** comercial, la **Web Application** para la administración de restaurantes y la experiencia inmersiva de la **Carta Digital WebAR** orientada al comensal en mesa.

Esta propuesta se fundamenta estrictamente en los artefactos de análisis y especificación desarrollados en los capítulos precedentes:
1. **Trazabilidad con Requerimientos (Capítulo III):** Responde de forma directa a las necesidades críticas y dolores identificados en los arquetipos de usuario:
   * **Carlos Mendoza Vidal (Dueño de Restaurante MYPE):** Demanda una interfaz administrativa simple, intuitiva y ágil para digitalizar su menú en menos de 2 minutos mediante el pipeline de IA multimodal, sin necesidad de conocimientos técnicos avanzados ni dependencia de agencias de marketing (US01, US04, US06).
   * **Valeria Ramos Benavides (Comensal Celíaca):** Exige certidumbre visual inmediata del tamaño y presentación real del plato en mesa (escala 1:1), filtrado riguroso y transparente de alérgenos normados (gluten, lactosa, etc.) y una experiencia de cero fricción sin instalaciones obligatorias de aplicaciones móviles pesadas (US02, US03, US05, US08).
2. **Coherencia con la Arquitectura de Software (Capítulo IV):** Traduce visualmente las capacidades de los Bounded Contexts (*Dish Catalog*, *AI Analysis & Inference*, *WebAR Experience*, *Table & Session Management*), optimizando el consumo de modelos 3D ultraligeros comprimidos con Draco vía CDN y garantizando respuestas reactivas respaldadas por la infraestructura en la nube.
3. **Estándares de Diseño y Tecnología:** Adopta como marco de referencia los principios de **Material Design 3 (Material You)**, directrices de accesibilidad web **WCAG 2.1 nivel AA (a11y)**, soporte de internacionalización **i18n** (inglés como idioma base `en_US` y español latinoamericano `es_419`) y buenas prácticas de visualización espacial bajo **WebXR** y **AR Quick Look**.

---

## 6.1. Style Guidelines

La sección de Guías de Estilo sienta las bases para centralizar, normar y organizar el repositorio común de diseño visual del equipo. Este sistema de diseño garantiza una experiencia coherente, predecible y estéticamente atractiva a lo largo de todos los puntos de contacto del usuario con la plataforma Platter.

### 6.1.1. General Style Guidelines

#### 1. Branding e Identidad Visual

La identidad corporativa de **Platter** ha sido concebida para transmitir hospitalidad culinaria, modernidad digital y rigor tecnológico:
* **Concepto de Marca:** Platter actúa como el puente entre el arte gastronómico del salón físico y la dimensión digital inmersiva. El imagotipo combina la silueta limpia y armónica de un plato de cocina contemporánea con un nodo focal superior que representa la apertura espacial del lente de Realidad Aumentada y el procesamiento inteligente con IA.
* **Isotipo:** Glifo circular estilizado con bordes orgánicos suaves y un visor angular en el cuadrante superior derecho, alusivo a la proyección tridimensional en mesa.
* **Logotipo Tipográfico:** Construido sobre la tipografía *Outfit* en estilo Bold, con espaciado entre letras (*kerning*) calibrado para proyectar solidez, claridad y sofisticación gastronómica.
* **Variantes de Aplicación:**
  * *Versión Dark (Principal para Salón y Experiencia Nocturna):* Diseñada para minimizar el deslumbramiento en salones de restaurante tenue y maximizar el contraste de los modelos 3D iluminados por PBR. Fondo `#121C33` con imagotipo en blanco puro y acento terracota `#E76F51`.
  * *Versión Light (Secundaria para Documentación y Portal SaaS Diurno):* Fondo crema cálido `#F7F3ED` con logotipo en azul medianoche `#121C33` y acentos cálidos `#D4A373`.
* **Área de Reserva y Protección:** Se establece un margen de seguridad perimetral inviolable equivalente a la altura de la letra 'P' del logotipo en cualquiera de sus escalas de reproducción, evitando la interferencia de textos o elementos ajenos.
* **Usos Restringidos:** Queda estrictamente prohibido alterar las proporciones dimensionales, sustituir la paleta cromática por tonos fuera de guía, aplicar gradientes estridentes no estandarizados o rotar el símbolo gráfico.

#### 2. Typography (Tipografía)

El sistema tipográfico de Platter combina dos familias de código abierto de Google Fonts cuidadosamente seleccionadas para equilibrar presencia de marca y máxima legibilidad:

1. **Tipografía Primaria de Marca y Encabezados (Display & Headings):** `Outfit`  
   Tipografía sans-serif geométrica con terminaciones redondeadas sutiles que evocan la geometría de los platos y vajillas contemporáneas. Se emplea exclusivamente en logotipos, títulos principales, cifras de precios destacados y banners de impacto.
2. **Tipografía Secundaria de Lectura y Controles de Interfaz (Body & UI):** `Plus Jakarta Sans`  
   Diseñada específicamente para entornos digitales modernos, ofrece una amplia altura de x (*x-height*), contrastes ópticos refinados y gran rendimiento en pantallas móviles de comensales bajo diversas condiciones de iluminación ambiental.

##### Escala Tipográfica (Type Scale)

A continuación se detalla la escala jerárquica estandarizada en unidades relativas (`rem`) con su equivalencia en píxeles (`px`), considerando una base raíz de `16px`:

| Nivel / Token | Familia Tipográfica | Peso (*Weight*) | Tamaño (rem / px) | Interlineado (*Line-height*) | Espaciado (*Letter-spacing*) | Caso de Uso en Platter |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **H1 - Hero Title** | Outfit | Bold (700) | 2.50 rem / 40 px | 1.20 (48 px) | -0.02 rem (-0.32 px) | Titular principal en Hero de Landing Page y cabeceras de salón. |
| **H2 - Section Title** | Outfit | SemiBold (600) | 2.00 rem / 32 px | 1.25 (40 px) | -0.01 rem (-0.16 px) | Títulos de categorías gastronómicas y módulos de dashboard SaaS. |
| **H3 - Dish Title / Card** | Outfit | SemiBold (600) | 1.50 rem / 24 px | 1.30 (31 px) | 0.00 rem (0.00 px) | Nombres de platos en tarjetas de la carta y modales de WebAR. |
| **H4 - Subheading** | Plus Jakarta Sans | Medium (500) | 1.25 rem / 20 px | 1.35 (27 px) | 0.00 rem (0.00 px) | Subtítulos de secciones, nombres de ingredientes clave y métricas. |
| **H5 - Price / Emphasis** | Outfit | Bold (700) | 1.125 rem / 18 px | 1.40 (25 px) | 0.01 rem (0.16 px) | Precios destacados de platos y valores numéricos de conversión. |
| **H6 - Modal Header** | Plus Jakarta Sans | SemiBold (600) | 1.00 rem / 16 px | 1.40 (22 px) | 0.01 rem (0.16 px) | Títulos de diálogos de confirmación, configuración y filtros. |
| **Subtitle 1** | Plus Jakarta Sans | Regular (400) | 1.00 rem / 16 px | 1.50 (24 px) | 0.01 rem (0.16 px) | Descripciones breves de platos redactadas por Google Gemini. |
| **Body Regular** | Plus Jakarta Sans | Regular (400) | 0.875 rem / 14 px | 1.50 (21 px) | 0.00 rem (0.00 px) | Párrafos informativos, tablas de datos, términos y condiciones. |
| **Body Small** | Plus Jakarta Sans | Regular (400) | 0.75 rem / 12 px | 1.40 (17 px) | 0.02 rem (0.24 px) | Notas al pie, metadatos nutricionales, sellos normados de alérgenos. |
| **Button / CTA** | Plus Jakarta Sans | SemiBold (600) | 0.875 rem / 14 px | 1.00 (14 px) | 0.03 rem (0.42 px) | Botón "Ver en Realidad Aumentada", "Iniciar Sesión", "Filtrar". |
| **Caption / Badge** | Plus Jakarta Sans | Medium (500) | 0.6875 rem / 11 px | 1.30 (14 px) | 0.04 rem (0.44 px) | Badges de "Sin Gluten", "Recomendado", "Stock Bajo", calorías. |

#### 3. Colors (Paleta Cromática Oficial de Platter)

La paleta cromática de Platter articula tonos cálidos gastronómicos con superficies oscuras de alta inmersión visual. Cumple estrictamente el estándar de accesibilidad **WCAG 2.1 nivel AA**, garantizando un ratio de contraste superior a **4.5:1** en texto normal y **3.0:1** en componentes gráficos e interactivos.

| Rol / Categoría | Nombre del Token | Código HEX | Código RGB | Código HSL | Contraste WCAG (Fondo/Texto) | Propósito y Aplicación en Platter |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Primario (Fondo)** | `--color-bg-dark` | `#121C33` | rgb(18, 28, 51) | hsl(222, 48%, 14%) | 14.8:1 (vs `#FFFFFF`) | Superficie base de la aplicación, visualizador WebAR y modo nocturno. |
| **Primario (Acento CTA)** | `--color-coral-accent` | `#E76F51` | rgb(231, 111, 81) | hsl(12, 77%, 61%) | 5.2:1 (vs `#121C33`) | Llamado a la acción prioritario ("Ver en Mesa 3D", "Ordenar", "Guardar"). |
| **Secundario (Gastronómico)** | `--color-gold-culinary` | `#D4A373` | rgb(212, 163, 115) | hsl(30, 52%, 64%) | 6.8:1 (vs `#121C33`) | Sellos de recomendación del chef, estrellas de calificación y bordes AR. |
| **Secundario (IA / Tech)** | `--color-blue-ai` | `#3A86FF` | rgb(58, 134, 255) | hsl(217, 100%, 61%) | 5.4:1 (vs `#121C33`) | Indicadores de inferencia por IA (Gemini), enlaces y badges tecnológicos. |
| **Superficie (Tarjetas)** | `--color-card-dark` | `#1B2848` | rgb(27, 40, 72) | hsl(223, 45%, 19%) | 12.5:1 (vs `#FFFFFF`) | Contenedores de platos, paneles modales y secciones de lista. |
| **Superficie (Hover/Elevada)** | `--color-card-hover` | `#25365E` | rgb(37, 54, 94) | hsl(222, 44%, 26%) | 9.8:1 (vs `#FFFFFF`) | Estado hover de tarjetas de menú, botones secundarios y dropdowns. |
| **Fondo Claro (Alternativo)** | `--color-bg-light` | `#F7F3ED` | rgb(247, 243, 237) | hsl(40, 33%, 95%) | 13.9:1 (vs `#1A2238`) | Fondo alternativo para facturas impresas, modo diurno y Landing Page. |
| **Texto Principal** | `--color-text-light` | `#FFFFFF` | rgb(255, 255, 255) | hsl(0, 0%, 100%) | 14.8:1 (vs `#121C33`) | Títulos, precios y contenido de máxima prioridad en modo oscuro. |
| **Texto Secundario / Muted**| `--color-text-muted` | `#94A3B8` | rgb(148, 163, 184) | hsl(215, 20%, 65%) | 5.8:1 (vs `#121C33`) | Descripciones complementarias, notas de pie, calorías e iconos pasivos. |
| **Semántico: Éxito / Seguro** | `--color-status-success`| `#2A9D8F` | rgb(42, 157, 143) | hsl(173, 58%, 39%) | 5.1:1 (vs `#121C33`) | Disponibilidad en cocina activa, plato verificado libre del alérgeno buscado. |
| **Semántico: Alerta / Trazas**| `--color-status-warning`| `#E9C46A` | rgb(233, 196, 106) | hsl(43, 74%, 66%) | 7.9:1 (vs `#121C33`) | Contiene trazas de alérgenos, últimas 3 unidades en stock de salón. |
| **Semántico: Peligro / Alérgeno**| `--color-status-danger` | `#E63946` | rgb(230, 57, 70) | hsl(355, 78%, 56%) | 4.6:1 (vs `#FFFFFF`) | Advertencia médica crítica de alérgenos presentes, plato agotado. |

#### 4. Spacing, Grids & Elevation (Espaciado, Rejilla y Elevación)

Para garantizar consistencia espacial y ritmo visual matemáticamente armónico, Platter implementa un sistema modular basado en la cuadrícula de **8 puntos (8-Point Grid)** con subdivisión de 4 puntos para micro-alineaciones:

* **Escala de Espaciado:**
  * `space-xxs (4 px):` Espaciado mínimo entre icono y texto en botones compactos y chips de alérgenos.
  * `space-xs (8 px):` Padding interno de badges de estado, separación entre tags y campos de entrada compactos.
  * `space-sm (16 px):` Padding estándar en tarjetas de platos, separación entre filas de tabla y márgenes móviles.
  * `space-md (24 px):` Espaciado entre bloques de contenido, gutters entre columnas y padding de contenedores.
  * `space-lg (32 px):` Margen entre secciones de categorías culinarias y padding de diálogos modales.
  * `space-xl (48 px):` Espaciado vertical entre macro-secciones en la Landing Page comercial.
  * `space-xxl (64 px):` Margen superior e inferior del Hero Banner de presentación y pie de página.
* **Sistema de Elevación y Sombras (Material Elevations):**
  * *Elevation 0 (Flat):* Superficie plana integrada sin sombra (`box-shadow: none`).
  * *Elevation 1 (Card Rest):* Tarjetas de menú en reposo (`box-shadow: 0 4px 12px rgba(0, 0, 0, 0.20)`).
  * *Elevation 2 (Card Hover / Active):* Tarjetas al interactuar o activadas (`box-shadow: 0 8px 24px rgba(0, 0, 0, 0.35)`).
  * *Elevation 3 (Floating Controls / Modals):* Controles flotantes de Realidad Aumentada, selector de alérgenos y Bottom Sheets móviles (`box-shadow: 0 16px 40px rgba(0, 0, 0, 0.50)`).
* **Radios de Borde (Border Radius):**
  * `radius-sm (8 px):` Botones secundarios, inputs de texto, chips de filtros.
  * `radius-md (16 px):` Tarjetas de platos, contenedores de sección y modales.
  * `radius-lg (24 px):` Contenedores principales, ventanas de visor WebAR y paneles envolventes.
  * `radius-full (9999 px):` Badges circulares de contador y botones de acción flotante (FAB).

#### 5. Tono de Comunicación y Lenguaje Aplicado

Con base en el marco de trabajo de las cuatro dimensiones de tono de **Nielsen Norman Group**, la voz y comunicación de Platter se calibran según el contexto de interacción:

1. **Divertido vs. Serio (Funny vs. Serious):**  
   * **Posición (65% hacia lo Divertido / Vibrante):** En la experiencia del comensal en mesa, el tono es estimulante, sensorial y acogedor (ej. *"¡Descubre la textura y el montaje de este lomo saltado en tu mesa antes de pedirlo!"*). En la administración B2B (facturación, reportes de stock y declaraciones médicas de alérgenos), el tono transmuta a serio y estrictamente riguroso (ej. *"Advertencia sanitaria: este plato contiene frutos secos certificados por la cocina"*).
2. **Formal vs. Casual (Formal vs. Casual):**  
   * **Posición (70% hacia lo Casual y Cercano):** Se utiliza un trato de segunda persona cordial (*"tu carta"*, *"tu mesa"*, *"tus preferencias"*), eliminando barreras jerárquicas y lenguaje burocrático. En las comunicaciones B2B corporativas y contratos de servicio, se conserva profesionalismo pulcro y directo.
3. **Respetuoso vs. Irreverente (Respectful vs. Irreverent):**  
   * **Posición (90% hacia lo Respetuoso y Empático):** La seguridad alimentaria de comensales con celiaquía o intolerancias no tolera ambigüedades ni bromas. El sistema valida con absoluta seriedad las restricciones alimentarias, ofreciendo alternativas transparentes y reconociendo el valor del tiempo del restaurante y del comensal.
4. **Entusiasta vs. Sereno (Enthusiastic vs. Matter-of-fact):**  
   * **Posición (75% hacia lo Entusiasta):** Se celebra la riqueza gastronómica y la magia tecnológica de la Realidad Aumentada sin caer en exageraciones vacías, manteniendo serenidad y claridad en las confirmaciones transaccionales y tiempos de carga de modelos.

#### 6. Design System de Referencia

La arquitectura visual de Platter adopta y extiende las especificaciones de **Material Design 3 (Material You)** promovidas por Google:
* Adopción de tokens de diseño dinámicos (*design tokens*) gestionados mediante CSS Custom Properties.
* Empleo de componentes estandarizados: *Elevated Cards* con soporte de media enriquecida para platos, *Filter Chips* con selección múltiple para filtros de alérgenos, *Bottom Sheets* deslizables para desgloses nutricionales en smartphones y *Floating Action Buttons (FAB)* con micro-interacciones para el disparo de WebAR.

---

### 6.1.2. Web, Mobile & Devices Style Guidelines

#### 1. Responsive Web Interfaces (Interfaces Web Adaptables)

La plataforma garantiza una experiencia de usuario fluida y receptiva a través de múltiples factores de forma y densidades de píxeles:

* **Breakpoints Oficiales:**
  * **Mobile Small / Standard (`< 600 px`):** Orientado a smartphones de comensales en mesa (resoluciones típicas de 360x800 px a 430x932 px).
    * *Estructura de Rejilla:* 4 columnas fluidas, márgenes exteriores de `16 px`, canaletas (*gutters*) de `12 px`.
    * *Comportamiento UI:* Tarjeta de plato en disposición vertical única (1 columna), barra de navegación anclada en la parte inferior (*Bottom Navigation*), modales desplegados como *Bottom Sheets* deslizables.
  * **Tablet / Foldables (`600 px - 1024 px`):** Orientado a tablets utilizadas por camareros, capitanes de salón y comensales en modo horizontal.
    * *Estructura de Rejilla:* 8 columnas, márgenes exteriores de `24 px`, canaletas de `16 px`.
    * *Comportamiento UI:* Tarjetas de plato en rejilla de 2 columnas con previsualización intermedia, menú lateral colapsable (*Navigation Drawer*).
  * **Desktop / Large Displays (`> 1024 px`):** Orientado a la Landing Page comercial y al panel SaaS de administración de restaurantes.
    * *Estructura de Rejilla:* 12 columnas fijas, ancho máximo contenedor centrado de `1200 px`, márgenes automáticos, canaletas de `24 px`.
    * *Comportamiento UI:* Tarjetas de plato en rejilla de 3 o 4 columnas, visualizador 3D interactivo en Canvas WebGL al posar el cursor (*hover 3D preview*), barra de navegación superior horizontal completa.

#### 2. Native Mobile & WebAR Interfaces (Pautas para Dispositivos Móviles y Realidad Aumentada)

Dado que el visor de platos en mesa se ejecuta directamente sobre el navegador móvil del comensal utilizando estándares nativos de Realidad Aumentada sin instalación (**WebXR Device API** en Google Chrome para Android y **AR Quick Look** con archivos `.usdz` en Apple Safari para iOS), se establecen pautas estrictas de ergonomía táctil y espacial:

* **Touch Targets Mínimos:** Todas las áreas de interacción táctil (botones de selección, chips de filtro, controles de cámara y cierre de visor) poseen una superficie táctil mínima de **48 × 48 dp (px)**, cumpliendo la directriz de accesibilidad móvil para evitar toques accidentales con manos ocupadas en mesa.
* **Respeto a Zonas Seguras (Safe Areas):** Integración obligatoria de las variables CSS de entorno del dispositivo:
  ```css
  padding-top: max(16px, env(safe-area-inset-top));
  padding-bottom: max(16px, env(safe-area-inset-bottom));
  padding-left: max(16px, env(safe-area-inset-left));
  padding-right: max(16px, env(safe-area-inset-right));
  ```
  Esto previene que la barra de búsqueda o los botones flotantes de WebAR queden solapados por el notch de la cámara o la barra de gestos del sistema operativo.
* **Patrones de Interacción y Gestos en WebAR:**
  * **Retícula de Detección de Superficie:** Indicador animado en pantalla con borde dorado pulsante (`#D4A373`) que guía al comensal para enfocar la mesa con la cámara hasta detectar el plano horizontal.
  * **Toque Único (Single Tap):** Al detectar la mesa, un toque posiciona y ancla el plato virtual en el espacio físico.
  * **Bloqueo de Escala 1:1:** Por defecto, el plato se proyecta con factor de escala métrica real estricto 1:1 (bloqueado para evitar distorsiones cognitivas de tamaño). El usuario puede activar un interruptor secundario si desea inspeccionar detalles mediante *pinch-to-zoom*.
  * **Rotación Orbital Unidireccional (One-Finger Drag):** Permite rotar el plato 360° sobre su eje vertical central (eje Y) con un deslizamiento horizontal del dedo, manteniendo los ejes X y Z estables para impedir inclinaciones irreales de la vajilla.

---

## 6.2. Information Architecture

La Arquitectura de Información (IA) de Platter estructura, etiqueta y conecta el contenido y los servicios del sistema, asegurando que tanto los visitantes de la Landing Page comercial como los administradores de restaurante y comensales en mesa encuentren la información necesaria con un esfuerzo cognitivo mínimo.

### 6.2.1. Organization Systems

La organización del contenido responde a esquemas visuales y lógicos diferenciados según la naturaleza de la tarea:

#### 1. Sistemas de Organización Visual
* **Jerárquico (Visual Hierarchy):**  
  Aplicado en la **Ficha del Plato** y la **Landing Page**. La información se organiza de forma piramidal:
  * *Nivel 1 (Foco Primario):* Nombre del plato y precio destacado en fuentes *Outfit Bold*, acompañados del visor/tarjeta 3D interactiva.
  * *Nivel 2 (Foco Secundario):* Descripción sensorial generada por IA, ingredientes principales y botón prominente de llamado a la acción *"Ver en tu Mesa 3D"*.
  * *Nivel 3 (Foco de Seguridad y Detalle):* Badges normalizados de alérgenos (sellos de advertencia en rojo/ámbar o sellos de inocuidad en verde) e información calórica/macronutrientes.
* **Secuencial (Step-by-Step / Flujo Guiado):**  
  Aplicado en los procesos de alta complejidad o toma de decisión crítica:
  * *Flujo del Administrador (Digitalización de Plato):* Paso 1: Captura fotográfica con smartphone -> Paso 2: Procesamiento multimodal con Google Gemini (extracción automática de nombre, ingredientes, alérgenos y calorías) -> Paso 3: Asignación y calibración de modelo 3D -> Paso 4: Confirmación y publicación inmediata en carta.
  * *Flujo del Comensal (Consumo en Mesa):* Paso 1: Escaneo de código QR de mesa -> Paso 2: Configuración rápida opcional de restricciones dietéticas (ej. "Soy celíaco") -> Paso 3: Exploración de carta filtrada -> Paso 4: Apertura de WebAR y anclaje en mesa -> Paso 5: Decisión final de pedido informada.
* **Matricial:**  
  Aplicado en el **Dashboard de Administración de Restaurante**, permitiendo a los dueños y administradores cruzar múltiples variables en una sola vista: estado de stock en cocina (*Disponible / Agotado*), categoría culinaria, métricas de visualización 3D por plato y rotación de mesas activas.

#### 2. Esquemas de Categorización de Contenido
* **Por Tópicos / Categorías Culinarias:** Estructura natural de la gastronomía que agrupa la oferta en: *Entradas & Piques*, *Platos de Fondo*, *Guarniciones*, *Postres Artesanales*, *Bebidas & Coctelería*, y *Especialidades del Chef*.
* **Por Audiencia / Segmentos:** Separación estricta de dominios de acceso:
  * *Público / Comensal:* Acceso universal, liviano, anónimo y sin login mediante URLs dinámicas firmadas por mesa (`/menu/:restaurantSlug?mesa=:tableId`).
  * *B2B / Restaurante:* Portal administrativo seguro (`/admin/dashboard`) protegido mediante autenticación JWT y control de acceso basado en roles (Administrador, Chef de Cocina, Mozo).
* **Alfabético:** Catálogo normado de alérgenos y glosario de términos gastronómicos en los selectores de búsqueda avanzada.
* **Cronológico:** Registro de auditoría de modificaciones de platos y precios en la administración, e historial de pedidos del salón.

---

### 6.2.2. Labeling Systems

El sistema de etiquetado utiliza términos breves, directos y universalmente comprensibles en el ámbito de la gastronomía y la tecnología móvil, evitando tecnicismos oscuros y reduciendo la carga cognitiva:

| Contexto / Entorno | Etiqueta en Español | Etiqueta en Inglés (`i18n`) | Componente UI | Significado y Asociación Mental del Usuario |
| :--- | :--- | :--- | :--- | :--- |
| **Landing Page** | `Digitaliza tu Carta` | `Digitize Your Menu` | CTA Button (Hero) | Comunica transformación inmediata de la carta física a formato digital 3D. |
| **Landing Page** | `Ver Demo 3D en Vivo` | `Live 3D Demo` | Secondary Button | Promesa de interacción real e instantánea con Realidad Aumentada sin registro. |
| **Landing Page** | `Calcula tu Retorno (ROI)` | `Calculate Your ROI` | Navigation Link / CTA | Asociación con rentabilidad financiera y ahorro de costos frente a impresiones. |
| **Landing Page** | `Planes y Tarifas` | `Pricing & Plans` | Navigation Link | Claridad sobre costos de suscripción mensual sin comisiones ocultas. |
| **Carta WebAR** | `Ver en tu Mesa` | `View on Table` | Primary CTA Button | Invita a activar la cámara para proyectar el modelo 3D a escala real en la mesa física. |
| **Carta WebAR** | `Libre de Gluten` | `Gluten-Free` | Filter Badge / Chip | Certeza médica instantánea para personas con celiaquía o intolerancia. |
| **Carta WebAR** | `Alergias Alimentarias` | `Food Allergies` | Filter Trigger Chip | Acceso al selector de exclusión de los 14 alérgenos de declaración obligatoria. |
| **Carta WebAR** | `Información Nutricional`| `Nutritional Info` | Accordion / Sheet | Muestra calorías inferidas, proteínas y grasas sin saturar la tarjeta principal. |
| **Carta WebAR** | `Agotado en Cocina` | `Out of Stock` | Status Tag (Rojo) | Previene pedidos fallidos indicando indisponibilidad de insumos en tiempo real. |
| **Portal SaaS** | `Escanear Plato con IA` | `Scan Dish with AI` | Action Button (Icon) | Dispara la cámara para fotografiar el plato e iniciar la inferencia con Gemini. |
| **Portal SaaS** | `Mis Platos` | `My Dishes` | Sidebar Navigation | Directorio maestro del catálogo gastronómico del restaurante. |
| **Portal SaaS** | `Códigos QR de Mesa` | `Table QR Codes` | Sidebar Navigation | Módulo de generación, descarga e impresión de códigos QR dinámicos por salón. |
| **Portal SaaS** | `Métricas de Salón` | `Dining Room Analytics`| Sidebar Navigation | Visualizaciones de platos más vistos en 3D, tiempo en carta y conversiones. |
| **Footer / Legal** | `Términos del Servicio`| `Terms of Service` | Footer Link | Respaldo ético y legal acorde a códigos de conducta ACM/IEEE y CIP. |
| **Footer / Legal** | `Privacidad y Cookies` | `Privacy Policy` | Footer Link | Compromiso de protección de datos personales y uso anónimo de cámaras en WebAR. |

---

### 6.2.3. Searching Systems

El sistema de búsqueda de Platter está diseñado para que el comensal encuentre preparaciones compatibles con su presupuesto, apetito y requerimientos médicos de salud en menos de 3 interacciones:

#### 1. Mecanismos de Búsqueda Provistos
* **Búsqueda en Tiempo Real con Autocompletado Predictivo (Live Search):**
  * Campo de texto persistente en la cabecera de la carta con respuesta instantánea basada en *debounce* de 250 ms.
  * Tolerancia a errores tipográficos y variantes fonéticas culinarias (ej. coincidencia automática entre *"ceviche"*, *"cebiche"* o *"seviche"*).
  * Despliegue de sugerencias dinámicas y platos populares al enfocar el cursor o pulsar sobre la barra sin necesidad de escribir.

#### 2. Filtros Avanzados Combinables
* **Filtro de Seguridad Alimentaria (Alérgenos y Dietas Específicas):**
  * Chips interactivos de exclusión que permiten deseleccionar platos que contengan alérgenos críticos: *Sin Gluten*, *Sin Lactosa*, *Sin Mariscos*, *Sin Frutos Secos*, *Sin Huevo*, *Vegano*, *Vegetariano*.
  * Al activar el filtro *"Soy Celíaco"*, el catálogo oculta de forma preventiva y automática toda preparación que contenga trigo, avena, cebada o centeno, o que comparta freidora.
* **Filtro por Rango de Precios:**
  * Control deslizante (*Range Slider*) que permite acotar el presupuesto por plato (ej. *Hasta S/ 30.00*, *S/ 30 - S/ 60*, *Más de S/ 60*).
* **Filtro de Experiencia Inmersiva:**
  * Interruptor booleano rápido: *"Solo platos con visualización WebAR 3D disponible"*.
* **Filtro por Tiempo de Preparación y Aporte Calórico:**
  * Para comensales con prisa en horario de almuerzo (*"Menos de 15 minutos"*) o regímenes hipocalóricos (*"Menos de 500 kcal"*).

#### 3. Visualización de Resultados y Manejo de Estados Vacíos
* **Presentación de Resultados:** Rejilla dinámica de tarjetas con contador en vivo (*"7 platos encontrados con tus preferencias"*), destacando en cada tarjeta los sellos de seguridad alimentaria y el botón de WebAR.
* **Estado de Búsqueda Vacía (*Zero Results State*):**  
  En caso de que una combinación muy restrictiva de filtros no arroje resultados (ej. plato de fondo vegano, sin frutos secos y por menos de S/ 15), la interfaz presenta una ilustración amigable en tonos beige y azul, acompañada de:
  1. Mensaje empático: *"No encontramos platos que cumplan todos los filtros seleccionados simultáneamente"*.
  2. Sugerencias guiadas: *"Prueba quitando el filtro de precio"* o *"Ver platos vegetarianos alternativos"*.
  3. Botón de acción inmediata: *"Restablecer Filtros"*.

---

### 6.2.4. SEO Tags, Meta Tags y ASO Elements

Para maximizar el posicionamiento orgánico en motores de búsqueda de la Landing Page comercial y facilitar la indexación de las cartas digitales públicas de los restaurantes asociados, se formalizan las siguientes especificaciones:

#### 1. SEO Tags y Meta Tags para Páginas Web

A continuación se detallan las etiquetas SEO y meta tags configuradas para las tres vistas principales de la plataforma:

##### A. Landing Page Comercial Principal (`/`)

```html
<!-- Metadatos Primarios -->
<title>Platter | Menús Digitales con Realidad Aumentada (WebAR) e Inteligencia Artificial</title>
<meta name="title" content="Platter | Menús Digitales con Realidad Aumentada (WebAR) e Inteligencia Artificial">
<meta name="description" content="Digitaliza la carta de tu restaurante con Realidad Aumentada en 3D e IA multimodal. Permite a tus comensales ver el plato a escala real en mesa sin instalar apps. Aumenta tus ventas y elimina quejas.">
<meta name="keywords" content="carta digital restaurante, menu realidad aumentada, platos 3d en mesa, webar restaurante, ia gastronomica, gemini vision restaurantes, carta qr interactiva, alergenos restaurante">
<meta name="author" content="Platter Technologies - 1ASI0728 Arquitecturas de Software Emergentes UPC">
<meta name="robots" content="index, follow">
<link rel="canonical" href="https://platter.app/">

<!-- Open Graph / Facebook / WhatsApp / LinkedIn -->
<meta property="og:type" content="website">
<meta property="og:url" content="https://platter.app/">
<meta property="og:title" content="Platter | Cartas Gastronómicas en Realidad Aumentada sin Instalación">
<meta property="og:description" content="Multiplica el apetito y las ventas de tu restaurante. Tus comensales proyectan la comida en su mesa en escala 1:1 desde el navegador web.">
<meta property="og:image" content="https://platter.app/assets/og-platter-hero-preview.png">
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
<meta property="og:locale" content="es_PE">
<meta property="og:locale:alternate" content="en_US">

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:url" content="https://platter.app/">
<meta name="twitter:title" content="Platter | Digitalización Gastronómica con WebAR e IA">
<meta name="twitter:description" content="Visualiza tus platos favoritos a tamaño real en tu mesa con Realidad Aumentada escaneando el QR del restaurante.">
<meta name="twitter:image" content="https://platter.app/assets/og-platter-hero-preview.png">
```

##### B. Carta Digital Pública por Restaurante (`/menu/:restaurantSlug`)

```html
<title>Carta Digital 3D de {Nombre del Restaurante} | Menú WebAR Interactivo en Platter</title>
<meta name="description" content="Explora la carta de {Nombre del Restaurante} en Realidad Aumentada. Mira cada plato en tu mesa en escala 1:1, consulta ingredientes reales, alérgenos normados e información nutricional.">
<meta name="keywords" content="menu {Nombre del Restaurante}, carta 3d {Nombre del Restaurante}, pedir en {Nombre del Restaurante}, platos en realidad aumentada, comida sin gluten {Nombre del Restaurante}">
<meta name="robots" content="noindex, follow">
<link rel="canonical" href="https://platter.app/menu/{restaurantSlug}">
<meta property="og:type" content="restaurant.menu">
<meta property="og:title" content="Carta Digital Interactiva - {Nombre del Restaurante} en Platter">
<meta property="og:description" content="Mira los platos de nuestra carta en Realidad Aumentada 3D directamente sobre tu mesa.">
<meta property="og:image" content="https://platter.app/assets/restaurants/{restaurantSlug}-cover.png">
```

##### C. Portal de Registro y Onboarding B2B (`/onboarding`)

```html
<title>Comienza Gratis con Platter | Digitaliza tu Restaurante en 2 Minutos</title>
<meta name="description" content="Únete a cientos de restaurantes que aumentan su ticket promedio con cartas en Realidad Aumentada. Prueba gratuita de 14 días sin tarjeta de crédito.">
<meta name="robots" content="index, nofollow">
<link rel="canonical" href="https://platter.app/onboarding">
```

#### 2. Elementos ASO (App Store Optimization) para la Aplicación Móvil / PWA

Para la distribución de la Progressive Web App (PWA) de Platter y su eventual empaquetamiento en Google Play Store y Apple App Store para administradores de salón, se establecen los siguientes metadatos ASO:

* **App Title (Título de la App):** `Platter: Menús 3D & Cartas WebAR` *(35 caracteres)*  
  Incorpora la marca y las palabras clave de mayor volumen de búsqueda en el sector.
* **App Subtitle (Subtítulo de la App - iOS):** `Platos en Realidad Aumentada & IA` *(33 caracteres)*  
  Sintetiza la propuesta de valor diferenciada en una frase contundente.
* **App Keywords (Palabras Clave ASO):** `carta digital,menu restaurante,realidad aumentada,webar,platos 3d,alergenos,sin gluten,qr restaurante,ia gastronomica,modelado comida` *(separadas por comas, sin espacios innecesarios)*.
* **App Description (Descripción ASO para Tiendas):**  
  * *Párrafo Promocional:* "¿Cansado de cartas impresas desactualizadas o fotos que no reflejan el tamaño real de tus preparaciones? Platter transforma la experiencia culinaria de tus clientes permitiéndoles proyectar cada plato directamente en su mesa a escala 1:1 mediante Realidad Aumentada instantánea."  
  * *Características Destacadas:*
    * Digitalización express en menos de 2 minutos tomando una sola foto con tu smartphone.
    * Inferencia automática de ingredientes, alérgenos y calorías con Google Gemini Vision.
    * Experiencia WebAR para comensales sin necesidad de descargar aplicaciones pesadas.
    * Códigos QR dinámicos por mesa con actualización en tiempo real de platos agotados.
    * Aumento comprobado del 25% al 35% en la conversión de venta de platos destacados en salón.

---

### 6.2.5. Navigation Systems

La navegación en Platter sigue una arquitectura multicanal orientada a guiar al usuario a sus objetivos sin callejones sin salida:

1. **Navegación Global (Persistente):**
   * *Landing Page:* Barra superior fija con logotipo oficial, enlaces ancla a secciones (*Cómo Funciona*, *Beneficios*, *Demostración 3D*, *Precios*, *Preguntas Frecuentes*), selector de idioma (EN / ES) y botón CTA destacado *"Iniciar Prueba Gratis"*.
   * *Carta Digital WebAR:* Barra superior compacta con botón de regreso, indicador de mesa activa (*"Mesa 04"*), buscador en vivo, selector de idioma y botón flotante de acceso al carrito o resumen de selección.
2. **Navegación Local (Contextual de Menú):**
   * Barra de pestañas horizontales fija (*Sticky Category Bar*) debajo del buscador con desplazamiento lateral suave (*scroll horizontal*) que permite saltar entre categorías gastronómicas (*Entradas*, *Fondos*, *Bebidas*, *Postres*). Incluye sincronización de desplazamiento (*scrollspy*) que resalta la categoría visible automáticamente al deslizar la pantalla.
3. **Navegación Contextual (Nivel de Componente):**
   * Dentro de cada tarjeta de plato: botón secundario *"Ver alérgenos y detalles nutricionales"* que despliega un Bottom Sheet, botón primario con icono de cubo 3D *"Ver en tu Mesa"* que activa el visor WebXR / AR Quick Look, y botones de sugerencia de maridaje (*"Combina perfecto con..."*).
4. **Navegación Suplementaria (Footer y Ayuda):**
   * Pie de página estructurado en 4 columnas:
     * *Columna 1:* Identidad corporativa, propósito de Platter y redes sociales.
     * *Columna 2 (Producto):* Enlaces a características, WebAR, IA gastronómica y compatibilidad de dispositivos.
     * *Columna 3 (Recursos y Soporte):* Centro de ayuda para restaurantes, calculadora de ROI y canal de contacto.
     * *Columna 4 (Marco Ético y Legal):* Enlaces a Términos y Condiciones, Política de Privacidad, declaración ética de IA y cumplimiento de estándares de ingeniería de software.

---

## 6.3. Landing Page UI Design

El diseño de interfaz del Landing Page traduce las decisiones de arquitectura de información (sección 6.2) en una página estática de una sola columna, pensada para dos segmentos con objetivos distintos: los **dueños y administradores de restaurantes**, que deben entender el valor del producto y solicitar un piloto, y los **comensales**, que pueden probar la experiencia de Realidad Aumentada desde su navegador.
Cada sección responde a una User Story del Epic EP01 (US01 a US04)

Las llamadas a la acción (CTA) están separadas por segmento para cumplir el enunciado del proyecto:
 
| CTA | Segmento | Destino |
| :--- | :--- | :--- |
| Solicitar piloto gratis / Solicitar piloto | Dueños y administradores | Formulario de piloto del mismo Landing (US04) y, una vez aprobada la cuenta, descarga de la app móvil de gestión |
| Probar demo en AR / Ver plato en AR | Comensales y visitantes | Demostrador WebAR (US01) |
| Elegir plan | Dueños y administradores | Formulario de piloto con el plan preseleccionado (US03) |

### 6.3.1. Landing Page Wireframe

Los wireframes están en escala de grises para validar estructura, jerarquía y recorrido antes de aplicar identidad visual. Cada bloque tiene una etiqueta numerada con su nombre para facilitar su referencia en la explicación.

![Landing Page Wireframe - Desktop1](./assets/6.3.1-landing-wireframe-desktop1.png)

![Landing Page Wireframe - Desktop2](./assets/6.3.1-landing-wireframe-desktop2.png)

| # | Sección | Propósito | User Story |
| :-: | :--- | :--- | :-: |
| 01 | Header | Logo, navegación por anclas (Cómo funciona, Beneficios, Demo AR, Planes, Contacto), selector de idioma ES / EN y CTA principal. En móvil se reduce a logo, idioma y menú hamburguesa. | US01 |
| 02 | Hero | Propuesta de valor, dos CTA diferenciados por segmento e imagen del producto en uso. | US01, US04 |
| 03 | Cómo funciona | Tres pasos (foto, modelo 3D, QR) en tarjetas de igual jerarquía. | US01 |
| 04 | Demo AR interactiva | En desktop muestra un código QR para probar en el celular y un botón de visor 3D en pantalla; en móvil activa directamente la vista AR. | US01 |
| 05 | Beneficios y ROI | Tres métricas destacadas y un espacio para el testimonio de un restaurante piloto. | US02 |
| 06 | Casos de uso | Tarjetas por tipo de cocina (criolla, marina, pollerías y especialidades). | US02 |
| 07 | Planes y calculadora MYPE | Tres planes mensuales sin cobro por plato y calculadora por número de mesas y platos. | US03 |
| 08 | Solicitud de piloto | Formulario con nombre del restaurante, correo, teléfono y número de mesas, con validación de campos obligatorios. | US04 |
| 09 | Footer | Enlaces de producto, contacto, Términos y Condiciones, privacidad y selector de idioma. | - |

**Principios aplicados**
- **Jerarquía visual y patrón de lectura en F:** el título y la propuesta de valor ocupan la parte superior izquierda en desktop; la imagen balancea el lado derecho.
- **Un CTA primario por bloque:** el botón principal siempre es el de mayor peso visual; la acción secundaria usa estilo contorno.
- **Arquitectura de información:** el orden de las secciones sigue el recorrido de decisión del dueño (entender, ver beneficios, comparar precio, solicitar piloto) y el menú ancla a las mismas secciones.
- **Diseño inclusivo:** objetivos táctiles de al menos 44 px de alto, un campo por fila en móvil, selector de idioma visible (es_419 / en_US) y estructura pensada para atributos ARIA y navegación por teclado en la implementación.
- **Responsive:** en móvil las tarjetas de tres columnas pasan a una sola columna y los botones ocupan el ancho completo.

### 6.3.2. Landing Page Mock-up

El mock-up aplica color y tipografía sobre los wireframes: la paleta oficial de la sección 6.1.1 (coral, azul medianoche y crema), tipografía Outfit y Plus Jakarta Sans, tarjetas con esquinas redondeadas y sombras suaves, manteniendo los criterios de contraste, espaciado de 8 puntos y objetivos táctiles de las secciones 6.1.1 y 6.1.2.

![Landing Page Mock-up - Desktop1](./assets/6.3.2-landing-mockup-desktop1.png)

![Landing Page Mock-up - Desktop2](./assets/6.3.2-landing-mockup-desktop2.png)

| Elemento | Valor | Uso |
| :--- | :--- | :--- |
| Coral de acento (`--color-coral-accent`) | `#E76F51` | CTA, números de pasos, plan destacado |
| Azul medianoche (`--color-bg-dark`) | `#121C33` | Títulos, texto principal y footer |
| Fondo claro (`--color-bg-light`) | `#F7F3ED` | Hero, demo AR y planes |
| Éxito (`--color-status-success`) | `#2A9D8F` | Íconos de verificación y etiquetas de alérgenos |
| Línea cálida | `#E5DDD0` | Bordes de tarjetas y campos de formulario |
| Tipografía de títulos | Outfit (SemiBold, Bold) | Títulos, precios y cifras destacadas (tamaño 20 px o más) |
| Tipografía de lectura y UI | Plus Jakarta Sans (Regular, Medium, SemiBold, Bold) | Párrafos, botones, formularios y etiquetas |

## 6.4. Applications UX/UI Design

La solución tiene dos aplicaciones con las que interactúan directamente los segmentos objetivo:
 
- **Platter Admin - aplicación móvil Flutter:** usada por el dueño o administrador del restaurante para registrar platos con IA, asignar modelos 3D, generar códigos QR, controlar disponibilidad y revisar métricas (Epics EP02, EP03, EP06).
- **Platter AR Viewer - aplicación web móvil, WebAR:** usada por el comensal al escanear el QR de su mesa, sin instalación ni registro (Epics EP04 y EP05).

### 6.4.1. Applications Wireframes

![Wireframes Platter Admin (Flutter)](./assets/6.4.1-wireframes-admin.png)
 
![Wireframes Platter AR Viewer (WebAR)](./assets/6.4.1-wireframes-viewer.png)

**Platter Admin (Flutter)**
| ID | Pantalla | Contenido principal | User Story |
| :-: | :--- | :--- | :-: |
| A01 | Inicio de sesión | Correo, contraseña y acceso | - |
| A02 | Inicio | Resumen de platos, escaneos y vistas AR; accesos rápidos | US19 |
| A03 | Catálogo | Lista de platos con estado e interruptor de disponibilidad | US18 |
| A04 | Capturar plato | Cámara o galería, validación de formato y peso (JPEG/PNG, máximo 10 MB) | US05 |
| A05 | Analizando con IA | Estado de carga y opción de continuar manualmente si falla | US06, US21 |
| A06 | Ficha sugerida | Nombre, categoría, descripción, ingredientes, alérgenos y calorías editables | US06 a US09 |
| A07 | Modelo 3D | Modelo sugerido por categoría y galería para elegir otro | US10 |
| A08 | Plato publicado | Confirmación y acceso al catálogo | US09 |
| A09 | Mesas y QR | Alta por rango de mesas y lista con estado | US11 |
| A10 | Descarga de QR | Vista previa de la plantilla con logo y descarga PDF/PNG | US12 |
| A11 | Analítica | Ranking de platos vistos en AR y exportación CSV | US19 |
| A12 | Mi plan | Plan vigente, método de pago y estado de la suscripción | US20 |

**Platter AR Viewer (WebAR)**
| ID | Pantalla | Contenido principal | User Story |
| :-: | :--- | :--- | :-: |
| D01 | Carta digital | Número de mesa, categorías y platos con alérgenos | US13 |
| D02 | Filtros de alérgenos | Selección de alérgenos a excluir y mensaje cuando no hay resultados | US15 |
| D03 | Detalle del plato | Foto, ingredientes, calorías, advertencias y botón Ver en mi mesa | US17 |
| D04 | Vista AR | Plato a escala 1:1 sobre la mesa con escala bloqueada | US14, US16 |
| D05 | Visor 3D | Alternativa para dispositivos sin compatibilidad AR | US14 |
| D06 | Mesa inactiva | Mensaje amigable y enlace al menú general | US13 |
 
Decisiones de diseño: navegación inferior de cuatro destinos en Platter Admin (Inicio, Platos, Mesas, Plan), flujo secuencial paso a paso para el alta de platos, y en AR Viewer una sola pantalla de carta con acceso al AR en máximo 2 toques

### 6.4.2. Applications Wireflow Diagrams

Cada wireflow representa un User Goal y reutiliza los wireframes de la sección anterior. Las flechas continuas indican el camino principal (happy path) y las discontinuas los caminos alternativos.

| ID | User Goal | Persona | Recorrido | User Stories |
| :-: | :--- | :--- | :--- | :-: |
| WF-01 | Registrar un plato con ayuda de IA | Carlos Mendoza | A02, A04, A05, A06, A07, A08. *Alternativo:* si la IA falla o tarda más de 5 s, A05 pasa a A06 con campos vacíos para completar manualmente. | US05 a US10, US21 |
| WF-02 | Generar e imprimir los QR de las mesas | Carlos Mendoza | A02, A09, A10 | US11, US12 |
| WF-03 | Controlar disponibilidad y revisar interacción | Carlos Mendoza | A02, A03 (marcar agotado), A11 | US18, US19 |
| WF-04 | Ver un plato en AR antes de ordenar | Valeria Ramos | D01, D02, D03, D04. *Alternativos:* D01 a D06 si el QR no está activo; D03 a D05 si el dispositivo no soporta AR. | US13 a US17 |

**WF-01. Registrar un plato con ayuda de IA**
 
![Wireflow WF-01](./assets/6.4.2-wireflow-wf01.png)
 
**WF-02. Generar e imprimir los QR de las mesas**
 
![Wireflow WF-02](./assets/6.4.2-wireflow-wf02.png)
 
**WF-03. Controlar disponibilidad y revisar interacción**
 
![Wireflow WF-03](./assets/6.4.2-wireflow-wf03.png)
 
**WF-04. Ver un plato en AR antes de ordenar**
 
![Wireflow WF-04](./assets/6.4.2-wireflow-wf04.png)


*Nota: Las secciones 6.4.3 (Applications Mock-ups), 6.4.4 (Applications User Flow Diagrams) y 6.5 (Applications Prototyping) corresponden al siguiente hito de entrega (TB2 - Semana 12), conforme a la estructura curricular y alcance del proyecto.*


# Conclusiones

1. **Alineación con la problemática y eliminación de fricción para el usuario final:**
   Se evidenció que la brecha tradicional entre la expectativa visual del comensal y el plato servido en mesa representaba un factor crítico de indecisión, quejas y pérdida de reputación para los negocios gastronómicos. Mediante la adopción de una arquitectura orientada a la eliminación de fricción basada en **WebAR sin instalación** (aprovechando estándares nativos como WebXR Device API para Android y AR Quick Look para iOS), Platter resuelve la reticencia del usuario final. El comensal logra visualizar el plato en su entorno a escala física real 1:1 en menos de 2 segundos y con un máximo de 2 toques tras escanear el código QR de mesa, sin requerir descargas de aplicaciones ni registros obligatorios.

2. **Liderazgo en costos y viabilidad operativa para el segmento MYPE:**
   Las soluciones de Realidad Aumentada existentes en el mercado imponen tarifas de modelado fotogramétrico prohibitivas (desde £49 por plato) y flujos manuales lentos incompatibles con la realidad económica de los restaurantes pequeños y medianos. Platter supera esta barrera económica mediante la convergencia de una biblioteca de modelos 3D normalizados y calibrados métricamente junto a un pipeline de procesamiento automatizado con **Google Gemini Vision**. Dicha integración reduce la carga operativa del administrador del restaurante, autogenerando fichas gastronómicas completas (descripción, ingredientes, calorías y etiquetado normado de alérgenos) en menos de 3.5 segundos a partir de una simple fotografía tomada con el smartphone.

3. **Gobernanza del dominio mediante Domain-Driven Design (DDD):**
   La aplicación sistemática de EventStorming, Candidate Context Discovery y Bounded Context Canvases permitió descomponer el dominio en Bounded Contexts cohesivos, aislando el núcleo de valor competitivo (*Core Domain*: Catálogo de Platos, Análisis Gastronómico con IA y Experiencia WebAR) de los servicios de soporte y genéricos (Gestión de Mesas y Facturación). La formalización del *Context Map* mediante la incorporación de una **Capa Anticorrupción (ACL)** para aislar la API de Google Gemini y un contrato **Open Host Service / Published Language (OHS / PL)** para la publicación de la carta digital, blindó el núcleo del sistema frente a cambios de contratos externos y facilitó la trazabilidad técnica entre requerimientos y diseño.

4. **Robustez y resiliencia arquitectónica (ADD y C4 Model):**
   A través del modelado con el C4 Model y el proceso de Attribute-Driven Design (ADD), se fundamentaron decisiones técnicas orientadas a cumplir escenarios de calidad estrictos:
   * **Rendimiento:** Despacho de activos 3D comprimidos con Draco a través de Amazon S3 y CloudFront (CDN) con cabeceras de caché inmutable, alcanzando tiempos de entrega inferiores a 1.5 segundos en redes móviles 4G.
   * **Tolerancia a fallos:** Protección del backend mediante el patrón **Circuit Breaker (Resilience4j)** ante posibles degradaciones de la API de Google Gemini, garantizando degradación elegante hacia la carga manual en menos de 100 ms sin bloquear los hilos del servidor.
   * **Escalabilidad y Concurrencia:** Adopción de un monolito modular en Spring Boot 3 / Java 21 respaldado por Redis para retener catálogos en memoria, permitiendo atender hasta 500 peticiones concurrentes por segundo y reduciendo en más de un 85% las consultas directas a PostgreSQL durante horas pico.

5. **Diseño Táctico y Experiencia de Usuario Centrada en la Conversión (Hito TP1):**
   La transición del diseño estratégico al diseño táctico (Capítulo V) permitió formalizar la separación de responsabilidades en capas limpias (Domain, Application, Infrastructure e Interfaces) para cada uno de los cuatro Bounded Contexts, asegurando que la lógica de negocio permanezca desacoplada de frameworks y protocolos de transporte. Esta solidez arquitectónica se articula directamente con las definiciones de diseño de experiencia de usuario (Capítulo VI), donde la arquitectura de información, las directrices de estilo accesibles bajo WCAG 2.1 nivel AA y los flujos de interacción de pantalla (wireflows) garantizan una curva de aprendizaje mínima para el administrador del restaurante y una interacción inmersiva libre de fricción para el comensal.

# Recomendaciones

1. **Gestión y control de calidad del pipeline de modelos 3D:**
   Se recomienda implementar un control estricto sobre los modelos poligonales y texturas integrados en la biblioteca compartida de Platter, garantizando que el peso de los archivos .glb y .usdz no supere el umbral de 3.0 MB una vez procesados con compresión Draco. Asimismo, debe auditarse continuamente la compatibilidad de sombreado PBR tanto en navegadores móviles Android (Chrome / WebXR) como en iOS (Safari / AR Quick Look) para evitar artefactos visuales en mesa.

2. **Estrategia de invalidación reactiva de caché:**
   Considerando que los restaurantes actualizan la disponibilidad de insumos en tiempo real ante quiebres de stock en cocina, se aconseja que las operaciones de actualización de catálogo emitan eventos de dominio que purguen reactivamente las claves correspondientes en Redis. De este modo, se asegura que los comensales no ordenen preparaciones agotadas, sin incurrir en una limpieza global que degrade el rendimiento del servidor en horas pico.

3. **Supervisión de cuotas y manejo de contingencia para la API de IA:**
   A medida que se incorporen nuevos restaurantes durante la fase piloto, se debe monitorear el consumo de tokens y los límites de peticiones por minuto (RPM) de Google Gemini Vision. Es recomendable instrumentar alertas tempranas al alcanzar el 80% de la cuota y prever colas de reintento asíncronas para momentos de alta concurrencia de registro de cartas.

4. **Validación empírica en pruebas de campo (Salón Piloto):**
   Para los siguientes sprints de desarrollo e implementación, se sugiere realizar pruebas de usabilidad y telemetría de red directamente en salones de prueba. Esto permitirá evaluar el comportamiento de detección de superficies horizontales del visor WebAR bajo distintas condiciones de iluminación física y mantelería, asegurando que el bloqueo de escala métrica 1:1 funcione de forma idéntica en diversos dispositivos de gama media y alta.

5. **Auditoría continua de accesibilidad y pruebas de contraste en interfaces:**
   Para las fases de construcción y prototipado del siguiente hito (TB2), se recomienda implementar linters automáticos de accesibilidad (axe-core / Lighthouse) en los entornos de integración continua para validar que todas las pantallas mantengan los ratios de contraste establecidos (mínimo 4.5:1) y que los atributos ARIA definidos en las guías de estilo se respeten estrictamente en la Landing Page y en el visor WebAR.

# Bibliografía

<div style="text-align: justify">

ARInsider. (2020, 22 de junio). *Does AR really boost eCommerce conversions?* https://arinsider.co/2020/06/22/does-ar-really-boost-ecommerce-conversions/

Ecosire. (2024). *Realidad aumentada en comercio electrónico y venta minorista: pruébelo antes de comprar*. https://ecosire.com/es/blog/augmented-reality-ecommerce-retail

Evans, E. (2003). *Domain-Driven Design: Tackling Complexity in the Heart of Software*. Addison-Wesley Professional.

Gothelf, J., & Seiden, J. (2021). *Lean UX: Designing Great Products with Agile Teams* (3rd ed.). O'Reilly Media.

Ministerio de la Producción [Produce]. (2021, 14 de mayo). *Terrazas gastronómicas se cuadruplicaron en menos de un mes* [Comunicado de prensa]. Andina, Agencia Peruana de Noticias. https://andina.pe/agencia/noticia-terrazas-gastronomicas-se-cuadruplicaron-menos-un-mes-845218.aspx

Nielsen Norman Group. (2020). *Wireframing and Prototyping Best Practices*. https://www.nngroup.com/

Perú Retail. (2024, 7 de diciembre). *Hay 50 mil restaurantes menos que en 2019 y las ventas siguen un 3% por debajo, alerta el gremio*. https://www.peru-retail.com/?p=355115

Rosenfeld, L., Morville, P., & Arango, J. (2015). *Information Architecture: For the Web and Beyond* (4th ed.). O'Reilly Media.

World Wide Web Consortium [W3C]. (2018). *Web Content Accessibility Guidelines (WCAG) 2.1*. https://www.w3.org/TR/WCAG21/

</div>

# Anexos

### Anexo A. Repositorios Oficiales del Proyecto

- **Repositorio de Documentación (Reporte Oficial):** [https://github.com/upc-pre-1ASI0728-2620-9046-Platter/platter-report](https://github.com/upc-pre-1ASI0728-2620-9046-Platter/platter-report)
- **Repositorio de Solución de Software:** [https://github.com/upc-pre-1ASI0728-2620-9046-Platter/platter](https://github.com/upc-pre-1ASI0728-2620-9046-Platter/platter)

### Anexo B. Organización de Componentes Digitales

La solución se estructura como un monorepo compuesto por los siguientes módulos:
- `landing`: Aplicación web estática para adquisición y portal comercial (HTML5, CSS3, JavaScript).
- `webar`: Experiencia inmersiva en mesa para comensales (Three.js, WebXR, AR Quick Look).
- `admin_app`: Aplicación móvil multiplataforma para administración del restaurante (Flutter / Dart).
- `backend`: Arquitectura de servicios basada en DDD y Spring Boot 3 con base de datos PostgreSQL y Redis.
