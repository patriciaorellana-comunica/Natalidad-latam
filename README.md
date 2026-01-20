# Natalidad-latam

Proyecto: Análisis Demográfico de Natalidad en LATAM (2001-2023)
Objetivo: Demostrar un flujo de trabajo reproducible de limpieza, procesamiento estadístico y ranking de indicadores demográficos para comunicación de datos y análisis de políticas públicas.

Fuente: Datos históricos de tasas de natalidad por cada 1,000 habitantes en América Latina (periodo de 23 años).

Outputs (Data Pipeline):

data/natalidad_latam_25_anios_limpio.csv: Serie temporal depurada con registros anuales por país desde 2001 hasta 2023.

data/natalidad_latam_ranking.csv: Clasificación de países basada en el promedio histórico de natalidad (liderado por Guatemala y Honduras).

data/summary.csv: Matriz estadística completa que incluye valores máximos, mínimos, desviaciones estándar y rangos por cada país analizado.

Cómo correr el análisis:

Bash
# 1. Instalar dependencias
pip install pandas numpy

# 2. Ejecutar script de limpieza y procesamiento
python src/clean_natalidad.py

# 3. Generar ranking y estadísticas descriptivas
python src/generate_summary.py
Website: Visualización interactiva de las tendencias demográficas publicada con GitHub Pages en la carpeta /docs. El sitio incluye gráficos comparativos que muestran el descenso generalizado de la natalidad en la región, destacando casos como el de Argentina y Perú.
