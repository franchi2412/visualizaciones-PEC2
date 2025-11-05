# Visualizaciones PEC 2 – UOC

## Introducción

El objetivo de esta actividad es explorar y aplicar diferentes **técnicas de visualización de datos** con el fin de comprender sus características, ventajas y limitaciones según el tipo de información representada.  
Esta práctica forma parte de la **PEC 2 de la asignatura Visualización de Datos (UOC)**, y su propósito principal es **experimentar con herramientas y técnicas menos comunes**, trabajando desde la técnica hacia los datos.

En todas las representaciones se han utilizado datos abiertos sobre **emisiones de CO₂ (año 2023)**, obtenidos del portal [Our World in Data](https://ourworldindata.org/co2-emissions).  
Los datos fueron **procesados y limpiados en una hoja de cálculo**, conservando únicamente la información relevante para cada técnica de visualización (por continente y país).  
El archivo resultante —[`co2_by_continent_country_2023_cleaned.csv`](./co2_by_continent_country_2023_cleaned.csv)— se incluye en este repositorio como conjunto de datos final y estructurado.

---

## 1. Circle Packing (RAWGraphs)

**Técnica de visualización:**  
El *Circle Packing* es una técnica jerárquica que representa las relaciones de inclusión entre categorías mediante círculos anidados.  
Cada círculo representa una categoría (en este caso, un país o continente), y su tamaño está determinado por el valor total de emisiones de CO₂.

**Herramienta utilizada:** [RAWGraphs.io](https://app.rawgraphs.io)

**Datos:** Emisiones de CO₂ por continente y país, año 2023.  
**Fuente:** [Our World in Data](https://ourworldindata.org/co2-emissions)

**Recursos disponibles en este repositorio:**
- Archivo del proyecto RAWGraphs: [`CirclePacking.zip`](./CirclePacking.zip)
- Imagen exportada (SVG): [Circle_Packing.svg](./Circle_Packing.svg)

---

## 2. Box Plot (Flourish)

**Técnica de visualización:**  
El *Box Plot* (diagrama de caja) permite analizar la distribución de un conjunto de valores y comparar su dispersión entre diferentes categorías.  
En esta visualización se comparan las **emisiones de CO₂** entre continentes, mostrando valores mínimos, máximos, mediana y cuartiles.

**Herramienta utilizada:** [Flourish Studio](https://flourish.studio/)

**Datos:** Emisiones de CO₂ por continente, año 2023.  
**Fuente:** [Our World in Data](https://ourworldindata.org/co2-emissions)

**Recursos disponibles:**
- Visualización interactiva en línea: [Ver en Flourish](https://public.flourish.studio/visualisation/25982695/)
- Imagen exportada (SVG): [Box_Plot_CO2_continent.svg](./Box_Plot_CO2_continent.svg)

---

## 3. Hyperbolic Tree / Sunburst (Python + Plotly + Pyvis)

**Técnica de visualización:**  
El *Hyperbolic Tree* o *árbol hiperbólico* es una técnica jerárquica que representa relaciones de tipo árbol en un espacio radial o hiperbólico, permitiendo explorar estructuras complejas sin perder el contexto global.  
En este caso, se utiliza para visualizar la jerarquía **Continente → País**, destacando el volumen relativo de emisiones de CO₂.

**Herramientas utilizadas:**  
- [`Plotly`](https://plotly.com/python/) (visualización *Sunburst*)  
- [`Pyvis`](https://pyvis.readthedocs.io/) (red jerárquica navegable)  
- `Jupyter Notebook` para análisis y generación de los gráficos

**Recursos disponibles:**
- Notebook con el código completo: [`PEC2_HyperbolicTree_Sunburst_CO2.ipynb`](./PEC2_HyperbolicTree_Sunburst_CO2.ipynb)
- Visualización Sunburst exportada a HTML: [sunburst_co2_2023.html](./sunburst_co2_2023.html)
- Visualización Pyvis interactiva: [hyperbolic_tree_CO2_2023.html](./hyperbolic_tree_CO2_2023.html)

---

## Conclusión

Estas tres visualizaciones permiten comparar diferentes enfoques para representar relaciones jerárquicas y distribuciones de datos cuantitativos.  
El uso combinado de **RAWGraphs**, **Flourish** y **Python (Plotly/Pyvis)** demuestra cómo distintas herramientas pueden complementar la comprensión visual de un mismo fenómeno.  
Asimismo, el dataset limpio y estructurado incluido en el repositorio sirve como base común para todas las representaciones, garantizando coherencia y comparabilidad entre las técnicas empleadas.

---

Autor: **Francisco Jesús Castro García**  
Curso 2024–2025  
Grado en Ciencia de Datos – Universitat Oberta de Catalunya (UOC)
