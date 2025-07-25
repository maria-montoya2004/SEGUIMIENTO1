# SEGUIMIENTO1
**1) a.Describa los campos que se encontrará en este tipo de archivos. ¿Qué información está allí contenida? Proporcione ejemplos.**
   columna 1: **sequid**: es el identificador de la secuencia. Ejemplo:
   columna 2: **source**: fuente o herramienta que realizo la anotacion. Generalmente es el nombre de la base de datos. Ejemplo: GenBank
   columna 3: **type**: indica el elemento genomico que se esta anotando. Ejemplo: CDS
   columna 4-5: **start and end**: posición inicial del feature en la secuencia, la numeracion es positiva y comienza desde el 1.Siempre "start"<= "end" Ejemplo:
   columna 6: **score**: representa un valor númerico que evalua la confianza de la predicción usando valores p para la predicción génetica.
   columna 7: **strand**: indica en que cadena del ADN se encuentra el feature. se indica con + si el feature esta en hebra positiva y con - si el feature esta en la hebra negativa
   columna 8: **Phase**: se solo para features CDS. se usa para mantener el marco de lectura correcto e indica desde donde inicia la lectura con el 0,1 o 2
   columna 9: **attributes**: guarda informacion adicional sobre la caracteristica biologica. la informacion se da en el formato de pares tag=value Ejemplo:
   **3) a. Proporcione
