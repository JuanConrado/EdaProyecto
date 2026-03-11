# EDA — Stocks OHLCV

Libro de análisis exploratorio de datos del **Proyecto de Machine Learning sobre precios de acciones**.
Integrantes:
Sergio Cadavid
Mateo Chang
Juan Camilo Conrado
---

## ¿De qué trata este libro?

Este libro documenta paso a paso el proceso de **Análisis Exploratorio de Datos (EDA)** realizado sobre datos históricos de precios de acciones del mercado estadounidense, con el objetivo de preparar los datos para un modelo de predicción basado en patrones de velas japonesas.

---

## Estructura del libro

| Sección | Contenido |
|---------|-----------|
| **1. Configuración** | Rutas, librerías y carga inicial del dataset |
| **2. Exploración inicial** | Inspección de un ticker: estructura, limpieza y visualización |
| **3. Patrones de velas** | Doji, Hammer, Engulfing Bull/Bear |
| **4. EDA Multi-ticker** | Análisis sobre muestra de 20 tickers |
| **5. Control de Calidad (QA)** | Duplicados, días faltantes, consistencia OHLC |
| **6. Selección del ticker** | Ranking por score y elección de INTC (Intel) |
| **7. EDA Profundo — INTC** | Log-returns, volatilidad rolling, distribución de retornos |
| **8. Split Temporal** | División 75% train / 25% test sin data leakage |
| **9. Conclusiones** | Hallazgos clave y próximos pasos |

---

## Dataset

- **Fuente:** [Kaggle — Price Volume Data for all US Stocks & ETFs](https://www.kaggle.com/datasets/borismarjanovic/price-volume-data-for-all-us-stocks-etfs)
- **Formato:** Archivos `.txt` con columnas `Date, Open, High, Low, Close, Volume`
- **Ticker principal analizado:** `INTC` (Intel Corporation)

---

## Herramientas utilizadas

- `pandas` — manipulación de datos
- `numpy` — operaciones numéricas
- `matplotlib` — visualizaciones
- `jupyter` — entorno de desarrollo

---

```{note}
Este EDA es el primer paso de un proyecto más amplio de predicción de precios
usando patrones de velas y modelos de machine learning.
```
