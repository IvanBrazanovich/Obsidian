# Temas 
Subunidad A: Noción de Secuencia Noción de secuencia. Definición formal de secuencia. Funciones de acceso a elementos de una secuencia. Operadores de construcción de secuencias.

Subunidad B: Descomposición y Tratamiento de Secuencias. Subalgoritmos. Noción de parámetro. Parametrización de acciones. Noción de procedimientos y funciones. Acciones condicionadas. Análisis por caso. Alternativa, ejecución condicionada y selección múltiple. Acciones que se repiten. Noción de las estructuras ..REPETIR...HASTA QUE..,MIENTRAS.... REPETIR, ITERAR. Teorema fundamental de la programación estructurada y unicidad de puntos de entrada y salidas. La prueba de escritorio. Noción de acumulación e invariante.


### Secuencia 
Diremos que un conjunto de objetos está organizado en forma de secuencia si es posible definir lo siguiente: 

#### Primer objeto de la secuencia 
El acceso a él, permite el acceso a todos los demás elementos. 


#### Relación de sucesión entre los objetos 
Todo objeto de la secuencia (salvo el último elemento) precede a uno de los demás objetos (sucesor) o a todo elemento de la secuencia (excepto el primero), es el sucesor de otro y así hasta el final.




#### Finitud 
Debe estar definido un indicador de fin de secuencia. Este puede ser:
+ un **elemento final conocido** (permite detener la enumeración de la secuencia por observación de la característica del último elemento) 
+  **una marca** (elemento que no debe ser considerado como tal) 
+ El conocimiento exacto de la **cantidad de elementos** que conforman la secuencia 



Las secuencias así definidas no autorizan el acceso a un elemento más que a través del elemento que le precede



### Características complementarias de una secuencia 
#### orden 
Existe un orden cuando la relación sucesión es estricta. 
![[Pasted image 20220511063051.png]]



#### Completitud 
No se puede suponer, tiene que estar definida en el planteo del problema, al igual que el orden. 
![[Pasted image 20220511063130.png]]


#### Clasificación de secuencias 
![[Pasted image 20220511063226.png]]

![[Pasted image 20220511063248.png]]

#### ¿Cuáles son los esquemas generales y por máquina de las impuras?
![[Pasted image 20220511063759.png]]
![[Pasted image 20220511063809.png]]


#### ¿Cuáles son los esquemas generales y por máquina de las puras?
![[Pasted image 20220511063827.png]]
![[Pasted image 20220511063902.png]]



#### Su tamaño no es fijo
Una de las principales características asociadas a las Secuencias es que su tamaño no es fijo, sino que dentro del algoritmo que las crea su longitud puede variar.



#### Memoria 
Si bien la condición de finitud siempre se debe tener en cuenta, para su procesamiento se debe emplear un esquema de asignación de almacenamiento en memoria dinámico.


### Acciones con secuencias 
![[Pasted image 20220511064300.png]]
![[Pasted image 20220511064309.png]]
![[Pasted image 20220511064339.png]]
![[Pasted image 20220511064404.png]]



















