- [ ] Vectores.
- [ ]  Definición
- [ ] . Adición vectorial. 
- [ ] Propiedades de la adición. 
- [ ] Multiplicación de un vector por un escalar.
- [ ]  Propiedades. 
- [ ] Producto interno o producto escalar. 
- [ ] Propiedades. 
- [ ] Interpretación geométrica del producto escalar. 
- [ ] Vectores ortogonales. Producto exterior o producto vectorial.
- [ ]  Propiedades. Interpretación geométrica del producto vectorial. 
- [ ] Producto mixto. Interpretación geométrica del producto mixto





# Matrices

- [ ] Matrices. 
- [ ] Definición, clasificación Matriz: traspuesta, nula, opuesta. 
- [ ] Matrices cuadradas especiales: matriz identidad, simétrica, triangular, regular, singular.
- [ ]  Igualdad de matrices. 
- [ ] Operaciones: suma, resta, multiplicación por un escalar, multiplicación de matrices. 
- [ ] Propiedades. 
- [ ] Operaciones elementales entre líneas de una matriz Matrices separadas o particionadas.
- [ ]  Multiplicación por bloques. Matrices elementales. Rango de una matriz. Problemas de aplicación



# Determinantes
- [ ] Determinante de una matriz.
- [ ]  Definición. Solución de un determinante. 
- [ ] Regla de Sarrus. Solución de un determinante por los elementos de una línea. 
- [ ] Determinante de una matriz y de su traspuesta.
- [ ]  Determinante de una matriz triangular. Propiedades de los determinantes. 
- [ ] Determinante de una matriz no singular. 
- [ ] Adjunta de una matriz. Inversa de una matriz.




### ¿Qué es una matriz?
Una matriz de clase “mxn” es un conjunto  de números ordenado en “m” renglones (o filas) y “n” columnas.


#### ¿Cuándo las matrices son iguales?
Dos matrices A = (aij)m×n y B = (bij)p×q son iguales, sí y solo si, tienen en los mismo lugares elementos iguales, es decir :



### Dependencia lineal entre filas 
#### ¿Qué es una combinación lineal?
La fila 1 de una matriz es combinación lineal si existen los escalares k1, k2, k3, etc. distintos de cero, tal que. 
![[Pasted image 20220504185559.png]]


#### ¿Qué es una fila dependiente?
Las filas de una matriz son linealmente dependientes si existen los escalares k1, k2, k3, etc. distintos de cero, tal que se cumpla: 
![[Pasted image 20220504190600.png]]



#### ¿Qué es la combinación trivial?
Cuando para la ecuación de dependencia lineal 
![[Pasted image 20220504185211.png]]
Alfa es igual a cero. Debido a que en caso de que alfa sea cero en todas siempre se cumple.



#### ¿Cuándo las filas de una matriz son linealmente independientes?
Cuando se cumple 
![[Pasted image 20220504190651.png]]
Solo para k iguales a cero. 



#### ¿Qué es el rango de una matriz?
Es el número máximo de filas, o de columnas, linealmente independientes de dicha matriz. 


#### ¿Qué son las operaciones elementales?
Son las operaciones que podemos realizar en una matriz sin que su rango varíe:
+ Permutar 2 filas ó dos columnas.
+ Multiplicar o dividir una línea (fila o columna) por un número no nulo.
+ Sumar o restar a una línea  otra paralela multiplicada por un número no nulo. 




### Cálculo del rango de una matriz por el método de Gauss
+ Aplicar op. elementales => triangular la matriz
+ Rango => Número de filas no nulas.

![[Pasted image 20220504191610.png]]





# Determinantes 
Es toda función que asigna a cada matriz cuadrada un escalar llamado determinante de la matriz.

### Determinantes de primer orden 
Si la matriz es de 1x1, el determinante es igual al único elemento de dicha matriz. 




### Determinantes de segundo orden 
Dada una matriz de orden dos, se llama determinante de la matriz al número que se obtiene así: 
![[Pasted image 20220504193135.png]]

![[Pasted image 20220504193141.png]]

Se representa Det(A) ó |A|



### Determinantes de tercer Orden 
Si A es una matriz cuadrada de orden 3, se llama determinante de A al número que se obtiene aplicando la regla de Sarrus. LA REGLA DE SARRUS ES VÁLIDA ÚNICAMENTE PARA DETERMINATNES DE ORDEN 3. 



### Calcular determinante para cualquier orden 
Desarrollo por los elementos de una línea 


### Definición Axiomática de determinante

![[Pasted image 20220504193359.png]]



### ¿Qué propiedades se deducen de los axiomas?

![[Pasted image 20220508070639.png]]
![[Pasted image 20220508070645.png]]



### Menor complementario del elemento aij.
![[Pasted image 20220504194115.png]]
![[Pasted image 20220508070830.png]]

### Cofactor o adjunto de un elemento 
![[Pasted image 20220508070907.png]]
![[Pasted image 20220504194326.png]]




### Desarrollo de un determinante por los elementos de una línea 
![[Pasted image 20220508071038.png]]
![[Pasted image 20220508071056.png]]

### Otras propiedades de los determinantes
![[Pasted image 20220508071209.png]]



### Matriz Regular 
Cuando su determinante no es nulo


### Matriz Singular 
Cuando su determinante es nulo



### Matriz Adjunta 

Dada una matriz A cuadrada se llama adjunta de A a la matriz que se obtiene reemplazando cada elemento de la transpuesta de A por su adjunto. 

![[Pasted image 20220504194732.png]]

### Propiedad de la matriz adjunta 
![[Pasted image 20220508071323.png]]

### Matriz Inversa 
![[Pasted image 20220508071458.png]]

#### Demostración de que las inversas de las matrices son únicas
![[Pasted image 20220508071645.png]]




### Propiedades de la inversa
1. La inversa de una matriz es única
![[Pasted image 20220508071727.png]]



### Cálculo de la matriz inversa utilizando matriz adjunta 
![[Pasted image 20220508072028.png]]
![[Pasted image 20220508071839.png]]
![[Pasted image 20220508071846.png]]






### Hallar vector unitario 
![[Pasted image 20220509214934.png]]



### Encontrar el vector que haga perpendicular al vector
![[Pasted image 20220509215320.png]]


![[Pasted image 20220509215852.png]]





























