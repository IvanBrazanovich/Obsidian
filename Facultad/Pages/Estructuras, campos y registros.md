

### ¿Qué es un campo?
Es un conjunto de caracteres capaz de suministrar una determinada información referida a un concepto. 

Un campo es un dato elemental tal como nombre y apellido, número de documento, domicilio, etc. 

Al igual que en las variables, al definir un campo hay que indicar claramente tres características: 
+ Nombre: Nombre que identifica a ese conjunto de caracteres. 
+ Tipología: Tipo de caracteres que puede contener (alfabético, entero, etc.)
+ Tamaño: Cantidad de caracteres que puede contener. 

#### Ejemplo 
Nombre: Document 
Tipo: numérico
Tamaño: 8 enteros.
	 **Document: N(8)**

Un campo es la entidad lógica más pequeña, consiste en un conjunto de bytes que conforman un dato

### Registro 
Un registro es un conjunto de campos referentes a una entidad en particular, o sea, es un conjunto de información referido a algo. 

Un ejemplo puede ser la información de un determinado alumno universitario que contiene distintos campos. 
![[Pasted image 20220518063240.png]]


#### Un campo es la unidad mínima de información de un registro
![[Pasted image 20220518063307.png]]





## Ventajas y desventajas: guardar información 
### Utilizando marcas
![[Pasted image 20220518063430.png]]
#### Desventajas 
+ Hay que manejar los datos como subsecuencias encerradas por marcas. 
+ Para trabajar aritméticamente hay que convertir de carácter a numérico. 

#### Ventajas
+ La secuencia mayor que los contiene a todos ocupa menor espacio
+ Cuando sabemos que mucha información no estará completa es buena opción



### Utilizando registros 
#### Desventajas
+ Si un campo necesita más espacio, hay que arreglar la longitud del campo en todos los registros, y se pierde espacio y tiempo. 
+ La secuencia mayor que contiene los registros (archivo) tiene a ser más grande. 


#### Ventajas
+ Cuando sabemos que nuestros campos siempre tendrán la misma longitud es buena opción
+ Es más rápido el acceso y la programación de campos que recorrer secuencias. 
+ Puedo definir numéricos y trabajar con aritméticos sin convertir. 



### Definición de registros 
#### Definición arbórea o jerárquica de registros
Suele utilizarse como borrador. Consiste en una serie de nodos que se vinculan con flechas. 
![[Pasted image 20220518064130.png]]

#### Definición gráfica 
Es una estructura de forma lineal, que usualmente utiliza el analista/ingeniero para definir la estructura cuando le suministra el problema al programador. 
![[Pasted image 20220518064225.png]]


#### Definición por nivel o literaria 
Esta es la forma de representar los datos en el ambiente del algoritmo. 
Cuando se debe ocupar varias veces, se lo guarda en una biblioteca de estructuras y luego se lo busca de allí nomás. 
![[Pasted image 20220518064334.png]]



#### Registro lógico 
