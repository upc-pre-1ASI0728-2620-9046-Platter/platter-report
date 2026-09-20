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

**Septiembre - 2026**

</h3>
</div>

# Contenido

## Tabla de contenidos

- [Registro de versiones del informe](#registro-de-versiones-del-informe)

- [Project Report Collaboration Insights](#project-report-collaboration-insights)

- [Contenido](#contenido)

- [Student Outcome](#student-outcome-1)

- [Capítulo I: Introducción](#capitulo-i-introduccion)

# Student Outcome

El curso contribuye al cumplimiento del Student Outcome ABET:

**ABET – EAC - Student Outcome 3**

**Criterio:** *Capacidad de comunicarse efectivamente con un rango de audiencias.*

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 3.

| Criterio específico | Acciones realizadas | Conclusiones |
| :--- | :--- | :--- |
| **Comunica oralmente sus ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerárquicos, en el marco del desarrollo de un proyecto en ingeniería.** | **Alvarado De La Cruz, Juan Carlos**<br>*TB1*<br>Expuse ante el equipo y en el video de sustentación los fundamentos de la descomposición estratégica bajo Domain-Driven Design (DDD), justificando la delimitación de Bounded Contexts y la implementación de una Capa Anticorrupción (ACL) para la integración con Google Gemini. Adapté el lenguaje técnico para comunicar claramente cómo la arquitectura soporta los requerimientos de negocio de restaurantes e inversionistas.<br><br>**Duran Diaz, Antonio Rodrigo**<br>*TB1*<br>Participé activamente en las sesiones de discusión grupal y en la grabación del video de presentación de la entrega, explicando con objetividad los escenarios de atributos de calidad priorizados en Attribute-Driven Design (ADD) y cómo la infraestructura en la nube de AWS responde a las demandas de alta concurrencia en horas pico.<br><br>**Nakasone Gomes, Marco Antonio**<br>*TB1*<br>Presenté oralmente en las reuniones de sincronización y en la exposición grabada los resultados del análisis de problemáticas del sector gastronómico y los supuestos de Lean UX, transmitiendo con claridad a perfiles tanto técnicos como de negocio el valor de la proyección en Realidad Aumentada sin fricción para el comensal.<br><br>**Teves Samaniego, Joan Fernando**<br>*TB1*<br>Expuse en el video grupal y en las reuniones técnicas los diagramas de interacción y flujo de mensajes mediante Domain Storytelling, describiendo detalladamente la secuencia técnica entre los clientes móviles, las APIs REST y los servicios en la nube de forma estructurada, fluida y comprensible para el equipo evaluador. | Durante el desarrollo del hito TB1, el equipo demostró capacidad para transmitir conceptos técnicos complejos de ingeniería de software a diversas audiencias. Se articularon con precisión técnica y pertinencia de negocio las decisiones de diseño estratégico, modelado de dominio y esquemas de infraestructura en la nube. A través de reuniones de retrospectiva internas y la sustentación en video, cada integrante adaptó su registro comunicativo para justificar de forma objetiva la viabilidad técnica y operativa de la solución ante evaluadores académicos y potenciales interesados del sector gastronómico. |
| **Comunica en forma escrita ideas y/o resultados con objetividad a público de diferentes especialidades y niveles jerárquicos, en el marco del desarrollo de un proyecto en ingeniería.** | **Alvarado De La Cruz, Juan Carlos**<br>*TB1*<br>Redacté y consolidé los capítulos de diseño estratégico en Markdown, elaborando la especificación formal del Context Mapping y los diagramas C4 (Contexto, Contenedores y Despliegue). Cuidé la consistencia del lenguaje ubicuo del proyecto, documentando los contratos de integración y las decisiones arquitectónicas conforme al estándar de ingeniería solicitado.<br><br>**Duran Diaz, Antonio Rodrigo**<br>*TB1*<br>Elaboré las especificaciones técnicas de los escenarios de calidad (Quality Attribute Scenarios) y el Backlog de Drivers Arquitectónicos, documentando de forma estructurada los requisitos de rendimiento, disponibilidad y escalabilidad, así como las tácticas arquitectónicas seleccionadas para mitigarlos.<br><br>**Nakasone Gomes, Marco Antonio**<br>*TB1*<br>Redacté la caracterización de la startup, la problemática del sector gastronómico, las declaraciones de problema de Lean UX, supuestos e hipótesis. Documenté los hallazgos en tablas y formatos estandarizados dentro del informe, facilitando la comprensión de los dolores del cliente tanto para perfiles de negocio como de desarrollo.<br><br>**Teves Samaniego, Joan Fernando**<br>*TB1*<br>Documenté la especificación formal de requerimientos mediante To-Be Scenario Mapping, User Stories bajo el formato Gherkin y los diagramas de secuencia de Domain Storytelling en Mermaid. Garanticé que la documentación escrita fuera rigurosa, no ambigua y completamente trazable con los objetivos del sistema. | La redacción colaborativa del informe técnico en GitHub bajo estándares de Markdown y conventional commits permitió consolidar un cuerpo documental riguroso, coherente y profesional. Se logró comunicar con claridad el análisis del problema, los modelos formales de dominio y las decisiones de arquitectura de software, empleando notaciones estándar (C4 Model, diagramas UML/secuencia y plantillas Lean UX). El producto escrito evidencia objetividad técnica y una estructura que satisface las exigencias metodológicas del curso y de la práctica profesional de la ingeniería de software. |

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

### 4.1.2. Attribute-Driven Design Inputs.

#### 4.1.2.1. Primary Functionality (Primary User Stories).

#### 4.1.2.2. Quality Attributes Scenarios.

#### 4.1.2.3. Constraints.

### 4.1.3. Architectural Drivers Backlog.

### 4.1.4. Architectural Design Decisions.

### 4.1.5. Quality Attribute Scenario Refinements.

## 4.2. Strategic-Level Domain-Driven Design.

### 4.2.1. EventStorming.

### 4.2.2. Candidate Context Discovery.

### 4.2.3. Domain Message Flows Modeling.

### 4.2.4. Bounded Context Canvases.

### 4.2.5. Context Mapping.

## 4.3. Software Architecture.

### 4.3.1. Software Architecture System Landscape Diagram.

### 4.3.2. Software Architecture Context Level Diagrams.

### 4.3.3. Software Architecture Container Level Diagrams.

### 4.3.4. Software Architecture Deployment Diagrams.

# Conclusiones

## Conclusiones y recomendaciones.

# Video About-the-Team.

# Bibliografía

<div style="text-align: justify">
ARInsider. (2020, 22 de junio). *Does AR really boost eCommerce conversions?* https://arinsider.co/2020/06/22/does-ar-really-boost-ecommerce-conversions/
 
Ecosire. (2024). *Realidad aumentada en comercio electrónico y venta minorista: pruébelo antes de comprar*. https://ecosire.com/es/blog/augmented-reality-ecommerce-retail
 
Ministerio de la Producción [Produce]. (2021, 14 de mayo). *Terrazas gastronómicas se cuadruplicaron en menos de un mes* [Comunicado de prensa]. Andina, Agencia Peruana de Noticias. https://andina.pe/agencia/noticia-terrazas-gastronomicas-se-cuadruplicaron-menos-un-mes-845218.aspx
 
Perú Retail. (2024, 7 de diciembre). *Hay 50 mil restaurantes menos que en 2019 y las ventas siguen un 3% por debajo, alerta el gremio*. https://www.peru-retail.com/?p=355115
 
</div>

# Anexos
