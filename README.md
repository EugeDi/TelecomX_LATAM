# Análisis de Evasión de Clientes en TelecomX (Challenge de Alura LATAM)

Este proyecto se basa en un análisis de los datos de clientes de la empresa TelecomX, con el objetivo de identificar los factores que influyen en la **pérdida de clientes** (churn). A través del procesamiento y análisis de datos, se busca brindar **conclusiones y recomendaciones** que permitan diseñar estrategias para mejorar la fidelización de los clientes.

## Descripción del Proyecto

El proyecto se basa en un conjunto de datos proporcionado en formato JSON con información de más de 7.000 clientes. La tarea principal consistió en:

- Transformar y limpiar los datos.
- Analizar las variables que influyen en la baja de clientes.
- Presentar conclusiones, clarificadas a través de gráficos dinámicos.

## Instalación

### Requisitos

- Cuenta en **Google Colab** para ejecutar el archivo AluraStoreLatam.ipynb
- Python 3.10+
- pandas (`pip install pandas`)
- matplotlib (`pip install matplotlib`)
- seaborn (`pip install seaborn`)
- plotly (`pip install plotly`)

## 1. **Extracción de Datos**

Se obtuvo el dataset directamente desde un repositorio público de GitHub en formato JSON.
https://raw.githubusercontent.com/ingridcristh/challenge2-data-science-LATAM/main/TelecomX_Data.json

## 2. **Transformación**

- Se normalizó la estructura anidada del JSON.
- Se eliminaron registros con valores vacíos o NaN.
- Se convirtieron variables tipo `Yes/No` a binario.
- Se estandarizaron columnas categóricas en lowercase.
- Se creó la variable `Cuentas_Diarias` dividiendo el pago mensual por 30.

## 3. **Análisis**

### Gráficos

- Gráfico de distribución de evasión / Porcentaje de clientes que se dieron de baja.
- Gráfico de distribución de evasión de clientes por variables categóricas.
- Gráfico de distribución de evasión de clientes por variables binarias.

## 4. **Conclusiones**

- **Churn general**: 26,58% de los clientes se dieron de baja.
- **Internet por fibra óptica** y **contrato mensual** son los factores más asociados a una alta tasa de baja.
- Servicios como **seguridad online** y **soporte técnico** están correlacionados con mayor fidelización.
- Los primeros meses son críticos: la tasa de churn supera el 50% en los primeros 2 meses.

## 5. **Recomendaciones**

- Implementar **acciones de fidelización temprana**, especialmente en los primeros 3 meses.
- Fomentar el uso de servicios que reducen el churn como Online Security y Tech Support.
- Ofrecer incentivos para extender el plazo de los contratos.
- Realizar **encuestas específicas** para profundizar sobre:
  - Dificultades con la facturación electrónica.
  - Calidad del servicio de fibra óptica.
  - Percepción del valor/costo del servicio.
