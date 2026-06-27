# Manejo de Outliers con Python

📊 Análisis de Datos de Sesiones de Gimnasio

🏋️‍♂️ ¿Qué hace este código?

Este notebook realiza un análisis completo de datos de sesiones de entrenamiento en un gimnasio, aplicando técnicas de manipulación de datos y detección de outliers para obtener insights precisos.

🔄 Procesos principales:

🔗 Joins de datos - Combina tablas de sesiones, miembros y entrenadores usando:

LEFT JOIN (sesiones + miembros)

RIGHT JOIN (miembros + sesiones)

INNER JOIN (sesiones + entrenadores)

📈 Análisis exploratorio - Calcula métricas clave:

🔥 Promedio de calorías quemadas por entrenador

⏱️ Duración promedio de sesiones por tipo de membresía

📊 Cantidad total de sesiones por miembro (ordenado)

🏆 Máximo de calorías quemadas por entrenador

🧹 Detección y limpieza de outliers:

📐 Usa método IQR (Rango Intercuartílico)

🎯 Detecta valores atípicos en calories_burned

🧽 Crea dataset limpio sessions_clean

🔄 Análisis comparativo - Recalcula métricas después de limpiar outliers

🎯 Resultados obtenidos:

📊 Antes de limpiar outliers:

Entrenador con mayor promedio: Daniel Herrera (1,570 calorías)

Entrenador con menor promedio: Andres Vega (235 calorías)

Duración promedio por membresía: VIP (97.5 min), Premium (67.5 min), Basic (50 min)

🧹 Después de limpiar outliers:

Promedios más realistas: Daniel Herrera (690 calorías)

Máximos de calorías ajustados: de 3500 → 760 para Daniel Herrera

Duración promedio VIP: ajustada de 97.5 → 58.75 minutos

💡 Insights clave:

✅ Los outliers afectan significativamente la media de calorías quemadas

📊 Los miembros VIP tienen sesiones más largas pero menos consistentes

🏋️ Los entrenadores de HIIT muestran mayor variabilidad en calorías

🔍 La limpieza de datos es crucial para análisis precisos

🛠️ Tecnologías utilizadas:

🐼 Pandas (manipulación de datos)

📊 GroupBy operations

📐 IQR method for outlier detection

🔄 Merge operations (left, right, inner joins)

🚀 Recomendaciones para el gimnasio:

Revisar sesiones extremas (especialmente > 2,000 calorías)

Estandarizar duración de sesiones VIP

Analizar consistencia de entrenadores de HIIT

Considerar membresías Premium para sesiones más balanceadas
