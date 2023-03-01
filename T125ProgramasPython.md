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

### 10.  
```


```

### 11.  
```


```

### 12.  
```


```

### 13.  
```


```

### 14.  
```


```

### 15.  
```


```

### 16.  
```


```

### 17.  
```


```

### 18.  
```


```

## Problemas Nivel Avanzado:

### 19.  
```


```

### 20.  
```


```

### 21.  
```


```

### 22.  
```


```

### 23.  
```


```

### 24.  
```


```

### 25.  
```


```
