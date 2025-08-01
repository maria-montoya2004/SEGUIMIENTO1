# SEGUIMIENTO1

**1) a.Describa los campos que se encontrará en este tipo de archivos. ¿Qué información está allí contenida? Proporcione ejemplos.**

El archivo GFF3 contiene 9 columnas que describen distintos aspectos de las anotaciones genomicas.
<img width="910" height="191" alt="image" src="https://github.com/user-attachments/assets/b6ff13f4-15e8-4361-9ffa-d5261161e523" />

Tomado de: https://github.com/The-Sequence-Ontology/Specifications/blob/master/gff3.md


   **Columna 1: sequid:** indica el ID del feature.
   **Ejemplo:** como se puede observar en la imagen, en la columna 1 el ID corresponde a "ctg123"
   
   **Columna 2: source:** describe el algoritmo o procedimiento que identificó el feature. Generalmente corresponde al nombre de la base de datos o herramienta utilizada.
   **Ejemplo:**  como se observa en la imagen, en ese caso se omite el valor y por eso aparece un punto (.); sin embargo, comúnmente se encuentran source como GenBank.
   
   **Columna 3: type:** indica el elemento genomico que se está anotando. 
   **Ejemplo:** en la imagen superior se puede observar que, para la columna 3, aparecen tipos como mRNA y gene.
   
  **Columna 4-5: start and end:** indican la posición inicial y final del feature en la secuencia. La numeración es positiva y comienza desde 1. Siempre se cumple que start ≤ end.
  **Ejemplo:** se puede ver en la imagen que, para la línea 2, en la columna 4 correspondiente a start, el feature inicia en la posición 1000 de la secuencia, y en la columna 5 correspondiente a end, finaliza en     la posición 9000.
  
   **Columna 6: score:** representa un valor númerico que evalua la confianza de la predicción usando valores p para la predicción génetica.
   **Ejemplo:** en el caso de la imagen, en la columna 6 se encuentra un punto (.); esto puede significar que el score no está disponible o que no se asignó puntaje. Sin embargo, en otros casos se pueden             encontrar números decimales como 0.95, que indican la probabilidad o la confianza de que la secuencia anotada sea real.
   
   **Columna 7: strand:** indica en qué cadena del ADN se encuentra el feature. Se utiliza (+) si el feature está en la hebra positiva (sentido 5'→3'), y (-) si está en la hebra negativa (sentido 3'→5').
   **Ejemplo:** en la imagen se puede observar que en la línea 2, la columna 7 contiene el signo +, lo que indica que la secuencia se encuentra en la hebra positiva.
   
   **Columna 8: Phase:** se utiliza solo para elementos de tipo CDS e indica cuántos nucleótidos hay antes del primer nucleótido del primer codón. Los valores posibles son 0, 1 o 2. Para los elementos que no son     CDS, esta columna se llena con un punto (.).
   **Ejemplo:** en la imagen se puede observar que en todas las líneas, la columna 8 contiene un punto (.), lo que indica que no son elementos de tipo CDS. Si en cambio se encontrara un 0, significaría que el         codón comienza justo en la primera base del feature; un 1 indicaría que el codón comienza después de una base, y así sucesivamente.
   
   **Columna 9: attributes:** guarda información adicional sobre el feature. La información se da en el formato de pares tag=value  y puede incluir varios, separados por (;). Es importante porque permite conocer     el ID, el nombre, la jerarquía,entre otros datos.
   **Ejemplo:** en la imagen, justo en la línea 2, se puede observar que para la columna 9 los atributos son ID=gene00001;Name=EDEN.
   
   **3) a. Proporcione una breve descripción del organismo asignado**

   **Angila Asiática de Pantano** (*Monopterus albus*)
   
   <img width="1047" height="588" alt="image" src="https://github.com/user-attachments/assets/45b8e8ab-2630-426a-bcde-0ca23d33e61a" />

   Imagen tomada de: https://colombia.inaturalist.org/taxa/53511-Monopterus-albus
   
La anguila asiática de pantano, también conocida como anguila arrocera, es una especie de pez aerofítico que se puede encontrar en el este y sudeste de Asia (India, el sur de China, Malasia, Indonesia), donde se vende y consume comúnmente. Tiene un cuerpo anguiliforme y sin escamas; puede alcanzar un metro o menos (25 a 40 cm) en la edad adulta. Su color es variable, pero generalmente oliva o marrón, con manchas irregulares oscuras. Su boca es grande y tanto en la mandíbula superior como inferior tienen dientes diminutos para comer peces, gusanos, crustáceos y otros pequeños animales acuáticos. Su entorno preferido son los humedales fangosos, de agua dulce y poco profundos, como lagos, ríos y estanques. *Monopterus albus* puede vivir en una amplia gama de niveles de oxígeno. La anguila de pantano asiática es hermafrodita: todas las crías son hembras y, a medida que los más jóvenes comienzan a madurar, algunos adquieren el fenotipo masculino, y los machos pueden cambiar de sexo, lo que les permite reponer poblaciones cuando la densidad de hembras es baja, pero este cambio de sexo puede tardar hasta un año.(Wikipedia, 2025)

**Referencia bibliográfica**

Wikipedia. (2025, enero 23). Asian swamp eel. Wikipedia, The Free Encyclopedia. https://en.wikipedia.org/w/index.php?title=Asian_swamp_eel&oldid=1271391020

**3) b. investigue, usando las herramientas de la linea de comandos de unix, y conteste las siguientes preguntas:**

**i. ¿ Cuántos features contiene el archivo?**

**R//** El archivo contiene 790340 features. En la siguiente imagen se muestra una foto de la terminal donde se pide la cantidad detallada de cada feature.
<img width="1376" height="784" alt="image" src="https://github.com/user-attachments/assets/726d7fb2-41dc-4894-baa0-61683102a24b" />

**ii) ¿Cuantas regiones de la secuencia (cromosomas) contiene el archivo?**

**R//** El archivo contiene 20622 regiones de la secuencia(cromosomas).

**iii) ¿ Cuántos genes están listados en el organismo?**

**R//** En el organismo estan listados 22145 genes.

**iv) ¿Cuál es el top 10 de tipo de features( columna 3) más anotados en el genoma?**

**R//** El top 10 de los tipos de features más anotados en el genoma se muesta en la siguiente imagen tomada de la terminal:

<img width="386" height="296" alt="image" src="https://github.com/user-attachments/assets/36b2b25b-2076-477a-95ca-0d37048dcc1d" />










   
