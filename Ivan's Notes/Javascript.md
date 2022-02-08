# Variables
¿Qué es LET?
Es una forma de inicializar una variable que puede cambiarse luego 


¿Qué es const?
Es una forma de inicializar una constante.


¿Cuáles son las diferencias entre const y let?
Que const no se puede cambiar y debe iniciar con un valor.



# Strings 

### Métodos
Los métodos de strings son: 
> console.log(variable.length)

Básicamente te dice la cantidad de letras que tiene un texto 

> console.log(variable.indexOf("tablet"))

Básicamente te dice cuándo comienza esa palabra en un string.

> console.log(variable.includes("tablet"))

Te dice si en el string está esa palabra


> console.log(variable.trim())
> console.log(variable.trimStart())
> console.log(variable.trimEnd())
> 

Recorta los espacios en blanco. Ya sea todo, al inicio o al final.


> console.log(variable.replace("pulgadas", " " " ))
> console.log(variable.replace("monitor", " monitor curvo " ))

Reemplaza lo primero por lo segundo en un string


> console.log(variable.slice(0, 1))

Recorta del 0 al 1 en un string 

>console.log(variable.charAt(0))

Te da la primera letra


> console.log(variable.repeat(3))

Repite la cadena de texto 3 veces


> const variable = "leer, caminar, cocinar, volar"  
> console.log(variable.split(", "))

Divide la cadena de texto cada vez que hay una ,


> console.log(variable.toUpperCase())
> console.log(variable.toLowerCase())
> console.log(variable.toString())

Convierte todo en mayúsculas, convierte todo en minusculas, convierte en un string.

### Concatenar
> console.log(producto.concat(precio))
> console.log(producto.concat("En descuento"))


> console.log("El producto tiene un valor de " + precio )
> console.log("El producto tiene un valor de ", precio )


> console.log('El producto tiene un valor de $ ${precio}')








# Objetos
+ **¿Cómo acceder a los valores de un objeto?**
	> console.log (producto.precio)
	> console.log(producto["precio"])

+ ¿Cómo agregar una propiedad a un objeto?
	> producto.imagen = "imagen.jpg" 

+ ¿Cómo eliminar una propiedad de un objeto?
	> delete producto.nombre;

+ ¿Cómo hacer destructuring?
	> const { nombre, precio } = producto;

+ ¿Cómo hacer destructuring de objetos anidados?
	> const {nombre, información, información: {fabricación, fabricación: {país}}} } = producto;

+ ¿Cómo evitar que se cambie un objeto? O sea congelarlo
	Hay que utilizar el método de Freeze.
	> "use strict";
	> Object.freeze(producto)

	Y luego si quieres ver si tiene un freeze puedes usar
	> console.log(Object.isFrozen(producto))

+ ¿Cuál es la diferencia entre Freeze y Seal?
	 Que seal te permite cambiar las llaves existentes pero no te permite crear ni eliminar. Mientras que freeze no te deja hacer nada

+ ¿Cómo puedo unir dos objetos?
	>const resultado = Object.assign(producto, medidas)
	
	Como también se puede 
	> const resultado = { ...productos, ...medidas }
	> 

+ ¿Para qué sirve la palabra this en un objeto?
	+ Sirve para hacer referencia a sí misma. O sea si tienes una variable fuera del objeto y la quieres llamar puedes, pero si tienes una dentro del objeto no. La solución a esto es utilizar this.
	> const producto = {
			>nombre: "Tablet",
			>precio: 200,
			>disponible: true,
			>mostrarInfo: function () {
					>console.log('El producto ${this.nombre} tiene un precio de ${this.precio}')
			>}
	> }

+ ¿Cómo se puede crear objetos de manera dinámica?
	Con el object constructor
	> function Producto (nombre, precio) {
		> this.nombre = nombre;
		> this.precio = precio;
	> }

	this.nombre lo que hace es asociar el nombre que le pasas en esa instancia a ese objeto en particular.

	Y luego lo que haces es hacer una instancia.
	> const producto1 = new Producto ("monitor", 200)

+ ¿Para qué sirven los métodos keys, values y entries?
	+ Para saber la información de las llaves, valores y todo en orden. 
	> console.log(Object.keys(producto))
	> console.log(Object.values(producto))
	> console.log(Object.entries(producto))


# Arreglos
+ ¿Cómo acceder a lo valores de un arreglo?
	utilizando los índices
	> console.log(producto[0])

+ ¿Cómo puedo acceder a todos los valores de un arreglo?
	+ Con un for loop 
	> for (let i = 0; i < meses.length; i++ ) {
		> console.log(meses[i])
	> }

+ ¿Puedo cambiar un valor de un arreglo o agregar uno nuevo?
	+ Si, de la siguiente manera
	> meses[0] = "Cambio de valor"
	> meses [10] = "Arreglo nuevo"

+ ¿Cómo puedo agregar un valor al inicio o al final de un arreglo?
	> meses.push("abril") -- agrega al final del arreglo--
	> meses.unshiift("diciembre") --agrega al inicio del arreglo--


	O también

	> const carrito = [];
	> const producto = { mes: "enero",  numero: 20};
	> let resultado = [producto, ...carrito]

+ ¿Cómo puedo eliminar valores de un arreglo?
	+ Se puede utilizando 3 métodos: pop (el último), shift (el primero) y spllice.
	> meses.Splice (3, 1) ---significa que debe eliminar de la posición 3 en adelante--

+ ¿Cómo puedo hacer un destructuring de arreglos?
	+ Casi de la misma forma que los objetos.
	> numeros = [1, 2, 3, 4. 5]
	> const {primero, segundo} = numeros; --esto me dará 1 y 2--
	> const {primero, segundo, ...tercero} = numeros; --esto me dará 1, 2 y de 3 a 5 en un solo arreglo.--
	> const {, , , cuarto} = numeros; --esto me  dará el 4--

+ ¿Qué hace un forEach?
	+ Es un for loop para arreglos básicamente. Itera por todos los valores
	> meses.forEach( function (producto)  {
		> console.log(producto)
	> } )

+ ¿Qué hace un map y cuál es la diferencia con forEach?
	+ Lo que hace es crear un nuevo arreglo. 
	>const nuevoArreglo = meses.map( function (producto)  {
		> return producto;
	> } )

+ ¿Qué es un some y un includes?
	+ Some es para arreglos de objetos de la siguiente manera
	> const existe = carrito.some( producto => producto.nombre === "Monitor");

	En el caso de que sea un arreglo tradicional se utiliza includes
	> const resultado = meses.includes("febrero")

+ ¿Qué es findIndex?
	Es para encontrar el índice dependiendo del que incluya algo 
	> const indice = mes.findIndex( mes => mes === "diciembre")

	En el caso de que sea un arreglo de objetos sería así
	> const indice = carrito.findIndex(producto => producto.nombre === "monitor")
	
+ ¿Qué es un reduce?
	+ Es una forma de tomar una gran cantidad de datos, operar con ellos y entregar un resultado 
	> const resultado = carrito.reduce( (total, producto) => total + producto.precio, 0 )

+ ¿Qué es un filter?
	>const resultado = carrito.filter( producto => producto.precio > 300)
 
+ ¿Qué es find?
	Devuelve el primer igual que corresponde
	>const resultado = carrito.find( producto => producto.precio === 300)

+ ¿Qué es every?
	+ Retorna un booleano.
	> const booleano = carrito.every ( producto => producto.precio > 100)




# Function
+ ¿Cómo crear una función?
	Function declaration
	>function sumar () {
		>console.log(2 + 2)
	>}

	Como también se puede utilizar function expression
	> const Sumar2 = function () {
	> }

+ ¿Cuál es la diferencia entre Function declaration y function expression?
	Que la function declaration te permite llamarla antes en el código debido al hoisting, en cambio la function expression no, debes llamarla después de crearla, o sea que el llamado de la función debe estar debajo del código de inicialización. 

+ ¿Cuál es la diferencia entre un método y una función?
	Son básicamente lo mismo, pero se llaman de manera distinta.
	El método se llama de la siguiente manera 
	>console.log( numero.toString())

	Mientras que la función se llama de la siguiente manera 
	>console.log( parseInt(numero))

+ ¿Cuáles son los parámetros por default en una función?
	> function sumar( numero1= 1, numero2 = 2) {
	> }

+ ¿Cómo agregar funciones dentro de un objeto?
	 De la siguiente manera 
	> const reproductor = {
		> reproducir: function() {
			> console.log("Esto es una función dentro de un objeto")
		> } 
	> }
	> Y se llama de la siguiente manera 
	> reproductor.reproducir()

+ ¿Qué es un Switch?
	+ Es una forma de analizar varias opciones como un else if pero repetido
	> switch (metodoPago) {
		> case "Efectivo":
			 console.log('Pagaste con ${metodoPago}')
				>break;
			case "Tarjeta" ;
				console.log('Pagaste con ${metodoPago}')
					break;
			default:
				break;
	> }



# Iteradores
+ ¿Cuál es la diferencia entre un break y un continue en un for loop?
	+ La diferencia es que en el caso de un break va a dejar de ejecutar el foor loop. En el caso de continue va cortar con ese ciclo pero va a seguir ejecutando el foor loop.

+ ¿Qué iteradores existen?
	+ For (común)
	+ while (mientras se cumpla una condición ejecuta)
	+ do while (ejecuta si o si una vez un ciclo)
	+ forEach  y map (es para arreglos)
	+ for of (es para arreglos) 
	+ for in (es para objetos)

# Prototypes
+ ¿Qué problemas solucionan los prototypes?
	En caso de tener un proyecto grande con mucho código, muchas veces se confunde las funciones para cada cosa. Es por eso que se pueden usar los prototypes. Básicamente son funciones que solamente se pueden usar dentro de un objeto por así decirlo. ![[Pasted image 20220206175839.png]]
+ ¿Cómo heredar funciones en prototypes?
	+ ![[Pasted image 20220206180851.png]]

+ ¿Cuál es la diferencia entre arrow function y functions normales para prototypes?
	+ Que al tener que usar this. debes utilizar functions normales porque toma como referencia el objeto. En el caso de utilizar arrow function va a tomar referencia de todo el código, la ventana global.













# Programación Orientada a Objetos
+ ¿Qué es la POO?
	+ Se utilizan clases en las que las funciones pueden ser utilizadas solo por las clases para las cuales se crearon.  
+ ¿Cómo se crean las clases?
	+  ![[Pasted image 20220207171115.png]]
+ ¿Qué son los métodos y los métodos estáticos?
	+ Los métodos son básicamente funciones que solamente puede usar la clase para la que se crearon. Los métodos estáticos son funciones creadas para las clases en sí y que no se pueden usar en las instancias de las clases.  
+ ¿Cómo se heredan las clases y los constructores de una clase?
	+  ![[Pasted image 20220207171147.png]]
+ ¿Se pueden rescribir funciones?
	+ si
+ ¿Qué son las propiedades privadas en POO?
		+ Son básicamente formas de que no se pueda acceder a las propiedades de una instancia de una clase a partir de una instancia. Solo se puede acceder a la propiedad a partir de la clase en sí. 
	+ ![[Pasted image 20220207171356.png]]
+ 
+ 