#PROGRAMACI�N B�SICA 
## TUTORIAL DE PYTHON

##TEMA 1.CONCEPTOS B�SICOS 
####�Qu� es Python?
>Es un lenguaje de programaci�n, creado por Guido van Rossum a los principios de los a�os 90, cuyo nombre esta inspirado en el grupo de c�micos ingleses "Monty Python". Es un lenguaje similar a "C", pero con una sintaxis muy limpia y que favorece un c�digo legible.

EJEMPLO :                                                     
    
    (Lenguaje "C"):                                                                                                                                                
    # include <stdio.h>                                             
    void.mainvoid{printf"Hola"}
    printf(" a tod@s")
    
    (Lenguaje Python):
    print('Hola a tod@s')
 
----
#### Lenguaje interpretado o de script
>Un lenguaje interpretado o de script es aquel que se ejecuta utilizando un programa intermedio llamado **int�rprete**. En lugar de compilar el c�digo a lenguaje m�quina que pueda comprender y ejecutar directamente una computadora (lenguajes compilados). 
>La ventaja de lo lenguajes compilados es que su ejecuci�n es mas r�pida sin embargo los los lenguajes interpretados son mas flexibles y portados.

>**Interprete: Python, Java, Matla, Basic Ruby**

>**Compilado: HTML, Pascal**


----
##TEMA 2.INTRODUCCI�N A LOS EJERCICIOS DE PROGRAMACI�N 
Los ejercicios estan dise�ados para volverse familiar la sintaxis de Python desarrollando los siguientes temas:

    1.Generar una salida con la sentencia print.
    2.Leer la entrada del usuario con el teclado usando "raw-input".
    3.Realizar c�lculos sencillos como suma +, resta -, multiplicaci�n *, divisi�n % y potencia **.
    4.Realizar c�lculos m�s complejos con el m�dulo "math".

Para entrar a la terminal se debe escribir el comando **Python**. 

Para salir de **Python** debemos escribir **exit()**.

>Existen dos formas de ejecutar c�digo Python, la cual puede ser mediante una sesi�n interactiva (l�nea a l�nea) con el int�rprete, o bien de la forma habitual, escribiendo el c�digo en un archivo de c�digo fuente y ejecut�ndolo. En la primera parte de este tutorial lo haremos con el interprete.

El primer programa que vamos a escribir en Python es el cl�sico **"Hola Mundo"**, y en este lenguaje es tan simple como:
   
                  print ('Hola Mundo')
    Donde print: Es el comando 
    Donde 'Hola Mundo': Son el argumento o cadena de texto 

###Cadena de texto 
Ejemplo:
    
         mi_cadena='Tengo hambre y faltan 60 minutos para salir'
         print(mi_cadena)
         >>Un comentario en python inicia con el car�cter reservado "#"
         Variable = mi_cadena
         Valor = 'Tengo hambre y faltan 60 minutos para salir'

###Tipos de datos b�sicos 
En python los tipos de datos b�sicos se dividen en:

>�	 N�meros, como pueden ser 3 (entero), 15.57 (de coma flotante) o 7 + 5j (complejos)

>�	 Cadenas de texto, como �Hola Mundo�

>�	 Valores booleanos: True (cierto) y False (falso).

Para poder conocer el tipo de dato de una variable usaremos la instruccion **type()**

Como se puede notar a diferencia de muchos otros lenguaje. en python no se puede declarar el tipo de variable al crearla.

En python se pueden representar numeros enteros, reales y complejos, donde los numero enteros se representan con la variable **(int)** la cual puede almacenar numero en la plataforma de 64 bits. 

Los numeros flotantes son los que tienen decimales. En python se expresa mediante el tipo **(float)**.

Los numeros complejos son aquellos que tienen una parte imaginaria. Para definir una variable compleja se utiliza en termino **Complex**.

Ejemplo:

    # esto es una cadena
    c = �Hola Mundo�
    # y esto es un entero
    e = 23
    # podemos comprobarlo con la funci�n type
    type(c)
    type(e)
    
###Operadores 
>Veamos ahora qu� podemos hacer con nuestros n�meros usando los operadores por defecto. Para operaciones m�s complejas podemos recurrir al **m�dulo math.**

####Operadores aritm�ticos
    Operador   Descripci�n           Ejemplo
       +          Suma        r = 3 + 2 # r es 5
       -          Resta       r = 4 - 7 # r es -3
       -        Negaci�n      r = -7 # r es -7
       *     Multiplicaci�n   r = 2 * 6 # r es 12
       **       Exponente     r = 2 ** 6 # r es 64
       /        Divisi�n      r = 3.5 / 2 # r es 1.75
      //     Divisi�n entera  r = 3.5 // 2 # r es 1.0
       %         M�dulo       r = 7 % 2 # r es 1

###Tipos de variables 

Es un nombre que se refiere a un objeto que reside en la memoria. El objeto puede ser de alguno de los tipos vistos (n�mero o cadena de texto), o alguno de los otros tipos existentes en Python.

    String----> 'Blanca'=Cadena de texto 
    Integer----> 18 = N�mero 

###Concatenar 
>Unir varias variables del tipo **String** en una sola.

###Salto de linea 
>Para poder hacer un salto de linea tendro de un comando debemos agregar **'\n'**

Ejemplo:

    print(nombre + '\n' + calle)

###Variable "input()"
>Permite obtener texto escrito por teclado. Al llegar a la funci�n, el programa se detiene esperando que se escriba algo y se pulse la tecla Intro, como muestra el siguiente ejemplo:

    print('Inserta tu nombre')
    nombre=input()
    print('Hola' + nombre)

###Variable flotante 
>Es una variable que puede guardar datos num�ricos con punto decimal, para forzar a una variable a que sea flotante usaremos el comando **float()**.

    float=n�mero decimal
    int=n�mero entero

##TEMA 3.CONTROL DE FLUJO 
###Sentencias condicionales 
>Si un programa no fuera m�s que una lista de �rdenes a ejecutar de forma secuencial, una por una, no tendr�a mucha utilidad. Los condicionales nos permiten comprobar condiciones y hacer que nuestro
programa se comporte de una forma u otra, que ejecute un fragmento de c�digo u otro, dependiendo de esta condici�n.

>Aqu� es donde cobran su importancia el tipo booleano y los operadores l�gicos.

####Condicional if...else
La forma m�s simple de un estamento condicional es un if (del ingl�s SI) seguido de la condici�n a evaluar, dos puntos (:) y en la siguiente l�nea e indentado, el c�digo a ejecutar en caso de que se cumpla dicha condici�n.
 
    LINEA 1  if comparaci�n o condici�n:
    LINEA 2  identaci�n(4espacios) #C�digo a ejecutar 
                                   en caso de que la 
                                   condici�n sea verdadera 
    LINEA 3  else: 
    LINEA 4  identaci�n(4espacios) #C�digo a ejecutar 
                                   en caso de que la  
                                   condici�n sea falsa 

                              Comparaci�n
                             a=b ---> a==b
                     a no es igual a  b ---> a!=b
                             a>b ---> a>b
                             a<b ---> a<b
                   a es mayor o igual a b ---> a>=b
                   a es menor o igual a b ---> a<=b

Ejemplo:

    entero=int(input('Introduzca un numero entero: '))
    par=entero%2
    if par == 0:
        print('El numero es par')
    else:
        print('El numero no es par')

![imagen1](/imagenes/zadigOptions.png)

####Sentencias if 
Nos encontraremos con  sentencias que tendr�n que ver con el �mbito matem�tico ya sea graficar vectores o simplemente crear uno  de ellos , por lo que se usaran los siguientes c�digos:

    import "numpy" as "np"
    import "matplotlib.pyplot" as "plt"

    #Creando un vector n�merico 
       x = np.orange(100)
       y = np.sin(x)
    #Graficando
       plt.plot (x,y)
       plt.show ()

 
###Bucles 

>Mientras que los condicionales nos permiten ejecutar distintos fragmentos de c�digo dependiendo de ciertas condiciones, los bucles nos permiten ejecutar un mismo fragmento de c�digo un cierto n�mero de veces, mientras se cumpla una determinada condici�n.

####While