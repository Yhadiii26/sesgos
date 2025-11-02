# sesgos
Análisis de sesgos en noticias
El corpus utilizado tiene un total de 1217 noticias.
Las noticias cuentan con una variedad de temas, como se observa en la columna Type (Otra, Regulaciones, Alianzas, Macroeconomia, Innovacion, Sostenibilidad). Esto demuestra que el modelo Word2Vec fue entrenado en un conjunto de diversos datos en cuanto a contenido.
La columna news contiene el texto de las noticias, que fue preprocesado (convertido a minúsculas y dividido en palabras) antes de entrenar el modelo.
Se seleccionaron las siguientes palabras para visualizar en 2D:
mujer
hombre
indigente
extranjero
becario
joven
mesero
adulto
niño
adinerado
trabajador
emprendedora
comersiante
desempleado
Estas palabras fueron elegidas para explorar las posibles relaciones y sesgos  relacionados con características demográficas, socioeconómicas y roles laborales. Se incluyeron términos que podrían estar asociados a estereotipos o representaciones desiguales en los medios de comunicación.

A continuación el gráfico generado por el código, muestra la proyección de las palabras seleccionadas :
La distancia entre las palabras en el gráfico 2D sugiere su similitud con el contexto del corpus de noticias. Palabras que aparecen juntas o en contextos similares en las noticias tienden a estar más cerca en este espacio.
Se puede observar agrupaciones o cercanías entre ciertas palabras que reflejan las asociaciones presentes en el corpus. Por ejemplo, si "mujer" y "emprendedora" aparecen cerca, podría indicar que relaciona a las mujeres con el emprendimiento. La cercanía entre "hombre" y "trabajador" podría sugerir una asociación similar.
Las posiciones relativas entre pares de palabras (ej "hombre"  "mujer") pueden revelar relaciones aprendidas por el modelo, aunque estas relaciones pueden no ser tan claras.
En base a la visualización y las posibles cercanías entre palabras, se podrían identificar posibles sesgos si ciertas palabras relacionadas con grupos demográficos (como "mujer", "hombre", "indigente", "extranjero") aparecen cerca de términos asociados a roles, características o juicios específicos.
Por ejemplo, si "indigente" aparece cerca de palabras relacionadas con la criminalidad o la pobreza extrema de manera desproporcionada, o si "extranjero" se asocia principalmente con temas de inmigración ilegal o inseguridad, esto podría ser un indicio de sesgo en la forma en que estos grupos son representados en las noticias.
 Si el corpus de noticias contiene sesgos en la forma en que se describen los grupos, estos sesgos se verán  en las relaciones y distancias entre los vectores de palabras. La visualización en 2D nos permite observar estas relaciones de una manera simplificada.

 Los modelos sesgados pueden perpetuar y amplificar los estereotipos y la discriminación presentes en los datos de entrenamiento. Si un modelo asocia consistentemente ciertos grupos con características negativas o limitantes, esto puede reforzar prejuicios en las aplicaciones que utilizan estos modelos.
Impacto en la Audiencia: Las noticias influyen en la percepción pública y en la formación de opiniones. Si los sistemas de PLN sesgados se utilizan para generar resúmenes, recomendar contenido o analizar noticias, pueden presentar una visión distorsionada de la realidad que afecte negativamente a la audiencia, perpetuando malentendidos y prejuicios hacia ciertos grupos o temas.
 En conlusiones generales, para gestionar el sesgo en PLN, hay que auditar los datos y modelos para detectar y medir las injusticias, aplicar técnicas para corregirlas (ajustando datos o modelos), usar datos de entrenamiento muy diversos y hacer que los modelos sean transparentes para entender sus decisiones, hcaer conciencia a todos sobre la ética en IA, y evaluar constantemente para asegurarse que los sesgos no reaparezcan.


En conclusión, si bien los embeddings son una herramienta poderosa para capturar relaciones semánticas, es crucial ser conscientes de que heredan los sesgos presentes en los datos de entrenamiento. Un enfoque ético y responsable en el desarrollo y la aplicación del PLN es fundamental para minimizar el impacto negativo de estos sesgos en la sociedad.
