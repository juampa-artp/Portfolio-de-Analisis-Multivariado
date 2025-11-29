# Portfolio-de-An-lisis-Multivariado
MA2003B - Aplicación de Métodos Multivariados en Ciencia de Datos

### Cluster Analysis
Este Notebook se trata de una realización de clustering no supervisado para ver los tipos de consumidores que tenía una empresa y a partir de ello, reestructurar las finanzas, re-enfocar las campañas publicitarias y mejorar la experiencia del usuario dado que antes la empresa trataba todos sus clientes por igual el cual generaba zonas de alto consumo de recursos y poco retorno.

#### Análisis Preliminar
Luego de realizar una limpieza a los datos se realizó un análisis para ver los comportamientos de los datos y la factibilidad de los diferentes tamaños de clusters. Una métrica que se encontró fue que la cantidad total que un usuario gasta es proporcional a el promedio del tamaño de sus canastas y que aunque la variabilidad del promedio del tamaño de las canastas y la cantidad total gastada este baja estos contienen los valores más alejados de la media de todos los datos, por lo que nos demuestra que se tiene una buena base de datos para trabajar.
Lo siguiente que se hizo fue hacer un Dendrograma para ver posibles números de clusters que posteriormente se vio su factibilidad por otro método el cual nos terminó de guiar a que el mejor corte fuera de 5 segmentos.


#### Grupos
Ya que se tenía la cantidad de clusters lo siguiente fue ver las características que tenía cada grupo y sus respectivos nombres.

**Segmento 1: "Leales Premium"** (15% de clientes)

Perfil de Comportamiento: Estos clientes representan el valor más alto para MegaMart. Realizan
compras frecuentes (promedio 12-15 transacciones mensuales), mantienen cestas de compra
significativamente superiores al promedio ($25-30 por transacción), y muestran el gasto total
más elevado ($3,500-$4,500). Su tasa de apertura de emails es excepcional (85-95%), indicando
alto engagement con la marca. Presentan baja tasa de devoluciones (< 5%) y antiguedad
promedio de 24-30 meses como clientes.


**Segmento 2: "Cazadores de Ofertas"** (25% de clientes)

Perfil de Comportamiento: Este segmento visita con frecuencia moderada-alta (8-10
transacciones mensuales) pero mantiene cestas pequeñas ($8-12 por transacción). Su gasto
total es moderado-bajo ($800-$1,200). Son altamente sensibles al precio, concentrando
compras en categorías de descuento. Tasa de apertura de emails baja (0-20%) excepto para
promociones. Recency moderada (15-25 días) y tenure medio (12-18 meses).


**Segmento 3: "Compradores Ocasionales"** (23% de clientes)

Perfil de Comportamiento: Frecuencia de compra baja (2-4 transacciones mensuales) con largos
intervalos entre visitas. Cesta de compra moderada ($15-20) cuando compran. Gasto total bajomoderado ($600-$1,000). Engagement digital limitado (tasa de apertura 20-40%). Recency alta
(25-35 días), sugiriendo que MegaMart es opción secundaria. Tenure variable (8-20 meses).


**Segmento 4: "Familias en Crecimiento"** (20% de clientes)

Perfil de Comportamiento: Frecuencia moderada-alta (9-11 transacciones mensuales) con cestas
grandes ($28-35), reflejando compras familiares. Gasto total significativo ($2,800-$3,500).
Engagement moderado con emails (40-60%). Baja tasa de devoluciones. Recency baja (8-15
días), indicando visitas regulares. Alto número de vistas de productos por visita, sugiriendo
navegación extensiva.


**Segmento 5: "Alto Valor en Riesgo"** (17% de clientes)

PRIORIDAD CRÍTICA - RIESGO DE CHURN
Perfil de Comportamiento: Este segmento es particularmente preocupante. Son clientes con
historial de gasto alto ($3,000-$4,000 lifetime value) pero frecuencia en declive (actualmente 3-
5 transacciones mensuales vs. 10-12 histórico). Recency muy alta (35-50 días), indicando
alejamiento progresivo. Engagement en caída (apertura emails 10-30%). Tenure significativo
(20-28 meses), lo que indica que fueron buenos clientes. Tasa de devoluciones creciente, posible
señal de insatisfacción.

#### Recomendaciones
Ya que se tiene los perfiles de cada grupo y sus tamaños, ahora se realizarán las recomendaciones para cada grupo, su estrategia de marketing y qué aspectos se tienen que cuidar para cada uno.

**Estrategia A: Programa VIP "Circle Premium"** (Leales Premium)
• Acciones Específicas:
• Crear tier exclusivo de membresía con beneficios premium
• Acceso anticipado 48h a nuevos productos y ventas especiales
• Línea de atención personalizada con personal dedicado
• Eventos exclusivos trimestrales (degustaciones, lanzamientos)
• Envío gratuito sin mínimo de compra
• Objetivo Estratégico:
• Incrementar "share of wallet" del 60% actual al 75%. Reducir riesgo de churn de este
segmento crítico al <2% anual. Estos clientes generan 30-35% de ingresos totales siendo
solo 15% de base.
• Inversión Estimada:
• $45,000 - $60,000 anuales para 450 clientes = $100-$133 por cliente VIP


**Estrategia B: "Bundle Builder"** (Cazadores de Ofertas)
• Acciones Específicas:
• • ELIMINAR descuentos porcentuales en items individuales
• • Implementar ofertas tipo "Compra 2 Lleva 3" o "Compra $50 Recibe $5"
• • Crear packs de productos complementarios con descuento bundle
• • Gamificación: "Completa tu lista de 8 productos, obtén 15% descuento"
• Objetivo Estratégico:
• Incrementar ticket promedio de $10 a $18-20 (aumento 80-100%). Aunque visitan
frecuentemente, su valor actual es bajo. Forzar bundling aumenta rentabilidad sin
perder frecuencia de visita.
• Métrica Clave:
• Unidades por transacción debe crecer de 1.8 a 3.5+


**Estrategia C: "Top of Mind" Campaign** (Compradores Ocasionales)
• Acciones Específicas:
• Campaña de recordatorio inteligente basada en categorías de compra previa
• Email semanal "Tu lista podría incluir..." con productos complementarios
• Push notifications geo-localizadas: "Estás cerca de MegaMart - 20% off hoy"
• Programa de referidos: "Trae un amigo, ambos reciben $10"
• Objetivo Estratégico:
• Aumentar frecuencia de 2-4 visitas/mes a 5-6 visitas/mes. Convertir a MegaMart en
primera opción vs. segunda opción. Reducir recency promedio de 30 días a 18 días.


**Estrategia D: "Family First" Program** (Familias en Crecimiento)
• Acciones Específicas:
• Crear secciones temáticas "Compra Familiar Completa"
• Ofertas multi-pack en productos de alto consumo familiar (pañales, cereales, etc.)
• Programa de lealtad con puntos dobles en categoría infantil
• Newsletter especializado con tips de ahorro familiar y recetas
• Objetivo Estratégico:
• Mantener alta frecuencia actual (9-11 visitas/mes) y aumentar ticket promedio de $30 a
$38-40. Este segmento tiene alto potencial de crecimiento conforme familias crecen.


**Estrategia E: "Operation Win-Back"** PRIORIDAD MÁXIMA (Alto Valor en Riesgo)
ACCIÓN INMEDIATA REQUERIDA - IMPLEMENTAR EN 7 DÍAS
• Acciones Específicas:
• Trigger automático cuando recency supera 30 días para este segmento
• Secuencia multi-canal: SMS (Día 1) → Email Personalizado (Día 3) → Llamada (Día 7)
• Oferta de alto valor: "$30 de crédito válido por 10 días" o "30% descuento en próxima
compra $50+"
• Mensaje personalizado: "Te extrañamos [Nombre]. Como cliente preferencial..."
• Survey de salida: "¿Qué podemos mejorar?" con incentivo de respuesta
• Objetivo Estratégico:
• Recuperar mínimo 25% de este segmento en 90 días. Cada cliente recuperado
representa $3,500+ en lifetime value. Con 510 clientes en riesgo, recuperar 25% = 127
clientes = $444,500 en revenue preservado.
• ROI Estimado:
• Inversión: $25,000 (incentivos + sistema automático). Retorno: $444,500. ROI = 1,678%