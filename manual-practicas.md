# Manual de Prácticas de Laboratorio

## Tablas Dinámicas en Excel

**UA:** Tablas Dinámicas en Excel

**Institución:** Universidad Autónoma del Carmen

**Periodo:** 2025-2026

**Autores:**
- Rolando Gelabert Fernández
- [Autor 2]
- [Autor 3]
- [Autor 4]

**Fecha de elaboración:** Junio 2026

**Versión:** 1.0

---

## Índice de Prácticas

| No. | Práctica | Pág. |
|-----|----------|------|
| 1 | Preparación y limpieza de datos para tablas dinámicas | 3 |
| 2 | Creación de tablas dinámicas básicas | 6 |
| 3 | Personalización y formato de tablas dinámicas | 9 |
| 4 | Segmentaciones, escalas de tiempo y filtros | 12 |
| 5 | Gráficos dinámicos y dashboards | 15 |
| 6 | Proyecto integrador: análisis completo | 18 |

---

## Introducción

El presente Manual de Prácticas de Laboratorio ha sido diseñado como un recurso didáctico complementario para la Unidad de Aprendizaje "Tablas Dinámicas en Excel", dirigido a estudiantes de nivel medio superior y superior. Su propósito es desarrollar en el alumno las competencias necesarias para transformar datos en información útil mediante el uso de tablas dinámicas, una de las herramientas más poderosas de Microsoft Excel para el análisis, resumen y presentación de grandes volúmenes de datos.

El manual está estructurado en seis prácticas progresivas que guían al estudiante desde los fundamentos básicos hasta un proyecto integrador final. La Práctica 1 sienta las bases con la preparación y limpieza de datos, etapa crítica para garantizar resultados confiables. Las Prácticas 2 y 3 introducen la creación y personalización de tablas dinámicas. La Práctica 4 incorpora herramientas interactivas de filtrado como segmentaciones y escalas de tiempo. La Práctica 5 aborda la visualización mediante gráficos dinámicos y dashboards. Finalmente, la Práctica 6 integra todos los conocimientos en un proyecto de análisis completo.

Cada práctica incluye: título, objetivo de aprendizaje, fundamento teórico, procedimiento detallado paso a paso y criterios de evaluación. Se recomienda que el estudiante realice las prácticas en el orden propuesto, ya que cada una construye sobre los conocimientos adquiridos en la anterior.

Este manual cumple con los requisitos establecidos en el indicador 1.2.4 del Cuadernillo ESDEPED UNACAR (2025-2026) y ha sido validado por la academia correspondiente.

---

## Práctica 1: Preparación y limpieza de datos para tablas dinámicas

### Objetivo

Al finalizar la práctica, el estudiante será capaz de preparar y limpiar un conjunto de datos en Excel aplicando las reglas fundamentales de estructuración, eliminación de inconsistencias y conversión a Tabla de Excel, garantizando que los datos estén listos para ser utilizados como origen de una tabla dinámica.

### Fundamento teórico

La preparación de datos constituye la etapa más crítica en el proceso de análisis con tablas dinámicas. Un conjunto de datos mal estructurado produce resultados incorrectos o incompletos, independientemente de la habilidad del analista. Los principios fundamentales para una base de datos adecuada incluyen: encabezados en la primera fila que describan claramente cada columna, ausencia de filas o columnas completamente vacías, eliminación de celdas combinadas (que impiden la correcta lectura de los datos por parte de Excel), y formatos consistentes en cada columna (por ejemplo, todas las fechas en el mismo formato).

La Tabla de Excel (insertada mediante Ctrl + T) es una funcionalidad que convierte un rango de celdas en una estructura de datos inteligente. Al utilizar una Tabla de Excel como origen de datos, la tabla dinámica obtiene la capacidad de detectar automáticamente nuevos registros agregados, eliminando la necesidad de redefinir el rango de origen cada vez que los datos se actualizan. Además, las Tablas de Excel ofrecen beneficios adicionales como encabezados persistentes al desplazarse, fórmulas que se extienden automáticamente y formato consistente.

Errores comunes en la preparación de datos incluyen: espacios en blanco al inicio o final de celdas de texto (invisibles pero que Excel interpreta como valores distintos), formatos numéricos almacenados como texto (impiden operaciones de suma y promedio), y valores duplicados no deseados. La herramienta "Quitar duplicados" y las funciones de limpieza de texto (RECORTAR, LIMPIAR) son esenciales para sanear los datos antes del análisis.

### Procedimiento

1. Abrir Microsoft Excel y crear un nuevo libro de trabajo.
2. Descargar el archivo de datos "Ventas_Ejemplo.xlsx" proporcionado por el docente.
3. Identificar la estructura del archivo: revisar encabezados, tipos de datos en cada columna y número de registros.
4. Verificar que no existan filas o columnas completamente vacías dentro del rango de datos.
5. Eliminar cualquier celda combinada seleccionando las celdas y usando Inicio → Combinar y centrar → Separar celdas.
6. Revisar la columna de fechas: asegurar que todas estén en formato de fecha (dd/mm/aaaa). Convertir usando Formato de celdas → Fecha.
7. Revisar la columna de montos: asegurar que todos los valores sean numéricos. Las celdas con triángulo verde indican número almacenado como texto; seleccionarlas y convertir a número.
8. Aplicar la función RECORTAR a columnas de texto para eliminar espacios adicionales: insertar una columna auxiliar con =RECORTAR(celda), copiar y pegar como valores sobre la original.
9. Eliminar filas duplicadas usando Datos → Quitar duplicados, seleccionando todas las columnas.
10. Convertir el rango de datos en Tabla de Excel: seleccionar cualquier celda dentro de los datos y presionar Ctrl + T, asegurando que "Mi tabla tiene encabezados" esté marcado.
11. Asignar un nombre descriptivo a la tabla desde la pestaña Diseño de tabla (ej. "tblVentas").
12. Guardar el archivo como "Practica1_Preparacion_Datos.xlsx".

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Identifica y corrige datos con formato incorrecto | 20% |
| Elimina espacios, duplicados y celdas combinadas | 25% |
| Convierte el rango a Tabla de Excel correctamente | 25% |
| Asigna nombre descriptivo a la tabla | 10% |
| El archivo guardado contiene todos los datos limpios y estructurados | 20% |

---

## Práctica 2: Creación de tablas dinámicas básicas

### Objetivo

Al finalizar la práctica, el estudiante será capaz de crear una tabla dinámica a partir de un conjunto de datos estructurados, asignar correctamente los campos a las cuatro áreas (Filas, Columnas, Valores y Filtros), y generar resúmenes básicos de información utilizando las funciones de agregación (suma, promedio, conteo).

### Fundamento teórico

Una tabla dinámica (PivotTable) es una herramienta interactiva de Excel que permite resumir, analizar y explorar grandes volúmenes de datos sin necesidad de escribir fórmulas. Su funcionamiento se basa en cuatro áreas fundamentales: Filas, Columnas, Valores y Filtros. El área de Filas organiza los datos de forma vertical (por ejemplo, nombres de productos o categorías). El área de Columnas los organiza horizontalmente (por ejemplo, meses del año). El área de Valores contiene los datos numéricos que se desean resumir mediante funciones de agregación como suma, promedio, conteo, máximo o mínimo. El área de Filtros permite restringir los datos mostrados a un subconjunto específico.

La versatilidad de las tablas dinámicas radica en su naturaleza interactiva: el usuario puede arrastrar y soltar campos entre las áreas para reorganizar el análisis en segundos, sin modificar los datos originales. Esta capacidad de reorganización multidimensional permite responder preguntas de negocio desde múltiples perspectivas.

Las funciones de agregación disponibles son: Suma (valores totales), Promedio (media aritmética), Contar (número de registros), Máx (valor máximo), Mín (valor mínimo) y Producto (multiplicación de valores). La elección de la función depende del tipo de análisis: suma para totales de ventas, promedio para calificaciones o temperaturas, y conteo para número de transacciones o clientes.

### Procedimiento

1. Abrir el archivo "Practica1_Preparacion_Datos.xlsx" guardado en la práctica anterior.
2. Seleccionar cualquier celda dentro de la Tabla de Excel creada.
3. Ir a la pestaña Insertar → Tabla dinámica (o presionar Alt + N + V).
4. En el cuadro de diálogo, verificar que el rango/tabla de origen esté correctamente seleccionado.
5. Elegir "Nueva hoja de cálculo" y hacer clic en Aceptar.
6. En la lista de campos de tabla dinámica (panel derecho), identificar las columnas disponibles.
7. Arrastrar el campo "Producto" al área Filas.
8. Arrastrar el campo "Mes" al área Columnas.
9. Arrastrar el campo "Total_Venta" al área Valores (por defecto mostrará suma).
10. Observar cómo la tabla dinámica genera el resumen de ventas por producto y mes.
11. Modificar la función de agregación: hacer clic derecho en un valor → Configuración de campo de valor → Cambiar Suma por Promedio.
12. Agregar un filtro: arrastrar el campo "Región" al área Filtros y seleccionar una región específica.
13. Crear una segunda tabla dinámica en la misma hoja que muestre el conteo de transacciones por vendedor.
14. Guardar el archivo como "Practica2_Tablas_Dinamicas_Basicas.xlsx".

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Crea la tabla dinámica seleccionando correctamente el origen de datos | 20% |
| Asigna campos a las cuatro áreas de forma correcta | 25% |
| Cambia la función de agregación (suma a promedio) | 15% |
| Utiliza el filtro de región para segmentar datos | 15% |
| Crea una segunda tabla dinámica con conteo de transacciones | 25% |

---

## Práctica 3: Personalización y formato de tablas dinámicas

### Objetivo

Al finalizar la práctica, el estudiante será capaz de personalizar el diseño, formato y presentación de una tabla dinámica aplicando estilos predefinidos, formato de números, diseños de informe y opciones de visualización como mostrar valores como porcentaje del total y subtotales.

### Fundamento teórico

Las tablas dinámicas ofrecen múltiples opciones de personalización que mejoran la legibilidad y el impacto visual de los informes. El diseño de informe puede presentarse en tres formatos principales: Compacto (ahorra espacio mostrando los encabezados de fila en una sola columna), Tabular (similar a una tabla tradicional con cada campo en una columna separada) y Esquemático (con sangrías que indican jerarquías). La elección del diseño depende del público objetivo y del propósito del informe.

El formato de números es esencial para comunicar correctamente la información. Los valores monetarios deben mostrar el símbolo de moneda y dos decimales; los porcentajes requieren el formato de porcentaje; y los números grandes pueden beneficiarse del separador de miles. La opción "Formato de número" en la Configuración de campo de valor permite aplicar estos formatos sin afectar los datos originales.

Mostrar valores como porcentaje del total es una de las funcionalidades más poderosas. Las opciones incluyen: % del total general (cada valor como proporción del total global), % del total de fila (proporción dentro de cada fila) y % del total de columna (proporción dentro de cada columna). Esta capacidad transforma datos absolutos en información relativa, facilitando comparaciones y la identificación de tendencias.

Los estilos predefinidos de tabla dinámica ofrecen combinaciones profesionales de colores y formatos. Es posible personalizar aún más mediante la opción "Nuevo estilo de tabla dinámica", que permite definir formatos específicos para encabezados, filas, columnas y subtotales.

### Procedimiento

1. Abrir el archivo "Practica2_Tablas_Dinamicas_Basicas.xlsx".
2. Seleccionar la tabla dinámica creada.
3. Cambiar el diseño a formato tabular: pestaña Diseño → Diseño de informe → Mostrar en forma tabular.
4. Repetir todos los rótulos de elementos: Diseño → Diseño de informe → Repetir todas las etiquetas de elementos.
5. Desactivar los subtotales: Diseño → Subtotales → No mostrar subtotales.
6. Aplicar formato de moneda a los valores: hacer clic derecho en un valor → Configuración de campo de valor → Formato de número → Moneda → Símbolo $, 2 decimales.
7. Mostrar valores como porcentaje del total: clic derecho en un valor → Mostrar valor como → % del total general.
8. Revertir a suma y aplicar formato de número con separador de miles.
9. Aplicar un estilo predefinido: pestaña Diseño → galería de estilos → seleccionar un estilo de color verde/azul.
10. Cambiar el nombre de la tabla dinámica: pestaña Analizar → Propiedades → Nombre de tabla dinámica → "ResumenVentas".
11. Ajustar el ancho de columnas para que los datos se visualicen correctamente.
12. Guardar el archivo como "Practica3_Formato_Tablas_Dinamicas.xlsx".

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Cambia el diseño de informe a formato tabular | 15% |
| Aplica formato de moneda y separador de miles | 20% |
| Muestra valores como porcentaje del total general | 20% |
| Aplica un estilo predefinido de tabla dinámica | 15% |
| Modifica subtotales y opciones de visualización | 15% |
| Asigna nombre descriptivo a la tabla dinámica | 15% |

---

## Práctica 4: Segmentaciones, escalas de tiempo y filtros

### Objetivo

Al finalizar la práctica, el estudiante será capaz de insertar y configurar segmentaciones de datos y escalas de tiempo, conectarlas a una o más tablas dinámicas, y utilizarlas como herramientas interactivas de filtrado para mejorar la experiencia de análisis.

### Fundamento teórico

Las segmentaciones de datos (Slicers) son controles visuales interactivos que permiten filtrar tablas dinámicas mediante botones, ofreciendo una experiencia más intuitiva que los filtros tradicionales desplegables. Cada botón representa un valor único del campo seleccionado; al hacer clic en uno o varios botones, la tabla dinámica se actualiza instantáneamente para mostrar únicamente los registros correspondientes. Los botones se iluminan en color cuando el valor está seleccionado, y se atenúan cuando no lo está, proporcionando retroalimentación visual inmediata sobre el estado del filtro.

Las escalas de tiempo (Timeline) son controles específicos para campos de fecha que permiten filtrar por períodos de tiempo (días, meses, trimestres o años) mediante un control deslizante interactivo. Son particularmente útiles para análisis temporales donde se necesita explorar tendencias mes a mes o comparar trimestres.

Una de las funcionalidades más potentes es la capacidad de conectar una segmentación o escala de tiempo a múltiples tablas dinámicas simultáneamente. Esto significa que un solo clic puede actualizar varios informes al mismo tiempo, garantizando coherencia en el análisis. Esta conexión múltiple es la base para construir dashboards integrados donde todos los elementos responden sincronizadamente a las selecciones del usuario.

La personalización de segmentaciones incluye: cambio de estilo y color, ajuste del número de columnas de botones, modificación del tamaño y disposición, y reordenación de los valores. Las escalas de tiempo también ofrecen opciones de formato y disposición.

### Procedimiento

1. Crear dos tablas dinámicas en una hoja: una resumiendo ventas por producto y otra resumiendo ventas por vendedor.
2. Seleccionar la primera tabla dinámica.
3. Insertar una segmentación: pestaña Analizar → Insertar segmentación → Seleccionar los campos "Región" y "Categoría".
4. Posicionar las segmentaciones en la hoja, una al lado de la otra, a la izquierda de las tablas.
5. Probar la segmentación: hacer clic en "Norte" en la segmentación de Región y observar cómo se filtran ambas tablas (la segunda tabla aún no se filtra).
6. Conectar la segmentación a ambas tablas: hacer clic derecho en la segmentación → Conexiones de informe → Marcar ambas tablas dinámicas → Aceptar.
7. Verificar que ahora ambas tablas se filtran simultáneamente.
8. Personalizar la segmentación: pestaña Opciones → Cambiar el número de columnas a 2, aplicar un estilo de color.
9. Ajustar el tamaño de los botones desde Opciones → Botones → Alto y Ancho.
10. Insertar una escala de tiempo: seleccionar la tabla dinámica → Analizar → Insertar escala de tiempo → Seleccionar el campo de fecha.
11. Conectar la escala de tiempo a ambas tablas dinámicas.
12. Usar la escala de tiempo para filtrar por mes, trimestre y año.
13. Guardar el archivo como "Practica4_segmentaciones.xlsx".

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Inserta segmentaciones de datos correctamente | 20% |
| Conecta segmentaciones a múltiples tablas dinámicas | 25% |
| Personaliza la apariencia y disposición de las segmentaciones | 15% |
| Inserta y configura una escala de tiempo | 20% |
| Utiliza los controles interactivos para filtrar datos correctamente | 20% |

---

## Práctica 5: Gráficos dinámicos y dashboards

### Objetivo

Al finalizar la práctica, el estudiante será capaz de crear gráficos dinámicos vinculados a tablas dinámicas, personalizar su apariencia, combinar múltiples gráficos y segmentaciones en un dashboard interactivo, y aplicar principios básicos de visualización de datos para comunicar hallazgos de forma efectiva.

### Fundamento teórico

Un gráfico dinámico es una representación visual vinculada directamente a una tabla dinámica. Cualquier cambio en la tabla dinámica se refleja automáticamente en el gráfico, y viceversa. Esta vinculación bidireccional permite explorar visualmente los datos modificando campos, aplicando filtros o usando segmentaciones, con actualización inmediata del gráfico.

Los tipos de gráfico recomendados para tablas dinámicas incluyen: gráficos de columnas (comparación entre categorías), gráficos de líneas (tendencias temporales), gráficos de barras (jerarquías horizontales), gráficos circulares (composición porcentual) y gráficos combinados (columnas + línea para valores y porcentaje simultáneamente). La elección del tipo de gráfico debe basarse en la naturaleza de los datos y la historia que se desea comunicar.

Un dashboard es un conjunto integrado de tablas dinámicas, gráficos dinámicos y segmentaciones organizados en una sola hoja, diseñado para proporcionar una visión general interactiva del negocio. Los principios fundamentales del diseño de dashboards incluyen: disposición lógica de los elementos (de arriba a abajo, de lo general a lo particular), uso consistente de colores, etiquetas claras, y eliminación de elementos innecesarios que generen ruido visual.

La actualización de datos en un dashboard se simplifica cuando el origen es una Tabla de Excel: al agregar nuevos datos a la tabla, solo es necesario hacer clic en "Actualizar" (o presionar Alt + F5) para que todos los elementos del dashboard se actualicen simultáneamente.

### Procedimiento

1. Abrir el archivo "Practica4_segmentaciones.xlsx" o iniciar desde el archivo con datos limpios.
2. Crear una tabla dinámica con Producto en Filas y Total_Venta en Valores.
3. Seleccionar la tabla dinámica → Insertar → Gráfico dinámico → Columna agrupada.
4. Mover el gráfico a una ubicación en la misma hoja.
5. Crear una segunda tabla dinámica con Mes en Filas y Total_Venta en Valores.
6. Insertar un gráfico dinámico de líneas para esta segunda tabla.
7. Crear una tercera tabla dinámica con Categoría en Filas y Total_Venta en Valores.
8. Insertar un gráfico dinámico circular (pastel) o de barras.
9. Insertar segmentaciones para Región y conectar a todos los gráficos.
10. Insertar una escala de tiempo conectada a todos los gráficos.
11. Organizar los elementos en la hoja: segmentaciones en la parte superior, gráficos en una cuadrícula de 2x2.
12. Personalizar títulos de gráficos, colores y formato.
13. Agregar un título general al dashboard usando un cuadro de texto.
14. Probar la interactividad: seleccionar diferentes regiones y períodos; verificar que todos los gráficos se actualicen.
15. Guardar el archivo como "Practica5_Dashboard.xlsx".

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Crea al menos tres gráficos dinámicos de diferentes tipos | 20% |
| Vincula todos los gráficos a los mismos datos de origen | 15% |
| Inserta y conecta segmentaciones a todos los gráficos | 15% |
| Organiza los elementos en un dashboard coherente | 20% |
| Personaliza títulos, colores y formato de los gráficos | 15% |
| El dashboard es funcional e interactivo | 15% |

---

## Práctica 6: Proyecto integrador: análisis completo

### Objetivo

Al finalizar la práctica, el estudiante será capaz de integrar todos los conocimientos adquiridos en las prácticas anteriores para llevar a cabo un análisis completo de un conjunto de datos real, desde la preparación inicial hasta la presentación ejecutiva, demostrando capacidad para tomar decisiones informadas basadas en datos.

### Fundamento teórico

El análisis de datos es un proceso estructurado que comprende varias etapas: definición del problema, recolección de datos, preparación y limpieza, análisis exploratorio, interpretación de resultados y comunicación de hallazgos. Cada etapa es interdependiente y requiere habilidades específicas. La etapa de definición del problema establece qué preguntas se quieren responder, guiando todo el proceso analítico.

La preparación de datos consume aproximadamente el 80% del tiempo en cualquier proyecto de análisis. Incluye la integración de múltiples fuentes, la corrección de errores, el manejo de valores faltantes y la transformación de variables. Una limpieza rigurosa en esta etapa previene errores en etapas posteriores.

El análisis exploratorio mediante tablas dinámicas permite descubrir patrones, tendencias y anomalías. La combinación de múltiples tablas dinámicas, gráficos y filtros interactivos facilita el análisis desde diferentes perspectivas: por producto, región, período, vendedor o cualquier combinación de dimensiones.

La comunicación de resultados es la etapa final y quizás la más importante. Un dashboard bien diseñado permite a los tomadores de decisiones explorar los datos por sí mismos, respondiendo preguntas emergentes sin necesidad de nuevos informes. Las recomendaciones deben estar respaldadas por los datos y presentadas de forma clara y accionable.

Este proyecto integrador simula un escenario real donde el estudiante asume el rol de analista de datos, responsable de transformar datos brutos en información valiosa para la toma de decisiones.

### Procedimiento

1. El docente proporcionará un archivo de datos simulado (ej. "Ventas_Anuales.xlsx" con más de 500 registros, múltiples productos, regiones, vendedores y meses).
2. **Fase 1 - Preparación**: abrir el archivo, identificar problemas de estructura, limpiar datos (espacios, formatos, duplicados), convertir a Tabla de Excel y nombrarla.
3. **Fase 2 - Análisis descriptivo**: crear tablas dinámicas que respondan:
   - a) Ventas totales por producto y mes
   - b) Ventas totales por región y categoría
   - c) Producto más vendido y menos vendido
   - d) Vendedor con mayores ventas
   - e) Tendencia mensual de ventas
4. **Fase 3 - Visualización**: crear un dashboard con:
   - a) Gráfico de columnas: ventas por producto
   - b) Gráfico de líneas: tendencia mensual
   - c) Gráfico de barras: ventas por región
   - d) Segmentaciones para Región, Categoría, Mes
   - e) Escala de tiempo
5. **Fase 4 - Conclusiones**: en una hoja separada, escribir un breve informe (10-15 líneas) con hallazgos principales y al menos 3 recomendaciones basadas en datos.
6. **Fase 5 - Presentación**: preparar el archivo final con formato profesional, nombres claros, sin errores de visualización.
7. Guardar el archivo como "Practica6_Proyecto_Integrador.xlsx".

### Criterios de evaluación

| Criterio | Ponderación |
|----------|-------------|
| Fase 1: Preparación y limpieza completa de datos | 15% |
| Fase 2: Tablas dinámicas correctas que responden las preguntas planteadas | 25% |
| Fase 3: Dashboard funcional con gráficos, segmentaciones y escalas de tiempo | 25% |
| Fase 4: Informe de conclusiones con recomendaciones basadas en datos | 20% |
| Fase 5: Archivo profesional con formato consistente y buena presentación | 15% |

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
