## Nombre: Juan Ignacio Colombo

## Padron: 103471

## Link Repo: https://github.com/juanicolombo97/tp0


### Consigna

El trabajo consta en realizar una serie de Pasos sobre un programa escrito en C. La idea del mismo es poder familiarizarse con el SERCOM, el cual es el sitio de la materia, y a su ves con algunos conceptos basicos de C, y asi como tambien algunas maneras de poder controlar nuestro codigo y debuggearlo correctamente.


### Paso 0

#### A

#### Ejecucion aplicativo sin Valgring:
![SInValgrind](https://user-images.githubusercontent.com/49823710/95149066-54bca680-075b-11eb-891f-cb2c923551fd.png)

#### Ejecucion aplicativo con Valgring:

![ConValgrind](https://user-images.githubusercontent.com/49823710/95149117-7b7add00-075b-11eb-9533-a86596fc7a30.png)

#### B

Valgrind es una herramiento utilizada para debuggear. Esta es muy util al momento de trabajar con lenguajes como C o C++ en el cual se debe alocar memoria manualmente para las variables y liberarla tambien. A medida que el programa crece, cada ves se hace mas dificil seguir errores o perdidas en memoria. Aca es donde entra valgrind en la cual nos resume los errrores de memoria que encuentra y da cierta informacion sobre el error , para asi el usuario poder resolver el problema.

#### C

sizeof() es una funcion utilizada para conocer la cantidad de bytes que ocupa la variable o tipo de dato que se le pase al mismo.
![c](https://user-images.githubusercontent.com/49823710/95150043-b4b44c80-075d-11eb-8718-b4cab3e169f9.png)



#### D

![sizeofStruct](https://user-images.githubusercontent.com/49823710/95151005-f9d97e00-075f-11eb-9f7d-89b2ab24e481.png)

#### E

El stdin, stdout y stderr son flujos de datos que se crean al iniciar un commando en Linux. El stdin es usado para todos los inputs interactivos, como por ejemplo las llamadas a la funcion input(). Por otro lado el stdout es usado para la salida del print y declaraciones de expresion.Finalmente el stderr es donde van las indicaciones del interprete y sus mensajes de error.
Redirigir sirve para capturar la salida de uin programa y poder mandrsela a otro o programa o a un archivo.Esto se hace mediante el operador n>. En este caso n representa el numero del descriptor de archivo, si lo omitimos usa por default el 1, osea el stdout. una forma de usarlo seria "command > file".
Por otro lado pipe sirve para enviar la salida estandar de un comando o programa a la entrada estandar de otro. para esto se utiliza el caracter "|". 


### Paso 1

#### A

![problemasEstilo](https://user-images.githubusercontent.com/49823710/95153482-edf0ba80-0765-11eb-8f58-e6a4879b2854.png)

Missing space before... : Este error ocurre porque no deja un espacio entre el while y la condicion encerrada en los parentesis.

Mismatching spaces inside () in if: Este error se genera cuando dejamos un espacio del parentesis inicial y no en el final de if.Ej: ( "holla" == "chau").

Should have zero or one spaces inside ( and ) in if: Este error se genera debido a que dejamos un espacio desde el primer parentesi y a su ves un espacio entre los valores y el operador logico.

An else should appear on the same line as the preceding: Este error se da porque ponemos un salto de linea entre el parentecis que cierra el if de arriba con el, else if que le sigue.

 If an else has a brace on one side, it should have it on both : Este error se da ya que el else no posee un "}" a su izquierda pero al terminar el statement condicional, si posee un "}".
 
 Extra space before last semicolon.: esto se debe a que hacemos return next_State ; y no return next_State;
 
 Lines should be <= 80 characters long: Este error se produce porque el comentario tiene una longitud de mas de 80 caracteres.
 
 Almost always, snprintf is better than strcpy: Este error dice que es mejor usar snprintf, ya que deja en 0 lo copiado al contrario de lo que pasa con strcopy.
 
 #### B
 
 ![errorCOmpilador](https://user-images.githubusercontent.com/49823710/95154751-ef6fb200-0768-11eb-8323-550b65b9c1b5.png)

Los errores que vemos en esta captura son errores del compilador. Estos errores se producen ya que no incluimos el paso1_wordscounter.h en nuestro main. Esto genera que cuando en la funcion main se quieren usar funciones o estructuras definidas en el .h, el compilador no las conozca, entonces es donde tira el error. Para arreglarlo basta con incluir el .h como dijimos anteriormente.

#### C

EL sistema no reporto ningun warning ya que no pudo compilar correctamente el programa debido a que no encontro las funciones llamadas en el main.

### Paso 2

#### A

En el paso 2 se pasaron a corregir ciertos aspectos del codigo. EL mas notorio es que se corrigieron todos los errores de chequeo de normas de codificacion.

![diffPaso2](https://user-images.githubusercontent.com/49823710/95156157-3d39e980-076c-11eb-9673-005e9f3bace0.png)

#### B

![correctaVerificacionPaso2](https://user-images.githubusercontent.com/49823710/95156224-678ba700-076c-11eb-9812-41848a04c801.png)

#### C

![paso2COMpilador](https://user-images.githubusercontent.com/49823710/95156352-c3eec680-076c-11eb-9be3-3686922830d8.png)



