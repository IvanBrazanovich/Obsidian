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
Es una cadena donde el vértice inicial es igual al vértice final.



#### ¿Qué es la conectividad en la teoría de grafos?
Hay dos formas: 
Aplicado a vértices
+ Si un camino existe entre dos vértices, estos están conectados. 

Aplicado a grafos
+ Un grafo está conectado si todos los vértices están conectados entre si. 
![[Pasted image 20220512053716.png]]
Este grafo no está conectado. 

#### ¿Cuándo un vértice es accesible?
Un vértice Vj se dice accesible desde un vértice Vi si existe una cadena entre ellos. Todo vértice es accesible desde sí mismo.








#### ¿Qué son los componentes conectados?
Un componente conectado es un subconjunto en el gráfico que está conectado. 
![[Pasted image 20220512053851.png]]



### ¿Qué tipos de grafos existen?

#### Grafos no orientados 
Es no direccional cuando una arista significa que existe una conexión de v1 a v2 y lo contrario. 
![[Pasted image 20220512054051.png]]

La definición técnica es 
![[Pasted image 20220512062702.png]]
Donde v son los vértices o nodos. A son las aristas y el símbolo es una función de incidencia, que asigna a cada arista un par no ordenado de vértices llamados sus extremos. 



####  Grafos orientados
 Los grafos direccionales son unidireccionales, lo que significa que van hacia un solo lado nomás. 
![[Pasted image 20220512054139.png]]
![[Pasted image 20220512064836.png]]
Donde V son los vértices o nodos. A son los arcos y el símbolo es una función llamada función de incidencia orientada que asigna a cada arco un par de vértices llamados sus extremos. 
![[Pasted image 20220512064950.png]]



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
![[Pasted image 20220512070756.png]]
![[Pasted image 20220512070801.png]]
La suma de los elementos distintos de cero de la matriz es igual a dos veces el número de aristas (los elementos de la diagonal principal se cuentan dobles)



#### ¿Qué es una lista de adyacencia ?
Es una lista en la que se toma cada vértice y se le hace una lista con sus vecinos.
![[Pasted image 20220512055043.png]]





#### ¿Qué es una arista incidente?
Si v1 es un extremo de a1 entonces a1 y v1 son incidentes.


#### ¿Qué son los vértices adyacentes?
Dos vértices son adyacentes si existe una arista que los une. 


#### ¿Qué son las aristas adyacentes?
Dos aristas son adyacentes si tienen un vértice en común


#### ¿Qué es un vértice aislado?
Es un vértice de grado 0.



#### ¿Qué es un vértice pendiente?
Si el grado del vértice es uno. 


#### ¿Qué es un lazo?
Es una arista cuyos extremos coinciden.


#### ¿Qué son las aristas paralelas?
Dos aristas son paralelas cuando tienen el mismo vértice inicial y final. 



#### ¿Qué es una cadena?
Es una sucesión finita de aristas



#### ¿Qué es la longitud de una cadena?
Es el número de aristas que la componen


#### ¿Qué es una cadena sencilla?
Es la cadena en la que no se repiten aristas. 



#### ¿Qué es una cadena elemental?
Es la cadena en la que no se repiten vértices

#### ¿Qué es un grafo simple?
Es un grafo sin lazos ni aristas paralelas. 


#### ¿Qué es un grafo completo?
Es un grafo en el que tiene exactamente una arista entre cada par de vértices distintos.
![[Pasted image 20220512063907.png]]


#### ¿Qué es el grafo K-Regular?
Es el grafo en el que todos sus nodos tienen el mismo grado
![[Pasted image 20220512063954.png]]


#### ¿Qué es un grafo bipartito?
Es un grafo en el que un subconjunto del grafo "se conectan o van" hacia el otro conjunto, y del otro conjunto van al primero.
![[Pasted image 20220512064320.png]]


#### ¿Qué es un grafo bipartito completo?
Es un grafo en el que el subconjunto 1 se conecta en su totalidad con todos los vértices del subconjunto 2 y al revés. 
![[Pasted image 20220512064645.png]]
K3,1 significa que un subconjunto tiene  3 tiene y el otro 1 vértice.




#### ¿Qué es un rizo o bucle?
Es un arco cuyo vértice final coincide con el vértice inicial. 


#### ¿Qué son los arcos estrictamente paralelos?
Dos arcos son estrictamente paralelos si tienen el mismo vértice final y el mismo vértice inicial. 


#### ¿Qué son los arcos adyacentes?
Dos arcos son adyacentes si tienen un vértice común. 


#### ¿Qué son los vértices adyacentes?
Dos vértices son adyacentes si existe un arco que los une. 


#### ¿Qué es la incidencia positiva?
Un arco es incidente positivo a un vértice si el arco se origina en el mismo vértice. 

#### ¿Qué es la incidencia negativa?
Un arco es incidente negativo a un vértice si el vértice es extremo del arco. 



#### ¿Qué es el grado positivo de un vértice?
Es la cantidad de arcos que inciden positivamente en el vértice


#### ¿Qué es el grado negativo de un vértice?
Es la cantidad de arcos que inciden negativamente en el vértice



#### ¿Qué es el grado total?
Es la suma de los grados positivos y los grados negativos del vértice
![[Pasted image 20220512065559.png]]

#### ¿Qué es el grado neto?
Es la resta de los grados positivos y los grados negativos del vértice
![[Pasted image 20220512065618.png]]


#### ¿Cuáles son las propiedades de los grados de un vértice?
![[Pasted image 20220512065936.png]]
La suma de los grados positivos de los vértices es igual a la suma de los grados negativos de los vértices  y es igual a el número de arcos del grafo.


![[Pasted image 20220512070034.png]]
El grado total es la suma de ambos grados, es por eso que es 2 por el número de arcos del grafo. 

![[Pasted image 20220512070122.png]] 
Y el grado neto es igual a cero porque es la diferencia. 



#### ¿Qué es un camino en grafos?
Es una secuencia de arcos



#### ¿Qué es un camino sencillo en grafos?
Es el camino tal que no se repiten arcos- 


 #### ¿Qué es un camino elemental en grafos?
Es un camino donde no ser repiten vértices



#### ¿Qué es un circuito en grafos?
Es un camino donde el vértice final coincide con el vértice inicial



#### ¿Qué es un circuito sencillo en grafos?
Es el circuito donde no se repiten arcos



#### ¿Qué es un circuito elemental en grafos?
Es el circuito donde no se repiten vértices, con excepción del primero y el último.



#### ¿Qué es la longitud de un camino en grafos?
Es la cantidad de arcos que compone el camino. 




### ¿Qué es la matriz de incidencia de arcos?
Es aquella en la que se representan las incidencias positivas y negativas.
 ![[Pasted image 20220512153802.png]]
![[Pasted image 20220512153804.png]]
En el que: 
+ La suma de los elementos de cada fila es igual al grado neto del vértice correspondiente. 
+ La suma de los valores absolutos de los elementos es igual grado total. 




#### ¿Qué es un subgrafo?
Un subgrafo pertenece a otro grafo cuando: 
![[Pasted image 20220512154112.png]]



### SUBGrafos particulares 
+ Subgrafo restante respecto del vértice es el subgrafo de G que se obtiene al suprimir únicamente el vértice Vi. 
+ Subgrafo restante respecto de la arista Ai. Se obtiene al suprimir únicamente la arista Ai. 
+ 
#### Subgrafo minimal
 Subgrafo minimal: Un subgrafo S de G que goce de una propiedad P se llama minimal respecto de P, sin ningún subgrafo estrictamente menor que S que puede gozar de la propiedad.
Supongamos que P es la propiedad "tener un solo ciclo"
![[Pasted image 20220512155203.png]]
Serán esos subgrafos minimales: 
![[Pasted image 20220512155224.png]]


#### Subgrafo Maximal 
Un subgrafo S de G que goce de una propiedad P se llama maximal respecto de P, si ningún subgrafo estrictamente mayor que S goza de la propiedad P. 



#### Subgrafo cobertor 
Se llama cobertor si contiene a todos los vértices de G. 


#### ¿Qué es el grafo complementario?
Si contiene al mismo conjunto de vértices de G y cuyas aristas son las que le faltan a G para ser completo. 
![[Pasted image 20220512155707.png]]

![[Pasted image 20220512155712.png]]


 ### ¿Qué es la conexidad en los grafos? 
 Un grafo g no orientado es conexo, para todos dos vértices cualquiera, existe una cadena de uno a otro.
![[Pasted image 20220512103243.png]]
![[Pasted image 20220512103355.png]]





### ¿Qué es una componente conexa?
Es el conjunto de vértices pertenecientes al conjunto de vértices, tal que existe una cadena que va de Vn a v.
![[Pasted image 20220512103701.png]]
O sea si entre 5 vértices, 2 serían componente conexa de un vértice y se ponen así Cv1={v1, v2} Y como se hace la unión Cv1={v1, v2, v1}

El vértice aislado se considera que es una componente conexa.





### ¿Cuándo se considera a un grafo no orientado conexo?
Cuando solo tiene una componente conexa 





### ¿Qué es un grafo orientado conexo?
Cuando para todo par de vértices, distintos, del mismo existe un camino que los une por lo menos en un sentido. 

![[Pasted image 20220512110204.png]]
Es conexo 

![[Pasted image 20220512110232.png]]
No es conexo 





### ¿Cuándo un grafo orientado es fuertemente conexo?
Es fuertemente conexo cuando para todo par de vértices distintos por el mismo están unidos en ambos sentidos. 
