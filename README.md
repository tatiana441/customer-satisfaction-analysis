# Análisis EDA — Keimi (datos sintéticos)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tatiana441/customer-satisfaction-analysis/blob/main/analisis_eda_crudo_Keimi.ipynb)

**TL;DR:** EDA reproducible con datos sintéticos inspirado en un caso real de negocio. Incluye limpieza, exploración visual y hallazgos accionables.

- 📄 **Reporte HTML (web):** https://tatiana441.github.io/customer-satisfaction-analysis/
- 🗂️ **CSV:** [Customer_Satisfaction_Sample_Data.csv](Customer_Satisfaction_Sample_Data.csv)

## Objetivo
Explorar y diagnosticar el dataset para identificar patrones, calidad de datos y oportunidades de mejora de KPIs.

## Dataset
- **Ruta:** `Customer_Satisfaction_Sample_Data.csv`
- **Tipo:** CSV con datos sintéticos (sin PII)
- **Lectura directa en Colab/local (sin subir archivos):**
```python
import pandas as pd
url = "https://raw.githubusercontent.com/tatiana441/customer-satisfaction-analysis/main/Customer_Satisfaction_Sample_Data.csv"
df = pd.read_csv(url)
df.head()
