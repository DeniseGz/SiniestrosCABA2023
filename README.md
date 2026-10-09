# 📊 Análisis de Siniestros Viales en CABA

<p align="center">
  <img src="https://img.shields.io/badge/POWER%20BI-75AADB?style=flat&logo=powerbi&logoColor=white" />
  <img src="https://img.shields.io/badge/EXCEL-4682B4?style=flat&logo=microsoftexcel&logoColor=white" />
  <img src="https://img.shields.io/badge/POWER%20QUERY-1C39BB?style=flat&logoColor=white" />
  <img src="https://img.shields.io/badge/DAX-F8D347?style=flat&logoColor=black" />
</p>

🤍 *Tablero interactivo en Power BI para el análisis y visualización de incidentes viales en la Ciudad de Buenos Aires utilizando datos públicos.* 💙

---

### ☀️ Descripción del Proyecto 
* Desarrollo de dashboard interactivo en Power BI para visualizar y monitorear siniestros viales en CABA a partir de fuentes de datos públicos.
* Transformación y modelado de datos mediante Power Query y Excel, realizando limpieza y segmentación avanzada por barrios, tipología de incidentes y franjas horarias críticas. 
* Desarrollo de medidas y KPIs complejos con DAX para la detección precisa de zonas de alto riesgo vial.
* Automatización de reportes mensuales, optimizando los tiempos de actualización y facilitando el acceso a información clave para la toma de decisiones.

---

## 📈 Visualizaciones y Componentes del Tablero
El reporte interactivo incluye cuatro visualizaciones principales para el análisis de los datos:

* **Delitos por barrio (Gráfico de barras horizontales)**: Muestra la distribución de los registros clasificados por barrios de CABA (como Palermo, Balvanera, Flores, Almagro, Caballito, Recoleta, entre otros).
* **Ubicación exacta de los delitos (Mapa interactivo)**: Un mapa geolocalizado que abarca la zona de Buenos Aires y alrededores (incluyendo partidos del conurbano como Vicente López, San Martín, Tres de Febrero, Lanús, Lomas de Zamora, Quilmes, etc.).
* **Evolución mensual de delitos (Gráfico de líneas)**: Analiza la tendencia temporal de los hechos mes a mes (desde enero hasta diciembre), permitiendo identificar picos y caídas en la frecuencia de los incidentes.
* **Ranking de comunas con más delitos (Gráfico de barras verticales)**: Compara el volumen de casos agrupados por número de comuna, detallando métricas como la suma de hechos y el recuento total.

---

## 🏷️ Tipologías Analizadas en el Reporte
El tablero categoriza los incidentes bajo distintas tipologías y variables que se visualizan en las leyendas superiores:
* Amenazas
* Homicidio doloso
* Homicidio culposo
* Hurto automotor / Hurto total
* Lesiones dolosas / Lesiones por siniestro
* Muertes por siniestro
* Robo automotor / Robo total

---

## 🛠️ Estructura de Datos del Modelo
El modelo de datos maneja las siguientes dimensiones principales para el análisis de siniestros:

*   **Dim_Tiempo**: Fecha, Año, Mes, Día, Franja Horaria.
*   **Dim_Ubicación**: Comuna, Barrio, Latitud, Longitud, Cruce / Calle.
*   **Dim_Participantes**: Rol de la víctima ( peatón, pasajero, conductor), tipo de vehículo afectado y vehículo acusado.
*   **Hechos_Siniestros**: Tabla de hechos central que registra la cantidad de incidentes y la gravedad de los mismos.

*Designed and developed by DeniseGz © 2026*
