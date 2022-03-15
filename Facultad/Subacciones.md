## ¿Qué son las subacciones?
Los problemas complejos se pueden facilitar dividiéndolos en varias partes. Estos subproblemas se realizan  mediante subalgoritmos o subacciones. 

### ¿Cuáles son las características de las subacciones?
+ Son acciones que forman parte de una ACCIÓN PRINCIPAL
+ Son módulos que están escritos para ejecutar alguna tarea específica
+ Se definen en el AMBIENTE pues van a ser utilizadas e invocadas durante el PROCESO del algoritmo diseñado
+ Se escriben solamente una vez, pero pueden ser referenciados en diferentes puntos del algoritmo, de modo que se puede evitar la duplicación innecesaria del código


### Control de ejecución 
El algoritmo principal se ejecuta en una primera instancia, y da la orden de inicio de ejecución de los subalgoritmos. Esto puede suceder N veces. 

El control de ejecución es se conoce al proceso cuando  el programa realiza la solicitud, el algoritmo se detiene hasta que el subalgoritmo deja de realizar su tarea, luego continúa.


### Elementos de las subacciones
1. Nombre
2. Parámetros 
	1. Algunas veces las subacciones deben pasar o recibir datos para ejecutarse. Los parámetros son variables y/o constantes para pasar datos entre algoritmos y subalgoritmos en ambos sentidos. 

#### Tipos de parámetros 
1. Los parámetros que aparecen en la definición del subalgoritmo, se denominan parámetros formales o ficticios.
2. Los parámetros que se encuentran en la llamada al subalgoritmo se denominan parámetros actuales o argumentos. Son los datos que el algoritmo principal envía a la subacción. 