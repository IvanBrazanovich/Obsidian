# Temas
Digrafos y grafos: Primeros ejemplos. Nodos, arcos, adyacencia, incidencia, grado, caminos, ciclos. Subdigrafos y dígrafos parciales. Relaciones binarias y digrafos Conexidad. Matrices y digrafos. Matriz de adyacencia y de conexión. Suma y producto de digrafos. Grafos regulares, completos, eulerianos, hamiltonianos. Árboles. Árboles con raíz. Los árboles como estructuras ordenadas y etiquetadas.



### ¿Qué es un grafo?
Es una red que te permite visualizar las relaciones entre varios componentes. 
![[Pasted image 20220512052030.png]]
Los círculos representan los componentes y las líneas que los conectan pueden pensarse como las relaciones que existen entre ellos.

#### ¿Para qué sirve la teoría de grafos?
La teoría de grafos se encarga de estudiar este tipo de redes y cómo se pueden usar para modelar y resolver muchos tipos de problemas. 


#### ¿Por qué debería estudiar teoría de grafos?
Porque nos permite resolver muchos problemas y está en todos lados. Por ejemplo las aplicaciones de navegación que te pueden decir la mejor ruta hacia un destino.
![[Pasted image 20220512052439.png]]
También se puede utilizar en aplicaciones de redes sociales. Estas se pueden modelar mediante grafos y se pueden solucionar un montón de problemas mediante la utilización de sus teoremas. 

#### ¿Qué es el grado de un vértice?
La cantidad de aristas que tiene conectado al vértice.

#### ¿Qué es un camino en teoría de grafos?
Es una secuencia de vértices conectados por aristas. 
![[Pasted image 20220512053153.png]]
La extensión o el largo de un camino se define por la cantidad de aristas que posee.  



#### ¿Qué es un ciclo en la teoría de grafos?
Es un camino que comienza y termina en el mismo vértice.
![[Pasted image 20220512053344.png]]




#### ¿Qué es la conectividad en la teoría de grafos?
Hay dos formas: 
Aplicado a vértices
+ Si un camino existe entre dos vértices, estos están conectados. 

Aplicado a grafos
+ Un grafo está conectado si todos los vértices están conectados entre si. 
![[Pasted image 20220512053716.png]]
Este grafo no está conectado. 




#### ¿Qué son los componentes conectados?
Un componente conectado es un subconjunto en el gráfico que está conectado. 
![[Pasted image 20220512053851.png]]



### ¿Qué tipos de grafos existen?

#### Grafos no direccionales 
Es no direccional cuando una arista significa que existe una conexión de v1 a v2 y lo contrario. 
![[Pasted image 20220512054051.png]]




#### direccionales
 Los grafos direccionales son unidireccionales, lo que significa que van hacia un solo lado nomás. 
![[Pasted image 20220512054139.png]]



#### ¿Qué son los grafos pesados?
Son aquellos en los que las aristas no tienen las mismas importancias.
![[Pasted image 20220512054318.png]]



#### ¿Qué son los grafos árboles?
Deben cumplir 3 condiciones. 
+ Deben están conectados y ser acíclicos. 
+ Si remueves una arista desconectas el grafo. 
+ Agregar una arista crea un ciclo.
![[Pasted image 20220512054458.png]]



#### ¿Cómo se podría representar un grafo?
Se puede realizar mediante una matriz adyacencia, y una lista de adyacencia. 


#### ¿Qué es una matriz adyacencia?
Es una matriz en el que las filas y las columnas son los vértices y cada vez que exista una arista entre vértices se pone un 0. 
![[Pasted image 20220512054914.png]]


#### ¿Qué es una lista de adyacencia ?
Es una lista en la que se toma cada vértice y se le hace una lista con sus vecinos.
![[Pasted image 20220512055043.png]]







