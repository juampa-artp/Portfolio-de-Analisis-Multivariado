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

Contribuyentes y su contacto

- Juan Pablo Arteaga Patiño - A01665795
- Diego López Schmill - A01666290


## License

This project is licensed under the ITESM License - see the LICENSE.md file for details