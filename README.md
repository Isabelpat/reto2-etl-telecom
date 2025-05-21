# Proyecto ETL - Reto de Telecomunicaciones 📊

Este repositorio contiene el desarrollo de un pequeño proyecto de **extracción, transformación y carga (ETL)** a partir de un archivo JSON con información de clientes de una empresa de telecomunicaciones.

## 📁 Estructura del proyecto

- `TelecomX_Data.json`: archivo original de entrada en formato JSON.
- `Telecom_Clean.csv`: archivo transformado y limpio en formato CSV.
- `ETL_Telecom.ipynb`: notebook de Google Colab donde se realizó todo el análisis.

## 🔄 Proceso ETL

### 1. **Extracción**
El archivo JSON fue cargado desde Google Drive hacia Google Colab usando `pandas`.

### 2. **Transformación**
- Se detectaron datos anidados y se normalizaron usando `pd.json_normalize`.
- Se identificaron y eliminaron:
  - Valores nulos en columnas numéricas (`Charges Total`)
  - Filas duplicadas
- Se revisaron:
  - Inconsistencias en categorías (`Contract`, `InternetService`, `PaymentMethod`)
  - Errores de formato
  - Outliers (valores atípicos) en columnas numéricas
- Las columnas fueron renombradas para mayor legibilidad.

### 3. **Carga**
El DataFrame limpio fue exportado a un archivo `.csv`.

## 🛠 Herramientas utilizadas

- Python
- Pandas
- Google Colab
- Git / GitHub

## 📌 Objetivo

Este ejercicio forma parte de un reto educativo para reforzar habilidades de análisis de datos, limpieza de información y control de versiones.

---

#Autor: Patricia Isabel Benitez Ramos
#brpisabel@gmail.com
