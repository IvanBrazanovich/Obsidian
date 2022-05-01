### Ecuaciones lineares simultáneas
Existen tres posibilidades a la hora de ver ecuaciones lineales.
#### Que se encuentren en un punto
![[Pasted image 20220430173356.png]]



#### Que no se encuentren jamás por ser paralelas
![[Pasted image 20220430173422.png]]


#### Que sean linealmente dependientes, o sea que una se pueda derivar de otra mediante un cálculo (te da una cantidad infinitas de soluciones porque se superponen)
![[Pasted image 20220430173542.png]]


### Transformaciones lineales
Las transformaciones lineales son lo que suenan, son transformaciones lineales que se hacen al plano de los ejes cartesianos


![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 17-50-08.mp4]]


#### Transformaciones lineales al plano cartesiano

![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 17-51-47.mp4]]

#### Mediante las puntas de los vectores


![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 17-53-24.mp4]]


#### Como una grilla

![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 17-54-13.mp4]]



#### Dejando la grilla común de fondo para ver el cambio


![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 17-55-32 1.mp4]]



#### ¿Qué debe cumplir para ser una transformación lineal ?
+ Todas las líneas deben continuar siendo líneas
+ El origen no se puede mover




#### ¿Cómo representar transformaciones lineales?
Resulta que solo necesitas los versores i e j. Esto es debido a que las transformaciones lineales mantienen las proporcionalidades. 

![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-00-16.mp4]]


Básicamente lo que estás haciendo es multiplicar los números que tenías como coeficientes en un principio por las transformaciones de los versores. 

Ejemplo:
![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-03-22.mp4]]

Esto significa que podemos saber donde cae cualquier punto en el plano solamente sabiendo donde quedaron los versores.
![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-08-00.mp4]]



#### Más generalmente 
Dada la coordenada donde cayó  el versor i (a,c) y donde cayó versor j (b,c) vemos que la multiplicación de cualquier punto de x por la transformación de i y te dará la nueva ubicación de x de ese nuevo vector, lo mismo con el versor j. 

![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-17-37.mp4]]



#### ¿Qué pasa si roto 90 grados anti reloj? ¿Cómo puedo representarlo con matrices?

![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-20-41.mp4]]



#### ¿Qué pasa si los vectores donde caen los versores i y j son dependientes?

![[Linear transformations and matrices _ Chapter 3, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-22-16.mp4]]





#### ¿Qué es la composición de transformaciones?
Si primero le hacemos una transformación a un vector, y luego le hacemos otra transformación, es lo mismo que hacerle la multiplicación de las dos transformaciones por el vector. 

![[Matrix multiplication as composition _ Chapter 4, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-31-53.mp4]]
![[Pasted image 20220430183315.png]]
Recordemos que primero se aplica lo que está a la derecha y luego lo que está a la izquierda.

#### ¿Cómo podemos calcular la posición de los versores luego una composición de transformaciones?
Dada la primera transformación, la primera columna nos dará donde quedó el versor i, por lo que debemos multiplicar la segunda transformación por i para saber donde queda i al final. Luego multiplicaremos j por los valores que nos había dado en un principio, al igual que i. 

![[Matrix multiplication as composition _ Chapter 4, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-37-48.mp4]]

#### Más generalmente

![[Matrix multiplication as composition _ Chapter 4, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-39-18.mp4]]


#### las multiplicaciones generalmente no son conmutativas
![[Matrix multiplication as composition _ Chapter 4, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 18-41-05.mp4]]


#### ¿Qué pasa con las transformaciones lineales en 3 dimensiones?
Es lo mismo que con 2 dimensiones, se pueden representar las transformaciones con solo 9 números. 

![[Three-dimensional linear transformations _ Chapter 5, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-20-56.mp4]]


#### Calcular nuevo vector a partir de las transformaciones de los versores
![[Pasted image 20220430192220.png]]






### Vectores como matrices
Dada dos ecuaciones lineales del tipo 
![[Pasted image 20220430174159.png]]
Podemos decir que dados dos valores de x e y nos va a dar un valor x' e y' que se encuentra en el plano.





### Vectores a partir de matrices 
![[Pasted image 20220430191357.png]]
Dada 2 ecuaciones lineales, se puede dividir en vectores las ecuaciones de manera que nos den dos vectores tal que sumados nos den el vector resultado, en este caso (8,-2)

![[Pasted image 20220430193322.png]]
De manera que la columna izquierda 
![[Pasted image 20220430193844.png]]
Es básicamente donde el vector i queda, siendo 3 el vector que habla de las horizontales y el -2 de las verticales. Lo mismo sucede con la columna derecha. 



### De matrices a vectores 
![[Pasted image 20220430194103.png]]
Básicamente lo que te dice la ecuación es lo siguiente: ¿Qué vector de la columna del medio al aplicarle la transformación lineal  de la matriz de la izquierda me ubicará un vector de la columna derecha?


![[Inverse matrices, column space and null space _ Chapter 7, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 20-19-23.mp4]]







### Determinantes 
Una determinante es el factor por el cual una transformación lineal aumenta o decrece el área de una determinada región. 

![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-44-35.mp4]]

![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-49-53.mp4]]

#### Ejemplo de un determinante
![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-46-35.mp4]]


#### Aplicaciones generales 
![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-47-54.mp4]]
![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-48-51.mp4]]




#### ¿Cuándo una determinante es 0?
Cuando las columnas de la transformación son linealmente dependientes.

![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-51-53.mp4]]




#### ¿Cuándo una determinante es negativa?
Cuando se invierte el espacio, o sea que en vez de que j esté a la izquierda de i, será al revés.
![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-54-18.mp4]]




#### Ejemplo de una determinante negativa
![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-55-05.mp4]]


#### ¿Por qué es negativa una determinante?
Porque mientras i se va acercando a j, se va acercando a 0 el área de la determinante, luego de que la pasa, es natural que se considere como negativo.

![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-56-39.mp4]]




#### ¿Qué pasa con las determinantes en 3d?
Lo único que cambia es que ahora busca el factor por el cual aumenta o decrece el volumen
![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-58-01.mp4]]


#### Determinante 0 en 3d 
Es cuando el volumen termina siendo 0 porque las columnas de la transformación lineal son dependientes.
![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 19-59-38.mp4]]



#### Formula para el cálculo de la determinante de una matriz 2x2
![[The determinant _ Chapter 6, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 20-02-48.mp4]]


#### Gráficamente el cálculo
![[Pasted image 20220430200420.png]]




### ¿Qué es la inversa de una matriz?
Es la inversa de la transformación lineal, o sea, te devuelve el vector con el que empezaste si le das un vector cualquiera.

![[Inverse matrices, column space and null space _ Chapter 7, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 20-24-16.mp4]]![[Inverse matrices, column space and null space _ Chapter 7, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 20-26-14.mp4]]![[Inverse matrices, column space and null space _ Chapter 7, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 20-29-04.mp4]]



### ¿Qué transformación lineal no hace nada?
La identidad, debido a que deja a i en el lugar y a j en el lugar. Es por eso que multiplicar A por la inversa de A te da una matriz identidad.
![[Pasted image 20220430202804.png]]





### ¿Qué es el rango de una matriz?
Es la cantidad de dimensiones que presenta la salida de una transformación lineal.
+ Si una transformación lineal (matriz) pasada por una entrada bidimensional tiene una salida bidimensional tiene un rango de 2.
+ Si una entrada tridimensional tiene una salida bidimensional tiene rango 2.
+ Si una entrada tridimensional tiene una salida unidimensional tiene un rango 1.

Se podría decir que es el número de dimensiones en el espacio de las columnas
![[Inverse matrices, column space and null space _ Chapter 7, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 20-34-01.mp4]]


### ¿Qué pasa con las matrices rectangulares o las transformaciones lineales rectangulares?
Es lo mismo, en el caso de:
![[Pasted image 20220501073317.png]]
Pasa lo mismo, i cambiaría de lugar y j también. Lo único que pasa es que siguen siendo 2d, el plano se mueve solamente. 
![[Pasted image 20220501073450.png]]
![[Pasted image 20220501073549.png]]
En este caso podemos ver que es un plano que corta al origen del espacio. Sigue teniendo un rango total, debido a que sigue siendo solamente un plano. 
La cantidad de columnas indica cuántos versores tiene, mientras que la cantidad de filas indica que la ubicación se indica con 3 distintas coordenadas.


### Del espacio al plano 
En el siguiente caso vemos que tiene 3 columnas, lo que significa que empieza con 3 versores, y luego vemos que tiene 2 filas, lo que significa que los versores se pueden indicar solamente con 2 coordenadas, de manera que quedaron en el plano, pasaron de ser 3d a 2d.
![[Pasted image 20220501074015.png]]
![[Pasted image 20220501074146.png]]


### Del plano a una dimensión
También puede haber una transformación de 2d a 1d. 
![[Nonsquare matrices as transformations between dimensions _ Chapter 8, Essence of linear algebra - YouTube - Google Chrome 2022-05-01 07-44-25.mp4]]