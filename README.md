# REPO#5_UNAL
Resolveremos los siguientes problemas usando un notebook de python, cada codigo tiene su respectiva expolicación.

 - **1. Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.**
 
 ![image](https://user-images.githubusercontent.com/124611099/226738117-08c8007f-548b-40c1-b28a-0e3c5903ffef.png)


    n = int(input("lngrese un numero: ")) # aqui al ingresar un numero el programa lo esta leyendo como n
    a = chr(n) # usamos la funcion chr para que el programa recibe a n como un número y devuelve su representación como caráctera
    v = 'a' or 'e' or 'i' or 'o' or 'u' # asignamos a v para que sean todas las vocales en minusculas
    if str(a) == str(v) : # si v (es decir las vocales en minusculas) y a(el numero que nosotros escribimos definido en un caracter)
       print (str(n) + " QUE ES DEFINIDO COMO EL CARACTER " + chr(n) + ": es una vocal minuscula")# si la funcion es verdadera entonces imprimimos la parte verdadera
    else:
       print (str(n) + " QUE ES DEFINIDO COMO EL CARACTER " + chr(n) + ": NO es una vocal minuscula")# si la funcion no es verdadera entonces imprimimos la parte falsa


 - **2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.**
 
 ![image](https://user-images.githubusercontent.com/124611099/226746419-9f3a70f9-0c3c-413b-ae91-d06a2fa12e6c.png)

    letra = (input("ingrese una letra: ")) #aqui al ingresar una letra el programa lo esta leyendo como letra
    a = ord(letra) #usamos la funcion ord para que el programa reciba una letra y lo devuelve es su representación como letra.
    if a % 2 == 0: #si a(es decir la letra definida como numero) al dividirlo entre 2 y el residuo es 0 (este es el proceso para saber si un numero es par o impar)
       print (str(letra) + " QUE ES DEFINIDO COMO EL NUMERO " + str(a) + ": Pertenece a un numero par")# si la funcion es verdadera entonces imprimimos la parte verdadera
    else:
       print (str(letra) + " QUE ES DEFINIDO COMO EL NUMERO " + str(a) + ": Pertenece a un numero impar")# si la funcion no es verdadera entonces imprimimos la parte falsa
     
       
 - **3. Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.**
 
 ![image](https://user-images.githubusercontent.com/124611099/226750805-2e009a2c-5cb2-4c27-997b-ed3fbbb94d2a.png)

    n = (input("ingrese un caracter: ")) #aqui al ingresar una letra el programa lo esta leyendo como n
    a = ord(n)  #usamos la funcion ord para que el programa reciba un caracter y lo devuelve es su representación como un numero.
    digitos = "0" or "1" or "2" or "3" or "4" or "5" or "6" or "7" or "8" or "9" # le asignamos a la variable digitos todos los digitos
    if a == digitos: #si a(es decir la letra definida como numero) es igual a digitos
       print ("el caracter " + str(n) + " es un digito") # si la funcion es verdadera entonces imprimimos la parte verdadera
    else:
       print ("el caracter " + str(n) + " no es un digito") # si la funcion no es verdadera entonces imprimimos la parte falsa
       
       
 - **4. Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:**

 - Positivo: "El número x es positivo"
 - Negativo: "El número x es negativo"
 - Cero (0): "El número x es el neutro para la suma"
 
 ![image](https://user-images.githubusercontent.com/124611099/226753920-d6f76e00-2f36-4f82-a401-c67f842d0512.png)

    x = float(input("ingrese un numero real:")) #aqui al ingresar un numero el programa lo esta leyendo como x
    if x < 0: #si x es menor que 0 pues
       print ("el numero: " + str(x) + "es negativo")# si la funcion es verdadera entonces imprimimos la parte verdadera
    elif x >= 0: #si x es mayor que 0 pues
       print ("el numero: " + str(x) + "es positivo")# si la funcion es una opcion entonces imprimimos la parte verdadera
    else: #si x es igual que 0 pues
       print ("el numero: " + str(x) + "es el neutro para la suma")# si la funcion es falsa entonces imprimimos la parte falsa
       

- **5. Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.**

![image](https://user-images.githubusercontent.com/124611099/226759688-d5eff2c3-5fb7-48f9-af91-e12dc6796033.png)

    x = float(input("Ingrese las cordenadas X:")) #aqui al ingresar un numero el programa lo esta leyendo como x
    y = float(input("Ingrese las cordenadas y:")) #aqui al ingresar un numero el programa lo esta leyendo como y
    a = float(input("Ingrese las cordenadas a del centro:")) #aqui al ingresar un numero el programa lo esta leyendo como a
    b = float(input("Ingrese las cordenadas b del centro:")) #aqui al ingresar un numero el programa lo esta leyendo como b
    r = float(input("Ingrese el radio:")) #aqui al ingresar un numero el programa lo esta leyendo como r
    if ((x - a)**2) + ((y - b)**2)<=r**2: # lo que se debe realizar es la ecuacion ordinaria de un circulo asi se pobra saber si las cordenadas que nos dan hacen parte del circulo
       print ("las cordenadas (" + str(x) + ", " + str(y) + ") estan dentro del circulo con centro (" + str(a) + ", " + str(b) +  ") el cual tiene de radio " + str(r)) # si la funcion es una opcion entonces imprimimos la parte verdadera
    else:
       print ("las cordenadas (" + str(x) + ", " + str(y) + ") no estan dentro del circulo con centro (" + str(a) + ", " + str(b) +  ") el cual tiene de radio " + str(r)) # si la funcion es falsa entonces imprimimos la parte falsa

 
- **6. Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.**
 
 ![image](https://user-images.githubusercontent.com/124611099/226759864-ab76cdb4-3d71-44c5-b6dd-931fc81204ed.png)

    a = float(input("ingrese la longitud a:")) #aqui al ingresar un numero el programa lo esta leyendo como a
    b = float(input("ingrese la longitud b:")) #aqui al ingresar un numero el programa lo esta leyendo como b
    c = float(input("ingrese la longitud c:")) #aqui al ingresar un numero el programa lo esta leyendo como c
    if a > 0 and b > 0 and c > 0 and a + b > c and b + c > a and a + c > b: #para saber si con las lonquitudes se puede hacer un triangulo primero toca que todas las longuitudes sean mayores que 0 y tambien tienen que cumplir las desigualdades triangulares
       print ("con las cordenadas (" + str(a) + ", " + str(b) + ", " + str(c) + ") se puede construir un triangulo.") # si la funcion es una opcion entonces imprimimos la parte verdadera
    else:
       print ("con las cordenadas (" + str(a) + ", " + str(b) + ", " + str(c) + ") no se puede construir un triangulo.")  # si la funcion es falsa entonces imprimimos la parte falsa.
       
       
       
 
