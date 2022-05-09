### Teoría 
Si los niveles mayores son impuras, los niveles menores son impuros también. 


### Teoría 
Se dice que es enlazada cuando el último carácter de la secuencia cuando es la primera parte del siguiente.

Todas las ventanas tienen que tener la misma longitud. 


Un campo es un conjunto de caracteres capaz de suministrar una determinada información referida a un concepto. 

Un campo es un dato elemental como nombre y apellido, número de documento, domicilio. 

Tiene 2 partes:
+ Nombre: nombre que identifica a ese conjunto de caracteres. 
+ Topología: tipo de caracteres que puede contener
+ Tamaño: cantidad de caracteres que puede contener. 


nombre: document
tipo: numérico
tamaño: 8 enteros
Es decir document : N(8)




Una ventana puede ser un registro de información va a tener una longitud determinada fija de x caracteres. 

Definiendo un registro
PERSONA: registro de 
		Nombre-Apellido: AN(30)
		Domicilio: AN(20)
		Localidad: AN(15)
Fin registro



ALUMNO: registro de 
		Legajo: N(8)
		Apellido-Nombre: AN(30)
		DNI: N(8)
		Domicilio: AN(15)
		Nacimiento: registro de 
				fecha_year: N(4)
				fecha_mes: N(2)
				fecha_dia: N(2)
		fin fecha registro
Fin alumno registro


El registro de información siempre va a ser continente, y lo demás es el contenido. 

En este caso los dos registros son continentes y en el caso de fecha de nacimiento es continente y contenido, no se considera registro, sino que se considera un campo. Un solo registro de información existe. 