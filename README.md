# 📊 **Análisis Comercial Andes Capital Real State**

## 🇪🇦 Español

## 🎯 Descripción del Proyecto
Andes Capital Real State con presencia en Mexico y Colombia es una una inmobiliaria con más de 30 años de experiencia en la urbanización y venta de fraccionamientos campestres, necesita evaluar su **desempeño comercial** para comprender su crecimiento, rentabilidad y comportamiento de clientes. 

El análisis realizado se llevo a cabo en Power BI en 5 etapas: Calidad de datos, creación de tabla de calendario, modelado de datos, creacion de medidas y KPIs, y estructura de Dashboard.

## 🔍 Pregunta de Investigación
¿Cuál es el ingreso total generado por las ventas de propiedades?
¿Qué tipo de propiedad genera más ingresos?
¿Qué segmentos de clientes compran más?
¿Cómo evolucionan las ventas en el tiempo?
¿El negocio está creciendo año contra año?
¿Los clientes vuelven a comprar después de su primera compra?

## 📋 Objetivos
Realizar una limpieza adecuada de los datos para garantizar la validez de los mismos en los análisis posteriores.
Identificar KPIs financieros para determinar la rentabilidad del negocio.
Dividir a los clientes en cohortes para identificar la retención de los mismos a lo largo del tiempo.
Comunicar los hallazgos en un dashboard en Power BI

## 🗂️ Dataset
Fuente: hecho_ventas_propiedades.csv
Tamaño: 8,500 registros de ventas

Fuente: dim_clientes.csv
Tamaño: 3,500 registros de clientes

Fuente: dim_propiedades.csv
Tamaño: 8,000 registros de propiedades

## **Variables Analizadas**
| Variable | Tipo | Descripción |
|---------|-------------|-------------------|
| precio_venta	| Numérica | Precio final de venta de la propiedad |
| monto_comision | Numérica |	Monto de comisión generado por la venta |
| ciudad | Categórica	| Ciudad donde se realizó la venta |
| tipo_propiedad	| Categórica	| Tipo de propiedad vendida |
| segmento_comprador | Categórica | Tipo o perfil del comprador |
| canal_venta	| Categórica	| Canal utilizado para la venta |
| tipo_propiedad | Categórica	| Tipo de propiedad |
| fecha_venta	| Fecha	| Fecha en que se realizó la venta |

## 🛠️ Metodología
Limpieza de datos.
Modelado de datos.
Herramientas Utilizadas: *Power BI, Visualizaciones nativas (barras, líneas, tablas, KPI), Modelado de datos en esquema estrella, Cálculos analíticos (medidas y columnas calculadas).*

## 🔄 Etapas del Análisis
Este proyecto sigue un flujo estructurado de análisis dividido en 5 etapas principales:

| Etapa	 | Descripción | Resultado Esperado |
|---------|-------------|-------------------|
| 1. Exploración y limpieza | Cargar y explorar el dataset | Entender estructura, columnas, tipos, métricas clave, corregir formatos, valores nulos y eliminar duplicados |
| 2. Creación de tabla de calendario | Se creó el la tabla dim_fecha | Calcular KPIs y cohortes de retención | 
| 3. Modelado de datos | Crear el modelo estrella, y definir las relaciones adecuadas entre tablas | Tener un modelo que pueda calcular medidas DAX y KPIs sin presentar errores de ejecución o de cálculo |
| 4. Creacion de medidas y cohortes | Calcular medidas qué contesten las preguntas de negocio | Entender el desempeño del negocio y el comportamiento del cliente a lo largo del tiempo |
| 5. Visualización | Crear visualizaciones |	Dashboard interactivo en Power BI |
 
### 🎯 Enfoque del Análisis
Naturaleza: Descriptivo (KPIs de negocio) y Exploratorio (cohortes)
Variable objetivo: Revenue y profit, y Tasa de retención mensual
Tipos de relaciones analizadas: Comportamiento del usuario por tipo de cliente, ingresos por tipo de propiedad, Actividad anual y mensual por cohorte de registro.

### 🗂 Producto Final
Un reporte de rentabilidad y retención que combina:

✅ Evidencia visual (Dashboard interactivo en PowerBI)
✅ Evidencia numérica (KPIs de performance)
✅ Retención por cohortes
✅ Implicaciones de negocio accionables

### **📊 Resultado del Análisis**
- El tipo de propiedad que genera mayor revenue son las casas con $2.24 mil millones (37.3% del total).
- La ciudad con mayor volumen de ventas es Ciudad de México con 53.92% de participación.
- El canal de venta más eficiente en términos de ingresos son los corredores con 72.85% de participación.
- El negocio registró un crecimiento del 14.28% en 2024 vs 2023.
- Las ventas muestran patrones estacionales con picos en marzo-abril y septiembre-noviembre.
- Las ventas muestran un crecimiento sostenido del 14.28% YoY.
- Los corredores generan 2.7 veces más ingresos que las ventas directas.

## **🖋 Conclusiones y recomendaciones**
- Priorizar la comercialización de propiedades tipo comercial por su alto ticket promedio ($1.79M).
- Fortalecer el canal de corredores que presenta mayor participación en el revenue (72.85%).
- Implementar estrategias de upselling para clientes primerizos hacia propiedades de mayor valor.
- Desarrollar campañas estacionales aprovechando los picos de marzo-abril y septiembre-noviembre.
- Crear programas de fidelización para el segmento de inversionistas (24.47%) con potencial de recompra.
- Optimizar la eficiencia de costos en el canal de corredores manteniendo su efectividad comercial.

## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:
[Google Colab](https://colab.research.google.com/drive/1AeliHUxdl8CC2TGrKDZelCq_pRMMwOKm?usp=sharing)

## 📘 Cómo reproducir el análisis

1. Abre `notebooks/S11 Proyecto_InmobiliarioGrupoAndes.ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/`

# 📊 Commercial Analysis - Andes Capital Real Estate

## 🇬🇧 English

## 🎯 Project Description
Andes Capital Real Estate, operating in Mexico and Colombia, is a real estate firm with over 30 years of experience in land development and country estate sales. The firm required an evaluation of its **commercial performance** to understand growth trajectories, profitability, and customer behavior dynamics.
The analysis was executed in Power BI across 5 main stages: Data quality & cleaning, calendar table generation, data modeling, DAX measures & KPIs engineering, and interactive dashboard architecture.

## 🔍 Research Questions
- What is the total revenue generated from property sales?
- Which property type generates the highest revenue?
- Which customer segments account for the highest purchase volume?
- How do sales evolve over time?
- Is the business demonstrating year-over-year (YoY) growth?
- Do customers make repeat purchases following their initial acquisition?

## 📋 Objectives
- Perform thorough data cleaning to ensure data validity for subsequent analytical stages.
- Define core financial KPIs to assess business profitability.
- Segment customers into cohorts to evaluate retention trends over time.
- Communicate actionable business insights through an interactive Power BI dashboard.

## 🗂️ Datasets Used
Source: `hecho_ventas_propiedades.csv`  
Size: 8,500 sales transactions  
Source: `dim_clientes.csv`  
Size: 3,500 customer records  
Source: `dim_propiedades.csv`  
Size: 8,000 property records  

## **Analyzed Variables**

| Variable | Type | Description |
| :--- | :--- | :--- |
| precio_venta | Numerical | Final sale price of the property |
| monto_comision | Numerical | Commission amount generated by the sale |
| ciudad | Categorical | City where the transaction occurred |
| tipo_propiedad | Categorical | Type of property sold |
| segmento_comprador | Categorical | Buyer profile or customer segment |
| canal_venta | Categorical | Acquisition channel used for the sale |
| fecha_venta | Date | Date when the sale transaction took place |

## 🛠️ Methodology
Data Cleaning, Data Modeling.  
Tools Used: *Power BI, Native Visualizations (bar charts, line charts, tables, KPIs), Star Schema Data Modeling, Analytical DAX Calculations (Measures and Calculated Columns).*

## 🔄 Analysis Stages
This project follows a structured analytical workflow divided into 5 main stages:

| Stage | Description | Expected Outcome |
| :--- | :--- | :--- |
| 1. Exploration & Cleaning | Load and inspect datasets | Understand structure, data types, key metrics; fix formatting, null values, and remove duplicates |
| 2. Calendar Table Engineering | Create the `dim_fecha` table | Enable Time Intelligence calculations, KPIs, and cohort retention tracking |
| 3. Data Modeling | Build a Star Schema model with proper relationship cardinalities | Establish a robust data model capable of calculating DAX measures and KPIs without runtime or calculation errors |
| 4. DAX Measures & Cohort Creation | Engineer analytical metrics answering core business questions | Evaluate overall performance trends and customer lifetime behavior over time |
| 5. Visualization | Build visual dashboard components | Interactive Power BI dashboard |

### 🎯 Analytical Focus
Nature: Descriptive (Business KPIs) and Exploratory (Cohorts).  
Target Variables: Revenue, Profit, and Monthly Retention Rate.  
Relationship Types Analyzed: Customer purchasing behavior by segment, revenue distribution by property type, and annual/monthly activity by registration cohort.

### 🗂 Final Product
A comprehensive commercial performance and retention report featuring:
✅ Visual evidence (Interactive Power BI Dashboard)  
✅ Numerical evidence (Performance KPIs)  
✅ Cohort-based retention analysis  
✅ Actionable business implications  

### 📊 **Key Findings**
- Residential Houses represent the top revenue-generating property type, driving $2.24 billion (37.3% of total revenue).
- Mexico City accounts for the highest transaction volume, holding a 53.92% market share.
- Real Estate Brokers emerged as the most efficient sales channel, driving 72.85% of total revenue.
- The business achieved a 14.28% YoY revenue growth rate (2024 vs. 2023).
- Sales display clear seasonal patterns, with demand peaking in March–April and September–November.
- Broker-driven sales generate 2.7 times more revenue compared to direct sales channels.

## 🖋 **Conclusions & Recommendations**
- Prioritize the commercialization of Commercial properties due to their high average order value ($1.79M AOV).
- Strengthen broker partnerships and channel incentives, given their dominant revenue contribution (72.85%).
- Implement targeted upselling strategies to transition first-time buyers toward higher-value property portfolios.
- Capitalize on seasonal demand surges by aligning marketing campaigns with March–April and September–November peaks.
- Develop dedicated loyalty and retention initiatives for the Investor segment (24.47% of customer base) to maximize repeat purchase potential.
- Optimize broker channel cost structures to maximize margin efficiency without compromising commercial volume.

## ▶ How to open the notebook in Google Colab
Click on the following button:  
[Google Colab](https://colab.research.google.com/drive/1AeliHUxdl8CC2TGrKDZelCq_pRMMwOKm?usp=sharing)

## 📘 How to reproduce the analysis
1. Open `notebooks/S11 Proyecto_InmobiliarioGrupoAndes.ipynb`
2. Execute the cells in sequential order
3. The notebook automatically loads datasets from `/data/`
