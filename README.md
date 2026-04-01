# 🛍️ EverPeak Retail — Limpieza y Preparación de Datos

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NicolasMesa27/everpeak-analysis/blob/main/everpeak-limpieza-datos.ipynb)


## Descripción del caso

EverPeak es una empresa de retail con datos de clientes y órdenes de compra.
El dataset original contenía valores centinela (-999, 999, "?"), datos faltantes
en columnas clave y fechas inválidas. El objetivo fue construir un pipeline de
limpieza reutilizable para dejar los datos listos para análisis.

---

## ¿Qué contiene este notebook?

- Reemplazo de valores centinela en columnas numéricas y de texto
- Creación de flags de valores faltantes antes de imputar
- Imputación por mediana, reemplazo por "unknown" y eliminación de filas con fechas inválidas
- Pipeline unificado en una función `clean_data()` reutilizable
- Exportación del dataset limpio como `everpeak_clean.csv`

---

## ¿Cómo abrirlo en Google Colab?

1. Haz clic en el archivo `everpeak_limpieza_datos.ipynb`
2. En la parte superior aparece la opción **"Open in Colab"** — haz clic ahí
3. Una vez en Colab, sube el archivo `everpeak_retail.csv` usando el panel de archivos lateral
4. Ejecuta todas las celdas en orden

---

## Estructura del repositorio
```
everpeak-analysis/
│
├── everpeak_limpieza_datos.ipynb   # Notebook con el pipeline completo
└── README.md                       # Documentación del proyecto
```

---

## Herramientas utilizadas

- Python 3
- pandas
- Google Colab

---

*Proyecto desarrollado durante el Sprint 7 de TripleTen — Análisis estadístico para detectar patrones.*
