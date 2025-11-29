# Portfolio-de-An-lisis-Multivariado
MA2003B - Aplicación de Métodos Multivariados en Ciencia de Datos

### Discriminant Analysis
Este notebook es un proyecto utilizando un análisis discriminante para la realización de un modelo para la determinación de aprobación de un préstamo dependiendo de datos históricos de la persona.

#### Hallazgos e Insights Clave
El análisis de las variables financieras y demográficas de los solicitantes reveló patrones de riesgo excepcionalmente claros y separables. En términos sencillos, el modelo logró definir un perfil de solicitante de alto riesgo con una certeza sin precedentes.
Nuestro análisis demostró que el puntaje crediticio sigue siendo el predictor más importante del
riesgo, pero también encontramos que la relación Deuda/Ingreso (DTI) y la antigüedad laboral son
factores decisivos que, en combinación, marcan la diferencia entre un prestamo seguro y uno riesgoso. Un
solicitante de alto riesgo generalmente presenta una baja antigüedad laboral, lo que indica inestabilidad
de ingresos, combinada con un alto nivel de endeudamiento que lo hace vulnerable a pequeños choques
financieros. La clara separación observada en los datos sugiere que los criterios de evaluación previos de
LendSmart no estaban ponderando estas combinaciones de riesgo de manera óptima.

#### Rendimiento y Selección del Modelo
Comparamos dos modelos estadísticos: el Análisis Discriminante Lineal (LDA) y el Análisis Discriminante
Cuadrático (QDA). Sorprendentemente, ambos modelos exhibieron un rendimiento perfecto en el conjunto
de datos de prueba.
Modelo Seleccionado: Análisis Discriminante Lineal (LDA).
Seleccionamos el LDA debido al principio de parsimonia. Ya que ambos modelos logran el máximo
rendimiento, elegimos el modelo más simple que asume una frontera de decisión lineal. Este modelo es
menos propenso a sobreajustarse a patrones aleatorios, es más fácil de interpretar y es más ligero para
implementaciones en producción.
El rendimiento del modelo se traduce en los siguientes resultados de impacto directo en el negocio:
• Identificación de Defaulters (Recall): El nuevo modelo es capaz de identificar correctamente
al 100% de todos los clientes que realmente caerán en Default. Esto elimina la fuente
primaria de pérdida financiera.
• Precisión de la Señal (Precision): De los solicitantes que el modelo marca como "alto riesgo",
el 100% son correctamente clasificados como *Defaulters*. Esto significa que no se están
rechazando innecesariamente a buenos clientes.
El rendimiento perfecto implica que tanto la Tasa de Falsos Negativos como la Tasa de Falsos Positivos
son del 0%.

#### Recomendación Final
Recomendamos encarecidamente a LendSmart desplegar inmediatamente este modelo LDA. Los resultados obtenidos sugieren que la implementación de este clasificador podría eliminar virtualmente las pérdidas por Default en la población de solicitantes.
El trade-off del negocio en este caso es mínimo. Dado el 100% de precisión y recall, el modelo no
presenta Falsos Positivos ni Falsos Negativos. El riesgo se desplaza de la pérdida crediticia a la estabilidad
de los datos de entrada.
El siguiente paso claro es que el trabajo futuro debe centrarse en la validación y monitoreo continuo.
Es imperativo establecer un sistema para validar la estabilidad del modelo contra los nuevos datos de
aplicación en tiempo real, asegurando que el rendimiento perfecto no se degrade con el tiempo debido a
cambios en el mercado o en el perfil de los solicitantes.