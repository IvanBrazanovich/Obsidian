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

