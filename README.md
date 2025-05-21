# 🎮 Análisis de Ventas y Tendencias en Videojuegos - Tienda Ice

Este proyecto analiza un conjunto de datos históricos del mercado de videojuegos con el objetivo de identificar patrones que expliquen el éxito comercial de los títulos en distintas plataformas, regiones y géneros. A través de herramientas de análisis exploratorio y estadístico, se busca brindar recomendaciones estratégicas para campañas publicitarias y selección de productos para el año siguiente.

## 🧠 Contexto

Trabajamos para **Ice**, una tienda online que vende videojuegos en todo el mundo. Disponemos de datos públicos sobre ventas, reseñas de usuarios y críticos, plataformas (como Xbox o PlayStation), géneros y clasificaciones ESRB.

El proyecto simula estar en diciembre de 2016, utilizando los datos disponibles hasta ese momento para planear de manera informada las campañas de marketing para 2017.

## 📊 Dataset

El archivo `games.csv` incluye las siguientes columnas:

- `Name`: Nombre del videojuego  
- `Platform`: Plataforma en la que se lanzó  
- `Year_of_Release`: Año de lanzamiento  
- `Genre`: Género del juego  
- `NA_sales`: Ventas en Norteamérica (en millones de USD)  
- `EU_sales`: Ventas en Europa (en millones de USD)  
- `JP_sales`: Ventas en Japón (en millones de USD)  
- `Other_sales`: Ventas en otras regiones (en millones de USD)  
- `Critic_Score`: Calificación promedio de críticos (escala 0–100)  
- `User_Score`: Calificación promedio de usuarios (escala 0–10)  
- `Rating`: Clasificación ESRB (por ejemplo, E, T, M)

## 🎯 Objetivos del Proyecto

1. **Preparar y depurar los datos** para asegurar su calidad, estandarización y coherencia para el análisis.  
2. **Analizar el comportamiento histórico de las ventas** por plataforma, género y región, enfocándose en las tendencias recientes que puedan influir en la planificación de 2017.  
3. **Explorar el impacto de las reseñas y calificaciones** (de críticos y usuarios) en las ventas globales y regionales de los videojuegos.  
4. **Identificar plataformas y géneros prometedores**, destacando los más rentables y con mayor crecimiento.  
5. **Desarrollar perfiles de usuario regionales** (Norteamérica, Europa y Japón) para entender las preferencias específicas por plataforma, género y clasificación ESRB.  
6. **Probar hipótesis estadísticas** relacionadas con las calificaciones de usuarios entre plataformas y géneros, aplicando pruebas de significancia para obtener conclusiones objetivas.  
7. **Extraer conclusiones accionables** que permitan recomendar estrategias de marketing y selección de productos para el año siguiente.

## 🔧 Tecnologías utilizadas

- **Python**
- **Pandas**, 
- **NumPy**
- **Matplotlib**, **Seaborn**
- **SciPy** (para pruebas estadísticas)


## 📈 Análisis Realizado

- Limpieza y transformación de datos
- Análisis de ventas por año, plataforma y género
- Exploración del impacto de las reseñas en las ventas
- Comparación de ventas entre regiones (NA, EU, JP)
- Pruebas de hipótesis con `ttest_ind` para comparar medias entre plataformas y géneros
- Visualización de datos con gráficos de dispersión, histogramas, diagramas de caja, y más

## 📌 Principales Hallazgos

- **PS4**, **Xbox One** y **3DS** fueron líderes en ventas en 2016.
- El género **Acción** fue el más común, pero **Shooter** y **Deportes** generaron mayores ingresos por juego.
- Las reseñas de **críticos** tienen una mayor correlación con las ventas que las reseñas de **usuarios**.
- **Japón** muestra fuertes preferencias por plataformas de Nintendo, mientras que **Norteamérica** y **Europa** se inclinan hacia consolas de Sony y Microsoft.
- La clasificación ESRB tiene **diferente impacto** en las ventas según la región.
- Existe evidencia suficiente para **predecir el éxito comercial de un videojuego** si se consideran factores como:
  - Región de lanzamiento (con especial atención a las diferencias del mercado japonés),
  - Plataforma (PC se mantiene como opción sólida a futuro),
  - Género (Action y Sports tienen alto potencial en EU y NA),
  - Calificaciones positivas de usuarios (aumentan las probabilidades de éxito).
