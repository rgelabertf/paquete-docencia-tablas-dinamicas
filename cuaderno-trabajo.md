# Cuaderno de Trabajo

## Bioestadística — Herramientas de Análisis de Datos con Excel

---

### Portada

```
╔══════════════════════════════════════════════════════════════════╗
║              UNIVERSIDAD AUTÓNOMA DEL CARMEN                     ║
║           DIRECCIÓN GENERAL DE DOCENCIA Y FORMACIÓN              ║
║                    PROFESIONAL INTEGRAL                          ║
║                                                                  ║
║                    CUADERNO DE TRABAJO                           ║
║                                                                  ║
║              Bioestadística                                      ║
║      Herramientas de Análisis de Datos con Excel                ║
║                                                                  ║
║   Programa Educativo: Biología Marina                            ║
║                                                                  ║
║   Autores:                                                       ║
║   • Dr. Rolando Gelabert Fernández                               ║
║   • Dr. Juan Carlos Pérez López                                  ║
║   • Mtra. Ana María Sánchez Ruiz                                 ║
║   • Ing. Luis Alberto Domínguez Hernández                        ║
║                                                                  ║
║                                                                  ║
║   Periodo: Febrero - Junio 2026                                  ║
║                                                                  ║
║   Cd. del Carmen, Campeche, México                               ║
╚══════════════════════════════════════════════════════════════════╝
```

---

### Índice

| Sección | Contenido | Pág. |
|---------|-----------|------|
| **1** | Introducción | 3 |
| **2** | Ejercicios de Autoaprendizaje | 4 |
| 2.1 | Ejercicio 1: Autofiltros básicos | 4 |
| 2.2 | Ejercicio 2: Filtros avanzados (AND/OR) | 6 |
| 2.3 | Ejercicio 3: Filtros por selección y formato condicional | 8 |
| 2.4 | Ejercicio 4: Power Query / ETL — Limpieza de datos pesqueros | 10 |
| 2.5 | Ejercicio 5: Tabla dinámica — Peso desembarcado por especie y año | 13 |
| 2.6 | Ejercicio 6: Tabla dinámica — Peso vivo por litoral y entidad | 15 |
| 2.7 | Ejercicio 7: Tabla dinámica — Valor en pesos por especie, origen y mes | 17 |
| 2.8 | Ejercicio 8: Agrupación de datos y campos calculados | 19 |
| 2.9 | Ejercicio 9: Mostrar valores como (% del total, diferencias, rankings) | 21 |
| 2.10 | Ejercicio 10: Proyecto integrador — Dashboard de capturas pesqueras | 23 |
| **3** | Clave de Respuestas | 26 |
| **4** | Fuentes de Información y Bibliografía | 30 |

---

## 1. Introducción

El presente Cuaderno de Trabajo ha sido diseñado como un recurso didáctico para la Unidad de Aprendizaje **Bioestadística**, dirigido a estudiantes del Programa Educativo de **Biología Marina** de la Universidad Autónoma del Carmen (UNACAR). Su propósito es desarrollar competencias en el análisis de datos biológicos y pesqueros mediante herramientas computacionales de Excel.

La Bioestadística proporciona los fundamentos teóricos y metodológicos para la recolección, organización, análisis e interpretación de datos en ciencias marinas. Dentro de este marco, las **tablas dinámicas (PivotTables)** constituyen una herramienta transversal de gran valor: permiten resumir, explorar y visualizar grandes volúmenes de datos de forma interactiva, sin necesidad de escribir fórmulas complejas. Su dominio es esencial para el análisis de capturas pesqueras, monitoreo de poblaciones, evaluación de temporadas de veda, distribución espacial de especies y cualquier escenario donde se requiera tomar decisiones basadas en evidencia cuantitativa.

Este cuaderno contiene **10 ejercicios prácticos progresivos** organizados en cuatro etapas: (1) filtros en Excel como preparación para el análisis, (2) limpieza y transformación de datos con Power Query, (3) tablas dinámicas básicas sobre datos de capturas pesqueras, y (4) tablas dinámicas avanzadas con campos calculados, porcentajes y dashboards. Cada ejercicio incluye título, objetivo, saberes a reforzar, estrategia metodológica, lecturas sugeridas y actividades con espacios para registrar resultados. Todos los datos de ejemplo provienen del contexto marino-pesquero del Golfo de México, el Pacífico y el Caribe mexicano.

Se espera que el estudiante desarrolle cada ejercicio de forma autónoma, registre sus respuestas y conclusiones, y al finalizar consulte la clave de respuestas para verificar su aprendizaje.

---

## 2. Ejercicios de Autoaprendizaje

---

### Ejercicio 1: Autofiltros básicos

**Nivel:** Básico

**Objetivo:** El estudiante aplicará autofiltros en Excel para explorar y segmentar datos de capturas pesqueras por año, litoral y entidad federativa, identificando patrones básicos en los registros.

**Saberes a reforzar:**
- Concepto de filtro de datos
- Autofiltro de Excel (ficha Datos)
- Filtrado por valores numéricos y texto
- Limpieza de filtros

**Estrategia metodológica:** Aprendizaje guiado paso a paso. El estudiante trabajará con una tabla de capturas pesqueras y aplicará filtros para responder preguntas específicas.

**Lecturas sugeridas:**
- Microsoft Support. (s.f.). *Aplicar filtros en Excel*. https://support.microsoft.com/es-es/office/aplicar-filtros-en-excel
- CONAPESCA. (2025). *Anuario estadístico de pesca y acuacultura*. https://www.gob.mx/conapesca

---

**Caso: Capturas pesqueras del litoral mexicano (año 2022)**

| Año | Litoral | Entidad | Puerto | Especie | Origen | Peso_Desembarcado_kg | Peso_Vivo_kg | Valor_Pesos |
|-----|---------|---------|--------|---------|--------|---------------------|--------------|-------------|
| 2022 | Golfo de México | Campeche | Ciudad del Carmen | Camarón blanco | Captura | 125,000 | 135,000 | $18,750,000 |
| 2022 | Golfo de México | Campeche | Champotón | Mero rojo | Captura | 45,000 | 48,000 | $9,000,000 |
| 2022 | Golfo de México | Tabasco | Frontera | Ostión | Captura | 80,000 | 85,000 | $4,800,000 |
| 2022 | Golfo de México | Veracruz | Alvarado | Pargo rojo | Captura | 30,000 | 32,000 | $6,000,000 |
| 2022 | Pacífico | Sinaloa | Mazatlán | Camarón café | Captura | 200,000 | 215,000 | $30,000,000 |
| 2022 | Pacífico | Sonora | Guaymas | Sardina | Captura | 350,000 | 370,000 | $7,000,000 |
| 2022 | Pacífico | Nayarit | San Blas | Huachinango | Captura | 28,000 | 30,000 | $5,600,000 |
| 2022 | Caribe | Quintana Roo | Chetumal | Langosta espinosa | Captura | 15,000 | 16,500 | $6,750,000 |
| 2022 | Caribe | Quintana Roo | Isla Mujeres | Pulpo maya | Captura | 22,000 | 24,000 | $7,920,000 |
| 2022 | Golfo de México | Campeche | Sabancuy | Jaiba | Captura | 18,000 | 19,500 | $1,800,000 |

**Instrucciones:**

1. Abre una hoja de cálculo en Excel y copia los datos anteriores en el rango A1:J11. Asegúrate de que la primera fila contenga los encabezados.
2. Selecciona cualquier celda dentro de los datos.
3. Ve a **Datos > Filtro** (o presiona Ctrl + Mayús + L).
4. Observa cómo aparecen flechas de despliegue en cada encabezado de columna.
5. Haz clic en la flecha de la columna **Litoral** y selecciona solo "Golfo de México".
6. Haz clic en la flecha de la columna **Año** y selecciona solo "2022".
7. Sin quitar el filtro anterior, haz clic en la flecha de **Especie** y selecciona "Camarón blanco".

---

**Resultado del ejercicio:**

Describe qué registros se muestran después de aplicar los tres filtros simultáneamente:

```
_________________________________________________________________
_________________________________________________________________
```

**Preguntas de reflexión:**

a) ¿Cuántos registros cumplen con la condición Litoral = "Golfo de México" y Especie = "Camarón blanco"?

```
_________________________________________________________________
```

b) ¿Cuál es el peso desembarcado total de las capturas del Pacífico?

```
_________________________________________________________________
```

c) ¿Qué entidad federativa tiene el mayor valor en pesos en la tabla completa?

```
_________________________________________________________________
```

d) ¿Cómo harías para ver solo los registros del Caribe mexicano?

```
_________________________________________________________________
```

e) ¿Qué especie del Golfo de México tiene el mayor peso desembarcado?

```
_________________________________________________________________
```

---

**Autoevaluación:**

| Indicador | Sí | No |
|-----------|----|----|
| Apliqué el autofiltro correctamente | - | - |
| Pude filtrar por una columna específica | - | - |
| Apliqué filtros combinados en varias columnas | - | - |
| Limpié los filtros después del ejercicio | - | - |
| Comprendo la utilidad de los filtros para explorar datos | - | - |

---

### Ejercicio 2: Filtros avanzados (criterios AND/OR)

**Nivel:** Básico

**Objetivo:** El estudiante aplicará filtros avanzados con criterios lógicos AND/OR para extraer subconjuntos específicos de datos de capturas pesqueras.

**Saberes a reforzar:**
- Filtro avanzado (Datos > Avanzadas)
- Área de criterios
- Criterios AND (misma fila)
- Criterios OR (distintas filas)
- Extraer a otra ubicación

**Estrategia metodológica:** Aprendizaje basado en problemas. El estudiante debe extraer subconjuntos de datos que cumplen condiciones múltiples.

**Lecturas sugeridas:**
- Microsoft Support. (s.f.). *Filtrar datos aplicando criterios avanzados*. https://support.microsoft.com/es-es/office/filtrar-datos-aplicando-criterios-avanzados
- Gelabert Fernández, R. (2026). *Conceptos básicos de filtros en Excel* [Material inédito]. UNACAR.

---

**Caso: Captura por especie, litoral y temporada**

| Año | Litoral | Entidad | Especie | Temporada | Meses | Peso_Desembarcado_kg | Valor_Pesos |
|-----|---------|---------|---------|-----------|-------|---------------------|-------------|
| 2020 | Golfo de México | Campeche | Mero rojo | Veda | Ene-Feb | 12,000 | $2,400,000 |
| 2020 | Golfo de México | Campeche | Mero rojo | Libre | Mar-Dic | 55,000 | $11,000,000 |
| 2020 | Pacífico | Sinaloa | Camarón café | Veda | Mar-Jun | 8,000 | $1,200,000 |
| 2020 | Pacífico | Sinaloa | Camarón café | Libre | Jul-Feb | 210,000 | $31,500,000 |
| 2021 | Golfo de México | Campeche | Mero rojo | Veda | Ene-Feb | 10,500 | $2,100,000 |
| 2021 | Golfo de México | Campeche | Mero rojo | Libre | Mar-Dic | 48,000 | $9,600,000 |
| 2021 | Pacífico | Sinaloa | Camarón café | Veda | Mar-Jun | 7,500 | $1,125,000 |
| 2021 | Pacífico | Sinaloa | Camarón café | Libre | Jul-Feb | 195,000 | $29,250,000 |
| 2022 | Golfo de México | Campeche | Mero rojo | Veda | Ene-Feb | 11,000 | $2,200,000 |
| 2022 | Golfo de México | Campeche | Mero rojo | Libre | Mar-Dic | 52,000 | $10,400,000 |
| 2022 | Pacífico | Sinaloa | Camarón café | Veda | Mar-Jun | 8,500 | $1,275,000 |
| 2022 | Pacífico | Sinaloa | Camarón café | Libre | Jul-Feb | 220,000 | $33,000,000 |
| 2022 | Caribe | Quintana Roo | Langosta | Veda | Mar-Jun | 3,000 | $1,350,000 |
| 2022 | Caribe | Quintana Roo | Langosta | Libre | Jul-Feb | 14,000 | $6,300,000 |

**Instrucciones:**

1. Captura los datos en Excel en el rango A1:H15.
2. **Filtro avanzado AND:** En un área de criterios separada (ej. celdas J1:K2), escribe:
   - J1: `Litoral`, J2: `Pacífico`
   - K1: `Temporada`, K2: `Libre`
3. Ve a **Datos > Avanzadas**, selecciona "Filtrar la lista in situ" y define el Rango de criterios como $J$1:$K$2.
4. **Filtro avanzado OR:** En J4:K6, escribe:
   - J4: `Especie`, J5: `Mero rojo`
   - K4: `Especie`, K6: `Langosta`
5. Aplica el filtro avanzado con criterios OR para ver ambas especies.

---

**Resultados:**

**a)** Completa la siguiente tabla con los registros filtrados con criterio AND (Litoral = Pacífico Y Temporada = Libre):

| Año | Entidad | Especie | Peso Desembarcado | Valor |
|-----|---------|---------|-------------------|-------|
| | | | | |
| | | | | |
| | | | | |

**b)** ¿Cuántos registros se obtienen con el filtro OR (Mero rojo O Langosta)?

```
_________________________________________________________________
```

**Preguntas:**

a) ¿Cuál es la diferencia práctica entre poner criterios AND en la misma fila vs. OR en distintas filas?

```
_________________________________________________________________
_________________________________________________________________
```

b) ¿Qué litoral tiene mayor producción en temporada libre?

```
_________________________________________________________________
```

c) ¿Cuánto vale la producción total de langosta en el Caribe en temporada libre?

```
_________________________________________________________________
```

d) Diseña un filtro avanzado que muestre solo las capturas del año 2022 con peso desembarcado mayor a 50,000 kg. ¿Cómo escribirías los criterios?

```
_________________________________________________________________
```

e) ¿Qué especie muestra mayor diferencia entre captura en veda vs. libre?

```
_________________________________________________________________
_________________________________________________________________
```

---

**Conclusiones del estudiante:**

```
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
```

---

### Ejercicio 3: Filtros por selección y formato condicional

**Nivel:** Básico

**Objetivo:** El estudiante utilizará filtros por selección (clic derecho) y filtros por color/formato condicional para identificar visualmente tendencias y valores atípicos en datos de capturas pesqueras.

**Saberes a reforzar:**
- Filtro por selección (clic derecho)
- Filtro por color de celda
- Filtro por color de fuente
- Formato condicional combinado con filtros

**Estrategia metodológica:** Aprendizaje por descubrimiento. El estudiante explorará formas alternativas de filtrar datos basadas en atributos visuales.

**Lecturas sugeridas:**
- Microsoft Support. (s.f.). *Agregar, cambiar o eliminar formato condicional*. https://support.microsoft.com/es-es/office/agregar-cambiar-o-eliminar-formato-condicional
- Ninja Excel. (2024). *Filtros y formato condicional en Excel*. https://www.ninjaexcel.com

---

**Caso: Rendimiento pesquero por puerto (2022)**

| Puerto | Litoral | Entidad | Especie_Principal | Captura_Total_kg | Valor_Total | Embarcaciones | Días_de_Pesca |
|--------|---------|---------|-------------------|-----------------|-------------|--------------|---------------|
| Ciudad del Carmen | Golfo de México | Campeche | Camarón blanco | 125,000 | $18,750,000 | 120 | 180 |
| Champotón | Golfo de México | Campeche | Mero rojo | 48,000 | $9,600,000 | 45 | 150 |
| Sabancuy | Golfo de México | Campeche | Jaiba | 19,500 | $1,800,000 | 30 | 120 |
| Frontera | Golfo de México | Tabasco | Ostión | 85,000 | $4,800,000 | 60 | 200 |
| Alvarado | Golfo de México | Veracruz | Pargo rojo | 32,000 | $6,000,000 | 40 | 160 |
| Mazatlán | Pacífico | Sinaloa | Camarón café | 215,000 | $30,000,000 | 200 | 220 |
| Guaymas | Pacífico | Sonora | Sardina | 370,000 | $7,000,000 | 80 | 180 |
| San Blas | Pacífico | Nayarit | Huachinango | 30,000 | $5,600,000 | 35 | 140 |
| Chetumal | Caribe | Quintana Roo | Langosta espinosa | 16,500 | $6,750,000 | 25 | 100 |
| Isla Mujeres | Caribe | Quintana Roo | Pulpo maya | 24,000 | $7,920,000 | 40 | 130 |
| Progreso | Golfo de México | Yucatán | Pulpo maya | 55,000 | $18,150,000 | 90 | 170 |
| Lázaro Cárdenas | Pacífico | Michoacán | Sardina | 120,000 | $2,400,000 | 35 | 110 |
| Salina Cruz | Pacífico | Oaxaca | Pargo rojo | 18,000 | $3,600,000 | 25 | 90 |
| Tampico | Golfo de México | Tamaulipas | Camarón blanco | 65,000 | $9,750,000 | 55 | 160 |

**Instrucciones:**

1. Captura los datos en Excel.
2. Aplica **Formato Condicional** > **Barras de datos** a la columna "Captura_Total_kg" para visualizar la magnitud relativa de cada puerto.
3. Aplica **Formato Condicional** > **Escalas de color** (verde-amarillo-rojo) a la columna "Valor_Total".
4. Ahora haz clic derecho sobre una celda con un valor alto en Captura_Total_kg y selecciona **Filtrar > Filtrar por valor de celda seleccionada**.
5. Aplica un **Filtro por color** usando la flecha de autofiltro en la columna "Valor_Total": selecciona "Filtrar por color de celda" y elige el color verde (valores altos).

---

**Resultados:**

**Tabla 1 - Puertos con mayor captura (aplica filtro por selección sobre un valor alto):**

| Puerto | Captura Total | Valor Total |
|--------|---------------|-------------|
| | | |
| | | |
| | | |

**Tabla 2 - Puertos con valor más alto (filtro por color verde en Valor_Total):**

| Puerto | Valor Total |
|--------|-------------|
| | |
| | |
| | |

**Preguntas:**

a) ¿Cuántos puertos del Golfo de México tienen capturas superiores a 50,000 kg?

```
_________________________________________________________________
```

b) ¿Qué puerto del Pacífico tiene el mayor valor en pesos?

```
_________________________________________________________________
```

c) ¿Cuál es la relación visual entre captura total y valor total? ¿Todos los puertos con alta captura tienen alto valor?

```
_________________________________________________________________
_________________________________________________________________
```

d) ¿Qué puerto tiene el mayor valor por kg capturado? (Pista: divide Valor_Total / Captura_Total_kg en una columna adicional)

```
_________________________________________________________________
```

e) ¿Cómo ayudan las barras de datos a identificar rápidamente los puertos más productivos?

```
_________________________________________________________________
_________________________________________________________________
```

---

**Reflexión del estudiante:**

```
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
```

---

### Ejercicio 4: Power Query / ETL — Limpieza de datos pesqueros

**Nivel:** Intermedio

**Objetivo:** El estudiante aplicará técnicas de Extracción, Transformación y Carga (ETL) mediante Power Query de Excel para limpiar, normalizar y preparar un dataset de capturas pesqueras para su análisis posterior con tablas dinámicas.

**Saberes a reforzar:**
- Concepto de proceso ETL
- Power Query (Obtener y transformar datos)
- Eliminación de duplicados y filas vacías
- División y combinación de columnas
- Cambio de tipos de datos
- Reemplazo de valores y eliminación de errores

**Estrategia metodológica:** Aprendizaje basado en problemas reales. El estudiante recibe un archivo con datos simulados que contiene inconsistencias, valores nulos, formatos mixtos y errores típicos de bases de datos pesqueras. Deberá aplicar Power Query para normalizarlo.

**Lecturas sugeridas:**
- Microsoft Support. (s.f.). *Introducción a Power Query*. https://support.microsoft.com/es-es/office/introducción-a-power-query
- Gelabert Fernández, R. (2026). *Limpieza de datos con Power Query* [Material inédito]. UNACAR.

---

**Caso: Normalización del dataset "datos capturas 2005 2022"**

El docente proporcionará un archivo de datos simulado (ej. **"datos capturas 2005 2022.xlsx"** con más de 500 registros, años, litoral, entidad, mes, especie, origen, peso desembarcado, peso vivo, valor en pesos, entre otras). Puede ser otro archivo que necesite normalizar mediante técnicas de limpieza de datos (ETL) y con el uso de Power Query.

**Estructura esperada del dataset después de la limpieza:**

| Columna | Tipo | Descripción |
|---------|------|-------------|
| Año | Número (entero) | 2005 a 2022 |
| Litoral | Texto | Golfo de México, Pacífico, Caribe |
| Entidad | Texto | Campeche, Yucatán, Sinaloa, etc. |
| Puerto | Texto | Ciudad del Carmen, Mazatlán, etc. |
| Mes | Texto | Enero, Febrero, ..., Diciembre |
| Especie | Texto | Camarón blanco, Mero rojo, etc. |
| Origen | Texto | Captura o Acuacultura |
| Peso_Desembarcado_kg | Número | Peso en kilogramos |
| Peso_Vivo_kg | Número | Peso vivo en kilogramos |
| Valor_Pesos | Número | Valor en pesos mexicanos |

**Instrucciones:**

1. Abre el archivo **"datos capturas 2005 2022.xlsx"** proporcionado por el docente.
2. Selecciona cualquier celda dentro de los datos y ve a **Datos > Desde tabla/rango** (o **Datos > Obtener y transformar datos > Desde tabla/rango**). Si Excel lo solicita, confirma que los datos tienen encabezados.
3. Se abrirá el Editor de Power Query. Aplica las siguientes transformaciones en orden:

   a) **Eliminar filas innecesarias:** En la pestaña Inicio, usa **Quitar filas > Quitar filas superiores** si hay filas de encabezado repetido o títulos. Usa **Quitar filas en blanco** para eliminar filas vacías.

   b) **Promover encabezados:** Si la primera fila contiene los nombres de columna, usa **Inicio > Usar la primera fila como encabezados**.

   c) **Cambiar tipo de datos:** Asegúrate de que cada columna tenga el tipo correcto:
      - Año → Número entero
      - Mes → Texto
      - Peso_Desembarcado_kg → Número decimal
      - Valor_Pesos → Número decimal
      Para cambiarlo, haz clic en el ícono de tipo junto al nombre de la columna.

   d) **Reemplazar valores:** Si hay celdas con texto inconsistente (ej. "N/A", "-", "Sin dato"), selecciona la columna y usa **Inicio > Reemplazar valores** para sustituirlos por valores nulos o por ceros según corresponda.

   e) **Dividir columnas:** Si alguna columna combina información (ej. "Especie - Origen"), selecciona la columna y ve a **Transformar > Dividir columna > Por delimitador** y elige el guion (-).

   f) **Eliminar duplicados:** Si hay registros repetidos, selecciona todas las columnas y usa **Inicio > Quitar filas > Quitar duplicados**.

   g) **Filtrar errores:** Haz clic en el ícono de filtro de cada columna y desmarca cualquier valor que sea claramente un error (ej. valores negativos en peso, texto donde debería haber número).

4. Una vez que los datos estén limpios, ve a **Inicio > Cerrar y cargar > Cerrar y cargar en...** y selecciona "Nueva hoja de cálculo".

---

**Resultado del ejercicio:**

Describe las transformaciones que aplicaste y cuántos registros tenía el dataset original vs. después de la limpieza:

```
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
```

**Preguntas de reflexión:**

a) ¿Qué tipo de inconsistencias encontraste en el dataset original?

```
_________________________________________________________________
_________________________________________________________________
```

b) ¿Cuántos registros duplicados eliminaste?

```
_________________________________________________________________
```

c) ¿Qué columnas requirieron cambio de tipo de dato?

```
_________________________________________________________________
```

d) ¿Por qué es importante normalizar los datos antes de crear tablas dinámicas?

```
_________________________________________________________________
_________________________________________________________________
```

e) ¿Qué ventajas tiene Power Query frente a hacer la limpieza manualmente?

```
_________________________________________________________________
_________________________________________________________________
```

---

**Autoevaluación:**

| Indicador | Sí | No |
|-----------|----|----|
| Abrí correctamente el archivo en Power Query | - | - |
| Eliminé filas vacías y duplicados | - | - |
| Cambié los tipos de datos según correspondía | - | - |
| Reemplacé valores inconsistentes | - | - |
| Cargué los datos limpios a una nueva hoja | - | - |
| Comprendo la utilidad del proceso ETL | - | - |

---

### Ejercicio 5: Tabla dinámica — Peso desembarcado por especie y año

**Nivel:** Básico

**Objetivo:** El estudiante creará su primera tabla dinámica a partir del dataset limpio de capturas pesqueras, analizando el peso desembarcado por especie a través de los años.

**Saberes a reforzar:**
- Creación de tabla dinámica
- Áreas de tabla dinámica (filas, columnas, valores, filtros)
- Agregación de datos con suma
- Ordenamiento en tabla dinámica

**Estrategia metodológica:** Aprendizaje guiado paso a paso. El estudiante aplicará por primera vez una tabla dinámica sobre datos marinos reales.

**Lecturas sugeridas:**
- Microsoft Support. (s.f.). *Crear una tabla dinámica para analizar datos de una hoja de cálculo*. https://support.microsoft.com/es-es/office/crear-una-tabla-dinamica-para-analizar-datos-de-una-hoja-de-calculo-a9a84538-bfe9-40a9-a8e9-f99134456576
- Daxus Latam. (2025). *Aprende a crear tablas dinámicas desde cero* [Video]. YouTube. https://www.youtube.com/watch?v=WGH-k_vURuE

---

**Caso: Dataset de capturas pesqueras (2005-2022) — ya limpio del Ejercicio 4**

Utiliza el dataset ya limpio del ejercicio anterior. Si no completaste el Ejercicio 4, el docente proporcionará una versión limpia del archivo.

**Instrucciones:**

1. Asegúrate de tener los datos limpios en una hoja de Excel.
2. Selecciona cualquier celda dentro de los datos.
3. Ve a **Insertar > Tabla dinámica** (o presiona Alt + N + V).
4. Selecciona "Nueva hoja de cálculo" y haz clic en Aceptar.
5. En el panel de Campos de tabla dinámica, arrastra los campos a las siguientes áreas:
   - **Filas:** Especie
   - **Columnas:** Año
   - **Valores:** Suma de Peso_Desembarcado_kg
6. Ordena las especies de mayor a menor por el total general.
7. Agrega un **Filtro** con el campo "Litoral" y selecciona solo "Golfo de México".

---

**Resultado del ejercicio:**

**Tabla 1 - Peso desembarcado (kg) por especie y año (filtrado: Golfo de México):**

| Especie | Año 2005 | Año 2006 | ... | 2022 | Total General |
|---------|----------|----------|-----|------|--------------|
| | | | | | |
| | | | | | |
| | | | | | |
| **Total General** | | | | | |

*Nota: completa con los datos que arroje tu tabla dinámica.*

**Preguntas de reflexión:**

a) ¿Qué especie tiene el mayor peso desembarcado total en el Golfo de México?

```
_________________________________________________________________
```

b) ¿En qué año se registró el mayor peso desembarcado de la especie líder?

```
_________________________________________________________________
```

c) ¿Cómo cambia el ranking de especies si cambias "Suma" por "Promedio" en los valores?

```
_________________________________________________________________
_________________________________________________________________
```

d) ¿Qué año presenta la mayor captura total en el Golfo de México?

```
_________________________________________________________________
```

e) Si eliminas el filtro de Litoral, ¿cómo se modifica el ranking de especies?

```
_________________________________________________________________
_________________________________________________________________
```

---

**Autoevaluación:**

| Indicador | Sí | No |
|-----------|----|----|
| Creé la tabla dinámica siguiendo los pasos | - | - |
| Identifiqué las cuatro áreas de la tabla dinámica | - | - |
| Pude ordenar las especies de mayor a menor | - | - |
| Apliqué correctamente el filtro de Litoral | - | - |
| Comprendo cómo la tabla dinámica resume los datos | - | - |

---

### Ejercicio 6: Tabla dinámica — Peso vivo por litoral y entidad federativa

**Nivel:** Básico

**Objetivo:** El estudiante analizará el peso vivo de las capturas distribuidas por litoral y entidad federativa, utilizando múltiples campos en una tabla dinámica para identificar las regiones más productivas.

**Saberes a reforzar:**
- Múltiples campos en filas y columnas
- Agrupación jerárquica (Litoral > Entidad)
- Cambio de cálculo entre suma, promedio y conteo
- Interpretación de subtotales y totales

**Estrategia metodológica:** Aprendizaje basado en problemas. El estudiante responde preguntas sobre la distribución geográfica de las capturas.

**Lecturas sugeridas:**
- Excel Total. (2021). *Tablas dinámicas en Excel (tutorial completo)*. https://exceltotal.com/tablas-dinamicas-en-excel
- CONAPESCA. (2025). *Anuario estadístico de pesca y acuacultura*. https://www.gob.mx/conapesca

---

**Caso: Captura por litoral y entidad (2005-2022)**

Utiliza el dataset limpio del Ejercicio 4. Vamos a analizar cómo se distribuye el peso vivo de las capturas geográficamente.

**Instrucciones:**

1. Con los datos limpios visibles, crea una nueva tabla dinámica (**Insertar > Tabla dinámica**).
2. Configura los campos de la siguiente manera:
   - **Filas:** Litoral y luego Entidad (arrastra Litoral primero, luego Entidad debajo)
   - **Valores:** Suma de Peso_Vivo_kg
3. Agrega un segundo campo a **Valores**: Promedio de Peso_Vivo_kg.
4. Agrega un tercer campo a **Valores**: Conteo de Registros (arrastra cualquier campo texto, como Especie, y cambia su cálculo a "Conteo").
5. Expande y contrae los niveles haciendo clic en los signos + y - junto a cada litoral.

---

**Resultados:**

**Tabla 1 - Peso vivo por litoral y entidad:**

| Litoral | Entidad | Suma Peso Vivo (kg) | Promedio Peso Vivo (kg) | Conteo de Registros |
|---------|---------|-------------------|------------------------|---------------------|
| **Golfo de México** | | | | |
| | Campeche | | | |
| | Veracruz | | | |
| | Tabasco | | | |
| | Tamaulipas | | | |
| | Yucatán | | | |
| **Pacífico** | | | | |
| | Sinaloa | | | |
| | Sonora | | | |
| | Nayarit | | | |
| | Michoacán | | | |
| | Oaxaca | | | |
| **Caribe** | | | | |
| | Quintana Roo | | | |
| **Total General** | | | | |

**Preguntas:**

a) ¿Qué litoral tiene el mayor peso vivo total?

```
_________________________________________________________________
```

b) ¿Qué entidad federativa es la más productiva dentro del Golfo de México?

```
_________________________________________________________________
```

c) ¿Qué litoral tiene el mayor promedio de peso vivo por registro?

```
_________________________________________________________________
```

d) ¿Cuántos registros de captura tiene Quintana Roo (Caribe)?

```
_________________________________________________________________
```

e) ¿Qué entidad del Pacífico tiene la menor cantidad de registros?

```
_________________________________________________________________
```

f) ¿Cómo interpretas la diferencia entre "Suma de Peso Vivo" y "Promedio de Peso Vivo" al comparar litorales?

```
_________________________________________________________________
_________________________________________________________________
```

---

**Conclusiones del estudiante:**

```
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
```

---

### Ejercicio 7: Tabla dinámica — Valor en pesos por especie, origen y mes

**Nivel:** Intermedio

**Objetivo:** El estudiante analizará el valor económico de las capturas (en pesos) desglosado por especie, origen (captura vs. acuacultura) y mes, identificando tendencias estacionales y de mercado.

**Saberes a reforzar:**
- Múltiples campos en columnas
- Filtros de informe
- Análisis estacional
- Comparación de origen (captura vs. acuacultura)

**Estrategia metodológica:** Aprendizaje contextualizado. El estudiante analiza datos económicos pesqueros para detectar estacionalidad.

**Lecturas sugeridas:**
- El Tio Tech. (2021). *6 ejercicios de tablas dinámicas para practicar*. https://eltiotech.com/6-ejercicios-tablas-dinamicas
- Gelabert Fernández, R. (2026). *Técnicas avanzadas de tablas dinámicas* [Material inédito]. UNACAR.

---

**Caso: Valor económico por especie, origen y mes**

El dataset de capturas pesqueras contiene información sobre el valor en pesos de cada registro, así como el origen (Captura o Acuacultura). Analizaremos cómo varía el valor económico a lo largo del año.

**Instrucciones:**

1. Crea una nueva tabla dinámica.
2. Configura:
   - **Filas:** Especie
   - **Columnas:** Origen
   - **Valores:** Suma de Valor_Pesos
3. Agrega un **Filtro de informe** con el campo "Mes" para poder seleccionar meses específicos.
4. Crea una segunda tabla dinámica (en la misma hoja o en otra nueva):
   - **Filas:** Mes
   - **Columnas:** Origen
   - **Valores:** Suma de Valor_Pesos
5. En la segunda tabla, ordena los meses cronológicamente (Enero, Febrero, ...).

---

**Resultados:**

**Tabla 1 - Valor en pesos por especie y origen:**

| Especie | Captura | Acuacultura | Total General |
|---------|---------|-------------|--------------|
| Camarón blanco | | | |
| Camarón café | | | |
| Mero rojo | | | |
| Pargo rojo | | | |
| Huachinango | | | |
| Sardina | | | |
| Ostión | | | |
| Pulpo maya | | | |
| Langosta espinosa | | | |
| Jaiba | | | |
| **Total General** | | | |

**Tabla 2 - Valor en pesos por mes y origen:**

| Mes | Captura | Acuacultura | Total General |
|-----|---------|-------------|--------------|
| Enero | | | |
| Febrero | | | |
| Marzo | | | |
| Abril | | | |
| Mayo | | | |
| Junio | | | |
| Julio | | | |
| Agosto | | | |
| Septiembre | | | |
| Octubre | | | |
| Noviembre | | | |
| Diciembre | | | |
| **Total General** | | | |

**Preguntas:**

a) ¿Qué especie genera el mayor valor económico total?

```
_________________________________________________________________
```

b) ¿Qué especie tiene mayor participación de acuacultura frente a captura?

```
_________________________________________________________________
```

c) ¿En qué mes se registra el mayor valor en capturas?

```
_________________________________________________________________
```

d) ¿Existe algún patrón estacional en el valor de las capturas? ¿Qué meses son los más productivos?

```
_________________________________________________________________
_________________________________________________________________
```

e) ¿Qué especie depende casi exclusivamente de la captura (sin acuacultura significativa)?

```
_________________________________________________________________
```

f) Si quisieras ver solo los datos del Camarón blanco, ¿cómo lo harías con el filtro de informe?

```
_________________________________________________________________
```

---

**Reflexión del estudiante:**

```
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
```

---

### Ejercicio 8: Agrupación de datos y campos calculados

**Nivel:** Intermedio-Avanzado

**Objetivo:** El estudiante agrupará datos en intervalos (años, rangos de peso) y creará campos calculados para obtener indicadores derivados como el valor por kilogramo y la relación peso vivo / peso desembarcado.

**Saberes a reforzar:**
- Agrupar campos en tabla dinámica
- Crear grupos personalizados (quinquenios, rangos)
- Insertar campo calculado con fórmulas
- Interpretación de campos derivados

**Estrategia metodológica:** Aprendizaje basado en problemas. El estudiante crea indicadores que no existen en los datos originales.

**Lecturas sugeridas:**
- Microsoft Support. (s.f.). *Crear campos calculados en tabla dinámica*. https://support.microsoft.com/es-es/office/crear-campos-calculados-en-tabla-dinamica
- Caballero, M. & Torres, F. (s.f.). *Tablas dinámicas: la quinta dimensión* (1. ed.). [PDF].

---

**Caso: Análisis de capturas por quinquenios y rendimiento económico**

Trabajaremos con el dataset de capturas para agrupar años en quinquenios y crear indicadores de rendimiento.

**Instrucciones:**

1. Crea una tabla dinámica con:
   - **Filas:** Año
   - **Valores:** Suma de Peso_Desembarcado_kg, Suma de Valor_Pesos
2. Selecciona varios años en la tabla (ej. 2005 a 2009), haz clic derecho y elige **Agrupar**. Nombra el grupo como "2005-2009".
3. Repite para 2010-2014, 2015-2019 y 2020-2022.
4. **Inserta un campo calculado:**
   - Selecciona la tabla dinámica
   - Ve a **Analizar > Campos, elementos y conjuntos > Campo calculado**
   - Crea un campo llamado "Valor_por_kg" con la fórmula: `= Valor_Pesos / Peso_Desembarcado_kg`
   - Establece el formato con el botón "Formato de número" como moneda.
5. Crea un segundo campo calculado llamado "Rendimiento_Vivo" con la fórmula: `= (Peso_Vivo_kg - Peso_Desembarcado_kg) / Peso_Desembarcado_kg * 100`.

---

**Resultados:**

**Tabla 1 - Captura y valor por quinquenio:**

| Quinquenio | Suma Peso_Desembarcado (kg) | Suma Valor_Pesos | Valor Promedio por kg |
|------------|---------------------------|-----------------|----------------------|
| 2005-2009 | | | |
| 2010-2014 | | | |
| 2015-2019 | | | |
| 2020-2022 | | | |
| **Total General** | | | |

**Tabla 2 - Rendimiento peso vivo vs. desembarcado por especie:**

| Especie | Suma Peso_Desembarcado | Suma Peso_Vivo | Rendimiento_Vivo (%) |
|---------|----------------------|---------------|---------------------|
| | | | |
| | | | |
| **Total General** | | | |

**Preguntas:**

a) ¿Qué quinquenio registró el mayor valor total en capturas?

```
_________________________________________________________________
```

b) ¿Qué especie tiene el mayor valor por kilogramo (Valor_por_kg)?

```
_________________________________________________________________
```

c) ¿Qué especie tiene el mayor rendimiento (diferencia entre peso vivo y desembarcado)?

```
_________________________________________________________________
```

d) ¿Cómo ha evolucionado el valor por kg a lo largo de los quinquenios? ¿Ha aumentado o disminuido?

```
_________________________________________________________________
_________________________________________________________________
```

e) ¿Qué utilidad tiene agrupar años en quinquenios para el análisis temporal?

```
_________________________________________________________________
_________________________________________________________________
```

f) Crea un grupo adicional que clasifique las especies en "Alto valor" (Valor_por_kg > $100) y "Bajo valor" (≤ $100). ¿Cuántas especies caen en cada categoría?

```
_________________________________________________________________
_________________________________________________________________
```

---

**Autoevaluación:**

| Indicador | Sí | No |
|-----------|----|----|
| Agrupé correctamente los años en quinquenios | - | - |
| Creé el campo calculado Valor_por_kg | - | - |
| Creé el campo calculado Rendimiento_Vivo | - | - |
| Pude dar formato a los campos calculados | - | - |
| Comprendo cómo los campos calculados amplían el análisis | - | - |

---

### Ejercicio 9: Mostrar valores como (% del total, diferencias, rankings)

**Nivel:** Avanzado

**Objetivo:** El estudiante utilizará las opciones "Mostrar valores como" para calcular porcentajes, diferencias entre periodos, rankings y variaciones en los datos de capturas pesqueras.

**Saberes a reforzar:**
- % del total general
- % del total de fila/columna
- Diferencia respecto a periodo anterior
- % de diferencia
- Ranking (mayor a menor)

**Estrategia metodológica:** Aprendizaje analítico. El estudiante comparará datos entre litorales, años y especies para extraer conclusiones sobre la distribución y evolución de las capturas.

**Lecturas sugeridas:**
- Excel Total. (2021). *Tablas dinámicas en Excel (tutorial completo)*.
- Microsoft Support. (s.f.). *Mostrar valores como en tabla dinámica*. https://support.microsoft.com/es-es/office/mostrar-valores-como-en-tabla-dinamica

---

**Caso: Distribución y evolución de las capturas por litoral y especie**

**Instrucciones:**

1. Crea una tabla dinámica con:
   - **Filas:** Especie
   - **Columnas:** Litoral
   - **Valores:** Suma de Peso_Desembarcado_kg
2. Duplica la tabla (copia y pega) y en la copia, haz clic derecho sobre el campo de valores > **Mostrar valores como > % del total general**.
3. Crea una tercera tabla dinámica con:
   - **Filas:** Especie
   - **Valores:** Suma de Peso_Desembarcado_kg
   - Cambia a **Mostrar valores como > Ranking de mayor a menor**.
4. Crea una cuarta tabla dinámica:
   - **Filas:** Año
   - **Valores:** Suma de Peso_Desembarcado_kg
   - Cambia a **Mostrar valores como > Diferencia respecto al año anterior**.
5. Crea una quinta tabla dinámica (sobre la anterior):
   - Cambia a **Mostrar valores como > % de diferencia respecto al año anterior**.

---

**Resultados:**

**Tabla 1 - % del total general por especie y litoral:**

| Especie | Golfo de México (%) | Pacífico (%) | Caribe (%) | Total (%) |
|---------|--------------------|-------------|-----------|----------|
| | | | | 100% |
| | | | | 100% |
| **Total General** | | | | 100% |

**Tabla 2 - Ranking de especies por peso desembarcado:**

| Posición | Especie | Peso Desembarcado (kg) |
|----------|---------|----------------------|
| 1 | | |
| 2 | | |
| 3 | | |
| 4 | | |
| 5 | | |
| ... | | |

**Tabla 3 - Diferencia anual en peso desembarcado:**

| Año | Peso Desembarcado | Diferencia vs. Año Anterior | % de Diferencia |
|-----|------------------|---------------------------|----------------|
| 2005 | | — (base) | — |
| 2006 | | | |
| 2007 | | | |
| ... | | | |
| 2022 | | | |

**Preguntas:**

a) ¿Qué especie concentra el mayor porcentaje del peso desembarcado total?

```
_________________________________________________________________
```

b) ¿Qué litoral tiene la mayor participación porcentual en el total de capturas?

```
_________________________________________________________________
```

c) ¿Cuál fue el año con mayor crecimiento porcentual respecto al año anterior?

```
_________________________________________________________________
```

d) ¿Hubo años con decrecimiento en las capturas? ¿Cuáles?

```
_________________________________________________________________
```

e) ¿Qué especie ocupa el primer lugar en el ranking? ¿Y el último?

```
_________________________________________________________________
```

f) ¿Cómo cambia la participación porcentual del Pacífico a lo largo de los años?

```
_________________________________________________________________
_________________________________________________________________
```

---

**Reflexión del estudiante:**

```
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
```

---

### Ejercicio 10: Proyecto integrador — Dashboard de capturas pesqueras

**Nivel:** Avanzado

**Objetivo:** El estudiante integrará todos los conocimientos adquiridos para construir un dashboard interactivo completo que incluya tablas dinámicas, gráficos dinámicos, segmentaciones y escalas de tiempo, generando un reporte ejecutivo sobre las capturas pesqueras del dataset 2005-2022.

**Saberes a reforzar:**
- Todas las áreas de tabla dinámica
- Campos calculados
- Segmentaciones (slicers) y escalas de tiempo
- Gráficos dinámicos
- Conexión de segmentaciones a múltiples tablas
- Interpretación de resultados

**Estrategia metodológica:** Aprendizaje basado en proyectos. El estudiante desarrolla un análisis integral simulando un entorno profesional de reporte pesquero.

**Lecturas sugeridas:**
- Todas las lecturas de los ejercicios anteriores.
- SMARTpro Academy. (s.f.). *Cómo hacer tablas dinámicas en Excel + IA desde cero* [Video]. YouTube. https://www.youtube.com/watch?v=Mh93eaKbkkw
- Aprender21. (2026). *Tablas dinámicas en Excel: guía paso a paso*.

---

**Caso: Dashboard ejecutivo de pesca y acuacultura en México (2005-2022)**

Utilizando el dataset completo de capturas, construye un tablero de control que permita visualizar y filtrar la información de manera interactiva.

**Instrucciones — Construye tu dashboard en 4 hojas:**

**Hoja 1 - Resumen General:**

- Tabla dinámica: Filas = Especie, Valores = Suma de Peso_Desembarcado_kg, Suma de Valor_Pesos
- Gráfico dinámico de barras mostrando las 5 especies con mayor peso desembarcado
- Agrega un campo calculado "Participación_%" con la fórmula: `= Peso_Desembarcado_kg / ObtenerDatosDinamicos("Suma de Peso_Desembarcado_kg", $A$1) * 100`

**Hoja 2 - Análisis por Litoral:**

- Tabla dinámica: Filas = Litoral, Columnas = Origen (Captura / Acuacultura), Valores = Suma de Peso_Vivo_kg
- Gráfico dinámico circular que muestre la contribución de cada litoral al total
- Gráfico dinámico de columnas apiladas mostrando captura vs. acuacultura por litoral

**Hoja 3 - Evolución Temporal:**

- Tabla dinámica: Filas = Año, Valores = Suma de Peso_Desembarcado_kg, Suma de Valor_Pesos
- Gráfico dinámico de líneas mostrando la tendencia de captura a lo largo del tiempo (2005-2022)
- Agrega una escala de tiempo (Timeline) conectada a esta tabla

**Hoja 4 - Dashboard consolidado:**

- Agrupa los elementos más importantes de las 3 hojas anteriores en una sola hoja
- Agrega **segmentaciones (slicers)** para los campos:
  - Litoral (Golfo de México, Pacífico, Caribe)
  - Especie
  - Origen (Captura, Acuacultura)
- Conecta CADA segmentación a TODAS las tablas dinámicas del dashboard
- Ajusta el formato: colores profesionales, títulos, alineación

---

**Resultado - Hoja 1: Resumen General**

| Especie | Peso Desembarcado (kg) | Valor Total ($) | Participación % |
|---------|----------------------|----------------|----------------|
| | | | |
| | | | |
| | | | |
| **Total General** | | | 100% |

**Resultado - Hoja 2: Análisis por Litoral**

| Litoral | Captura (kg) | Acuacultura (kg) | Total |
|---------|-------------|-----------------|-------|
| Golfo de México | | | |
| Pacífico | | | |
| Caribe | | | |
| **Total General** | | | |

**Resultado - Hoja 3: Evolución Temporal**

| Año | Peso Desembarcado (kg) | Valor Total ($) |
|-----|----------------------|----------------|
| 2005 | | |
| 2006 | | |
| ... | | |
| 2022 | | |

---

**Conclusiones del proyecto:**

Redacta un análisis ejecutivo respondiendo las siguientes preguntas:

- ¿Cuál es la tendencia general de las capturas pesqueras entre 2005 y 2022?
- ¿Qué especie y litoral son los más productivos?
- ¿Qué proporción de la producción proviene de acuacultura vs. captura?
- ¿Qué especie tiene el mayor valor económico por kilogramo?
- ¿Qué recomendaciones darías para la gestión pesquera con base en los datos?

```
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
_________________________________________________________________
```

---

### Ejercicio 10 (Continuación) — Rúbrica de evaluación del proyecto

| Criterio | Excelente (4 pts) | Bueno (3 pts) | Suficiente (2 pts) | Insuficiente (1 pt) |
|----------|------------------|---------------|-------------------|---------------------|
| Tablas dinámicas | Crea 3+ tablas correctas con múltiples campos | Crea 2 tablas correctas | Crea 1 tabla correcta | No crea tablas funcionales |
| Campos calculados | Crea 1+ campo calculado funcional | Crea campo con errores menores | Intenta crear campo | No crea campos |
| Gráficos dinámicos | 2+ gráficos correctos con formato | 2 gráficos básicos | 1 gráfico | Sin gráficos |
| Segmentaciones | Conectadas a todas las tablas | Conectadas parcialmente | Sin conectar | Sin segmentaciones |
| Análisis escrito | Conclusiones profundas y coherentes | Conclusiones básicas | Conclusiones confusas | Sin conclusiones |

**Calificación obtenida:** ______ / 20 puntos

---

## 3. Clave de Respuestas

---

### Ejercicio 1

a) 1 registro (Campeche, Litoral = Golfo de México, Especie = Camarón blanco).
b) Suma del peso desembarcado del Pacífico: 200,000 (Camarón café) + 350,000 (Sardina) + 28,000 (Huachinango) = 578,000 kg.
c) Mazatlán — Camarón café ($30,000,000).
d) Hacer clic en la flecha de filtro de Litoral y seleccionar solo "Caribe".
e) Camarón blanco con 125,000 kg.

### Ejercicio 2

a) Filtro AND (Pacífico + Libre):
- 2020, Sinaloa, Camarón café, 210,000 kg, $31,500,000
- 2021, Sinaloa, Camarón café, 195,000 kg, $29,250,000
- 2022, Sinaloa, Camarón café, 220,000 kg, $33,000,000

b) 5 registros (Mero rojo: 6 registros de Campeche + Langosta: 2 registros de Quintana Roo, pero el filtro OR muestra ambos). En total 8 registros.

Preguntas:
a) AND (misma fila): ambas condiciones deben cumplirse. OR (distintas filas): basta con que una condición se cumpla.
b) Pacífico (Sinaloa produce más en temporada libre).
c) $6,300,000 (Langosta en Caribe, temporada libre).
d) Criterios: J1: `Año`, J2: `2022`, K1: `Peso_Desembarcado_kg`, K2: `>50000`.
e) Camarón café: produce mucho más en temporada libre que en veda.

### Ejercicio 3

a) 4 puertos: Ciudad del Carmen (125,000), Frontera (85,000), Progreso (55,000), Tampico (65,000).
b) Mazatlán ($30,000,000).
c) No todos: Guaymas tiene alta captura (370,000 kg) pero bajo valor ($7,000,000). El valor depende de la especie, no solo del volumen.
d) Langosta espinosa en Chetumal: $6,750,000 / 16,500 kg ≈ $409/kg (alto valor unitario).
e) Permiten comparar visualmente la magnitud entre filas sin leer los números exactos.

### Ejercicio 4

(Las respuestas variarán según el dataset proporcionado por el docente)
a) Las inconsistencias típicas incluyen: valores nulos o "N/A", formatos mezclados (texto y número en misma columna), filas vacías, encabezados repetidos, errores ortográficos en nombres de especies o entidades, duplicados, valores negativos en peso.
b) Depende del dataset.
c) Típicamente: Año (texto → número), Valor_Pesos (texto → moneda), Peso_Desembarcado_kg (texto → decimal).
d) Las tablas dinámicas requieren datos limpios con estructura uniforme. Datos sucios producen resultados incorrectos o incompletos.
e) Power Query automatiza el proceso, es reproducible, maneja grandes volúmenes y registra cada transformación aplicada.

### Ejercicio 5

(Las respuestas variarán según el dataset)
a) La especie de mayor peso desembarcado en el Golfo de México dependerá del dataset. Típicamente: Camarón blanco o Mero rojo.
b) Depende de los datos. Se debe buscar el año con mayor valor en la fila de la especie líder.
c) El ranking cambia porque el promedio favorece a especies con pocos registros pero de alto volumen individual.
d) El año con mayor captura total se identifica en el Total General de cada columna.
e) Sin filtro, aparecen especies del Pacífico y Caribe que pueden ser más abundantes.

### Ejercicio 6

(Las respuestas variarán según el dataset)
a) Golfo de México (típicamente por mayor número de entidades costeras).
b) Campeche (principal productor pesquero del Golfo de México).
c) Caribe (por tener especies de alto valor por kg, aunque menor volumen total).
d) Depende del número de registros en el dataset para Quintana Roo.
e) Típicamente Oaxaca o Michoacán (menor tradición pesquera).
f) La suma refleja el volumen total, mientras el promedio indica la productividad por registro. Un litoral puede tener mucha suma pero bajo promedio si tiene muchos registros pequeños.

### Ejercicio 7

(Las respuestas variarán según el dataset)
a) Camarón blanco o Camarón café (especies de alto valor comercial).
b) Ostión o Camarón blanco (especies con producción acuícola significativa).
c) Diciembre o noviembre (temporada de mayor demanda).
d) Sí, típicamente hay picos en los meses de diciembre-marzo (cuaresma y fin de año) y valles en verano.
e) Mero rojo, Pargo rojo, Huachinango, Pulpo maya, Langosta (especies exclusivamente de captura).
f) Usar el filtro de informe de Mes; también se puede arrastrar Especie al filtro.

### Ejercicio 8

(Las respuestas variarán según el dataset)
a) Depende de los datos; típicamente el quinquenio más reciente (2020-2022) o el de mayor actividad pesquera.
b) Langosta espinosa o Pulpo maya (especies de alto valor unitario).
c) La especie con mayor diferencia relativa entre peso vivo y desembarcado (típicamente especies que pierden más agua o vísceras).
d) Depende del dataset; puede mostrar tendencia al alza o fluctuaciones.
e) Los quinquenios suavizan la variabilidad anual y permiten ver tendencias de largo plazo.
f) Depende del umbral; típicamente langosta y pulpo maya son "Alto valor".

### Ejercicio 9

(Las respuestas variarán según el dataset)
a) La especie con mayor porcentaje del total (típicamente sardina o camarón por volumen).
b) Golfo de México (por número de entidades y tradición pesquera).
c) El año con mayor incremento porcentual respecto al anterior.
d) Pueden identificarse años con capturas decrecientes (relacionados con veda, fenómenos climáticos, o sobrexplotación).
e) Depende del dataset. Se espera que el ranking muestre las especies ordenadas por volumen.
f) Se espera que el estudiante observe la evolución de la participación del Pacífico a lo largo de los años.

### Ejercicio 10

Las respuestas variarán según los datos generados y la interpretación del estudiante. Se espera que:

- Identifique correctamente la tendencia general de las capturas
- Compare litorales usando las sumas totales
- Calcule la proporción captura vs. acuacultura
- Identifique la especie de mayor valor por kilogramo
- Cree un dashboard funcional con al menos 3 tablas dinámicas
- Conecte las segmentaciones a todas las tablas
- Incluya gráficos dinámicos de tipo barra, circular y línea
- Redacte conclusiones coherentes basadas en los datos analizados
- Proponga recomendaciones viables para la gestión pesquera

**Rúbrica:** El estudiante debe obtener mínimo 12/20 puntos para considerar el proyecto integrador aprobado.

---

## 4. Fuentes de Información y Bibliografía

### Bibliografía básica

Caballero, M. & Torres, F. (s.f.). *Tablas dinámicas: la quinta dimensión* (1. ed.). [Documento PDF]. Incluido en el Paquete para la Docencia.

Gelabert Fernández, R. (2026). *Material didáctico de Bioestadística: filtros, Power Query y tablas dinámicas para datos pesqueros* [Material inédito]. Universidad Autónoma del Carmen.

Microsoft. (s.f.). *Crear una tabla dinámica para analizar datos de una hoja de cálculo*. Microsoft Support. https://support.microsoft.com/es-es/office/crear-una-tabla-dinamica-para-analizar-datos-de-una-hoja-de-calculo-a9a84538-bfe9-40a9-a8e9-f99134456576

### Bibliografía complementaria

Aprender21. (2026). *Tablas dinámicas en Excel: guía paso a paso*. https://www.aprender21.com/blog/excel-tablas-dinamicas-guia

CONAPESCA. (2025). *Anuario estadístico de pesca y acuacultura*. Secretaría de Agricultura y Desarrollo Rural. https://www.gob.mx/conapesca

Excel Total. (2021). *Tablas dinámicas en Excel (tutorial completo)*. https://exceltotal.com/tablas-dinamicas-en-excel

Ninja Excel. (2024). *Cómo hacer tablas dinámicas en Excel: paso a paso*. https://www.ninjaexcel.com/excel-en-el-trabajo/tablas-dinamicas

El Tio Tech. (2021). *6 ejercicios de tablas dinámicas para practicar*. https://eltiotech.com/6-ejercicios-tablas-dinamicas

Microsoft Support. (s.f.). *Introducción a Power Query*. https://support.microsoft.com/es-es/office/introducción-a-power-query

### Recursos audiovisuales

Daxus Latam. (2025). *Aprende a crear tablas dinámicas desde cero (con ejemplos)* [Video]. YouTube. https://www.youtube.com/watch?v=WGH-k_vURuE

El Tio Tech. (2025). *Domina las tablas dinámicas en Excel desde cero* [Video]. YouTube. https://www.youtube.com/watch?v=tN6_ZEaqYBo

Saber Programas. (2024). *Tablas dinámicas en Excel: de cero a experto* [Video]. YouTube. https://www.youtube.com/watch?v=6YOsIVH0STg

SMARTpro Academy. (s.f.). *Cómo hacer tablas dinámicas en Excel + IA desde cero* [Video]. YouTube. https://www.youtube.com/watch?v=Mh93eaKbkkw

### Referencias institucionales

DOF. (2018). *Ley General de Pesca y Acuacultura Sustentables*. Diario Oficial de la Federación. https://www.diputados.gob.mx/LeyesBiblio/pdf/LGPAS.pdf

INEGI. (2022). *Censo Nacional de Pesca y Acuacultura*. Instituto Nacional de Estadística y Geografía. https://www.inegi.org.mx

---

```
Firma de los autores:

Dr. Rolando Gelabert Fernández           Dr. Juan Carlos Pérez López
___________________________________       ___________________________________

Mtra. Ana María Sánchez Ruiz              Ing. Luis Alberto Domínguez Hernández
___________________________________       ___________________________________


Fecha de elaboración: Febrero 2026
Vo. Bo. del Comité de Pares Académicos
---

*Fin del Cuaderno de Trabajo*
```
