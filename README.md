# Portfolio de Analisis Multivariado

| Caso | Método | Dataset | Problema de Negocio | Notebook |
|------|--------|---------|---------------------|----------|
| **Caso 1** | Factor Analysis | Customer Behavior | Identificar factores latentes que explican el comportamiento de compra de clientes | [factor_analysis.ipynb](./case-01-factor-analysis/factor_analysis.ipynb) |
| **Caso 2** | Discriminant Analysis (LDA/QDA) | Classification Dataset | Clasificar observaciones en grupos predefinidos y evaluar la precisión de clasificación | [discriminant_analysis.ipynb](./case-02-discriminant-analysis/discriminant_analysis.ipynb) |
| **Caso 3** | Cluster Analysis | MegaMart Customers | Segmentar clientes de MegaMart para estrategias de marketing personalizadas | [cluster-analysis.ipynb](./case-03-cluster-analysis/cluster-analysis.ipynb) |

---

**Factor Analysis:**
- Cuando tienes muchas variables correlacionadas y quieres identificar dimensiones subyacentes
- Para validar cuestionarios o escalas psicométricas
- Cuando necesitas reducir dimensionalidad preservando la interpretabilidad

**Discriminant Analysis:**
- Cuando ya conoces los grupos y quieres clasificar nuevas observaciones
- Para entender qué variables mejor discriminan entre grupos
- Cuando necesitas probabilidades de pertenencia a grupos

**Cluster Analysis:**
- Cuando no tienes grupos predefinidos y quieres descubrirlos
- Para segmentación de clientes o mercados
- Cuando buscas patrones naturales en los datos sin hipótesis previas

---

## Comparación Metodológica

### Factor Analysis vs. Discriminant Analysis vs. Cluster Analysis

| Aspecto | Factor Analysis | Discriminant Analysis | Cluster Analysis |
|---------|----------------|----------------------|------------------|
| **Tipo de Aprendizaje** | No supervisado | Supervisado | No supervisado |
| **Objetivo Principal** | Reducción de dimensionalidad y descubrimiento de estructura latente | Clasificación y predicción de grupos conocidos | Descubrimiento de grupos naturales en los datos |
| **Variables de Entrada** | Variables continuas correlacionadas | Variables predictoras (continuas/categóricas) | Variables continuas (principalmente) |
| **Variable de Salida** | Factores latentes (no observables) | Variable categórica conocida | Etiquetas de cluster (descubiertas) |
| **Interpretabilidad** | Alta - identifica dimensiones subyacentes | Media - coeficientes de discriminación | Variable - depende del método y visualizaciones |
| **Supuestos Estadísticos** | Normalidad multivariada, linealidad | Normalidad, homogeneidad de varianzas (LDA) | Depende del método (K-means: clusters esféricos) |
| **Aplicaciones Típicas** | Psicometría, estudios de mercado, reducción de cuestionarios | Diagnóstico médico, credit scoring, reconocimiento de patrones | Segmentación de mercado, bioinformática, compresión de datos |
| **Ventajas** | - Reduce complejidad<br>- Identifica constructos latentes<br>- Facilita interpretación | - Maximiza separabilidad<br>- Proporciona probabilidades de pertenencia<br>- Útil para predicción | - Descubre patrones ocultos<br>- No requiere etiquetas previas<br>- Flexible en estructura |
| **Desventajas** | - Requiere decisiones subjetivas (# factores)<br>- Sensible a outliers | - Requiere grupos conocidos<br>- Asume distribuciones específicas | - Requiere especificar # clusters (K-means)<br>- Sensible a inicialización<br>- Resultados pueden variar |

### Cuándo Usar Cada Método

**Factor Analysis:**
- Cuando tienes muchas variables correlacionadas y quieres identificar dimensiones subyacentes
- Para validar cuestionarios o escalas psicométricas
- Cuando necesitas reducir dimensionalidad preservando la interpretabilidad

**Discriminant Analysis:**
- Cuando ya conoces los grupos y quieres clasificar nuevas observaciones
- Para entender qué variables mejor discriminan entre grupos
- Cuando necesitas probabilidades de pertenencia a grupos

**Cluster Analysis:**
- Cuando no tienes grupos predefinidos y quieres descubrirlos
- Para segmentación de clientes o mercados
- Cuando buscas patrones naturales en los datos sin hipótesis previas

---

### Mejores Prácticas Identificadas

- **Exploración de datos exhaustiva** antes de aplicar cualquier método
- **Validación cruzada** y evaluación en datos de prueba (cuando aplica)
- **Visualización** como herramienta fundamental para comunicar resultados
- **Documentación clara** del proceso y decisiones tomadas
- **Iteración**: Los primeros modelos raramente son los finales

---

## Getting Started

### Dependencies

```bash
# Crear un entorno virtual (opcional pero recomendado)
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate

# Instalar dependencias
pip install -r requirements.txt
```

## Authors

Contributors names and contact info

- Juan Pablo Arteaga Patiño - A01665795
- Diego López Schmill - A01666290

## License

This project is licensed under the ITESM License - see the LICENSE.md file for details