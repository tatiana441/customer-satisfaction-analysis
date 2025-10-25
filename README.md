# Análisis EDA — Keimi (datos sintéticos)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/USUARIO/REPO/blob/main/notebooks/analisis_eda_crudo_Keimi.ipynb)

**TL;DR:** EDA reproducible con datos sintéticos inspirado en un caso real de negocio. Incluye limpieza, exploración visual y hallazgos accionables.

## Objetivo
Explorar y diagnosticar el dataset para identificar patrones, calidad de datos y oportunidades de mejora de KPIs.

## Dataset
- **Ruta esperada:** `Customer_Satisfaction_Sample_Data.csv`
- **Tipo:** CSV con datos sintéticos (sin PII)
- **Nota de uso:** si ejecutas en Colab, puedes leer el CSV desde el `raw` del repo o subirlo manualmente.

## Metodología
1. Perfilamiento de datos (tipos, nulos, duplicados, outliers).
2. Limpieza y preparación (casting, imputación simple, normalización de variables).
3. EDA visual (distribuciones, relaciones bivariadas, segmentación inicial).
4. Métricas clave y correlaciones.
5. Hallazgos, limitaciones y siguientes pasos.

## Resultados clave (ejemplos de formato)
- Segmento X presenta variación significativa en métrica Y (+pp vs. promedio).
- Variables A y B correlacionan con el objetivo; sugerir pruebas A/B o features derivados.
- Calidad de datos: campos con >Z% nulos; recomendación de imputación/recaptura.

## Estructura del repositorio
```
notebooks/analisis_eda_crudo_Keimi.ipynb
data/Customer_Satisfaction_Sample_Data.csv
reports/EDA_Keimi.html  # export del notebook a HTML (opcional)
requirements.txt
README.md
```

## Índice del notebook
  - ⚠️ Important Note on Data Privacy
- Análisis Exploratorio de Datos (EDA) - Crudo Keimi
  - Objetivo Principal
  - Paso 1: Importar librerías necesarias
  - Paso 2: Cargar los datos
  - Paso 3: Exploración inicial de los datos
  - Paso 4: Análisis de CSAT (Satisfacción del Cliente)
  - Paso 5: Análisis de DSAT Reason - Agrupación Temática
  - Paso 6: Análisis de Correlación entre CSAT y Temas de DSAT
  - 📊 Resumen del Análisis
    - 🎯 Metodología Aplicada
    - 📈 Interpretación de Resultados
    - 💡 Conclusiones Clave
    - 🔍 Próximos Pasos Sugeridos
  - Paso 7: Análisis de CSAT vs Satisfaction Driver
  - 📊 Resumen del Análisis CSAT vs Satisfaction Driver
    - 🎯 Agrupación Temática de Satisfaction Drivers
    - 📈 Interpretación de la Correlación
    - 💡 Insights Clave
    - 🔍 Conclusiones del Análisis Completo

## Cómo ejecutar
```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
jupyter lab
```

## Ver sin instalar
- Exporta el notebook a HTML (File → Download as → HTML) y súbelo a `reports/`.

## Aviso de datos
Datos sintéticos para fines demostrativos. Cualquier parecido con datos reales es intencionalmente controlado.
