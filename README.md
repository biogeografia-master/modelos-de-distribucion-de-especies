Práctica de desarrollo 4. PD04. Modelos de distribución de especies
(SDM) por medio de aprendizaje automático (*machine
learning*)<small><br>Biogeografía (GEO-131)<br>Universidad Autónoma de
Santo Domingo (UASD)<br>Semestre 2024-02</small>
================
El Tali
2024-10-30

<!-- README.md se genera a partir de README.Rmd. Por favor, edita ese archivo. -->

Versión HTML (quizá más legible),
[aquí](https://biogeografia-master.github.io/modelos-de-distribucion-de-especies/README.html)

# Fecha/hora de entrega

**12 de noviembre de 2024, 11:59 pm.**

# Objetivos

# Mandato

1.  **Acepta la asignación, genera tu repositorio personalizado y
    clónalo en tu cuenta del servidor RStudio**. Este paso sigue el
    procedimiento estándar que aprendiste en PD anteriores. De todas
    formas, te lo refresco de forma resumida. Primero ve al [portal de
    la asignatura](https://github.com/biogeografia-202402), haz clic en
    el enlace de la PD04 y acepta la asignación. Se creará un
    repositorio personalizado en la [organización
    biogeografia-202402](https://github.com/biogeografia-202402). El
    nombre de tu repo personalizado normalmente será algo tal que: “base
    del repo” + “tu nombre de usuario de GitHub” (como sufijo). Clona tu
    repositorio personalizado en el servidor RStudio. Para ello, deberás
    acceder al servidor con tus credenciales, copiar la ruta en GitHub
    de tu repo personalizado (botón verde `Code` en GitHub) y realizar
    el procedimiento estándar de nuevo proyecto con control de versiones
    en RStudio.

2.  **REPRODUCE EL VÍDEO DE APOYO** para comprender el código de Python
    y sus resultados. Tienes un vídeo de apoyo exclusivo para esta
    práctica, disponible [aquí](). El vídeo explica cómo realizar, y en
    qué consisten, los análisis necesarios para modelizar distribución
    de especies usando algoritmos de *machine learning* en Python, con
    aplicación a la especie *Pinus occidentalis* en República
    Dominicana.

3.  Elige una especie en GBIF bien representada en República Dominicana.
    Esta fase es de exploración, así que usa mejor la [interfaz web de
    GBIF](https://gbif.org). “Bien representada” es difícil de definir,
    pero son elegibles aquellas especies con entre 200 y 500 registros
    de presencia. Si no logras una especie con un número de registros en
    ese rango, pues elige una que al menos tenga 100 registros. Lo más
    importante es que la especie elegida no tenga todos sus registros
    concentrados en un pequeño cúmulo. No se trata de elegir una especie
    que esté en todas partes, sino de una que tenga muchos registros
    bien distribuidos. Si notas que la especie candidata sigue el mismo
    patrón que el de alguna variable climática, de uso y cobertura,
    geológica o fisiográfica, es válida para la elección. Puedes
    preguntar al ChatGPT, aunque normalmente dicho LLM no acierta bien
    con los criterios.

4.  **IMPORTANTE**. Anuncia tu elección en el foro; si ya está elegida,
    deberás elegir otra.

5.  Inicia sesión en el servidor JupyterHub. Sube sólo los siguientes
    archivos a tu cuenta de JupyterHub (las cuentas del servidor de
    RStudio y de JupyterHub son independientes), tomándolos desde tu
    propio repo (los puedes obtener descárgandolos desde tu repo en
    GitHub, o desde el clon que tienes en el servidor de RStudio, y
    posteriormente subiéndolos a tu cuenta de JupyterHub):

    - Archivo: `modelos-de-distribucion-de-especies-SDM.ipynb`. Es un
      cuaderno Jupyter, que contiene el desarrollo de Modelos de
      distribución de especies (SDM) por medio de aprendizaje automático
      (*machine learning*) con plicación a *Pinus occidentalis*. El
      nombre de archivo es largo, así que coloca el puntero del ratón
      momentáneamente sobre cualquier archivo que comience por
      “modelos…” y verifica el nombre completo del archivo en el
      *tooltip* flotante.
    - Archivo: `all_sources_all_variables_res_7.gpkg`. Es un archivo
      GeoPackage, conteniendo más de 130 variables ambientales generadas
      por estadística zonal, referidas al índices espacial H3 a
      resolución 7 (hexágonos de aproximadamente 3.8 km<sup>2</sup>) y
      datos geoespaciales del catálogo de Earth Engine.

    Estos archivos te servirán para ver el ejemplo desarrollado por mí.
    En el cuaderno verás cómo realicé la predicción de distribución
    potencial de *Pinus occidentalis*. Usa dicho cuaderno base para
    adaptarlo a tu especie elegida. Te recomiendo que intentes
    comprender la lógica del código, sin perderte en los detalles; el
    vídeo será de gran ayuda en esta parte. Sin embargo, es importante
    que intentes ejecutar, celda a celda, el código de Python (recuerda
    **desactivar el traductor** para el servidor). Intentar comprender
    el código también es importante, pero puede resultar abrumador.
    Concéntrate en adaptar el código del cuaderno a tu especie elegida,
    controlando en todo momento los resultados obtenidos y editando las
    líneas allí donde tengas que hacerlo (no son muchos los lugares
    realmente que necesitas personalizar), sobre él propio cuaderno.
    Recuerda que el código sigue una lógica secuencial, por lo que los
    bloques posteriores dependerán de los anteriores.

6.  Revisa bibliografía sobre los algoritmos de predicción empleados (el
    ejemplo es una buena base, pero puedes incluir otras técnicas). No
    puedes usar estos algoritmos sin saber de qué tratan, aunque no
    tienes por qué entrar en los detalles. Los parámetros de
    configuración de los algoritmos, así como el criterio de selección
    de un algoritmo sobre otro, son extremadamente importantes. Eso sí,
    la bibliografía sobre este tema es muy densa, pero te recomiendo que
    consultes tanto libros como artículos científicos con casos de uso.

7.  **Finalmente, regresa a RStudio y redacta un manuscrito**. Para el
    procesamiento de tu texto y la redacción de tus análisis, usa la
    plantilla `manuscrito-modelos-de-distribucion-de-especies-SDM.Rmd`,
    que se encuentra en este mismo repositorio. Con esta plantilla
    generarás un PDF que tejeras a usando RStudio. Deberás usar estilos
    de formato (los títulos debidamente escritos, el texto normal
    también, siguiendo lo aprendido en las PD anteriores), referencias
    bibliográficas, referencias cruzadas a figuras y tablas (es decir,
    necesitarás que las figuras y tablas tengan título o “*caption*”).
    No podrás desarrollar tu redacción usando listas de viñetas ni
    listas numeradas. Debes usar la plantilla mencionada en RStudio,
    preferiblemente en mi servidor, tal como hiciste en las PD
    anteriores. Cuando termines tu manuscrito con tus análisis
    reproducibles, y lo tejas a PDF, no olvides hacer commit\>push de
    todos tus cambios para subirlos a GitHub. Esta vez, sólo usarás
    RStudio para integrar los resultados, especialmente para incluir los
    gráficos y mapas resultantes que generaste en JupyterHub (puedes
    descargar las figuras que generaste en el cuaderno de JupyterHub y
    subirlas a RStudio). Necesitarás citar bibliografía, no lo podrás
    evitar, tanto en la introducción, como en la metodología y la
    discusión. No olvides citar los datos de GBIF; en su página
    encontrarás métodos para ello.

Distribuye tu texto en las siguientes secciones:

- **Introducción** (tamaño recomendado: 3 párrafos). Desde lo amplio,
  puedes comenzar escribiendo sobre GBIF y su potencial, el repositorio
  de estadística zonal de RD (Martínez-Batlle, 2022), así como sobre la
  especie elegida y su importancia para RD o la isla. A continuación,
  explica en qué consisten la modelización de distribución de especies
  que aplicarás, en este caso, usando algoritmos de *machine learning*,
  destacando su importancia, por qué son útiles y que los hace
  especiales respecto de otros modelos. Plantea tu o tus objetivos, que
  en este caso están algo acotados. Cierra con la importancia que
  reviste la aplicación de la modelización de distribución para la
  especie elegida respecto del conjunto de la ciencia.

  - Dentro de esta sección, debes incluir al menos cinco citas. Los
    conceptos y afirmaciones ajenas, deben citarse bibliográficamente, y
    nunca deberás usar cita textual, pues se considera plagio. Las citas
    bibliográficas que incluyas, deberán estar respaldadas por su
    correspondiente lista referencias, la cual deberá aparecer en la
    sección final (Referencias); el propio tejido de RMarkdown debería
    generarla por ti, siempre que sigas las instrucciones
    correspondientes (vuelve al vídeo de la PD01 para refrescar). Las
    citas y la lista de referencias, deberán seguir el estándar APA 7ma
    edición (APA7), que es el que la propia plantilla tiene configurado
    por defecto; en principio, no tendrás que ocuparte de todos los
    detalles de sintaxis del formato APA7, pero no debes confiar
    ciegamente en lo que hace RMarkdown.

- **Materiales y métodos** (tamaño recomendado: cuatro párrafos).
  Explica cómo obtuviste los datos que usaste, y documenta en qué
  consiste la fuente (no sólo los datos de presencia de GBIF, sino
  también los de variables ambientales). Los registros de presencia de
  este ejercicio se generaron con el cuaderno
  `modelos-de-distribucion-de-especies-SDM.ipynb`, el cual ya habrás
  aplicado a tu especie y que se encuentra en este mismo repo. Debes
  citar específicamente GBIF, usando la recomendación que ofrecen en su
  página web. Debes citar el repo de estadística zonal, de donde vino el
  archivo de variables ambientales
  `all_sources_all_variables_res_7.gpkg`; dicho repo se encuentra en
  [este enlace](https://github.com/geofis/zonal-statistics), y dispone
  de una entrada BiTeX para ayudarte con la cita
  [aquí](https://github.com/geofis/zonal-statistics?tab=readme-ov-file#entrada-bibtex).

Debes igualmente citar el software y hardware usado, y las referencias
sobre la técnica o algoritmo empleados. Ten presente que la bibliografía
sobre *machine learning* en Python es muy pero que muy densa, así que
deberás hacer una selección apropiada. Si incluyes un diagrama de flujo
metodológico (“metodología gráfica”), te resultará más fácil explicar tu
metodología. **No adelantes resultados, sólo escribe qué fuentes y
herramientas usaste (materiales), qué técnicas concretas o algoritmos
utilizaste (métodos), y qué configuraciones aplicaste a los
algoritmos**. Toda figura y tabla que insertes debe citarse con
referencia cruzada, para lo cual dispones de una guía con ejemplos al
final de la plantilla de manuscrito (archivo:
`manuscrito-modelos-de-distribucion-de-especies-SDM.Rmd`).

- **Resultados** (tamaño recomendado: 4 párrafo). Los registros de
  presencia obtenidos, su número, sus descriptores básicos de posición y
  distribución, las variables ambientales y su relación con los
  registros de presencia y pseudoausencias, las predicciones obtenidas
  según cada algoritmo, descritas usando orientaciones cardinales y
  referencias geográficas. No hagas valoraciones en esta sección,
  simplemente incluye los resultados obtenidos.

- **Discusión** (tamaño recomendado: 4 párrafos). Abre la discusión
  indicando si alcanzaste tus objetivos. Describe por qué era importante
  alcanzarlos. Interpreta los resultados, e indica cuál de las
  modelizaciones se acerca más a lo que se esperaría, y/o cuáles
  modelizaciones ofrecen resultados poco fiables. Interpreta por qué, sí
  aplica, la probabilidad de presencia (o la presencia predicha en sí
  misma, dependiendo del enfoque que hayas usado), no concuerda en
  determinados lugares, o por qué concuerda en muchos lugares,
  apoyándote en el poder predictivo que, según entiendas, tienen
  determinadas variables ambientales. Comenta sobre las limitaciones, de
  cualquier tipo, ya sea las limitaciones de los datos, de la técnicas,
  de los objetivos de aprendizaje. Cierra indicando qué desafíos futuros
  quedan abiertos tras este trabajo.

- **Referencias**. Las referencias que hayas citado en el texto, se
  incluirán automáticamente en la sección “Referencias”. No obstante,
  debes verificar la integridad de las mismas.

> **RECUADRO: recomendaciones básicas de redacción**
>
> Usa una voz (activa o pasiva) de forma consistente, pero sólo ten
> presente que la redacción de manuscritos científicos a menudo se
> utilizan ambas voces, dependiendo del contexto y el mensaje que el/la
> autor/a quiera transmitir. Veamos algunos ejemplos:
>
> **Voz activa en manuscrito científicos:**
>
> - **Analicé** los datos utilizando el lenguaje de programación Python.
>
> - El experimento **mostró** que la temperatura afecta directamente la
>   tasa de reacción.
>
> - Los investigadores **encontraron** una correlación significativa
>   entre las dos variables.
>
> La voz activa puede hacer que la redacción parezca más directa y
> clara, y es especialmente útil cuando el/la autor/a quiere enfatizar
> quién llevó a cabo una acción o cuándo se desea hacer una afirmación
> fuerte.
>
> **Voz pasiva en artículos científicos:**
>
> - Los datos **fueron analizados** utilizando el lenguaje de
>   programación Python.
>
> - **Se observó** que la temperatura afecta directamente la tasa de
>   reacción.
>
> - Una correlación significativa **fue encontrada** entre las dos
>   variables.
>
> La voz pasiva es común en la redacción científica porque a menudo se
> prefiere un tono más impersonal, enfocando la atención en los
> resultados y procedimientos en lugar de en quienes llevaron a cabo la
> investigación. También puede ser útil cuando no se quiere o no es
> relevante especificar quién realizó la acción.
>
> **En todas mis prácticas, está completamente permitido usar IA
> (e.g. chatGPT), pero te recomiendo que la uses más como tutor que como
> redactor**. Tal como te sugerí arriba, no le pidas que te resuelva los
> problemas del mandato. Pídele que te dé ideas, y que luego tú las
> mejores o las descartes. No abuses tampoco del texto, pues mucha
> redacción no siempre es mejor; en redacción de ensayos “menos es más”.
> Cruza las redacciones que te ofrezca con tu conocimiento, y revisa si
> los términos o conceptos usados son descabellados (toda IA se inventa
> cosas, cuidate de no caer en esa trampa). Nunca le pidas referencias
> bibliográficas, porque se va equivocar.

# Referencias

<div id="refs" class="references csl-bib-body hanging-indent"
entry-spacing="0" line-spacing="2">

<div id="ref-jose_ramon_martinez_batlle_2022_7367180" class="csl-entry">

Martínez-Batlle, J. R. (2022). *geofis/zonal-statistics: Let there be
environmental variables* (Versión v0.0.0.9000). Zenodo.
<https://doi.org/10.5281/zenodo.7367256>

</div>

</div>
