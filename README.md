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


## 📈 Visualizaciones y Componentes del Tablero
El reporte interactivo desarrollado en Power BI se compone de cuatro paneles principales de análisis:

* **Delitos por barrio (Gráfico de barras horizontales)**: Muestra la distribución de los registros clasificados por los diferentes barrios de CABA (como Palermo, Balvanera, Flores, Almagro, Caballito, Recoleta, entre otros).
* **Ubicación exacta de los delitos (Mapa interactivo)**: Un mapa geolocalizado que abarca la zona de Buenos Aires y sus alrededores (incluyendo partidos del conurbano como Vicente López, San Martín, Tres de Febrero, Lanús, Lomas de Zamora, Quilmes, etc.).
* **Evolución mensual de delitos (Gráfico de líneas)**: Analiza la tendencia temporal de los hechos mes a mes (desde enero hasta diciembre), facilitando la detección de picos estacionales y caídas en la frecuencia.
* **Ranking de comunas con más delitos (Gráfico de barras verticales)**: Compara de forma directa el volumen de casos agrupados por número de comuna, detallando métricas de suma de hechos y recuento total.

---

## 🏷️ Tipologías Analizadas en el Reporte
El tablero categoriza los incidentes bajo las siguientes variables y leyendas de control:
* Amenazas
* Homicidio doloso
* Homicidio culposo
* Hurto automotor / Hurto total
* Lesiones dolosas / Lesiones por siniestro
* Muertes por siniestro
* Robo automotor / Robo total

---

## 🛠️ Diccionario de Datos y Modelo
El modelo en estrella de Power BI se compone de las siguientes tablas y dimensiones:

* **Dim_Tiempo**:
  * `Fecha` (Fecha del hecho)
  * `Año` (Año del siniestro)
  * `Mes` (Mes en formato numérico y texto)
  * `Día` (Día de la semana)
  * `Franja_Horaria` (Mañana, Tarde, Noche, Madrugada)
* **Dim_Ubicación**:
  * `Comuna` (Número de comuna CABA)
  * `Barrio` (Nombre del barrio)
  * `Latitud` / `Longitud` (Coordenadas geográficas para el mapa)
  * `Cruce_Calle` (Esquina o altura exacta)
* **Dim_Participantes**:
  * `Rol_Victima` (Peatón, conductor, pasajero, ciclista)
  * `Vehiculo_Victima` (Moto, auto, bicicleta, etc.)
  * `Vehiculo_Acusado` (Colectivo, auto, camión, utilitario, etc.)
* **Hechos_Siniestros (Tabla de Hechos)**:
  * `ID_Siniestro` (Clave única)
  * `Gravedad_Lesion` (Leve, grave, fatal)
  * `Cantidad_Victimas` (Métrica de conteo)

*Designed and developed by DeniseGz © 2026*
