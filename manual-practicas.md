# Manual de Prácticas de Laboratorio

## Bioestadística — Análisis de datos de pesquerías con Excel

**UA:** Bioestadística

**Institución:** Universidad Autónoma del Carmen — Facultad de Ciencias Naturales y Exactas, Programa de Biología Marina

**Periodo:** Febrero-Junio 2026

**Autores:**
- Dr. Rolando Gelabert Fernández
- [Autor 2]
- [Autor 3]
- [Autor 4]

**Fecha de elaboración:** Junio 2026

**Versión:** 1.0

**Dataset de trabajo:** `datos_capturas_2005_2022.xlsx`

---

## Índice de Prácticas

| No. | Práctica | Pág. |
|-----|----------|------|
| 1 | Filtros básicos en Excel | 3 |
| 2 | Filtros avanzados y Power Query | 6 |
| 3 | Tablas dinámicas básicas | 9 |
| 4 | Personalización y formato de tablas dinámicas | 12 |
| 5 | Gráficos dinámicos para Biología Marina | 15 |
| 6 | Dashboard integrador de pesquerías | 18 |

---

## Introducción

El presente Manual de Prácticas de Laboratorio ha sido diseñado como un recurso didáctico complementario para la Unidad de Aprendizaje de Bioestadística del Programa de Biología Marina de la Universidad Autónoma del Carmen (UNACAR). Su propósito es apoyar el desarrollo de competencias en el análisis estadístico de datos pesqueros utilizando Microsoft Excel como herramienta de cálculo y visualización, con énfasis en el manejo de tablas dinámicas como eje transversal para la síntesis, exploración e interpretación de grandes volúmenes de información.

El dataset principal para todas las prácticas es `datos_capturas_2005_2022.xlsx`, que contiene registros oficiales de capturas pesqueras en México, incluyendo variables como especie, año, litoral, entidad federativa, peso desembarcado, peso vivo y valor económico. Este contexto real permite al estudiante vincular los conceptos estadísticos con problemas concretos de la biología pesquera y el manejo de recursos marinos.

El manual está estructurado en seis prácticas progresivas. La Práctica 1 introduce los filtros básicos para exploración de datos. La Práctica 2 aborda filtros avanzados y Power Query para limpieza y transformación de datos. Las Prácticas 3 y 4 cubren la creación, personalización y formato de tablas dinámicas. La Práctica 5 se enfoca en gráficos dinámicos para visualización de tendencias y composición de capturas. Finalmente, la Práctica 6 integra todas las herramientas en un dashboard profesional de pesquerías.

Cada práctica incluye: título, objetivo de aprendizaje, fundamento teórico, procedimiento detallado paso a paso y criterios de evaluación con ponderaciones. Se recomienda realizar las prácticas en orden secuencial, ya que cada una construye sobre las competencias adquiridas en la anterior.

Este manual cumple con los requisitos del indicador 1.2.3 del Cuadernillo ESDEPED UNACAR (2025-2026) como producto académico integrador del Paquete para la Docencia.

---

## Práctica 1: Filtros básicos en Excel

### Objetivo

Al finalizar la práctica, el estudiante será capaz de aplicar autofiltros en Excel para explorar, seleccionar y segmentar registros del dataset de capturas pesqueras utilizando criterios de filtrado por texto, número y fecha, facilitando el análisis preliminar de los datos.

### Fundamento teórico

Los filtros en Excel son herramientas de exploración que permiten visualizar únicamente los registros que cumplen ciertas condiciones, ocultando temporalmente el resto sin alterar ni eliminar datos. El Autofiltro se activa desde la pestaña Datos → Filtro o mediante el acceso directo Ctrl + Mayús + L, agregando menús desplegables en cada encabezado de columna.

Existen tres tipos principales de filtros: filtros de texto (igual a, contiene, comienza con, termina con), filtros numéricos (igual a, mayor que, menor que, entre, los 10 mayores) y filtros de fecha (hoy, esta semana, este mes, este año, entre fechas, filtro por año/mes/trimestre). La combinación de múltiples filtros aplicados simultáneamente en diferentes columnas equivale a una condición AND (todos los criterios deben cumplirse).

En el contexto del análisis pesquero, los filtros permiten responder preguntas exploratorias como: ¿cuáles fueron las capturas de huachinango en el litoral del Golfo de México? ¿qué entidades reportaron capturas de mero en 2020? ¿cuáles fueron los años con mayor peso desembarcado de camarón? Estas preguntas guían el proceso de filtrado y familiarizan al estudiante con la estructura del dataset.

El manejo adecuado de filtros es un requisito previo indispensable para el trabajo con tablas dinámicas, ya que implica comprender la estructura de los datos, la naturaleza de cada campo y la formulación de criterios de selección.

### Procedimiento

1. Abrir Microsoft Excel y cargar el archivo `datos_capturas_2005_2022.xlsx`.
2. Identificar la estructura del dataset: revisar los encabezados de columna (año, litoral, entidad, especie, peso_desembarcado, peso_vivo, valor), el tipo de dato en cada columna y el número total de registros.
3. Activar Autofiltro: seleccionar cualquier celda dentro de los datos e ir a Datos → Filtro (o presionar Ctrl + Mayús + L).
4. Aplicar un filtro de texto en la columna Especie: hacer clic en el menú desplegable → Filtros de texto → Contiene → escribir "huachinango" → Aceptar. Observar cuántos registros cumplen el criterio.
5. Agregar un segundo filtro sobre el resultado anterior: en la columna Litoral, seleccionar únicamente "Golfo de México". Verificar que ambos filtros actúan en simultáneo (condición AND).
6. Limpiar los filtros: Datos → Borrar (o hacer clic en el icono de filtro → Borrar filtro de...).
7. Aplicar un filtro numérico en la columna Peso desembarcado: Filtros de número → Mayor que → ingresar 50000 → Aceptar. Identificar las especies con mayor volumen de captura.
8. Aplicar un filtro de fecha en la columna Año: Filtros de fecha → Entre → seleccionar 2015 y 2020 → Aceptar. Analizar el período seleccionado.
9. Combinar filtros: filtrar por año 2018, litoral "Pacífico" y especie "camarón". Registrar el peso desembarcado total visible en la barra de estado (seleccionar la columna numérica y ver Suma en la barra inferior).
10. Utilizar el cuadro de búsqueda dentro del menú desplegable de filtro para localizar rápidamente especies como "mero", "pulpo", "langosta", "robalo" o "sierra".
11. Exportar el resultado filtrado: seleccionar los registros visibles, copiar (Ctrl + C) y pegar en una nueva hoja como valores. Insertar una fila con la leyenda "Registros filtrados: [fecha]" como control de calidad.
12. Guardar el archivo como `Practica1_Filtros_Basicos.xlsx`.

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Activa Autofiltro y navega correctamente por los menús de filtro | 15% |
| Aplica filtros de texto para seleccionar especies y litorales específicos | 20% |
| Aplica filtros numéricos para segmentar por peso desembarcado | 20% |
| Combina múltiples filtros simultáneos (condición AND) correctamente | 25% |
| Exporta registros filtrados a una nueva hoja con control de calidad | 20% |

---

## Práctica 2: Filtros avanzados y Power Query

### Objetivo

Al finalizar la práctica, el estudiante será capaz de aplicar filtros avanzados con criterios AND/OR sobre el dataset de capturas pesqueras y utilizar Power Query para realizar operaciones de extracción, transformación y carga (ETL), incluyendo limpieza de datos, eliminación de columnas y filtrado previo al análisis.

### Fundamento teórico

Los filtros avanzados superan las limitaciones del Autofiltro al permitir condiciones OR entre columnas diferentes, criterios calculados y la extracción del resultado a una ubicación distinta sin alterar los datos originales. Funcionan mediante un rango de criterios, que es un área separada en la hoja donde se escriben las condiciones: los criterios en la misma fila se interpretan como AND; los criterios en filas diferentes se interpretan como OR.

Por ejemplo, para filtrar registros de "camarón" en el Pacífico O capturas de "pulpo" en cualquier litoral, se escriben dos filas de criterios: Fila 1: Especie = "camarón" AND Litoral = "Pacífico"; Fila 2: Especie = "pulpo". Al ejecutar el filtro avanzado con ambos criterios, Excel devuelve los registros que cumplen cualquiera de las dos condiciones.

Power Query (obtención y transformación de datos) es una herramienta de ETL integrada en Excel que permite conectar, combinar, limpiar y transformar datos de múltiples orígenes sin modificar la fuente original. A diferencia de los filtros tradicionales, Power Query registra cada paso de transformación como una consulta reutilizable, lo que garantiza reproducibilidad. Las operaciones comunes incluyen: eliminación de columnas irrelevantes, filtrado de filas, cambio de tipos de datos, reemplazo de valores, eliminación de duplicados y combinación de tablas.

En el contexto pesquero, Power Query permite estandarizar nombres de especies (corrigiendo variaciones como "camarón blanco" vs "camarón café"), unificar litorales escritos de forma inconsistente, filtrar únicamente los años de interés y eliminar columnas auxiliares que no participarán en el análisis.

### Procedimiento

1. Abrir el archivo `datos_capturas_2005_2022.xlsx` y crear una nueva hoja en blanco llamada "Criterios".
2. En la hoja "Criterios", copiar los encabezados Especie y Litoral en las celdas A1 y B1 respectivamente.
3. En A2 escribir "camarón" y en B2 escribir "Pacífico" (fila 2 = criterio AND).
4. En A3 escribir "pulpo" y dejar B3 vacío (fila 3 = criterio OR, cualquier litoral).
5. Seleccionar los datos originales (incluyendo encabezados), ir a Datos → Avanzadas.
6. En el cuadro de diálogo Filtro avanzado, seleccionar "Copiar a otro lugar", definir "Rango de la tabla" como los datos originales, "Rango de criterios" como A1:B3 de la hoja "Criterios", y "Copiar a" una celda en una hoja nueva. Aceptar y verificar el resultado.
7. Crear un filtro avanzado adicional que muestre capturas del año 2020 con peso desembarcado mayor a 100000, utilizando criterios en columnas Año y Peso desembarcado.
8. Abrir Power Query: seleccionar una celda en los datos originales → Datos → Desde tabla/rango (confirmar que los datos estén en formato Tabla de Excel).
9. En el editor de Power Query, eliminar columnas innecesarias (si existen): seleccionar columna → Eliminar columnas.
10. Filtrar filas: hacer clic en el menú desplegable de la columna Especie, desmarcar especies no relevantes o buscar especies específicas como "mero", "huachinango", "camarón", "pulpo", "langosta", "robalo". Aplicar el filtro.
11. Reemplazar valores: seleccionar columna Litoral → Reemplazar valores → corregir variaciones (ej. "Golfo" → "Golfo de México").
12. Cambiar tipos de datos: asegurar que Peso desembarcado y Peso vivo sean números decimales, Año sea número entero y Valor sea moneda.
13. Cerrar y cargar: Inicio → Cerrar y cargar → Cargar a → "Solo crear conexión" (para usar los datos transformados en prácticas posteriores).
14. Guardar el archivo como `Practica2_Filtros_Avanzados_PowerQuery.xlsx`.

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Construye correctamente rangos de criterios AND/OR para filtro avanzado | 20% |
| Ejecuta filtro avanzado copiando resultados a otra ubicación | 20% |
| Abre y navega el editor de Power Query correctamente | 15% |
| Realiza al menos tres transformaciones en Power Query (filtros, reemplazos, tipos) | 25% |
| Carga la consulta como conexión para uso posterior | 20% |

---

## Práctica 3: Tablas dinámicas básicas

### Objetivo

Al finalizar la práctica, el estudiante será capaz de crear tablas dinámicas a partir del dataset de capturas pesqueras, asignar campos a las cuatro áreas (Filas, Columnas, Valores y Filtros), y aplicar funciones de agregación (suma, promedio, conteo) para resumir peso desembarcado, peso vivo y valor por especie, año y litoral.

### Fundamento teórico

Una tabla dinámica (PivotTable) es una herramienta interactiva de Excel que resume, agrupa y analiza grandes volúmenes de datos sin requerir fórmulas escritas manualmente. Su arquitectura se basa en cuatro áreas: Filas (organiza datos verticalmente, por ejemplo especies o años), Columnas (organiza datos horizontalmente, por ejemplo litorales o trimestres), Valores (contiene los datos numéricos a resumir mediante funciones de agregación) y Filtros (restringe el análisis a un subconjunto de datos).

Las funciones de agregación disponibles son: Suma (total acumulado), Promedio (media aritmética), Contar (número de registros), Máx (valor máximo), Mín (valor mínimo) y Producto. La selección de la función depende de la pregunta de investigación: suma para volumen total de captura por especie, promedio para rendimiento promedio por año, conteo para número de registros de una especie en el período.

La naturaleza multidimensional de las tablas dinámicas permite rotar campos entre las áreas mediante arrastre, facilitando el análisis desde diferentes perspectivas. Por ejemplo, con un mismo conjunto de datos se puede responder: ¿cuál es el peso desembarcado total por especie? ¿cómo varía la captura de mero por litoral y año? ¿cuál es el valor económico promedio de las capturas de langosta por entidad?

El dataset `datos_capturas_2005_2022.xlsx` contiene las columnas clave para estos análisis: Especie (dimensión biológica), Año (dimensión temporal), Litoral y Entidad (dimensiones geográficas), Peso desembarcado y Peso vivo (variables de volumen de captura) y Valor (variable económica).

### Procedimiento

1. Abrir el archivo `datos_capturas_2005_2022.xlsx` y asegurarse de que los datos estén en formato Tabla de Excel (Ctrl + T si no lo están).
2. Seleccionar cualquier celda dentro de la tabla e ir a Insertar → Tabla dinámica (Alt + N + V).
3. Verificar que el rango o nombre de la tabla origen esté correctamente seleccionado. Elegir "Nueva hoja de cálculo".
4. En el panel Campos de tabla dinámica, arrastrar el campo `Especie` al área Filas.
5. Arrastrar el campo `Peso desembarcado` al área Valores. La tabla mostrará la suma de peso desembarcado por especie.
6. Arrastrar el campo `Año` al área Columnas. Ahora la tabla muestra peso desembarcado por especie (filas) y año (columnas).
7. Arrastrar el campo `Litoral` al área Filtros. Seleccionar "Golfo de México" en el filtro y observar cómo cambia la tabla.
8. Crear una segunda tabla dinámica que muestre el promedio de peso vivo por especie y litoral: arrastrar Especie a Filas, Litoral a Columnas, Peso vivo a Valores. Cambiar la función de agregación de Suma a Promedio (clic derecho → Configuración de campo de valor → Promedio).
9. Crear una tercera tabla dinámica que muestre el conteo de registros por año y entidad: arrastrar Año a Filas, Entidad a Columnas y cualquier campo no numérico (como Especie) a Valores. Excel automáticamente usará Contar como agregación.
10. Agregar el campo `Valor` al área Valores de la primera tabla dinámica, arrastrándolo debajo de Peso desembarcado. Observar que se agrega una segunda columna de valores.
11. Experimentar: mover el campo Año de Columnas a Filas y arrastrar Litoral a Columnas. Observar cómo cambia la orientación del análisis.
12. Guardar el archivo como `Practica3_Tablas_Dinamicas_Basicas.xlsx`.

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Crea tabla dinámica seleccionando correctamente el origen de datos | 15% |
| Asigna campos a las cuatro áreas (Filas, Columnas, Valores, Filtros) | 20% |
| Cambia función de agregación entre suma, promedio y conteo | 20% |
| Crea múltiples tablas dinámicas para diferentes preguntas de análisis | 25% |
| Utiliza filtros de tabla dinámica para segmentar por litoral o entidad | 20% |

---

## Práctica 4: Personalización y formato de tablas dinámicas

### Objetivo

Al finalizar la práctica, el estudiante será capaz de personalizar el diseño, formato y presentación de tablas dinámicas aplicando diseños de informe, formato de números, opciones "Mostrar valores como" y segmentaciones de datos, optimizando la visualización de información pesquera para distintos públicos.

### Fundamento teórico

Las tablas dinámicas ofrecen opciones de personalización que mejoran su legibilidad y efectividad comunicativa. El diseño de informe admite tres formatos: Compacto (ahorra espacio con encabezados anidados en una columna), Tabular (cada campo en una columna separada, similar a una base de datos) y Esquemático (con sangrías jerárquicas). El formato tabular es el más recomendado para informes formales y exportación a otros sistemas.

El formato de números es crítico para la correcta interpretación de datos pesqueros. Los valores de peso desembarcado y peso vivo (toneladas o kilogramos) deben mostrar separador de miles sin decimales excesivos. Los valores económicos requieren formato de moneda. El formato porcentual permite visualizar la contribución relativa de cada especie al total de capturas.

La opción "Mostrar valores como" transforma datos absolutos en medidas relativas: % del total general (cada valor como proporción del total global), % del total de fila (proporción dentro de cada especie), % del total de columna (proporción dentro de cada año o litoral), diferencia respecto al registro anterior (variación interanual) y clasificación (ranking de mayor a menor).

Las segmentaciones de datos (Slicers) son controles visuales interactivos que permiten filtrar tablas dinámicas mediante botones, ofreciendo retroalimentación visual inmediata sobre el estado del filtro. Al conectarse a una tabla dinámica, permiten al usuario final explorar los datos de forma intuitiva sin modificar la estructura del informe. En el contexto pesquero, las segmentaciones facilitan la exploración por especie, litoral o entidad con un solo clic.

### Procedimiento

1. Abrir el archivo `Practica3_Tablas_Dinamicas_Basicas.xlsx` y seleccionar la tabla dinámica principal.
2. Cambiar el diseño a formato tabular: pestaña Diseño → Diseño de informe → Mostrar en forma tabular.
3. Activar "Repetir todas las etiquetas de elementos" en Diseño → Diseño de informe.
4. Desactivar subtotales: Diseño → Subtotales → No mostrar subtotales.
5. Aplicar formato de número a Peso desembarcado: clic derecho en un valor → Configuración de campo de valor → Formato de número → Número → 0 decimales, separador de miles activado.
6. Agregar el campo Valor al área Valores y aplicar formato de moneda (símbolo $, 2 decimales).
7. Mostrar valores como porcentaje: clic derecho sobre un valor de Peso desembarcado → Mostrar valor como → % del total general. Interpretar el resultado: ¿qué especie aporta el mayor porcentaje?
8. Revertir a suma (sin porcentaje) y agregar una nueva instancia de Peso desembarcado a Valores. Configurar la segunda instancia como % del total de fila (participación de cada año dentro del total de cada especie).
9. Aplicar un estilo predefinido de tabla dinámica: pestaña Diseño → galería de estilos → seleccionar uno con tonos azules o verdes (asociados al contexto marino).
10. Insertar una segmentación: seleccionar la tabla dinámica → pestaña Analizar → Insertar segmentación → marcar los campos Especie, Litoral y Año.
11. Organizar las segmentaciones en la hoja, ajustar tamaño y columnas de botones (pestaña Opciones → Botones → Columnas: 3 para Especie, 1 para Litoral y Año).
12. Probar las segmentaciones: seleccionar "Pacífico" en Litoral y observar cómo se actualiza la tabla dinámica. Luego seleccionar especies específicas combinando Ctrl + clic.
13. Conectar las segmentaciones a una segunda tabla dinámica si existe en el mismo archivo: clic derecho en la segmentación → Conexiones de informe → marcar la segunda tabla dinámica.
14. Guardar el archivo como `Practica4_Formato_Segmentaciones.xlsx`.

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Cambia el diseño de informe a formato tabular con rótulos repetidos | 15% |
| Aplica formato de número y moneda a los campos de valor | 20% |
| Configura Mostrar valores como % del total general y % del total de fila | 20% |
| Inserta y personaliza segmentaciones de datos | 20% |
| Conecta segmentaciones a múltiples tablas dinámicas | 15% |
| Aplica estilo predefinido y organiza visualmente la hoja | 10% |

---

## Práctica 5: Gráficos dinámicos para Biología Marina

### Objetivo

Al finalizar la práctica, el estudiante será capaz de crear gráficos dinámicos vinculados a tablas dinámicas para visualizar tendencias temporales de capturas, histogramas de distribución por especie y gráficos de composición por litoral, aplicando principios de visualización de datos en el contexto de la biología pesquera.

### Fundamento teórico

Un gráfico dinámico es una representación visual que se actualiza automáticamente al modificar su tabla dinámica asociada, y viceversa. Esta vinculación bidireccional permite explorar visualmente los datos modificando dimensiones, aplicando filtros o usando segmentaciones, con respuesta inmediata del gráfico.

En el análisis de pesquerías, los tipos de gráfico más relevantes son:

- **Gráfico de columnas agrupadas**: compara volúmenes de captura entre especies, litorales o entidades. Útil para identificar las especies de mayor rendimiento pesquero.
- **Gráfico de líneas**: muestra tendencias temporales de captura a lo largo de los años (2005-2022). Permite detectar patrones de incremento, decrecimiento o ciclicidad en las poblaciones explotadas.
- **Gráfico circular o de anillos**: representa la composición porcentual de capturas por especie, litoral o grupo taxonómico. Adecuado para mostrar dominancia de especies en una región.
- **Gráfico de barras apiladas**: visualiza la contribución de cada litoral al total de captura por año, o la composición por especie dentro de cada entidad.
- **Histograma de frecuencias**: distribuye las capturas en intervalos de peso para analizar la estructura de tallas o volúmenes de desembarque.

Los principios de visualización en biología marina incluyen: uso de escalas logarítmicas cuando los datos abarcan varios órdenes de magnitud, etiquetas claras con nombres comunes de especies y unidades de medida (toneladas, kilogramos, pesos), y paletas de colores que distingan litorales y grupos taxonómicos sin generar confusión.

### Procedimiento

1. Abrir el archivo `Practica4_Formato_Segmentaciones.xlsx`.
2. Crear una tabla dinámica con Año en Filas y Suma de Peso desembarcado en Valores. Insertar un gráfico dinámico de líneas: seleccionar la tabla dinámica → Insertar → Gráfico dinámico → Línea.
3. Personalizar el gráfico de líneas: título "Tendencia de capturas 2005-2022 (toneladas)", etiqueta del eje Y "Peso desembarcado (ton)", etiqueta del eje X "Año". Agregar línea de tendencia lineal (clic derecho en la serie → Agregar línea de tendencia).
4. Crear una segunda tabla dinámica con Especie en Filas y Suma de Peso desembarcado en Valores. Ordenar de mayor a menor por el campo de valor. Insertar un gráfico dinámico de columnas agrupadas. Aplicar filtro de valor para mostrar solo las 10 especies con mayor captura (Filtros de etiqueta o filtrar directamente en el gráfico).
5. Personalizar el gráfico de columnas: título "Top 10 especies por volumen de captura", etiqueta del eje Y "Peso desembarcado (ton)", colores en azul y verde. Agregar etiquetas de datos en la parte superior de cada barra.
6. Crear una tercera tabla dinámica con Litoral en Filas y Suma de Peso desembarcado en Valores. Insertar un gráfico dinámico circular (pastel) o de anillos. Personalizar: título "Distribución de capturas por litoral", mostrar etiquetas con nombre y porcentaje, colores distintivos (azul para Golfo de México, verde para Pacífico, amarillo para Caribe).
7. Crear una cuarta tabla dinámica con Año en Filas, Litoral en Columnas y Suma de Peso desembarcado en Valores. Insertar un gráfico dinámico de barras apiladas. Este gráfico muestra cómo cambia la contribución de cada litoral a lo largo del tiempo.
8. Insertar segmentaciones de Especie, Litoral y Año. Conectarlas a todos los gráficos dinámicos existentes (clic derecho en cada segmentación → Conexiones de informe → marcar todas las tablas dinámicas asociadas a los gráficos).
9. Organizar la hoja en formato de dashboard: segmentaciones en la parte superior, gráfico de líneas (esquina superior izquierda), gráfico de columnas (esquina superior derecha), gráfico circular (esquina inferior izquierda), gráfico de barras apiladas (esquina inferior derecha).
10. Probar la interactividad: seleccionar un litoral en la segmentación y observar cómo todos los gráficos se actualizan simultáneamente. Seleccionar especies específicas y ver el cambio en la tendencia temporal y distribución geográfica.
11. Guardar el archivo como `Practica5_Graficos_Dinamicos.xlsx`.

12. **Aplicar principios de gráficos científicos (Handbook of Biological Statistics — McDonald, 2014):**
    - **Eliminar clutter:** Quitar gridlines (líneas de cuadrícula), fondos grises y efectos 3D del área del gráfico. Todo eso distrae del mensaje.
    - **Escalas de ejes:** El eje Y debe comenzar en 0 a menos que los valores observados varíen en un rango muy estrecho. Usa valores máximos redondos (ej. 5000, 10000, no 4783). Si tienes múltiples gráficos comparables, usa la misma escala en todos.
    - **Tipografía:** Usa fuente sans-serif (Arial, Helvetica) consistente en todos los elementos del gráfico (títulos, etiquetas de ejes, leyenda). Incluye unidades de medida en las etiquetas de los ejes.
    - **Marcos:** El área del gráfico debe tener borde negro en los 4 lados (Format Plot Area → Line → Black). El área exterior (Chart Area) debe ir sin borde (No Line).
    - **Barras de error:** Si agregas barras de error, especifica en la descripción si son IC 95 %, error estándar o desviación estándar. En Excel, usa Custom en lugar de las opciones predeterminadas "Standard Error" o "Standard Deviation" (que no calculan lo que parecen).
    - **Leyenda:** Si solo hay una serie de datos, elimínala; si hay varias, decide si va en el gráfico o se explica en la descripción.
    - **Color:** Para presentaciones usa color (evita combinar rojo+verde por daltonismo). Para publicación usa blanco, negro, grises, tramas (rayas, puntos, cross-hatching) — no uses tonos de gris similares porque no se distinguen en fotocopia.
    - **Exportación:** Para publicación, guarda el gráfico como PDF (clic derecho en el área del gráfico → Guardar como imagen → PDF) y edítalo en un programa vectorial como Inkscape si es necesario.

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Crea un gráfico de líneas con tendencia temporal de capturas y su línea de tendencia | 20% |
| Crea un gráfico de columnas con Top 10 de especies y etiquetas de datos | 20% |
| Crea un gráfico circular de composición por litoral con porcentajes | 15% |
| Crea un gráfico de barras apiladas combinando año y litoral | 15% |
| Conecta segmentaciones a todos los gráficos dinámicos | 15% |
| Organiza los gráficos en un dashboard coherente y prueba su interactividad | 15% |

---

## Práctica 6: Dashboard integrador de pesquerías

### Objetivo

Al finalizar la práctica, el estudiante será capaz de integrar filtros, Power Query, tablas dinámicas y gráficos dinámicos en un dashboard profesional de pesquerías, combinando múltiples fuentes de análisis para generar un informe ejecutivo con hallazgos, tendencias y recomendaciones basadas en los datos de capturas.

### Fundamento teórico

Un dashboard es un sistema de visualización que consolida en una sola vista los indicadores clave de rendimiento (KPI) y las métricas relevantes de un dominio específico. En el contexto de la biología pesquera, un dashboard de capturas permite a investigadores y tomadores de decisiones monitorear el estado de las pesquerías, identificar especies sobreexplotadas, detectar tendencias geográficas y evaluar el impacto económico de las capturas.

Las etapas del desarrollo de un dashboard son:

1. **Definición del problema**: ¿qué preguntas debe responder el dashboard? Ejemplos: ¿cuál es la tendencia general de capturas en el período 2005-2022? ¿qué litoral contribuye más al volumen total? ¿qué especies presentan mayor valor económico? ¿existe algún patrón de decrecimiento que sugiera sobreexplotación?

2. **Extracción y transformación (ETL)**: Power Query se utiliza para conectar el dataset original, limpiar inconsistencias, estandarizar nombres y cargar los datos transformados como modelo de datos. La reproducibilidad del proceso ETL garantiza que el dashboard pueda actualizarse con nuevos datos sin reconstruir manualmente las transformaciones.

3. **Modelado**: las tablas dinámicas constituyen el modelo de análisis, organizando los datos en dimensiones (especie, año, litoral, entidad) y medidas (peso desembarcado, peso vivo, valor). La combinación de múltiples tablas dinámicas permite abordar diferentes preguntas desde un mismo conjunto de datos.

4. **Visualización**: los gráficos dinámicos transforman los resúmenes numéricos en representaciones visuales intuitivas. La selección del tipo de gráfico debe alinearse con la naturaleza de los datos y la audiencia objetivo.

5. **Interactividad**: las segmentaciones y filtros conectados a todos los elementos del dashboard permiten la exploración autónoma por parte del usuario final, facilitando el análisis de escenarios específicos (un litoral particular, un rango de años, un grupo de especies).

6. **Interpretación y comunicación**: el dashboard debe incluir un espacio para hallazgos, conclusiones y recomendaciones. Las conclusiones deben estar respaldadas por los datos visibles en el dashboard y expresadas en lenguaje accesible para tomadores de decisiones no especializados en estadística.

### Procedimiento

1. Abrir Excel y cargar el archivo `datos_capturas_2005_2022.xlsx`. Convertir los datos a Tabla de Excel (Ctrl + T) y nombrarla `tblCapturas`.
2. **Fase 1 — ETL con Power Query**: ir a Datos → Desde tabla/rango. En el editor de Power Query:
   - Eliminar columnas irrelevantes si las hay.
   - Filtrar para conservar únicamente los años 2010-2022.
   - Reemplazar valores para estandarizar nombres de litorales.
   - Cambiar tipos de datos: Peso desembarcado y Peso vivo como número decimal, Valor como moneda.
   - Cerrar y cargar como "Solo crear conexión". Nombrar la consulta "Capturas Limpias".
3. **Fase 2 — Tablas dinámicas de análisis**:
   - **KPI 1 — Captura total por año**: tabla dinámica con Año en Filas, Suma de Peso desembarcado en Valores. Agregar una línea de promedio general como referencia.
   - **KPI 2 — Captura por especie**: tabla dinámica con Especie en Filas, Suma de Peso desembarcado en Valores. Filtrar para mostrar Top 10.
   - **KPI 3 — Captura por litoral**: tabla dinámica con Litoral en Filas, Suma de Peso desembarcado y Suma de Valor en Valores.
   - **KPI 4 — Matriz especie-año**: tabla dinámica con Especie en Filas, Año en Columnas, Suma de Peso desembarcado en Valores. Aplicar formato condicional con escala de colores para identificar celdas de alto y bajo rendimiento.
   - **KPI 5 — Análisis económico**: tabla dinámica con Entidad en Filas, Suma de Valor en Valores. Ordenar de mayor a menor.
4. **Fase 3 — Visualización**:
   - Gráfico de líneas (tendencia anual de captura) con línea de tendencia y etiquetas de datos.
   - Gráfico de columnas (Top 10 especies) con colores degradados y etiquetas.
   - Gráfico circular (participación por litoral) con porcentajes.
   - Gráfico de barras apiladas (composición de captura por litoral a través del tiempo).
   - Gráfico de columnas (valor económico por entidad) con formato de moneda en etiquetas.
5. **Fase 4 — Interactividad**:
   - Insertar segmentaciones para Especie, Litoral y Año.
   - Conectar cada segmentación a todas las tablas dinámicas del dashboard.
   - Organizar las segmentaciones en una franja superior con formato horizontal.
   - Insertar un control de escala de tiempo para el campo Año (opcional, si el campo está como fecha).
6. **Fase 5 — Diseño del dashboard**:
   - Crear una hoja llamada "Dashboard" y organizar los elementos:
     - Fila superior: título "Dashboard de Capturas Pesqueras 2010-2022" con formato grande y color azul marino.
     - Segunda fila: segmentaciones de Especie, Litoral, Año.
     - Tercera fila: KPI numéricos con tarjetas (Captura total, Especie principal, Litoral principal, Valor total) usando fórmulas GETPIVOTDATA o referencias a celdas de las tablas dinámicas.
     - Cuarta fila: gráfico de líneas (izquierda) y gráfico de columnas (derecha).
     - Quinta fila: gráfico circular (izquierda), gráfico de barras apiladas (centro) y gráfico de valor económico (derecha).
   - Aplicar una paleta de colores consistente (azules, verdes y tonos marinos).
   - Agregar bordes, sombras y formato limpio sin recargar visualmente.
7. **Fase 6 — Conclusiones y recomendaciones**:
   - En una hoja separada llamada "Conclusiones", escribir un informe de 15-20 líneas que incluya:
     - Tendencia general de capturas en el período analizado (¿creciente, decreciente, estable?).
     - Especies con mayor y menor volumen de captura; posibles causas biológicas o pesqueras.
     - Litoral con mayor contribución y su evolución temporal.
     - Entidades con mayor valor económico de capturas.
     - Al menos tres recomendaciones basadas en datos para el manejo pesquero (ej. "fortalecer la vigilancia en el litoral X", "promover la diversificación hacia especie Y", "establecer cuotas de captura para especie Z").
8. Guardar el archivo como `Practica6_Dashboard_Pesquerias.xlsx`.

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Fase 1: Transformación ETL con Power Query (filtros, reemplazos, tipos) | 10% |
| Fase 2: Tablas dinámicas que responden los KPI planteados | 20% |
| Fase 3: Gráficos dinámicos variados con formato y etiquetas correctas | 20% |
| Fase 4: Segmentaciones y controles conectados a todos los elementos | 15% |
| Fase 5: Diseño profesional del dashboard con organización y paleta cromática | 15% |
| Fase 6: Informe de conclusiones con hallazgos y recomendaciones basadas en datos | 20% |

---

## Bibliografía

Caballero, M. & Torres, F. (s.f.). *Tablas dinámicas: la quinta dimensión* (1.ª ed.). [Documento PDF]. Incluido en el Paquete para la Docencia.

Daxus Latam. (2025). *Aprende a crear tablas dinámicas desde cero (con ejemplos)* [Video]. YouTube. https://www.youtube.com/watch?v=WGH-k_vURuE

El Tío Tech. (2021). *6 ejercicios de tablas dinámicas para practicar*. El Tío Tech. https://eltiotech.com/6-ejercicios-tablas-dinamicas

El Tío Tech. (2025). *Domina las tablas dinámicas en Excel desde cero* [Video]. YouTube. https://www.youtube.com/watch?v=tN6_ZEaqYBo

Excel Total. (2021). *Tablas dinámicas en Excel (tutorial completo)*. Excel Total. https://exceltotal.com/tablas-dinamicas-en-excel

Gelabert Fernández, R. (2026). *Fuentes originales del cuaderno: conceptos básicos, tutorial práctico, técnicas avanzadas, gráficos dinámicos, errores comunes* [Material inédito]. Universidad Autónoma del Carmen.

Microsoft. (s.f.). *Crear una tabla dinámica para analizar datos de una hoja de cálculo*. Microsoft Support. https://support.microsoft.com/es-es/office/crear-una-tabla-din%C3%A1mica-para-analizar-datos-de-una-hoja-de-c%C3%A1lculo-a9a84538-bfe9-40a9-a8e9-f99134456576

Saber Programas. (2024). *Tablas dinámicas en Excel de cero a experto* [Video]. YouTube. https://www.youtube.com/watch?v=6YOsIVH0STg

SMARTpro Academy. (s.f.). *Cómo hacer tablas dinámicas en Excel + IA desde cero* [Video]. YouTube. https://www.youtube.com/watch?v=Mh93eaKbkkw
