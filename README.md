## MEMORIA TRABAJO FINAL DANIEL TALAVERA HERNÁNDEZ



## CONTEXTO: 
Mis datos tratan la evolución del emprendimiento en España, tanto a nivel nacional
como por provincias, con un seguimiento mensual, desde enero de 1995 hasta diciembre 
de 2023. Por otro lado, se han obtenido datos de la población de las provincias de 
España para  cada año desde 1995 hasta 2023 para facilitar el estudio de los datos, 
además de evitar obtener conclusiones falsas. Cabe destacar que tanto  los datos 
de emprendimiento como los datos de población se extrajeron del INE.  


## ESTADO ACTUAL Y OBJETIVOS: 
- La situación actual del emprendimiento en España se puede resumir de la siguiente manera:

La actividad emprendedora española ha regresado a niveles previos a la pandemia, 
con una mayor cantidad de iniciativas más digitalizadas e innovadoras. Además, el 
sector de servicios a empresas (B2B, business-to-business) se ha consolidado como 
un nicho de iniciativas emprendedoras de nivel tecnológico medio-alto.
Por otro lado, las motivaciones para emprender en España siguen siendo poco ambiciosas 
y se han visto afectadas negativamente por los años de pandemia, aunque, Mujeres y hombres, 
sin importar su nivel de ingresos, se lanzan a emprender por igual.
Por último, respecto a los obstáculos a la hora de emprender, destacan: La falta 
de financiación, la fiscalidad y exceso de burocracia y la escasa educación en emprendimiento.


- Motivación y objetivos:

En los últimos años, he estado bastante interesado en el emprendimiento, y en las 
diversas formas que hay de hacerlo, sin embargo, con el paso de los años, las 
dificultades para los emprendedores no han hecho más que aumentar, por ello he decidido
comprobar como han afectado estas dificultades y muchas otras que han surgido a 
lo largo de los años a los emprendedores y emprendedoras de nuestro país. Además, 
estudiaré si existe alguna época o mes en la que se constituyan más empresas,
es decir, si el momento en el que comiences a emprender es o no relevante.
Por otro lado, se observará como ha evolucionado el sector empresarial en España
desde 1995 hasta ahora tanto a nivel nacional como por provincias, tratando de 
centrarnos en la provincia de Las Palmas de Gran Canaria. También, veremos qué
provincia o qué provincias contienen un mayor número de emprendedores, valorando
también la población de la provincia, y comprobaremos si esto ha ido cambiando 
a lo largo de los años. Otro factor a estudiar, será la pandemia, y como afectó
al emprendimiento en las diferentes provincias y qué hubiese pasado si la pandemia 
no hubiese ocurrido. Además del número de empresas constituídas y del capital
invertido en ellas, se estudiará el número de empresas disueltas en las diferentes
épocas y para las diferentes provincias, permitiéndonos observar las provincias en 
las que más empresas se disuelven y en las que menos, y si estas son las mismas que 
las provincias en las que más provincias se constituyen.




## APORTACIONES:
Entorno Socioeconómico:
Al proporcionar datos detallados sobre la evolución del emprendimiento a lo largo 
del tiempo y a nivel provincial, este proyecto ofrece una visión completa de la actividad 
emprendedora en el país. Esto puede contribuir al entendimiento del panorama del 
emprendimiento en España.

Entorno Técnico (Uso de datos y análisis estadístico):
Este trabajo implica el manejo y análisis de grandes conjuntos de datos relacionados 
con el emprendimiento y la población. Esto implica el uso de técnicas de análisis 
de datos para identificar tendencias, patrones y correlaciones significativas.
Además, se aplican herramientas de visualización de datos para comunicar eficazmente 
los hallazgos. Algunas de estas herramientas de visualización de datos son
gráficos, mapas y otros medios visuales que ilustran las tendencias y patrones 
identificados en los datos.

Entorno Científico (Investigación sobre el impacto de la pandemia en el emprendimiento):
El estudio de cómo la pandemia ha afectado al emprendimiento en diferentes provincias 
puede generar conocimientos importantes sobre la resiliencia empresarial y las respuestas 
a crisis económicas. Estos hallazgos pueden tener implicaciones tanto para la investigación 
académica como para la formulación de políticas.
Otro factor importante será estudiar la relación entre la población de una provincia 
y la actividad emprendedora en esa área, este trabajo podría proporcionar bastante
información sobre cómo los factores demográficos influyen en la creación y sostenibilidad 
de empresas.

En resumen, este trabajo tiene el potencial de generar conclusiones valiosas que pueden 
informar la toma de decisiones en el ámbito político, económico y empresarial, así 
como contribuir al avance del conocimiento en áreas relacionadas con el emprendimiento, 
la economía y la sociedad.


## DESARROLLO:
**Fiabilidad de los datos**
Los datos se ha obtenido del INE. El Instituto Nacional de Estadística (INE) de 
España ha realizado numerosos esfuerzos para mantener la alta calidad y fiabilidad 
de sus productos estadísticos. Estos son algunos puntos clave sobre su fiabilidad:

- Gestión de la Calidad: El INE tiene una estrategia de gestión de la calidad basada 
en el Marco Común de Calidad de la Unión Europea, los Principios Fundamentales de l
as Naciones Unidas y el Código Ético del ISI. Esta estrategia incluye directrices 
de calidad integradas en la misión y visión del INE, y un sistema de gestión de 
calidad compuesto por normas e instrumentos.

- Código de Buenas Prácticas de las Estadísticas Europeas (CBPEE): El INE sigue el 
CBPEE, que establece el estándar para desarrollar, producir y difundir estadísticas 
europeas. Los principios del CBPEE cubren aspectos como la independencia profesional, 
la protección de la confidencialidad, la fiabilidad de los resultados, su precisión, 
oportunidad, puntualidad, accesibilidad, claridad, comparabilidad y coherencia.

En resumen, el INE se esfuerza por mantener la fiabilidad y la calidad de sus datos 
a través de una gestión de calidad rigurosa, el cumplimiento de los estándares europeos 
y la justificación metodológica de sus índices.

**Análisis exploratorio inicial  de los datos con una descripción de incidencias encontradas relativas al contenido y organización de los datos utilizados **
Respecto al análisis exploratorio inicial de los datos, no hubo grandes problemas
para encontrar los datos en un formato adecuado para su procesamiento, y su organización
era bastante buena, aunque necesitó algunas adaptaciones.

**Identificación de los requisitos de procesado de los datos, combinación de tablas, etc. necesarios para el proyecto. **
A continuación se muestra como se han procesado los datos. En primer lugar, cargo 
los datos correspondientesal número de empresas constituidas, disueltas y que 
aumentan o reducen capital en las diferentes provincias de España y a nivel nacional,
desde enero de 1995 hasta diciembre de 2023. Tras leer los datos en formato px y 
pasarlos a tibble, elimino los registros para los que el valor es NA, ordeno los 
datos y paso la fecha a formato Año-Mes-Día.

Además, cargo los datos correspondientes a la población en España organizada por 
provincias y por sexo, desde 1995 hasta 2023, aunque . Al igual que para el conjunto 
de datos anterior, leo el archivo con extensión px, lo paso a tibble y ordeno los datos. 
Sin embargo, además de los pasos ya mencionados, también se realiza un cambio de 
formato de la fecha, para que sea de tipo Date y para que coincida con el formato de 
nuestro  conjunto de datos. Por otro lado, filtramos los datos de manera que manejamos 
los datos de población totales de cada provincia, y no por rango de edades. Cabe
destacar que se utilizaron dos tablas del INE para poder abarcar el periodo completo
de los datos de la primera tabla.
