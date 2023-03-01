# T1. 25 PROGRAMAS USANDO PYTHON

## Problemas Nivel Basico:

### 1. Imprimir los enteros del 1 al 23.
```
calc = 1

while int(calc) <= 23:
    list.append(calc)
    calc = int(calc) + 1
print(list)
```

### 2. Convertir Pulgadas a Yardas y de Yardas a pulgadas.
```
in1 = int(input("Alimentar cantidad de Pulgadas (In): "))
yd1 = in1 * (1/36)
print("Pulgadas: ", in1 ,"(In)", " Equivale en Yardas: ", yd1,"(yd)")

yd2 = int(input("Alimentar cantidad de Yardas (yd) : "))
in2 = yd2 * (36 / 1)
print("Yardas: ", yd2 ,"(yd)", " Equivale en Pulgadas: ", in2,"(In)")
```

### 3. Introducir y determinar si es "Par" o "Impar".
```
numero = int(input("Introduce un número: "))

if(numero % 2 == 0):
    print("El número es par")
else:
    print("El número es impar")
```

### 4. Encontrar la suma de todos los numeros pares del 2 al 2000
```
numero = 0
suma = 0

while(numero <1000):
    numero = numero + 1
    suma = suma + numero

print(suma)
```

### 5. De dos números cualesquiera, encontrar la suma e indicar si es positiva, negativa o cero. 
```
num1 = int(input("Ingresa tu primer numero: "))
num2= int(input("Ingresa tu segundo numero: "))

suma = num1 + num2

if(suma < 0):
    print("El resultado es negativo")
elif(suma > 0):
    print("El resultado es positivo")
elif(suma == 0):
    print("El resultado da 0")
```

### 6. Determinar si la suma 3¹⁹⁷⁴ + 3¹⁹⁷⁴ + 3¹⁹⁷⁴ es igual a 3¹⁹⁷⁵ .
```
numero1 = pow(3,1974) + pow(3,1974) + pow(3,1974)
numero2 = pow(3,1975)

if(numero1 == numero2):
    print("Los numeros son iguales")
else:
    print("Los numeros son diferentes")
```

### 7. Convertir P libras inglesas a D dólares y C centavos. Usar el tipo de cambio $2.80 = 1 libra.
```
libras = int(input("Ingresa tu cantidad en libras: "))

dolares = 2.8 * libras

print(str(round(dolares, 2)) + " Dolares")
```

### 8. Introducir 12 valores de A y 10 de B. Calcular la suma de los valores A, la de los de B y la suma de los productos AB.
```
i = 0
j = 0
sumaA = 0
sumaB = 0

while i < 12:
    A = int(input())
    sumaA = sumaA + A
    i+=1

while j < 10:
    B = int(input())
    sumaB = sumaB + B
    j+=1


print("La suma de A es: " + sumaA)
print("La suma de B es: " + sumaB)
print("La suma de AB es: " + sumaA + sumaB)
```

### 9. Dados diez enteros, imprimir sólo el mayor. No suponer que los números están enlistados en los datos de un orden especial. Puede suponerse que no hay dos números iguales.
```
numeros = []
i = 0
while i < 10:
    numero = int(input())
    numeros.append(numero)
    i+=1

print(max(numeros))
```

## Problemas Nivel Intermedio:

### 10. Escribir un programa que convierta los pesos de los miembros del equipo de fútbol escolar de libras a kilogramos. (Sugerencia: 1kg = 2.204623 libras).
```
n = int(input("Ingresa el número de jugadores: "))

jugadores = []

i = 0
while i < n:
    lb = int(input("Ingresa el peso del jugador en libras: "))
    kg = lb / 2.204623
    jugadores.append(kg)
    i+=1

for j in jugadores:
    print(j)
```

### 11. Calcular z de acurdo a la fórmula siguiente. Asignar las variables numéricas aprobadas. Sean a = 4, b = 6, x = 8, y = 2, c = 5 cuando "corra" su programa: 

z = (a + b)³ - (x + y)² (a - c)⁴ + 1/2 (c + x)
```
a = 4
b = 6
x = 8
y = 2
c = 5

z = pow((a+b),3) - pow((x+y),2) * pow((a-c),4) + (1/2*(c+x))

print(z)
```

### 12. Dada una medida angular mayor que 0° pero menor que 180°, clasificar el ángulo como obtuso, recto o agudo. 
```
while True:
    angulo = int(input())
    if (angulo <= 0):
        print("Inserta un angulo mayor a 0")
    elif(angulo > 180):
        print("Inserta un angulo menor a 180")
    else:
        if (angulo > 90 and angulo <= 180):
            print("Es un angulo obtuso")
            break
        elif (angulo == 90):
            print("Es un agulo recto")
            break
        else:
            print("Es un angulo agudo")
            break
```

### 13. Encontrar el valor de x⁴ - 8x² - 14x + 7 para x = 2, 4, 6, 8, . . ., 40. 
```
r = []

x = 2

i = True
while i == True:
    y = (pow(x,4) - (8 * pow(x,2)) - (14 * x) + 7)
    r.append(y)
    if x == 40:
        break
    else:
        x+=2

for j in r:
    print(j)
```

### 14. Fermat, probablemente el más grande matemático francées del siglo XVII, propuso que todos los números de la forma 2²n + 1, donde n = 0, 1, 2, ..., son primos. Demostrar que esto es cierto para n = 1, 2, 3, 4 pero no para n = 5 . 
```
n = 0

while True:
    primos = (pow(2,2*n))
    if(primos % 2 != 1):
        print("Para n = " + str(n) + " es primo")
    elif (primos == 1):
        print("Para n = " + str(n) + " es primo")
    else:
        print("Para n = " + str(n) + " no es primo")
    n+=1

    if n == 5:
        break
```

### 15. El año 1973 lo recordarán muchos aficionados a la Matemática, pues se trata de un número primo, Generar todos los números primos en el periodo 1972-2000. 
```
años = []
i = 1972

while i < 2000:
    if(i % 2 != 0):
        años.append(i)
    i+=1

for j in años:
    print(j)
```

### 16. La suma de los primeros cinco enteros es igual a 15: 1 + 2 + 3 + 4 + 5 = 15. ¿Cuáles enteros principiando con 1 + 2 + 3 + 4 + ... tendrían que agregarse para alcanzar una suma de 820?
```
n = 0
i = 1
while True:
    n = n + i
    print(i)
    i+=1
    
    if(n == 820):
        break
```

### 17. Se ha conjeturado que existe una gran cantidad de números primos de la forma n^n + 1. Por ejemplo, 1 + 1 = 2 (un primo). Determinar para cada valor n = 1, 2, ..., 7 si n^n + 1 es o no primo. 
```
n = 1

while True:
    primo = pow(n, n) + 1
    if (primo % 2 != 0):
        print("N = " + str(n) + " es primo")
    else:
        print("N = " + str(n) + " no es primo")
    n = n + 1

    if(n == 8):
        break
```

### 18. Determinar el valor de X de tal manera que X30X8 sea divisible entre 23.
```
i = 0

while True:
    i = int(i) + 1
    numero = str(i) + "30" + str(i) + "8"
    
    if(int(numero)%23 == 0):
        break
print(i)
```

## Problemas Nivel Avanzado:

### 19. Dada la secuencia 1, 2, 4, 5, 7, 8, 10, 11, 13, 14, ... donde falta cada tercer entero, imprimir la suma y sus primeros cien términos.
```
numeros = []
n = 0
while True:
    if(n%3 != 0):
        numeros.append(n)
        print(n)
    n+=1

    if(n == 101):
        break

print(sum(numeros))
```

### 20.  Sacar al azar cinco cartas de una baraja de 52 e imprimir la colección y color de cada carta
```
import random

baraja = ["Diamantes", "Corazones", "Picas", "Treboles"]
numero = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "Jota", "Reyna", "Rey"]

def tomar_Carta():
    tipo = baraja[random.randint(0,3)]
    num = numero[random.randint(0,12)]
    print("Tu carta es: " + str(num) + " de " + str(tipo))

tomar_Carta()
tomar_Carta()
tomar_Carta()
tomar_Carta()
tomar_Carta()
```

### 21. La computadora trata de adivinar un número que tiene usted en mente. Primero, ella da un número y usted le dice si es demasiado alto, demasiado bajo o correcto. En base a la información que se le proporcione, la computadora ensaya de nuevo. El proceso continúa hasta que la computadora acierta el número. Generar un programa que desarrolle este juego de tanteos.
```
import random

print("La computadora intentara adivinar el numero que tiene en mente. Piense en un numero en el rango de 0 a 1000")
print("Usted indicara si el numero que le dio es: Numero alto, Numero bajo o Numero correcto")

rInf = 0
rSup = 1000
i = 0

while True:
    numero = random.randint(rInf, rSup)
    print("Usted piensa en el numero: " + str(numero))
    opc = input()
    i+=1
    if (opc == "Numero alto"):
        rSup = numero - 1
    elif (opc == "Numero bajo"):
        rInf = numero + 1
    elif (opc == "Numero correcto"):
        print("Juego terminado")
        print("La computadora obtuvo su numero en: " + str(i) + " intentos")
        break
    else:
        print("Ingrese una instruccion valida")
```

### 22. Escribir un programa que contabilice su cuenta de cheques. Debe sumar depósitos, restar cheques girados, sustraer los cargos bancarios e imprimir balances mensuales. 
```
balance = 5000

while True:
    print("""
    1. Deposito
    2. Emitir cheque
    3. Cargos Bancarios
    4. Balance Mensual
    5. Salir
    """)
    op = int(input("Selecciona un opción: "))
    
    if(op == 1):
        deposito = int(input("Ingresa el valor de tu deposito: "))
        balance = balance + deposito
    if(op == 2):
        cheque = int(input("Ingresa el valor del cheque: "))
        balance = balance - cheque
    if(op == 3):
        cargo = int(input("Ingresa el valor del cargo: "))
        balance = balance - cargo
    if(op == 4):
        print("Tu balance actual es: " + str(balance))
    if(op == 5):
        break
```

### 23. Los números 12 y 13 tienen la siguiente característica: 12 x 12 = 144, 21 x 21 = 441; y 13 x 13 = 169, 31 x 31 = 961. Encontrar un número de tres dígitos (si existe) para el cual sea también válido este tipo de relación.
```
def invertir_cadena(cadena):
    return cadena[::-1]

n = 100

while True:
    resultado1 = n * n
    ninvertido = invertir_cadena(str(n))
    resultado2 = int(ninvertido) * int(ninvertido)

    if(str(resultado2) == str(invertir_cadena(str(resultado1)))):
        print("El numero que cumple la condicion es: " + str(n))
        break

    n+=1
```

### 24. Hacer un programa que facilite al estudiante la solución de problemas de porcentajes
```
valor = int(input("Ingresa el valor: "))
porc = int(input("Ingresa el porcentaje que deseas del valor: "))

resultado = (porc * valor) / 100

print(str(resultado) + " es el " + str(porc) + "% de " + str(valor))

```

### 25. Escribir un programa que simule el lanzamiento de dos dados.
```
import random

print("Dado 1: "+ str(random.randint(1,6)))

print("Dado 2: "+ str(random.randint(1,6)))
```
