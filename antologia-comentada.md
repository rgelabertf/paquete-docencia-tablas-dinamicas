# ANTOLOGÍA COMENTADA

## Tablas Dinámicas en Excel

**Compilador:** Rolando Gelabert Fernández

**Institución:** Universidad Autónoma del Carmen

**Unidad de Aprendizaje:** Tablas Dinámicas en Excel

**Nivel:** Medio Superior

**Periodo:** Febrero — Julio 2026

**Participantes en la elaboración:**
- Rolando Gelabert Fernández (compilador)

---

## ÍNDICE DE LECTURAS

| No. | Lectura | Pág. |
|-----|---------|------|
| 1 | Historia y evolución de las tablas dinámicas | 1 |
| 2 | Principios de organización de datos | 4 |
| 3 | Del dato a la decisión: análisis con tablas dinámicas | 7 |
| 4 | Visualización de datos: gráficos dinámicos y dashboards | 10 |
| 5 | Excel en el ámbito profesional: competencias digitales | 13 |
| | Bibliografía general | 16 |

---

## INTRODUCCIÓN

La unidad de aprendizaje "Tablas Dinámicas en Excel" está diseñada para estudiantes de nivel medio superior que buscan desarrollar competencias digitales aplicadas al análisis de datos. En un mundo donde la información se genera exponencialmente, la capacidad de transformar datos en conocimiento útil se ha convertido en una habilidad transversal indispensable.

La presente antología comentada reúne cinco lecturas que abordan, desde distintas perspectivas, los fundamentos teóricos, metodológicos y prácticos de las tablas dinámicas. Cada texto ha sido seleccionado y comentado con la intención de ofrecer al estudiante no solo el conocimiento técnico necesario, sino también una visión crítica sobre el papel de estas herramientas en la toma de decisiones.

Los textos recorren un arco formativo completo: desde los orígenes históricos de las tablas dinámicas (lectura 1), pasando por la importancia de la organización de los datos (lectura 2), hasta su aplicación en análisis concretos (lectura 3), su visualización (lectura 4) y su relevancia en el ámbito profesional (lectura 5). Cada lectura incluye una valoración crítica del compilador y una nota explícita sobre cómo contribuye a los objetivos del curso.

Esta antología cumple con los lineamientos establecidos en el indicador 1.2.2 del Cuadernillo ESDEPED UNACAR (2025-2026) y constituye un material de apoyo para el Paquete para la Docencia de la unidad de aprendizaje.

---

## LECTURA 1

### Historia y evolución de las tablas dinámicas

**Datos de la fuente:**

Gelabert Fernández, R. (2026). *Historia y evolución de las tablas dinámicas*. En *Antología comentada: Tablas Dinámicas en Excel* (pp. 1-3). Universidad Autónoma del Carmen.

---

**Texto de la lectura**

Las tablas dinámicas, conocidas en inglés como *PivotTables*, son hoy una de las herramientas más poderosas de Excel, pero su origen se remonta a décadas antes de que Microsoft las integrara en su paquete ofimático. Comprender su evolución ayuda a apreciar no solo su funcionamiento, sino también la filosofía de diseño que las sustenta.

El concepto de "tabla dinámica" fue desarrollado originalmente por Pito Salas, un ingeniero de software que trabajaba en Lotus Development Corporation. En 1986, Salas creó una funcionalidad para Lotus Improv, un programa de hojas de cálculo orientado a la planificación financiera. La innovación radical de Improv era que separaba los datos de su presentación: el usuario podía definir dimensiones (filas y columnas) y luego arrastrarlas para reorganizar la vista sin modificar los datos subyacentes.

Lotus Improv se lanzó en 1991 exclusivamente para la plataforma NeXT, lo que limitó su difusión. Sin embargo, Microsoft observó el potencial de la idea. En 1993, la compañía de Redmond lanzó Excel 5.0, que incluía por primera vez una funcionalidad denominada *PivotTable*. La implementación inicial era modesta: permitía resumir datos en una cuadrícula arrastrando campos, pero carecía de muchas de las características que hoy damos por sentadas.

La adopción de las tablas dinámicas creció lentamente durante los años noventa. Muchos usuarios las consideraban complejas y preferían usar funciones como SUMAR.SI o BDSUMA para obtener resultados similares. No fue sino hasta Excel 2003 que Microsoft introdujo mejoras significativas en la interfaz, y con Excel 2007 la herramienta experimentó una transformación radical. La cinta de opciones (*Ribbon*) reemplazó los menús tradicionales, y la creación de tablas dinámicas se simplificó drásticamente. Aparecieron también los estilos predefinidos, las segmentaciones (introducidas en Excel 2010) y las escalas de tiempo (Excel 2013).

A partir de Excel 2016, las tablas dinámicas se integraron con el motor Power Pivot, permitiendo trabajar con conjuntos de datos mucho más grandes que el límite tradicional de filas de Excel. Esta integración marcó un punto de inflexión: las tablas dinámicas dejaron de ser una herramienta para datos "pequeños" y se convirtieron en un componente legítimo de las soluciones de *Business Intelligence*.

En la actualidad, Excel 365 ofrece tablas dinámicas con capacidades de inteligencia artificial, como la sugerencia automática de campos y la detección de patrones. Herramientas como "Analizar datos" (antes "Ideas") utilizan machine learning para proponer visualizaciones y resúmenes relevantes. El ciclo iniciado por Pito Salas en 1986 se cierra con una paradoja interesante: la herramienta que nació para facilitar el análisis manual de datos hoy se potencia con algoritmos que automatizan precisamente esa labor.

---

**Comentario crítico del compilador**

Esta lectura cumple una función fundamental en la antología: contextualizar. El estudiante de nivel medio superior suele acercarse a las tablas dinámicas como una herramienta técnica más, sin comprender la lógica de diseño que las sustenta. Conocer la historia —desde Lotus Improv hasta las capacidades de IA de Excel 365— permite al alumno entender que las tablas dinámicas no son un accidente, sino el resultado de décadas de evolución en el pensamiento sobre el análisis de datos. El texto está escrito en un tono accesible, aunque sacrifica profundidad técnica en algunos pasajes (por ejemplo, la explicación del motor Power Pivot podría ampliarse). Habría sido deseable incluir referencias a las críticas que recibió la herramienta en sus primeras versiones, particularmente la curva de aprendizaje pronunciada que alejó a muchos usuarios. No obstante, como pieza introductoria cumple su cometido.

**Contribución a los objetivos del curso**

Esta lectura contribuye directamente al objetivo de "Identificar el origen y propósito de las tablas dinámicas como herramienta de análisis". Proporciona el marco histórico necesario para que el estudiante valore la relevancia de la herramienta antes de aprender a usarla, situándola en el contexto más amplio de la evolución del software de análisis de datos.

---

## LECTURA 2

### Principios de organización de datos

**Datos de la fuente:**

Gelabert Fernández, R. (2026). *Principios de organización de datos*. En *Antología comentada: Tablas Dinámicas en Excel* (pp. 4-6). Universidad Autónoma del Carmen.

---

**Texto de la lectura**

Uno de los errores más frecuentes entre quienes inician en el análisis de datos es subestimar la importancia de la organización previa. Se suele pensar que la herramienta de análisis —en este caso, la tabla dinámica— resolverá cualquier desorden en los datos. La realidad es exactamente la opuesta: la calidad del análisis depende directamente de la calidad de la organización de los datos fuente. Este principio, conocido como "basura entra, basura sale" (*garbage in, garbage out*), es fundamental en cualquier disciplina que trabaje con información cuantitativa.

Los datos aptos para tablas dinámicas deben cumplir con una serie de condiciones que la literatura especializada denomina "datos tabulares" o "datos normalizados". Una tabla normalizada se caracteriza por las siguientes propiedades:

En primer lugar, cada columna representa una variable. Es decir, los encabezados de columna deben ser nombres de campos (por ejemplo: "Producto", "Región", "Ventas", "Fecha"), no valores de datos. Un error común es tener columnas como "Enero", "Febrero", "Marzo", etc., donde los meses son valores y no variables. Este formato, llamado "ancho", debe transformarse a formato "largo" antes de crear la tabla dinámica.

En segundo lugar, cada fila representa una observación o transacción única. No deben existir filas vacías ni filas de totales dentro de los datos fuente. Los totales se generan automáticamente en la tabla dinámica, por lo que incluirlos en los datos de origen produce duplicaciones y resultados incorrectos.

En tercer lugar, las celdas combinadas están terminantemente prohibidas en los datos fuente. Si bien Excel permite combinar celdas por razones estéticas, esta práctica destruye la estructura tabular necesaria para el análisis. Una celda combinada en los encabezados impide que Excel identifique correctamente los nombres de campo.

Además de estas condiciones estructurales, existen recomendaciones prácticas que facilitan el trabajo. Convertir el rango de datos en una "Tabla de Excel" (Ctrl + T) es quizás la más importante. Una Tabla de Excel ofrece ventajas decisivas: los nuevos datos agregados al final se incluyen automáticamente en el rango de la tabla dinámica, los encabezados permanecen visibles al desplazarse, y las fórmulas se replican automáticamente.

Otra recomendación esencial es la consistencia en los datos. Un mismo concepto debe escribirse siempre de la misma forma. Por ejemplo, si en una celda aparece "CDMX" y en otra "Ciudad de México", la tabla dinámica los tratará como dos categorías distintas, fragmentando el análisis. Herramientas como la validación de datos y los menús desplegables ayudan a mantener esta consistencia.

Finalmente, se recomienda documentar la estructura de los datos. Un diccionario de datos sencillo —que describa cada columna, su tipo de dato y los valores esperados— es una práctica profesional que ahorra horas de confusiones, especialmente cuando se trabaja en equipo.

---

**Comentario crítico del compilador**

Esta lectura aborda el eslabón más débil en la formación de estudiantes de nivel medio superior: la cultura del dato. Con frecuencia, los alumnos cuentan con habilidades técnicas para operar el software, pero carecen de criterio para juzgar si sus datos están en condiciones de ser analizados. El texto expone con claridad los principios de normalización, aunque utiliza una terminología que podría resultar árida para el estudiante promedio. Sería recomendable complementar esta lectura con un ejercicio práctico donde se presenten datos "sucios" y se pida al alumno que los limpie. El texto menciona la validación de datos y los menús desplegables, pero no profundiza en cómo implementarlos, lo cual es una oportunidad perdida. No obstante, la lectura sienta las bases conceptuales necesarias para que el estudiante entienda que el análisis no comienza en la tabla dinámica, sino en la hoja de cálculo donde se capturan los datos.

**Contribución a los objetivos del curso**

Esta lectura apoya directamente el objetivo de "Preparar y organizar datos fuente para la creación de tablas dinámicas". Al comprender los principios de organización tabular, el estudiante podrá estructurar sus datos correctamente desde el inicio, evitando los errores más comunes que invalidan los análisis posteriores.

---

## LECTURA 3

### Del dato a la decisión: análisis con tablas dinámicas

**Datos de la fuente:**

Gelabert Fernández, R. (2026). *Del dato a la decisión: análisis con tablas dinámicas*. En *Antología comentada: Tablas Dinámicas en Excel* (pp. 7-9). Universidad Autónoma del Carmen.

---

**Texto de la lectura**

La verdadera utilidad de una tabla dinámica no reside en su capacidad para resumir datos, sino en su potencial para transformar resúmenes en decisiones informadas. Esta lectura presenta un caso práctico comentado que ilustra el recorrido desde los datos brutos hasta una recomendación accionable.

**Caso: Análisis de ventas de una cadena de papelerías**

Imaginemos una pequeña cadena de papelerías con tres sucursales (Centro, Norte, Sur) que vende cinco categorías de productos (Cuadernos, Bolígrafos, Mochilas, Calculadoras, Papel). Los datos de un trimestre incluyen 1,200 transacciones con campos: Fecha, Sucursal, Categoría, Producto, Cantidad, Precio Unitario, Total.

El gerente quiere responder cuatro preguntas:
1. ¿Qué sucursal genera mayores ingresos?
2. ¿Qué categoría de producto tiene mayor margen?
3. ¿Existe un patrón estacional en las ventas?
4. ¿Qué producto debería promocionarse?

*Paso 1: Creación de la tabla dinámica.* Se seleccionan los datos y se inserta una tabla dinámica (Insertar → Tabla dinámica). En el panel de campos, se arrastra "Sucursal" a Filas y "Total" a Valores. El resultado muestra que la sucursal Centro genera el 45 % de los ingresos, seguida de la Sur (32 %) y la Norte (23 %).

*Paso 2: Profundización con segmentaciones.* Se agrega una segmentación por "Categoría". Al seleccionar "Mochilas", se descubre que la sucursal Norte, que en volumen total es la menor, lidera en ventas de mochilas con el 48 % del total de esa categoría. Este hallazgo contradice la primera impresión y sugiere que cada sucursal tiene un perfil distinto de cliente.

*Paso 3: Análisis temporal.* Se arrastra "Fecha" a Filas y se agrupa por meses (clic derecho → Agrupar → Meses). Se observa que las ventas de cuadernos se concentran en enero y agosto (inicios de ciclo escolar), mientras que las calculadoras tienen demanda constante. Este patrón permite planificar inventarios.

*Paso 4: Cálculos personalizados.* Se agrega nuevamente "Total" a Valores y se cambia la configuración para mostrar "% del total general". Esto revela que las mochilas representan el 35 % de los ingresos totales pero solo el 15 % de las unidades vendidas, lo que indica que son productos de alto valor unitario.

*Paso 5: Decisión informada.* Con estos datos, el gerente decide: (a) lanzar una promoción de mochilas en la sucursal Centro, donde el ticket promedio es más alto; (b) reforzar el inventario de cuadernos en todas las sucursales antes de enero; y (c) investigar por qué la sucursal Norte tiene menor volumen general, utilizando la tabla dinámica para desglosar por categoría y detectar oportunidades.

Este caso demuestra que el valor de la tabla dinámica no está en los números que produce, sino en las preguntas que permite responder. Cada reordenamiento de campos es una nueva hipótesis puesta a prueba.

---

**Comentario crítico del compilador**

Esta es, probablemente, la lectura más valiosa de la antología desde un punto de vista pedagógico. Al presentar un caso concreto con preguntas explícitas y pasos numerados, el texto tiende un puente entre la teoría y la práctica. El enfoque en la toma de decisiones —y no solo en la operación técnica— eleva el nivel del aprendizaje. Sin embargo, el caso resulta un tanto idealizado: en la vida real, los datos rara vez vienen limpios y completos como en el ejemplo. Se echa de menos una discusión sobre cómo manejar datos faltantes o valores atípicos durante el análisis. Además, el texto supone que el lector ya conoce la interfaz de Excel, lo que podría excluir a principiantes absolutos. Aun así, la estructura de pregunta-análisis-decisión es un modelo pedagógico que los estudiantes pueden replicar en sus propios contextos.

**Contribución a los objetivos del curso**

Esta lectura se vincula directamente con los objetivos "Crear tablas dinámicas para resumir y analizar información" y "Utilizar los resultados del análisis para fundamentar la toma de decisiones". El caso práctico ofrece un modelo replicable que integra las habilidades técnicas con el pensamiento analítico.

---

## LECTURA 4

### Visualización de datos: gráficos dinámicos y dashboards

**Datos de la fuente:**

Gelabert Fernández, R. (2026). *Visualización de datos: gráficos dinámicos y dashboards*. En *Antología comentada: Tablas Dinámicas en Excel* (pp. 10-12). Universidad Autónoma del Carmen.

---

**Texto de la lectura**

Una tabla dinámica puede contener toda la información necesaria para una decisión, pero si esa información no se comunica de manera efectiva, su impacto se diluye. La visualización de datos —el arte de presentar información cuantitativa de forma gráfica— es el complemento indispensable de cualquier análisis. Como señaló el pionero Edward Tufte, la excelencia en visualización consiste en "comunicar ideas complejas con claridad, precisión y eficiencia".

**Gráficos dinámicos**

Un gráfico dinámico es una representación visual vinculada directamente a una tabla dinámica. Cuando se modifica la tabla (al filtrar, agrupar o reorganizar campos), el gráfico se actualiza automáticamente. Esta sincronización es su principal ventaja: elimina la necesidad de recrear gráficos manualmente cada vez que cambian los datos.

Excel ofrece varios tipos de gráficos dinámicos. Los más utilizados en el análisis de negocios son: gráficos de columnas (para comparar categorías), gráficos de líneas (para tendencias temporales), gráficos circulares (para proporciones, aunque conviene usarlos con moderación) y gráficos de barras apiladas (para composición y comparación simultánea).

La selección del tipo de gráfico no es un asunto estético, sino funcional. Un error frecuente es usar gráficos circulares para comparar muchas categorías (más de cinco), lo que dificulta la percepción de las diferencias. En su lugar, un gráfico de barras ordenado de mayor a menor permite una lectura más precisa.

**Dashboards en Excel**

Un dashboard (tablero de control) es un conjunto integrado de visualizaciones que permite monitorear indicadores clave de un vistazo. En Excel, los dashboards se construyen combinando tablas dinámicas, gráficos dinámicos, segmentaciones y escalas de tiempo.

Los principios de diseño de dashboards incluyen:

1. **Jerarquía visual:** la información más importante debe ocupar la posición superior izquierda (donde la mirada se posa primero). Los detalles secundarios van hacia la derecha y abajo.

2. **Coherencia cromática:** usar una paleta limitada de colores (5 a 7 máximo) y aplicarla consistentemente. El color debe comunicar, no decorar. El verde suele asociarse con valores positivos y el rojo con valores negativos.

3. **Minimalismo:** eliminar todo elemento que no aporte información. Líneas de cuadrícula innecesarias, etiquetas redundantes y efectos 3D distraen sin añadir valor.

4. **Interactividad:** las segmentaciones y escalas de tiempo permiten al usuario explorar los datos por su cuenta. Un buen dashboard no cuenta una sola historia, sino que permite al usuario descubrir múltiples narrativas.

5. **Contexto:** los números aislados no significan nada. Incluir referencias como metas, promedios históricos o benchmarks del sector permite interpretar si un valor es bueno o malo.

**Recomendaciones finales**

El dashboard perfecto no existe, pero uno útil sí puede construirse siguiendo estos principios. La clave está en conocer a la audiencia: un dashboard para un director general debe responder "¿qué pasó?" con una mirada de segundos, mientras que uno para un analista debe permitir "¿por qué pasó?" mediante la exploración interactiva.

---

**Comentario crítico del compilador**

Esta lectura complementa adecuadamente las habilidades técnicas de creación de tablas dinámicas con la dimensión comunicativa del análisis. El texto presenta principios de diseño visual con claridad, aunque su extensión limitada impide profundizar en la implementación práctica dentro de Excel. Un aspecto que merece crítica es la ausencia de ejemplos visuales concretos: un texto sobre visualización se beneficiaría enormemente de incluir imágenes o descripciones detalladas de dashboards reales. Además, la referencia a Tufte es pertinente pero brevísima; una cita más sustancial de su obra enriquecería el marco conceptual. El texto también pasa por alto herramientas de visualización complementarias que los estudiantes podrían explorar, como Power BI o Google Data Studio, que aunque están fuera del alcance del curso, ampliarían su horizonte formativo. En conjunto, la lectura cumple su propósito de sensibilizar al estudiante sobre la importancia de la comunicación visual.

**Contribución a los objetivos del curso**

Esta lectura apoya el objetivo "Crear gráficos dinámicos a partir de tablas dinámicas para la comunicación visual de resultados". Proporciona los principios de diseño que permitirán al estudiante no solo generar gráficos, sino hacerlo con criterio profesional, maximizando el impacto comunicativo de sus análisis.

---

## LECTURA 5

### Excel en el ámbito profesional: competencias digitales

**Datos de la fuente:**

Gelabert Fernández, R. (2026). *Excel en el ámbito profesional: competencias digitales*. En *Antología comentada: Tablas Dinámicas en Excel* (pp. 13-15). Universidad Autónoma del Carmen.

---

**Texto de la lectura**

En un mercado laboral cada vez más competitivo y digitalizado, el manejo de Excel —y específicamente de tablas dinámicas— se ha convertido en un diferenciador profesional relevante. Diversos estudios de competencias laborales coinciden en que el análisis de datos es una de las habilidades más demandadas, independientemente del sector o del nivel jerárquico.

**La demanda de competencias digitales**

El Foro Económico Mundial, en su reporte *Future of Jobs 2025*, identifica el pensamiento analítico y el manejo de tecnología como dos de las competencias principales para los trabajadores de esta década. Dentro del espectro de herramientas tecnológicas, Excel ocupa un lugar destacado por su ubicuidad: está presente en más del 80 % de las empresas a nivel global, desde pequeñas PyMEs hasta corporaciones multinacionales.

Según datos de LinkedIn, la competencia "Excel avanzado" aparece entre las diez habilidades más mencionadas en perfiles profesionales de administración, finanzas, logística, marketing y recursos humanos. El dominio de tablas dinámicas es, precisamente, uno de los indicadores que distinguen un nivel "intermedio" de uno "avanzado".

**¿Qué buscan los empleadores?**

No se trata solo de saber dónde hacer clic. Los empleadores buscan profesionales capaces de:

- **Transformar datos en información:** la capacidad de tomar un conjunto de datos brutos y extraer conclusiones accionables es transferible a cualquier función. Un analista de ventas que identifica patrones estacionales, un administrador que detecta desviaciones presupuestarias y un gerente de recursos humanos que analiza tendencias de rotación están, en esencia, haciendo lo mismo: usando tablas dinámicas para convertir datos en decisiones.

- **Comunicar hallazgos con claridad:** la tabla dinámica es el puente entre el dato y la presentación ejecutiva. Un profesional que presenta un análisis respaldado por tablas dinámicas y gráficos dinámicos comunica rigurosidad y preparación.

- **Automatizar procesos repetitivos:** el conocimiento de tablas dinámicas permite reducir horas de trabajo manual. Una tarea que toma un día completo con filtros manuales y sumas individuales puede resolverse en minutos con una tabla dinámica bien configurada.

- **Adaptarse a nuevas herramientas:** quien comprende la lógica de las tablas dinámicas —campos, valores, filtros, relaciones— puede transferir ese conocimiento a herramientas más avanzadas como Power BI, Tableau o Google Data Studio. La tabla dinámica es, en este sentido, una puerta de entrada al ecosistema del *Business Intelligence*.

**La certificación como valor agregado**

Microsoft ofrece la certificación *Microsoft Office Specialist (MOS): Excel Associate*, que incluye la creación y modificación de tablas dinámicas como uno de los dominios evaluados. Obtener esta certificación representa una ventaja competitiva tangible para estudiantes que buscan incorporarse al mercado laboral.

**Conclusión**

Dominar las tablas dinámicas no es un fin en sí mismo, sino un medio para desarrollar una competencia más amplia: la capacidad de pensar analíticamente con datos. En un mundo donde la información abunda pero el conocimiento escasea, quienes saben extraer significado de los números llevan una ventaja decisiva.

---

**Comentario crítico del compilador**

Esta lectura cierra la antología con una perspectiva motivacional y profesionalizante que resulta particularmente útil para estudiantes de nivel medio superior que están definiendo su rumbo académico y laboral. La conexión entre el dominio técnico de Excel y las competencias demandadas por el mercado laboral está bien argumentada, y las referencias al *Future of Jobs* y a LinkedIn aportan credibilidad. Sin embargo, el texto incurre en un optimismo un tanto acrítico: no menciona las limitaciones de Excel frente a herramientas más modernas ni discute la creciente automatización que podría reducir la demanda de competencias manuales en Excel. Tampoco aborda la brecha digital que enfrentan muchos estudiantes que no tienen acceso a licencias de Office o a equipos actualizados. La lectura ganaría profundidad si reconociera estas tensiones y ofreciera una visión más equilibrada. Aun así, como cierre de la antología, cumple su función de motivar al estudiante y conectar el aprendizaje del curso con sus aspiraciones profesionales.

**Contribución a los objetivos del curso**

Esta lectura contribuye a los objetivos transversales del curso: "Reconocer la importancia de las tablas dinámicas en el ámbito profesional" y "Desarrollar competencias digitales aplicables al entorno laboral". Proporciona la motivación contextual necesaria para que el estudiante valore el curso no como un requisito administrativo, sino como una inversión en su desarrollo profesional.

---

## BIBLIOGRAFÍA GENERAL

Caballero, M. & Torres, F. (s.f.). *Tablas dinámicas: la quinta dimensión* (1.ª ed.). [Documento PDF]. Incluido en el Paquete para la Docencia.

Daxus Latam. (2025). *Aprende a crear tablas dinámicas desde cero (con ejemplos)* [Video]. YouTube. https://www.youtube.com/watch?v=WGH-k_vURuE

El Tío Tech. (2021). *6 ejercicios de tablas dinámicas para practicar*. El Tío Tech. https://eltiotech.com/6-ejercicios-tablas-dinamicas

El Tío Tech. (2025). *Domina las tablas dinámicas en Excel desde cero* [Video]. YouTube. https://www.youtube.com/watch?v=tN6_ZEaqYBo

Excel Total. (2021). *Tablas dinámicas en Excel (tutorial completo)*. Excel Total. https://exceltotal.com/tablas-dinamicas-en-excel

Foro Económico Mundial. (2025). *Future of Jobs Report 2025*. World Economic Forum.

Gelabert Fernández, R. (2026). *Fuentes originales del cuaderno: conceptos básicos, tutorial práctico, técnicas avanzadas, gráficos dinámicos, errores comunes* [Material inédito]. Universidad Autónoma del Carmen.

Microsoft. (s.f.). *Crear una tabla dinámica para analizar datos de una hoja de cálculo*. Microsoft Support. https://support.microsoft.com/es-es/office/crear-una-tabla-din%C3%A1mica-para-analizar-datos-de-una-hoja-de-c%C3%A1lculo-a9a84538-bfe9-40a9-a8e9-f99134456576

Ninja Excel. (2024). *Cómo hacer tablas dinámicas en Excel: paso a paso*. Ninja Excel. https://www.ninjaexcel.com/excel-en-el-trabajo/tablas-dinamicas

Saber Programas. (2024). *Tablas dinámicas en Excel de cero a experto* [Video]. YouTube. https://www.youtube.com/watch?v=6YOsIVH0STg

SMARTpro Academy. (s.f.). *Cómo hacer tablas dinámicas en Excel + IA desde cero* [Video]. YouTube. https://www.youtube.com/watch?v=Mh93eaKbkkw

Tufte, E. (2001). *The Visual Display of Quantitative Information* (2.ª ed.). Graphics Press.

---

*Compilado por Rolando Gelabert Fernández — Universidad Autónoma del Carmen — 2026*
