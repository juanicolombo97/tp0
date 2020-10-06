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
 Mismatching spaces inside () in if:
