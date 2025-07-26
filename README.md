# SEGUIMIENTO1
**1) a.Describa los campos que se encontrará en este tipo de archivos. ¿Qué información está allí contenida? Proporcione ejemplos.**

El archivo GFF3 contiene 9 columnas que describen distintos aspectos de las anotaciones genomicas.
<img width="910" height="191" alt="image" src="https://github.com/user-attachments/assets/b6ff13f4-15e8-4361-9ffa-d5261161e523" />

Tomado de:https://github.com/The-Sequence-Ontology/Specifications/blob/master/gff3.md


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
   
