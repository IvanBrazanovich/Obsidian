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









#### ¿De dónde salen las transformaciones lineales?
Nosotros cuando estamos haciendo un sistema de ecuaciones lineales estamos tratando de ver en qué punto satisface las ecuaciones que tenemos. En el caso de las transformaciones lineales, podemos encontrar donde quedaron los puntos que pueden resolver ecuaciones mediante la utilización de los versores i, j y  los lugares donde quedaron esos versores. O sea: 
+ Tenemos 1 vector cualquier (X1, Y1);
+ Se aplica al plano una transformación lineal.
+ Debido a que todo es proporcional y está todo bien repartido, se puede calcular a partir de un punto, otros puntos. 
+ Con ayuda de esta propiedad utilizamos donde quedaron los versores i y j para calcular donde quedó cualquier punto del sistema de referencia. 





# PIENSO 
En el caso de que tengamos una ecuación 2x + 3y = 4. Esta ecuación me está preguntando "¿Qué vector (x, y) aplicada la transformación lineal me va a dar que la suma de sus catetos será igual al resultado?" Supongamos que los componentes del vector inicial valen 0.8, podemos decir que la suma de sus catetos vale 1,6. Pero si aplicamos la transformación lineal. ()

![[Interactive Matrix Visualization - Google Chrome 2022-05-14 12-02-26.mp4]]



Pero cuando tenemos dos sistemas de ecuaciones lineales:
2x + 3y = 4
6x + 2y = 8
Resulta que la forma de encontrar una matriz de la forma 
![[Pasted image 20220514183916.png]]
Es igual a pasar los sistemas de ecuaciones lineares a esa notación matricial, y resulta lo mismo. Resulta lo mismo también entender a esa forma matricial como una transformación lineal.
![[Inverse matrices, column space and null space _ Chapter 7, Essence of linear algebra - YouTube - Google Chrome 2022-04-30 20-19-23.mp4]]

Y cada columna de la primera matriz A corresponde a dónde quedaron los versores. 
![[Pasted image 20220430192220.png]]
Donde las columnas son los versores i, j y k respectivamente.
En resumen
![[y2mate.com - Cramers rule explained geometrically  Chapter 12 Essence of linear algebra_1080pFHR.mp4 - Reproductor multimedia VLC 2022-05-14 18-47-23.mp4]]








Supongamos que quiero que el versor i quede en (1 en x, -2 en y). Lo que tengo que hacer es multiplicar ese vector i  por el lugar en notación matricial de donde quiero que quede.
![[Pasted image 20220514111755.png]]
Por lo que quedará i = (1 representando a x, -2 representando a y).
Lo mismo pasa con el versor j y a partir de ambos se pueden calcular donde quedan todos los otros puntos. 






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




### Cálculo del producto punto 
![[Pasted image 20220501101011.png]]



O sea que te transforma vectores a números porque los pasa a una dimensión
Ok no hace la transformación hacia el coso, sino lo que hace es como poner una unidad ahí medio rara.


### De punto a proyección a número 
![[Pasted image 20220503162139.png]]
Dada una línea de números, la proyección de cualquier punto en la línea de números te da un número. Esto significa que creaste una transformación linear que convierte puntos/vectores en unidades.

### Encontrando esa transformación lineal 
1. Primero debemos encontrar donde aterrizan i y j, debido a que serán las columnas de nuestra nueva transformación lineal.

![[Pasted image 20220503162532.png]]
2. Debido a que son vectores unitarios, la proyección de u en i es la misma que la de i en u. De la siguiente manera. 
 ![[Pasted image 20220503162648.png]]
3. Lo mismo para j
![[Pasted image 20220503162728.png]]

4. El resultado de la transformación será.
![[Pasted image 20220503162751.png]]

De esto resulta que para cualquier vector, la multiplicación de las proyecciones de u en i y j, resultan lo mismo que la multiplicación. ![[Pasted image 20220503162915.png]]
![[Pasted image 20220503163032.png]]



### Para vectores de u no unitarios. 
![[Dot products and duality _ Chapter 9, Essence of linear algebra - YouTube - Google Chrome 2022-05-03 16-32-44.mp4]]

### Conversión de vectores a 1d
![[Pasted image 20220503163557.png]]
Las proyecciones de los vectores 2d se pueden tomar como 1d bajo una transformación



# Cross Product
Es el área del paralelogramo formado por dos vectores. Se calcula con la determinante. 
![[Pasted image 20220503164235.png]]

### Deep 
Básicamente lo que se está buscando es un vector P tal que al hacerle el producto escalar con un vector que se comparte en ambas ecuaciones, nos va a dar igual.
![[Pasted image 20220503165909.png]]
Y como las componentes de la matriz derecha son:
![[Pasted image 20220503165952.png]]
Se da que las componentes de P son las mismas que las componentes del determinante. 
### Gráficamente 

![[Cross products in the light of linear transformations _ Chapter 11, Essence of linear algebra - YouTube - Google Chrome 2022-05-03 17-02-02.mp4]]


### La regla de Cramer
Te dice que como luego de una transformación lineal las áreas se escalan proporcionalmente, puedes decir que el área que forma el vector que quieres encontrar (x, y) con el eje X inicial, que comienza siendo 1, simplemente será el área igual a y, si consideras y, porque es la altura del paralelogramo que forman (y), por el largo del paralelogramo (1 porque es X inicial). Y ahora podemos repetir lo mismo para x, ya que sabemos que la altura será 1, debido a que Y inicial es igual a 1, y la x será la x del vector.
![[y2mate.com - Cramers rule explained geometrically  Chapter 12 Essence of linear algebra_1080pFHR.mp4 - Reproductor multimedia VLC 2022-05-14 19-10-49.mp4]]
![[y2mate.com - Cramers rule explained geometrically  Chapter 12 Essence of linear algebra_1080pFHR.mp4 - Reproductor multimedia VLC 2022-05-14 19-11-44.mp4]]


Y como todas las áreas escalan de la misma forma, podemos realizar un cálculo con estas áreas. 
Sabemos que el área de y va a ser igual al área inicial más lo que creció o se achicó (calculado con la determinante de la transformación lineal)
![[y2mate.com - Cramers rule explained geometrically  Chapter 12 Essence of linear algebra_1080pFHR.mp4 - Reproductor multimedia VLC 2022-05-14 19-14-37.mp4]]
Y como lo que queremos encontrar es el área que forman los dos vectores, debemos hacer el producto cruz, y para hacer el producto cruz debemos utilizar la determinante. La determinante nos da el área de un paralelogramo formado por el versor i transformado y el nuevo vector (que ya viene provisto por las ecuaciones)
![[Pasted image 20220514192020.png]]

Y también tenemos el determinante de la transformación, que en todos los casos nos dice el área o volumen (dependiendo de la cantidad de dimensiones), que se forma con los nuevos versores transformados, y este volumen o área cambia en todo el plano, porque antes era 1x1 y ahora es distinto, y como es todo proporcional, aplica a todo el plano.
![[y2mate.com - Cramers rule explained geometrically  Chapter 12 Essence of linear algebra_1080pFHR.mp4 - Reproductor multimedia VLC 2022-05-14 19-17-13.mp4]]
Lo mismo se aplica para x.
![[y2mate.com - Cramers rule explained geometrically  Chapter 12 Essence of linear algebra_1080pFHR.mp4 - Reproductor multimedia VLC 2022-05-14 19-25-31.mp4]]