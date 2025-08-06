📊 Análisis de Evasión de Clientes - Telecom X LATAM
Este proyecto forma parte del Challenge de Alura LATAM - Data Science, cuyo objetivo es analizar los datos de la empresa Telecom X para identificar patrones que expliquen la evasión (churn) de clientes, con el fin de proponer estrategias que ayuden a reducirla.


🚀 Objetivo
Comprender los factores que influyen en la cancelación del servicio por parte de los clientes de Telecom X, utilizando técnicas de limpieza de datos, análisis exploratorio (EDA) y visualización, para obtener insights clave que respalden futuras estrategias de retención o modelos predictivos.


🛠️ Tecnologías utilizadas
- Python (versión 3.10+)
- Pandas para manipulación de datos
- Matplotlib y Seaborn para visualización
- Google Colab como entorno de desarrollo
- JSON API para carga de datos
- Jupyter Notebook (.ipynb)

📂 Estructura del proyecto


- 📁 TelecomX_LATAM
│
├── TelecomX_LATAM.ipynb        # Notebook principal con todo el análisis
├── README.md                   # Este archivo
└── /data/                      # Carpeta opcional si se guarda una versión local del dataset


🔎 Etapas del análisis
1. Carga y Tratamiento de Datos
   
  - Se cargaron los datos desde una API con formato JSON.
  - Se expandieron campos anidados con json_normalize.
  - Se estandarizaron valores categóricos (“Sí/No” a 1/0).
  - Se eliminaron valores nulos en columnas clave.
  - Se creó la columna Cuentas_Diarias para análisis granular del gasto.

2. Análisis Exploratorio de Datos (EDA)
   
  - Análisis descriptivo: media, mediana, desviación estándar, etc.
  - Visualización de la distribución de evasión de clientes (27% abandonaron).
  - Análisis de evasión según variables categóricas (género, contrato, internet, etc.).
  - Boxplots y histogramas para analizar relación de variables numéricas con evasión.
  - Matriz de correlación entre variables numéricas.

3. Conclusiones e Insights
   
  - Contratos “Mes a mes” y método de pago con cheque electrónico tienen mayor churn.
  - Clientes nuevos (<12 meses) presentan mayor tasa de evasión.
  - El tipo de internet (fibra óptica) también está asociado a mayor churn.

4. Recomendaciones Estratégicas
   
  - Incentivar contratos de largo plazo.
  - Promover métodos de pago automatizados.
  - Desarrollar programas de retención para nuevos clientes.


| Variable            | Insight                                     |
| ------------------- | ------------------------------------------- |
| Tipo de contrato    | "Dos años" → solo 2.85% churn               |
| Método de pago      | Cheque electrónico → 45.29% churn           |
| Tiempo como cliente | Menos de 1 año → mayor probabilidad de baja |
| Tipo de internet    | Fibra óptica → 41.89% churn                 |


📈 Próximos pasos

Se recomienda utilizar estos insights como base para el desarrollo de modelos predictivos de churn, aplicando técnicas como:

- Árboles de decisión
- Random Forest
- Regresión logística

  
🤝 Créditos
Desarrollado por: Jose Luis Alvarado
Challenge por: [Alura Latam - Formación Data Science]


