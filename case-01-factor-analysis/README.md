# Portfolio-de-An-lisis-Multivariado
MA2003B - Aplicación de Métodos Multivariados en Ciencia de Datos

### Factor Analysis
En este proyecto se realizó un Análisis por Factores para identificar los factores para la retención de clientes y el crecimiento de la empresa 

#### Análisis Preliminar
Luego de una limpieza de la base de datos se realizó una prueba de validez para ver si los datos cumplian con las caracteristicas anecesarias para realizar el análisis por factores el cual la base de datos los cumplia

#### Hallazgos
El análisis identificó 5 factores distintos. A continuación, se clasifican por su impacto 
directo en la Probabilidad de Renovación. 

**Factor 1:** Colaboración Proactiva (Impacto: MUY ALTO) 
●  Variables que lo componen: project_management, timeline_adherence, 
communication_clarity, change_management. 
●  Análisis de Impacto: Este es el impulsor de retención más crítico. Es el predictor #1 de 
la Probabilidad de Renovación (r = 0.62) y la Satisfacción General (r = 0.75). Los 
clientes que puntúan alto aquí ven a TechnoServe no como un proveedor, sino como 
una extensión integrada de su propio equipo. 


**Factor 2:** Excelencia Técnica e Innovación (Impacto: ALTO) 
●  Variables que lo componen: technical_expertise, problem_solving, 
innovation_solutions, system_integration. 
●  Análisis de Impacto: Este es su "factor sorpresa" y la principal fortaleza de su marca. 
Es el impulsor #1 del NPS (r = 0.45) y de la generación de Referidos. Es 1.4 veces más 
influyente en el NPS que el Factor 1. Mientras la "Colaboración" impulsa la retención, la 
"Excelencia" impulsa la promoción. 


**Factor 3:** Relación Estratégica (Impacto: MODERADO) 
●  Variables que lo componen: trust_reliability, long_term_partnership, 
executive_access. 
●  Análisis de Impacto: Este factor mide la confianza a nivel de liderazgo (C-Suite). 
Asegura la lealtad a largo plazo más allá de los proyectos individuales y crea altas 
barreras de salida contra la competencia. 


**Factor 4:** Soporte Receptivo y Capacitación (Impacto: MODERADO-BAJO) 
●  Variables que lo componen: support_responsiveness, training_quality, 
documentation_help. 
●  Análisis de Impacto: Este factor es clave para la experiencia operativa diaria del 
cliente. Las puntuaciones altas aquí reducen la fricción y la carga sobre los equipos de 
soporte, pero no impulsan significativamente las decisiones de renovación por sí solas. 


**Factor 5:** Transparencia Financiera y Valor (Impacto: FACTOR DE HIGIENE) 
●  Variables que lo componen: cost_transparency, value_for_money, 
billing_accuracy, competitive_pricing. 
●  Análisis de Impacto: Este es un "factor de higiene" crítico. Tiene la correlación positiva 
más débil con la renovación (r = 0.12). Sin embargo, un análisis de los comentarios de 
los detractores (NPS 0-6) revela que los errores de facturación y la falta de 
transparencia en los costos son una de las razones más citadas para no renovar. Las 
puntuaciones bajas aquí tienen un poder de veto desproporcionado sobre la relación. 

#### Recomendaciones
Ya con los factores y sus respectivos impactos les presentará 3 recomendaciones.

**Duplicar la "Colaboración Proactiva"** (Factor 1) 
●  Referencia del Hallazgo: Es el impulsor #1 de la renovación (r = 0.62). 
●  Acción 1a: Lanzar un módulo de capacitación en habilidades blandas para todos los 
Gerentes de Proyecto (PMs) enfocado en "Comunicación Proactiva" y "Gestión de 
Cambios", a implementarse en Q2 2026. 
●  Acción 1b: Actualizar los dashboards de proyectos visibles para el cliente para incluir 
una métrica simple de "Salud de la Colaboración". 
●  KPI a Medir: Aumentar las puntuaciones promedio del Factor 1 en un 15% en 12 
meses. 


**Institucionalizar la "Excelencia Técnica"** (Factor 2) 
●  Referencia del Hallazgo: Es el impulsor #1 del NPS (r = 0.45). 
●  Acción: Requerir que todos los Gerentes de Cuenta (AMs) presenten una "Historia de 
Innovación y Resolución de Problemas" durante cada Revisión de Negocio Trimestral 
(QBR). Esto traduce la technical_expertise en valor de negocio tangible para el 
cliente. 
●  KPI a Medir: Aumentar el porcentaje de "Promotores" (NPS 9-10) en un 10% año contra 
año. 


**Neutralizar la Fricción Financiera** (Factor 5) 
●  Referencia del Hallazgo: Es un "factor de higiene" crítico que causa la pérdida de 
clientes. 
●  Acción: Formar un equipo de trabajo interfuncional (Finanzas, PMs, Cuentas) en Q1 
2026 para rediseñar las plantillas de facturas y los informes de costos en pro de la 
máxima claridad (cost_transparency). 
●  KPI a Medir: Reducir las quejas de clientes relacionadas con facturación en un 50%