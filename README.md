## Práctica: Implementación de una Pila Genérica

### Objetivo

El objetivo de esta práctica es que los alumnos implementen una pila genérica en Kotlin utilizando los principios de programación orientada a objetos (POO). La implementación debe seguir una estructura bien definida, asegurando el correcto almacenamiento y manipulación de elementos en una colección interna.

### Requisitos del ejercicio

#### 1. Implementación de la clase Pila

Se deberá diseñar una clase genérica que represente una estructura de datos tipo LIFO (Last In, First Out), donde los elementos se apilan y desapilan siguiendo este principio.

La clase debe contar con los siguientes elementos:

#### 2. Propiedades y constructores
	1.	**Descripción**
	- La pila debe incluir una descripción para identificarla.
	- Si la descripción está vacía, el programa debe lanzar un error.
	2.	**Lista interna de elementos**
	- Se debe utilizar una estructura de datos adecuada para almacenar los elementos de la pila.
	- La colección debe permitir operaciones eficientes de apilado y desapilado.
	3.	**Constructores**
  3.1. Se debe permitir la creación de una pila vacía con solo la descripción.
	3.2. Se debe permitir la creación de una pila a partir de una lista de elementos.
	- Si se intenta inicializar con una lista que contenga valores nulos, el programa debe lanzar un error.
  - Los elementos deben agregarse en orden inverso, es decir, el primer elemento del vararg debe quedar en la base de la pila.
  3.3. Se debe permitir la creación de una pila con una cantidad variable de elementos *(ver apuntes)*.
	- Los valores nulos deben eliminarse automáticamente antes de agregar los elementos a la pila.
	- Los elementos deben agregarse en orden inverso, es decir, el primer elemento del vararg debe quedar en la base de la pila.

#### 3. Métodos a implementar
	1.	Método para agregar elementos a la pila
	•	Permitir agregar elementos en la cima de la pila.
	2.	Método para extraer elementos de la pila
	•	Retornar y eliminar el elemento ubicado en la cima de la pila.
	•	Si la pila está vacía, debe devolver un valor nulo.
	3.	Método para consultar el elemento en la cima
	•	Retornar el elemento superior *sin eliminarlo*.
	•	Si la pila está vacía, debe devolver un valor null.
	4.	Método para consultar el primer elemento que fue agregado a la pila
	•	Retornar el elemento que se encuentra en la base de la pila.
	•	Si la pila está vacía, debe devolver un valor nulo.
	5.	Método para conocer el número de elementos en la pila
	•	Indicar cuántos elementos hay almacenados en la pila en un momento dado.
	6.	Método para verificar si la pila está vacía
	•	Retornar un valor booleano indicando si la pila contiene elementos o no.
	7.	Método para obtener los elementos de la pila en una lista
	•	Devolver todos los elementos en el orden en que están almacenados.
	•	Permitir que el usuario elija si desea la lista en orden normal o inverso.
	8.	Método para representar la pila como cadena de texto *(sobreescribir el método toString)*
	•	Retornar una representación clara de la pila, mostrando su descripción y los elementos que contiene.

  ```kotlin
  Pila(Descripción) => elemento1 - elemento2 - elemento3 - ... - elementoN
  ```

#### 4. Pruebas en main()

Una vez implementada la clase, los alumnos deberán realizar pruebas para verificar su correcto funcionamiento.

Debes probar lo siguiente en la función main():
	1.	Crear una pila con una descripción válida y verificar que se inicializa correctamente.
	2.	Intentar crear una pila sin descripción y comprobar que se lanza el error correspondiente.
	3.	Agregar varios elementos a la pila y verificar que se almacenan correctamente.
	4.	Consultar el elemento en la cima y asegurarse de que es el último que se agregó.
	5.	Extraer elementos de la pila y verificar que se eliminan en el orden correcto.
	6.	Consultar el primer elemento añadido a la pila (base) y asegurarse de que no cambia hasta que se desapilan todos los elementos.
	7.	Verificar el tamaño de la pila después de cada operación de inserción o eliminación.
	8.	Comprobar el funcionamiento del método que obtiene los elementos en orden normal e inverso.
	9.	Intentar desapilar cuando la pila está vacía y comprobar el comportamiento esperado.
	10.	Probar la representación en cadena de la pila antes y después de varias operaciones para asegurarse de que muestra los elementos correctamente.
