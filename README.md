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

# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

### 1.1.2. Perfiles de integrantes del equipo

## 1.2. Solution Profile

### 1.2.1 Antecedentes y problemática

### 1.2.2 Lean UX Process.

#### 1.2.2.1. Lean UX Problem Statements.

#### 1.2.2.2. Lean UX Assumptions.

#### 1.2.2.3. Lean UX Hypothesis Statements.

#### 1.2.2.4. Lean UX Canvas.

## 1.3. Segmentos objetivo.

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

## 3.1. To-Be Scenario Mapping

## 3.2. User Stories.

## 3.3. Impact Mapping.

## 3.4. Product Backlog.

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

# Anexos
