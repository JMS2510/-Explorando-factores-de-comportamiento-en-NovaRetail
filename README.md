# Proyecto 7 - Explorando drivers de comportamiento en NovaRetail+

Este proyecto forma parte de mi portafolio como analista de datos.  
El objetivo es identificar qué factores del comportamiento del cliente están más fuertemente asociados con el ingreso anual generado en la plataforma NovaRetail+ durante 2024.

## Contexto del negocio
NovaRetail+ es una plataforma de comercio electrónico en Latinoamérica.  
El equipo de Crecimiento y Retención busca entender qué comportamientos de los clientes impactan más en el ingreso anual, para diseñar estrategias de fidelización y crecimiento.

## Dataset
- Nombre: `novaretail_comportamiento_clientes_2024.csv`
- Tamaño: 15,000 registros
- Columnas principales:
  - `edad`, `nivel_ingreso`, `visitas_mes`, `compras_mes`, `gasto_publicidad_dirigida`, `satisfaccion`
  - `miembro_premium`, `abandono`
  - `tipo_dispositivo`, `region`
  - `ingreso_anual` (variable foco del análisis)

## Flujo del proyecto
1. **Exploración inicial**: revisión de tipos de datos, valores nulos y clasificación de variables.
2. **Visualización**: heatmaps y scatterplots para identificar patrones.
3. **Correlaciones**:
   - Pearson y Spearman (numéricas)
   - Punto-biserial (binarias vs numéricas)
   - V de Cramér (categóricas)
4. **Interpretación de resultados**: hallazgos clave con evidencia visual y numérica.
5. **Limitaciones y próximos pasos**: reconocimiento de sesgos y propuestas de mejora.

## Hallazgos principales
- **Compras vs ingreso anual**: correlación muy fuerte (≈0.97). Los clientes que compran más generan más ingresos.
- **Visitas vs compras**: correlación moderada (≈0.35). Más visitas suelen asociarse con más compras, aunque no siempre.
- **Premium vs ingreso anual**: relación positiva moderada. Los clientes premium aportan más ingresos.
- **Abandono vs ingreso anual**: relación negativa. Los clientes que abandonan generan menos ingresos.
- **Región y dispositivo**: asociaciones débiles. No son factores relevantes para explicar ingresos.

## Limitaciones
- Correlación ≠ causalidad.
- Dataset limitado a un año.
- No incluye factores externos (marketing, competencia, estacionalidad).
- Colinealidad entre algunas variables.

## Próximos pasos
- Segmentar clientes premium vs no premium.
- Construir modelos predictivos de ingreso anual.
- Analizar abandono con más detalle y probar estrategias de retención.
- Explorar el rol de la satisfacción en la fidelización.

## Tecnologías utilizadas
- Python (pandas, numpy, seaborn, matplotlib, scipy)
- Jupyter Notebook

## Autor
Proyecto realizado por Julio como parte de su portafolio de análisis de datos.  
