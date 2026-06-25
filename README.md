# Tableau: Análisis Socioeconómico y Censo de Árboles Urbanos en Nueva York (TREE & MONEY in NYC)

Este repositorio contiene un proyecto práctico de Business Intelligence desarrollado en **Tableau** enfocado en el cruce analítico entre la infraestructura verde urbana y los indicadores socioeconómicos de la Ciudad de Nueva York. El tablero correlaciona el volumen total de árboles registrados por distritos (*Boroname*), el estado de salud de la cobertura forestal por códigos postales (*Zipcode*) y las estimaciones de ingresos y hogares (*Salary Dates*), permitiendo identificar patrones de distribución ecológica y equidad ambiental en los diferentes barrios de la metrópoli.

---

## 📊 Visualización del Dashboard

Para desplegar la interfaz gráfica de forma directa en el repositorio, guarda tu captura de pantalla en la raíz con el nombre exacto de `dashboard_nyc_trees.png` y se enlazará automáticamente aquí:

<img width="675" height="607" alt="image" src="https://github.com/user-attachments/assets/5341e74b-7945-4fe8-9d8a-d081198fc383" />

🔗 **[Interactuar con el Tablero en Vivo en Tableau Public](https://public.tableau.com/app/profile/maria.del.cielo.robledo/viz/CitiesDateTreeofcensus2015/Dashboard1)**

---

## 📈 Componentes y Métricas del Tablero

El diseño del lienzo organiza la información mediante paneles coordinados que desglosan la relación entre naturaleza y economía urbana:

### 1. Volumen y Distribución de Árboles por Distrito (*Cities Dates Tree*)
* **Masa Forestal Absoluta:** Gráfico de barras horizontales que cuantifica la suma total de identificadores de árboles (`Suma de Tree Id`) agrupados por distritos (*Boroname*). La visualización expone que regiones como **Queens** y **Brooklyn** concentran la mayor densidad absoluta de árboles urbanos del censo, en contraste con distritos de menor superficie o mayor urbanización como el Bronx.

### 2. Análisis Relacional de Ingresos y Hogares (*Salary Dates*)
* **Diagrama de Dispersión (*Scatter Plot*):** Correlación bivariada que cruza estimaciones de volumen de hogares (`Households Estimate Total`) frente a indicadores de distribución del ingreso en los distritos. Los puntos están codificados por color y formas de anillo para segmentar geográficamente el comportamiento y los niveles socioeconómicos de las familias en la ciudad.

### 3. Auditoría de Salud Forestal por Códigos Postales (*Health Tree Stados*)
* **Gráfico de Barras Segmentadas y Apiladas:** Desglose detallado que mide el recuento de salud de los árboles (`Recuento de Health`) a nivel micro-geográfico por códigos postales específicos (ej. 10463, 10473, 10035). Cada columna segmenta proporcionalmente la condición física de los ejemplares, utilizando una paleta de tonos verdes y amarillos para identificar rápidamente zonas con alta concentración de árboles saludables o áreas que requieren intervención ecológica.

---

## 🛠️ Conceptos Técnicos Aplicados en Tableau

* **Análisis de Datos Cruzados (*Cross-Domain Data Blending*)**: Integración y modelado de conjuntos de datos de naturaleza dispar (registros ambientales botánicos e indicadores demográficos de censos económicos estructurales) bajo un mismo lienzo analítico unificado.
* **Segmentación Micro-Geográfica por Gránulos (*Zipcode Parsing*)**: Uso de dimensiones de alta granularidad como los códigos postales americanos para evitar sesgos por promedios macroestructurales, aislando la realidad sanitaria forestal cuadra por cuadra.
* **Codificación Dual de Atributos Visuales**: Configuración avanzada de marcas de gráficos aplicando color de relleno y tipos de bordes o formas de anillo en el diagrama de dispersión para representar múltiples dimensiones categóricas de manera simultánea sin saturar la legibilidad.
