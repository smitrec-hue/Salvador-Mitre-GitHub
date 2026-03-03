# Salvador-Mitre-GitHub

## Tabla de contenidos
1. [Dashboard de Tendencias Retail](#1-dashboard-de-tendencias-retail)
2. [Análisis de embudo y retención de clientes para Mercado Libre](#2-análisis-de-embudo-y-retención-de-clientes-para-mercado-libre)
3. [Sistema de Información Gerencial (Data Marts)](#3-sistema-de-información-gerencial-data-marts)
4. [Indicadores de Sustentabilidad (IMAVA)](#4-indicadores-de-sustentabilidad-imava)
5. [Optimización de Reportes Ejecutivos](#5-optimización-de-reportes-ejecutivos)




## 1\. Dashboard de Tendencias Retail

**Descripción del proyecto:** Visualización estratégica de indicadores clave mediante Dashboards dinámicos, transformando volúmenes de datos en hojas de ruta para la alta dirección.

- **Empresa:** Proyecto TripleTen Bootcamp.

- **Contexto:** Necesidad de transformar datos crudos de ventas en indicadores visuales interpretables para el sector retail.

La Dirección Comercial de la empresa buscaba responder estas dos preguntas centrales:

1.  **¿Qué categorías de departamento fueron más eficientes para generar ventas en el año?**

KPI 1: Ventas por metro cuadrado (eficiencia): Ventas / Tamaño.

1.  **¿Qué departamentos aportaron más al negocio y cuáles estuvieron por debajo de su potencial?**
    - KPI 2: Participación del departamento: VentasDepto / VentasTotales.

**Descripción del proyecto:** Desarrollo de un tablero interactivo para visualizar patrones de compra y realizar predicciones de tendencias de ventas.

1.  **Preparar datos** para el análisis (limpieza, enriquecimiento, documentación).
2.  **Construir KPIs clave** para evaluar la eficiencia y la participación.
3.  **Crear dashboards dinámicos** con filtros y visualizaciones útiles para los stakeholders.
4.  **Comunicar hallazgos ejecutivos** mediante el método C→F→I.
5.  **Aplicar QA** para asegurar la calidad y trazabilidad del análisis.

- **Logros:** Optimización de la toma de decisiones mediante la identificación clara de comportamientos históricos y proyectados.

- **Herramientas:** Python (Pandas), SQL y Excel avanzado.

## 2. Análisis de embudo y retención de clientes para Mercado Libre

**Descripción del proyecto:** Como analista de producto en MercadoLibre, dentro del equipo de Crecimiento y Retención, el **Director de Producto** planteó el siguiente requerimiento: “Necesitamos entender en qué etapa del proceso perdemos usuarios y cómo podemos mejorar su retención a lo largo del tiempo.”

Mi misión fue usar SQL para mapear el **embudo de conversión completo**, identificar los principales puntos de fuga y evaluar **la retención de usuarios por cohortes.**

**Objetivo:** Presentar p**ropuestas de mejoras accionables** basadas en los datos.

**Descripción de los procesos:**

1.  Construir embudos multietapa en SQL usando **CTEs (Expresiones de Tabla común)**.
2.  Calcular **tasas de conversión** entre pasos y detectar caídas.
3.  Analizar la retención de usuarios por cohortes.
4.  Simular mejoras en conversión o retención.
5.  Validar resultados y comunicar hallazgos ejecutivos.

**Contexto:** Se tomó la informaci{ó del 1 de enero de 2025 al 31 de agosto de 2025 con el objetivo responder las siguientes preguntas:

- ¿cuál es la tasa de conversión entre cada etapa clave del embudo?.
- ¿En qué paso se observa la mayor caída porcentual de usuarios?
- _¿Cómo varía esta pérdida por país ?_

**Métricas clave:**

- Tasa de conversión por etapa
- Agrupación de eventos por device_category y referral_source
- **¿Qué tan bien retenemos a los usuarios a lo largo del tiempo?**
- Para los usuarios que se registraron entre el 1 de enero de 2025 y el 1 de junio, ¿cuál es la tasa de retención en D7, D14, D21, D28?
    - _¿Cómo se comporta la retención por país (country)?_

**Métrica clave:** Retención por cohorte (D7, D14, D21, D28)

Proceso general realizado:

1.  Explorar el esquema y los datos base.
2.  Construir el embudo de conversión.
3.  Calcular tasas y caídas.
4.  Analizar retención y cohortes.
5.  Simular mejoras y redactar el informe ejecutivo.

**Resultados:** El análisis de embudo es un método utilizado en el **A**[**nálisis de Datos**](https://es.statisticseasily.com/herramientas-gratuitas-de-an%C3%A1lisis-de-datos/) y marketing para visualizar y comprender los pasos que dan los clientes potenciales antes de completar una acción deseada, como realizar una compra o suscribirse a un boletín informativo.

Este enfoque analítico ayuda a las empresas a **identificar dónde están perdiendo clientes potenciales en el proceso de conversión,** lo que les permite optimizar sus estrategias de marketing y mejorar el rendimiento general.

En este caso específico, ayudé a la empresa a entender que el comportamiento de los usuarios estaba siendo malo para el negocio, pero por otro lado, era muy similar en todos los países, razón por la cual se pudo determinar **que el problema no estaba en los usuarios, sino que estaba en otra(s) parte(s) del proceso**, pudiendo ser en el módulo específico de la plataforma en internet, o en la oferta de productos, en el nivel de atención de los servicios, o incluso en la parte de marketing de las promociones.

A partir de estos resultados se desprendió otro proyecto enfocado a analizar y resolver el problema de forma más clara y específica sobre los puntos idenitifocados, lo cual permitió identificar una modificación esencial en la palatforma que les llevó a mejorar en un 25% los resultados de retención de usuarios y evitar estas caídas tan abruptas.

## 3\. Sistema de Información Gerencial (Data Marts)

**Sistema de Información Gerencial (Datamarts) en Royal & Sun Alliance Seguros (México), ahora Seguros SURA, S.A.:**

Supervisé el análisis, diseño y desarrollo de un sistema de información gerencial basado en **Datamarts** para la integración y explotación de información ejecutiva y estadística de todos los ramos de seguros que gestionaba la empresa, en una base de datos única. Este Sistema de Información Gerencial (SIG) basado en Data Marts es la evolución natural de un almacén de datos centralizado hacia algo mucho más ágil y específico para la toma de decisiones.

La arquitectura de este sistema está basada en la integración y consolidación de varios Data Marts específicos por cada área operativa y financiera de la empresa, segmentando la información en "islas" especializadas pero interconectadas:

- - - Data Mart de Suscripción (Underwriting): Contiene datos de perfiles de riesgo, pólizas emitidas, renovaciones y tasas de cancelación.
        - Data Mart de Siniestralidad: Enfocado en la frecuencia y severidad de los reclamos, reservas técnicas y análisis de la siniestralidad a diferentes niveles: por póliza, por agente, por oficina, por ramo y a nivel consolidado.
        - Data Mart Comercial: Seguimiento de metas de agentes, comisiones y rentabilidad por canal.
        - Data Mart de Finanzas: Enfocado en primas cobradas, flujo de caja y cumplimiento regulatorio.

Para ello, se establecieron varios procesos de ETL (Extracción, Transformación y Carga) de datos, en estos procesos los datos crudos de los sistemas legacy (donde se emiten las pólizas y administran las pólizas) se limpian y se transforman.

**Beneficios Estratégicos para la Aseguradora:**

- - **Agilidad en el Reporteo**: Al ser bases de datos más pequeñas y especializadas, las consultas (queries) de SQL o los tableros de Power BI/Tableau cargan mucho más rápido que en un sistema general.
    - **Seguridad de la Información:** Puedes restringir el acceso; por ejemplo, que el equipo de ventas no vea datos sensibles de reservas matemáticas que solo competen a Actuaría y Finanzas.
    - **Análisis Predictivo:** Facilitan el uso herramientas de explotación de información (Cognos) para correr modelos de Machine Learning (como detección de fraude en siniestros) sobre un set de datos ya pre-procesado y confiable.
    - Este proyecto **consolidó la capacidad de reporte y análisis estadístico a nivel corporativo**.

- **Logros:** Consolidación de la capacidad de reporte corporativo, mejora en la seguridad de la información y agilidad en consultas SQL.

- **Herramientas:** SQL, Procesos ETL, Cognos y sistemas _legacy_.

- 1.  **Análisis Predictivo de Ventas**

**Empresa:** Proyecto TripleTen Bootcamp.

**Contexto:** Análisis de grandes volúmenes de datos para identificar el comportamiento del cliente a largo plazo.

**Descripción:** Ejecución de análisis exploratorio (EDA) y aplicación de modelos predictivos sobre el historial de ventas.

**Logros:** Implementación de modelos que permiten optimizar decisiones estratégicas basadas en el comportamiento histórico.

**Herramientas:** Python (Bibliotecas de Ciencia de Datos) y SQL.

## 4\. Indicadores de Sustentabilidad (IMAVA)

- **Empresa:** Secretaría del Medio Ambiente de la Cudad de México (S.M.A.)

- **Contexto:** Evaluación del impacto social, económico y ambiental en proyectos ambientales realizados por parte de la Secretaría del Medio Ambiente en 5 barrancas iubicadas en las delegaciones Álvaro Obregón, La Magdalena Contreras y Miguel Hidalgo de la Ciudad de México, que se encuentran en situación crítica de abandono, falta de higiene, acumulación de basura y de mal uso por falta de seguridad, para restablecerlas como Áreas de Valor Ambiental (AVA), y que sean verdaderos espacios urbanos que, aunque han sido transformados por la actividad humana, conservan características biofísicas esenciales para mantener el equilibrio ecológico de las ciudades.

- **Descripción:** Coordinación estadística para crear el Indicador de Medición de Áreas de Valor Ambiental (IMAVA) y explotación de bases de datos del INEGI.

**Trabajo interdisciplinario con los responsables especialistas de los sectores involucrados en el proyecto tales como:** gestión ambiental, antropología, geografía, biología, ingeniería, finanzas, economía y participación comunitaria.

**Desarrollo de un Taller expertos con la participación de más de 20 expertos de las diversas áreas.**

- **Logros:** Obtención de un indicador de medición de Recuperación de Áreas Ambientales **(IMAVA**). El proyecto recibió un reconocimiento oficial por su rigor metodológico y precisión en el análisis de datos.

**Beneficios esperados:** Contar con los elementos metodológicos para medir los avances de los diversos proyectos y dar seguimiento a los beneficios que se esperan generar en cuanto a las tres partes del Desarrollo Sustentable:

**1\. Beneficios Ambientales (Servicios Ecosistémicos)**

**Regulación de la temperatura:** Ayudan a mitigar el efecto de "isla de calor" urbana, refrescando el entorno a través de la vegetación.

**Recarga de acuíferos:** Permiten la infiltración de agua de lluvia al subsuelo, vital para el abastecimiento de agua en zonas urbanas.

**Mejora de la calidad del aire:** Actúan como pulmones urbanos que capturan dióxido de carbono () y filtran partículas contaminantes.

**Protección de la biodiversidad:** Sirven como refugio y corredores biológicos para especies locales de flora y fauna.

**2\. Beneficios Sociales y de Salud**

**Reducción del estrés:** Proporcionan espacios de recreación y contacto con la naturaleza que mejoran la salud mental de los ciudadanos.

**Cohesión social:** Funcionan como puntos de encuentro para la comunidad, fomentando el sentido de pertenencia.

**Control de ruido:** La vegetación densa actúa como una barrera natural contra la contaminación auditiva del tráfico y la industria.

**3\. Beneficios Económicos**

**Mitigación de riesgos:** Previenen inundaciones y erosión del suelo, reduciendo costos por desastres naturales.

**Valorización de la propiedad:** La cercanía a áreas verdes bien conservadas suele incrementar el valor de los bienes inmuebles circundantes.

**Sostenibilidad urbana:** Facilitan el cumplimiento de indicadores estratégicos y normativas ambientales internacionales.

- **Herramientas:** Excel avanzado y Análisis estadístico; así como metodologías Taller de Expertos y de evaluación de impacto del proyecto en las tres partes de esenciales del **Desarrollo Sustentable, tales como: social, económico y ambiental.**

## 5\. Optimización de Reportes Ejecutivos

- **Empresa:** Mega Solar S.A..
- **Contexto:** Deficiencia en los tiempos de entrega de informes diarios y mensuales de la operación.
- **Descripción:** Automatización integral de flujos de trabajo y estandarización de captura de datos.
- **Logros:** Reducción del 40% en los tiempos de procesamiento y un incremento del 25% en la eficiencia operativa.
- **Herramientas:** Excel (Macros/Funciones avanzadas) y rediseño de flujos operativos.

.

**Herramientas Técnicas**

- **Lenguajes:** Python (Pandas, NumPy, Seaborn), SQL.
- **BI & Visualización:** Dashboards estratégicos, Excel avanzado.
- **Especialidades:** Gestión de Riesgos (ISO 31000, ISO 9001), Modelado Estadístico, Estrategia Institucional.

**Idiomas: Español** nativo**. Inglés** nivel intermedio-avanzado**. Italiano** nivel intermedio.