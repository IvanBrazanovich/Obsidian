

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
Son los registros organizados en campos. 



#### Registro físico 
Es un conjunto de registros lógicos que constituyen una unidad de transferencia en una sola operación de entrada/ salida. Para transferencias entre dispositivos de almacenamiento o memoria principal. 



### Archivos 
Es un conjunto de registros homogéneos referidos a objetos de la misma naturaleza o del mismo tipo, almacenados en un soporte externo, que presenta entre sí una relación lógica y que pueden ser consultados individualmente de forma iterativa o sistemática.  O sea, básicamente vas a tener un tema principal y luego vas a tener registros de la misma temática dentro del archivo. ¿Puede el archivo tener dos tipos de registros, por ejemplo de un alumno y de cantidad de comida en la facultad?
![[Pasted image 20220518064917.png]]


Un archivo en una computadora es una estructura diseñada para contener datos, estos están organizados de forma tal que pueden ser recuperados fácilmente, borrados, actualizados, etc. 
Cabe recalcar que los archivos tienen nombres. 

![[Pasted image 20220518065117.png]]



### Base de datos 
Es una colección de archivos relacionados lógicamente, que se estructura en diferentes formas para reducir duplicaciones y proporcionar un mejor acceso a los datos. Constituye el nivel más alto de la jerarquía de organización de los datos, siendo el nivel más bajo el carácter. 

Así una base de datos de una universidad podría contener archivos de estudiantes, profesores, inventarios, libros, etc. 
![[Pasted image 20220518065343.png]]



### Campo clave
Un campo clave (key) es aquel que identifica al registro y lo diferencia de los otros registros. 
Debe ser ÚNICO, debe ser diferente para cada registro. Por ejemplo para un alumno puede ser la libreta universitaria.
![[Pasted image 20220518070424.png]]



### Campo clave secundaria 
Es aquel que aún siendo un campo importante puede no identificar al registro en el archivo. 
Considerando la definición que se utiliza para las bases de datos, es un valor que no necesariamente identifica totalmente a un registro(puede haber repeticiones), pero sirve para procesar la información en un orden adecuado, para algún proceso en particular.
Por ejemplo, la Fecha de una factura es importante para listar los Libros de IVA o para filtrar facturas entre fechas, por ello se la establece como Clave Secundaria.

### Campo clave simple 
Es aquel que está formado por un campo contenido, es decir, no se encuentra subdividido. 


### Clave foránea
Es una clave secundaria, pero esta implica una relación con otro archivo. Es decir, permite la relación entre dos estructuras externas. 




### Campo clave compleja 
Es aquel que está formado por un campo continente, es decir, se encuentra subdividido en campos contenidos. 
![[Pasted image 20220518070754.png]]
