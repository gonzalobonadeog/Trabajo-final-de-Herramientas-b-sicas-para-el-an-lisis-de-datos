# Trabajo final de Herramientas Básicas para el Analísis de Datos
## Análisis de Obras Públicas Paralizadas y Presupuesto Congelado

Este proyecto analiza el impacto financiero e institucional de las obras públicas paralizadas en la República Argentina. 

A partir de un dataset oficial procesado, se aplicaron técnicas de limpieza, análisis exploratorio y modelado de datos en Python, culminando en la creación de una medida DAX personalizada y un dashboard interactivo en Power BI para una visualización práctica que facilite la toma de decisiones.

## Objetivo del proyecto
- Cuantificar el **Monto Congelado** total retenido en obras públicas con avance físico $\le 1\%$.
- Analizar la concentración del presupuesto inmovilizado según el **rango de inversión** (Alto, Medio y Bajo).
- Evaluar la distribución territorial de las obras paralizadas por **Jurisdicción / Gobierno**.
- Visualizar la **evolución temporal** del presupuesto inmovilizado a lo largo de los ejercicios contractuales.

## Dataset utilizado
- **Fuente:** [Dataset de Obras Públicas (`dataset_obras_powerbi`).](https://data.buenosaires.gob.ar/dataset/ba-obras/resource/ef7449c8-1ba6-459b-9cd2-de6eda5ecc99)
- **Variables principales:** `MONTO_DEFINITIVO`, `AVANCE_FISICO_PCT`, `NOMBRE_JURISDICCION`, `EJERCICIO_CONTRATO`, `rango_monto`.
- **Métrica clave:** Medida DAX `Monto Congelado` ($1,424 billones acumulados).

## Herramientas utilizadas
- **Python** (Pandas, Matplotlib, Seaborn)
- **Google Colab / Jupyter Notebooks**
- **Power BI Desktop** (DAX, Visualizaciones, Modelado)
- **GitHub**

## Dashboard Ejecutivo
[![Dashboard de Obras Paralizadas](figs/dashboard_preview.png)
*(Reemplaza la ruta de la imagen con la captura de pantalla de tu informe final)*](https://github.com/gonzalobonadeog/Trabajo-final-de-Herramientas-b-sicas-para-el-an-lisis-de-datos/blob/b97a909b597097b184ddd68c46f3b7196c0b8638/Dataset_obras_Powerbi.pbix)

## Estructura del proyecto
```text
├── data/          -> Dataset original y procesado (CSV/XLSX)
├── notebooks/     -> Limpieza, EDA y categorización en Python
├── figs/          -> Gráficos exportados y captura del tablero
├── dashboard/     -> Archivo editable de Power BI (.pbix)
└── README.md      -> Documentación general del proyecto
