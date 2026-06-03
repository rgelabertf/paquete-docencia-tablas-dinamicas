# Secuencias de Aprendizaje — Bioestadística Aplicada con Excel

**UA:** Bioestadística
**Docente:** Dr. Rolando Gelabert Fernández
**Semestre:** Segundo Semestre — Febrero-Junio 2026
**Carrera:** Biología Marina
**Modalidad:** Presencial
**Horas totales:** 48 horas (16 horas por secuencia)
**Elaborado para:** Paquete para la Docencia — ESDEPED Indicador 1.2.3
**Formato base:** FormatoPlaneacion_BioestadisticavS1/S2/S3.pdf — Contenidos institucionales de la UA

> **Nota metodológica:** Las tablas dinámicas se utilizan como herramienta transversal de análisis bioestadístico. Cada secuencia parte de un conjunto de datos pesqueros (`datos capturas 2005 2022.xlsx`) y aplica las técnicas de Excel correspondientes. **Los filtros (autofiltros, avanzados, por selección) se enseñan y practican antes de introducir las tablas dinámicas.**

---

## Secuencia de Aprendizaje 1 — Bioestadística vS1

### Datos de identificación

| Campo | Valor |
|-------|-------|
| UA | Bioestadística |
| Sesión | vS1 |
| Unidad temática | Estadística Descriptiva: ETL, Power Query, Filtros y Tablas Dinámicas |
| Duración | 16 horas (5 sesiones de 3 h + 1 h de cierre) |
| Semestre | 2026-1 |
| Docente | Dr. Rolando Gelabert Fernández |
| Contenido institucional | `FormatoPlaneacion_BioestadisticavS1.pdf` |

### Competencia específica

Aplica procesos ETL (Extraer, Transformar, Cargar) utilizando Power Query para limpiar y normalizar datos de capturas pesqueras; utiliza autofiltros y filtros avanzados para explorar y segmentar la información; construye tablas dinámicas básicas para resumir variables como peso desembarcado, valor en pesos, captura por especie y litoral, sentando las bases del análisis bioestadístico descriptivo.

### Momento de apertura (3 horas)

| Elemento | Descripción |
|----------|-------------|
| **Actividad de encuadre** | Presentación del programa de la UA, competencias, criterios de evaluación basados en los 3 formatos institucionales PDF (vS1/vS2/vS3), y cronograma. |
| **Evaluación diagnóstica** | Cuestionario: conocimientos previos de Excel (rangos, tablas, formato), estadística descriptiva básica (media, frecuencia, porcentaje), familiaridad con datos biológicos. |
| **Estrategia** | Discusión guiada: "Con 500+ registros de capturas pesqueras, ¿cómo encontrarías la especie más capturada sin escribir fórmulas una por una?" |
| **Materiales** | Cuestionario impreso, proyector, presentación de encuadre, `FormatoPlaneacion_BioestadisticavS1.pdf`. |
| **Tiempo** | 3 horas (1 sesión) |

### Momento de desarrollo (11 horas)

| Elemento | Descripción |
|----------|-------------|
| **Actividades de enseñanza** | - **ETL conceptual:** Explicación del proceso Extraer-Transformar-Cargar aplicado a datos pesqueros. Fuentes: CSV, bases de datos institucionales, web.<br>- **Power Query:** Demostración de Power Query (Obtener datos → Desde archivo CSV/texto). Eliminar columnas, cambiar tipos, reemplazar valores, dividir columnas, combinar consultas.<br>- **Autofiltros:** Activación (Ctrl+Mayús+L), filtros por valores, por color, búsqueda en filtros.<br>- **Filtros avanzados:** Rango de criterios, condiciones AND/OR, filtrar in situ vs. copiar a otro lugar, extraer registros únicos.<br>- **Tablas dinámicas:** Concepto, preparación de datos (Tabla de Excel con Ctrl+T), inserción (Alt+N+V), asignación a las 4 áreas con datos de capturas, funciones de agregación (suma, conteo, promedio). |
| **Actividades de aprendizaje** | - **Ejercicio 1 — ETL con Power Query:** Cargar `datos capturas 2005 2022.xlsx` en Power Query. Eliminar columnas irrelevantes, cambiar tipos de datos (año como entero, peso como decimal), reemplazar valores nulos con 0. Cargar a hoja de Excel.<br>- **Ejercicio 2 — Autofiltros:** Aplicar autofiltros para responder: ¿cuántos registros hay del litoral "Golfo de México"?, ¿cuál es la especie con mayor peso desembarcado en 2020?<br>- **Ejercicio 3 — Filtros avanzados:** Crear rango de criterios para filtrar especies con peso > 1000 kg Y origen "captura". Extraer los resultados a otra hoja.<br>- **Ejercicio 4 — Tabla dinámica básica:** Convertir datos limpios en Tabla de Excel. Crear tabla dinámica con Filas = Especie, Valores = Suma de Peso Desembarcado. Ordenar descendente.<br>- **Ejercicio 5 — Tabla dinámica con filtros:** Agregar Filtro = Litoral y Columnas = Año. Analizar cómo cambia la captura por especie a lo largo del tiempo en cada litoral. |
| **Contenido temático** | 1. ETL y Power Query — Extraer, transformar y cargar datos; limpieza, tipos, combinación de consultas<br>2. Filtros en Excel — Autofiltros, filtros avanzados, criterios AND/OR, registros únicos<br>3. Tablas dinámicas — Concepto, preparación, 4 áreas, funciones de agregación |
| **Recursos** | `datos capturas 2005 2022.xlsx`, proyector, computadoras con Excel 2021/365, guía de Power Query, `FormatoPlaneacion_BioestadisticavS1.pdf` |
| **Tiempo** | 11 horas (3 sesiones de 3 h + 1 sesión de 2 h) |

### Momento de cierre (2 horas)

| Elemento | Descripción |
|----------|-------------|
| **Actividad integradora** | Los estudiantes reciben `datos capturas 2005 2022.xlsx` y deben: (1) aplicar Power Query para limpiar y normalizar los datos, (2) usar filtros avanzados para extraer capturas del Pacífico con peso > 500 kg en 2022, (3) crear una tabla dinámica que muestre el peso total desembarcado por especie y por año, con filtro de litoral. |
| **Estrategia de integración** | Socialización: 3 estudiantes proyectan su solución. Discusión grupal sobre decisiones de limpieza y hallazgos en los datos. |
| **Evaluación** | Lista de cotejo (ver instrumentos-evaluacion.md). Ponderación: 30 %. |
| **Tiempo** | 2 horas (sesión final) |

### Evidencias de aprendizaje

| Evidencia | Tipo | Instrumento |
|-----------|------|-------------|
| Cuestionario diagnóstico | Diagnóstica | Clave de respuestas |
| Ejercicios ETL con Power Query | Formativa | Rúbrica |
| Ejercicios de filtros (autofiltros + avanzados) | Formativa | Lista de cotejo |
| Tabla dinámica integradora vS1 | Sumativa | Lista de cotejo |

### Materiales y recursos didácticos

- Computadora con Microsoft Excel 2021 o Microsoft 365
- Proyector y pantalla
- `datos capturas 2005 2022.xlsx`
- `FormatoPlaneacion_BioestadisticavS1.pdf` — guía de contenidos oficial
- Guía de estudio (OVA) — secciones 1 a 4 (ETL, filtros, tablas dinámicas)
- Cuaderno de trabajo — Ejercicios 1 a 4
- Manual de prácticas — Prácticas 1 y 2

### Bibliografía

Gelman, A., et al. (2020). *Regression and Other Stories*. Cambridge University Press.

Microsoft. (s.f.). *Obtener datos con Power Query*. Microsoft Support. https://support.microsoft.com/es-es/office/obtener-datos-con-power-query

McKillup, S. (2012). *Statistics Explained: An Introductory Guide for Life Scientists* (2nd ed.). Cambridge University Press.

Zar, J. H. (2010). *Biostatistical Analysis* (5th ed.). Pearson.

---

## Secuencia de Aprendizaje 2 — Bioestadística vS2

### Datos de identificación

| Campo | Valor |
|-------|-------|
| UA | Bioestadística |
| Sesión | vS2 |
| Unidad temática | Medidas de Tendencia Central y Dispersión con Tablas Dinámicas |
| Duración | 16 horas (5 sesiones de 3 h + 1 h de cierre) |
| Semestre | 2026-1 |
| Docente | Dr. Rolando Gelabert Fernández |
| Contenido institucional | `FormatoPlaneacion_BioestadisticavS2.pdf` |

### Competencia específica

Calcula e interpreta medidas de tendencia central (media, mediana, moda) y de dispersión (rango, varianza, desviación estándar, coeficiente de variación) utilizando tablas dinámicas y funciones estadísticas de Excel sobre datos de capturas pesqueras, para describir y comparar distribuciones de variables biológico-pesqueras como peso desembarcado, valor económico y captura por unidad de esfuerzo.

### Momento de apertura (2 horas)

| Elemento | Descripción |
|----------|-------------|
| **Actividad de inicio** | Repaso: los estudiantes abren su tabla dinámica de vS1. Pregunta detonante: "Del peso desembarcado por especie, ¿cuál es el valor típico? ¿Qué tan dispersos están los datos?" |
| **Evaluación diagnóstica** | Preguntas: ¿Qué es la media aritmética? ¿La mediana? ¿Cómo se calcula la desviación estándar? ¿Qué significa que un conjunto de datos tenga alta varianza? |
| **Estrategia** | Caso motivacional: mostrar datos de captura de dos especies aparentemente similares pero con distribuciones muy diferentes (una estable, otra volátil). ¿Cómo medirlo? |
| **Materiales** | Archivos de vS1, proyector, `FormatoPlaneacion_BioestadisticavS2.pdf` |
| **Tiempo** | 2 horas |

### Momento de desarrollo (11 horas)

| Elemento | Descripción |
|----------|-------------|
| **Actividades de enseñanza** | - **Medidas TC:** Explicación de media, mediana y moda con ejemplos pesqueros. Cuándo usar cada una (media para distribuciones simétricas, mediana para datos con outliers).<br>- **Medidas de dispersión:** Rango, varianza (poblacional y muestral), desviación estándar, coeficiente de variación. Interpretación biológica: una especie con alta desviación estándar en peso desembarcado sugiere capturas irregulares.<br>- **Tabla dinámica para TC:** Usar Configuración de campo de valor → Promedio para media. Mostrar valores como para comparar proporciones.<br>- **Tabla dinámica para dispersión:** No existe función nativa de desviación estándar en tabla dinámica → usar tabla dinámica como resumen + funciones ESTIMAR (DESVEST, VAR) en celdas auxiliares.<br>- **Comparación entre grupos:** Tabla dinámica con promedios y conteos por especie/litoral/año, complementada con columnas de desviación estándar calculadas. |
| **Actividades de aprendizaje** | - **Ejercicio 1 — Media en tabla dinámica:** Crear tabla dinámica con Filas = Especie, Valores = Promedio de Peso Desembarcado. Interpretar: ¿qué especie tiene el mayor promedio?<br>- **Ejercicio 2 — Mediana:** Usar la función MEDIANA en celdas auxiliares sobre los datos filtrados por la tabla dinámica. Comparar media vs. mediana por especie. Identificar especies con asimetría.<br>- **Ejercicio 3 — Desviación estándar:** Agregar columna DESVEST (desviación estándar muestral) a los resúmenes por especie. Identificar la especie con captura más estable (menor desviación).<br>- **Ejercicio 4 — Coeficiente de variación:** Calcular CV = (DESVEST / MEDIA) * 100. ¿Qué especie tiene mayor variabilidad relativa?<br>- **Ejercicio 5 — Comparación por litoral:** Tabla dinámica con Filas = Litoral, Valores = Promedio de peso y Desviación estándar (calculada). Comparar la variabilidad entre litorales. |
| **Contenido temático** | 4. Medidas de tendencia central — Media, mediana, moda; cuándo usar cada una<br>5. Medidas de dispersión — Rango, varianza, desviación estándar, coeficiente de variación<br>6. Aplicación en Excel — Tablas dinámicas para promedios, funciones estadísticas auxiliares (MEDIANA, DESVEST, VAR) |
| **Recursos** | `datos capturas 2005 2022.xlsx`, `FormatoPlaneacion_BioestadisticavS2.pdf`, guía de funciones estadísticas de Excel |
| **Tiempo** | 11 horas |

### Momento de cierre (3 horas)

| Elemento | Descripción |
|----------|-------------|
| **Actividad integradora** | Con `datos capturas 2005 2022.xlsx`, el estudiante debe: (1) crear tabla dinámica con promedio de peso desembarcado por especie y por año, (2) calcular en celdas auxiliares la desviación estándar y coeficiente de variación para cada especie, (3) identificar la especie más estable y la más variable, (4) responder: ¿la media es representativa para todas las especies? ¿Dónde convendría usar la mediana? |
| **Estrategia de integración** | Retroalimentación entre pares: intercambiar archivos, verificar cálculos, discutir interpretaciones. |
| **Evaluación** | Rúbrica de análisis estadístico (ver instrumentos-evaluacion.md). Ponderación: 35 %. |
| **Tiempo** | 3 horas |

### Evidencias de aprendizaje

| Evidencia | Tipo | Instrumento |
|-----------|------|-------------|
| Ejercicios de media y mediana en tabla dinámica | Formativa | Lista de cotejo |
| Ejercicios de desviación estándar y CV | Formativa | Rúbrica |
| Análisis integrador vS2 | Sumativa | Rúbrica |

### Materiales y recursos didácticos

- Computadora con Excel 2021/365
- `datos capturas 2005 2022.xlsx`
- `FormatoPlaneacion_BioestadisticavS2.pdf`
- Cuaderno de trabajo — Ejercicios 5 a 7
- Manual de prácticas — Práctica 3
- Guía de estudio — sección 5 (medidas TC y dispersión)

### Bibliografía

Gelman, A., et al. (2020). *Regression and Other Stories*. Cambridge University Press.

McKillup, S. (2012). *Statistics Explained: An Introductory Guide for Life Scientists* (2nd ed.). Cambridge University Press.

Zar, J. H. (2010). *Biostatistical Analysis* (5th ed.). Pearson.

Microsoft. (s.f.). *Funciones estadísticas de Excel*. Microsoft Support.

---

## Secuencia de Aprendizaje 3 — Bioestadística vS3

### Datos de identificación

| Campo | Valor |
|-------|-------|
| UA | Bioestadística |
| Sesión | vS3 |
| Unidad temática | Distribuciones de Frecuencia, Histogramas y Análisis de Pareto con Tablas Dinámicas |
| Duración | 16 horas (5 sesiones de 3 h + 1 h de cierre) |
| Semestre | 2026-1 |
| Docente | Dr. Rolando Gelabert Fernández |
| Contenido institucional | `FormatoPlaneacion_BioestadisticavS3.pdf` |

### Competencia específica

Construye e interpreta distribuciones de frecuencia (absoluta, relativa, acumulada) para variables cuantitativas discretas y continuas; elabora histogramas y diagramas de Pareto utilizando tablas dinámicas y gráficos dinámicos; aplica estos análisis a datos pesqueros para identificar patrones de captura, especies prioritarias y tendencias temporales que fundamenten decisiones de manejo.

### Momento de apertura (2 horas)

| Elemento | Descripción |
|----------|-------------|
| **Actividad de inicio** | Repaso de vS2: ¿cómo describir numéricamente los datos de captura? Ahora preguntamos: ¿cómo se distribuyen? ¿Cuántas especies aportan la mayor parte del volumen? |
| **Evaluación diagnóstica** | Preguntas: ¿Qué es una distribución de frecuencia? ¿Cómo se construye un histograma? ¿Qué es el principio de Pareto (80/20)? |
| **Estrategia** | Presentar el principio de Pareto aplicado a pesquerías: "el 20 % de las especies genera el 80 % de la captura". ¿Será cierto para nuestros datos? |
| **Materiales** | Archivos de vS2, proyector, `FormatoPlaneacion_BioestadisticavS3.pdf` |
| **Tiempo** | 2 horas |

### Momento de desarrollo (11 horas)

| Elemento | Descripción |
|----------|-------------|
| **Actividades de enseñanza** | - **Distribuciones de frecuencia:** Tabla dinámica para obtener frecuencia absoluta (conteo) y frecuencia relativa (% del total). Frecuencia acumulada con Mostrar valores como → Total acumulado.<br>- **Histogramas con tablas dinámicas:** Agrupar datos numéricos (peso desembarcado) en rangos usando agrupación automática de tablas dinámicas (clic derecho → Agrupar). Definir intervalos (límite inicial, tamaño, límite final). Crear gráfico de columnas → histograma.<br>- **Diagrama de Pareto:** Ordenar tabla dinámica descendente por frecuencia. Calcular % individual y % acumulado. Gráfico combinado: columnas para frecuencia individual, línea para % acumulado. Identificar el punto donde se alcanza el 80 %.<br>- **Análisis de biodiversidad de captura:** Usar tabla dinámica para calcular índices simples: riqueza de especies (conteo de especies distintas por año/litoral), uniformidad (distribución de captura entre especies). |
| **Actividades de aprendizaje** | - **Ejercicio 1 — Frecuencia de captura por especie:** Tabla dinámica: Filas = Especie, Valores = Conteo de registros y % del total. ¿Cuáles son las 5 especies más frecuentes?<br>- **Ejercicio 2 — Histograma de peso desembarcado:** Agrupar Peso Desembarcado en intervalos de 500 kg. Crear gráfico de columnas. Interpretar la forma de la distribución (¿simétrica? ¿sesgada?).<br>- **Ejercicio 3 — Histograma por litoral:** Repetir con filtro de litoral. Comparar las distribuciones: ¿el Golfo de México tiene capturas más homogéneas que el Pacífico?<br>- **Ejercicio 4 — Diagrama de Pareto por especie:** Tabla dinámica con especies ordenadas por peso total descendente. Calcular % del total y % acumulado. Crear gráfico combinado. Identificar cuántas especies acumulan el 80 % del peso.<br>- **Ejercicio 5 — Evolución temporal:** Tabla dinámica: Filas = Año, Valores = Conteo de especies distintas (configurar campo para contar valores únicos si es posible, o usar tabla dinámica + función CONTAR.SI). ¿La riqueza de especies capturadas aumenta o disminuye? |
| **Contenido temático** | 7. Distribuciones de frecuencia — Absoluta, relativa, acumulada; agrupación en intervalos<br>8. Histogramas — Construcción con tablas dinámicas, interpretación de formas (simetría, asimetría, multimodalidad)<br>9. Diagrama de Pareto — Principio 80/20, aplicación a pesquerías, gráfico combinado |
| **Recursos** | `datos capturas 2005 2022.xlsx`, `FormatoPlaneacion_BioestadisticavS3.pdf`, guía de gráficos dinámicos |
| **Tiempo** | 11 horas |

### Momento de cierre (3 horas)

| Elemento | Descripción |
|----------|-------------|
| **Actividad integradora** | Proyecto final de secuencia: Con `datos capturas 2005 2022.xlsx`, el estudiante debe entregar un archivo .xlsx con: (1) tabla dinámica de frecuencia absoluta y relativa de captura por especie, (2) histograma de peso desembarcado con intervalos de 500 kg, (3) diagrama de Pareto de peso total por especie (identificar cuántas especies representan el 80 %), (4) hoja de conclusiones con al menos 3 hallazgos: ¿Hay concentración de captura en pocas especies? ¿La distribución del peso es simétrica? ¿Varía por litoral? |
| **Estrategia de integración** | Presentación breve (3 min): cada estudiante muestra su Pareto y explica el hallazgo más relevante. |
| **Evaluación** | Rúbrica de análisis de distribuciones (ver instrumentos-evaluacion.md). Ponderación: 35 %. |
| **Tiempo** | 3 horas |

### Evidencias de aprendizaje

| Evidencia | Tipo | Instrumento |
|-----------|------|-------------|
| Ejercicios de frecuencia y agrupación | Formativa | Lista de cotejo |
| Histogramas y diagramas de Pareto | Formativa | Rúbrica |
| Proyecto integrador vS3 | Sumativa | Rúbrica |

### Materiales y recursos didácticos

- Computadora con Excel 2021/365
- `datos capturas 2005 2022.xlsx`
- `FormatoPlaneacion_BioestadisticavS3.pdf`
- Cuaderno de trabajo — Ejercicios 8 a 10
- Manual de prácticas — Prácticas 4 a 6
- Guía de estudio — secciones 6 a 8 (histogramas, Pareto, dashboard)
- Acceso a NotebookLM: https://notebooklm.google.com/notebook/4998a49c-e05e-4258-8f06-9fef719f55e1

### Bibliografía

Gelman, A., et al. (2020). *Regression and Other Stories*. Cambridge University Press.

McKillup, S. (2012). *Statistics Explained: An Introductory Guide for Life Scientists* (2nd ed.). Cambridge University Press.

Zar, J. H. (2010). *Biostatistical Analysis* (5th ed.). Pearson.

Microsoft. (s.f.). *Crear un histograma en Excel*. Microsoft Support.

Excel Total. (2021). *Diagrama de Pareto en Excel*. https://exceltotal.com/diagrama-de-pareto-en-excel

---

## Resumen de evaluación

| Secuencia | Unidad | Evidencia principal | Ponderación |
|-----------|--------|---------------------|-------------|
| vS1 | ETL, Power Query, filtros, tablas dinámicas básicas | Tabla dinámica con datos de capturas | 30 % |
| vS2 | Medidas de tendencia central y dispersión | Análisis estadístico con tabla dinámica + funciones auxiliares | 35 % |
| vS3 | Distribuciones de frecuencia, histogramas, Pareto | Proyecto integrador con Pareto e histogramas | 35 % |
| | **Total** | | **100 %** |

---

*Documento elaborado para el Paquete para la Docencia — ESDEPED Indicador 1.2.3*
*Universidad Autónoma del Carmen — Junio 2026*
