<!-- No borrar o modificar -->
[Inicio](./index.md)

## Actividad 4

**Calculadora Básica: Crea una función llamada calculadora**

*que tome tres argumentos: dos números y un operador (+, -, *, /).*
*La función debe realizar la operación indicada en los dos números y devolver el resultado.*

```
def calcu(n1, n2, operador):
    if operador == '+':
        return n1 + n2
    elif operador == '-':
        return n1 - n2
    elif operador == '*':
        return n1 * n2
    elif operador == '/':
            return n1 / n2
    else:
        return "No existe"

resultado = calcu(5, 3, '/')
print(resultado)

```

**Conteo de Vocales: Crea una función llamada contar_vocales.**

*Que tome una cadena como argumento y devuelva el número de vocales (a, e, i, o, u) que contiene la cadena.*
 
 ```
def vocales(cadena):
    contador = 0
    for letra in cadena.lower():
        if letra in 'aeiou':
            contador += 1
    return contador

cant_vocales = vocales("Buenos dias compañeros, como estan")
print(cant_vocales)  

```

**Primo o No Primo: Escribe una función llamada es_primo.**

*Que tome un número entero positivo como argumento y determine si es un número primo (es decir, solo es divisible por 1 y por sí mismo).*
*La función debe devolver True si es primo y False si no lo es.*

```
def primo(numero):
    if numero < 2:
        return False
    if numero == 2:
        return True
    if numero % 2 == 0:
        return False
    for i in range(3, int(numero ** 0.5) + 1, 2):
        if numero % i == 0:
            return False
    return True

```

**Contador de Palabras: Escribe una función llamada contar_palabras.**

 *Que tome una cadena como argumento y devuelva el número de palabras en esa cadena.*
 *Supón que las palabras están separadas por espacios.*

```
def palabras(cadena):
    palabras = cadena.split()
    return len(palabras)

num_palabras = palabras("Que se dice pues")
print(num_palabras)  

```

**Cálculo de Potencia: Escribe una función llamada potencia.**

 *que tome dos números enteros como argumentos, uno como base y otro como exponente, y devuelva el resultado de elevar la base al exponente.*

```
def potencia(b, e):
    return b ** e

resultado_potencia = potencia(2, 3)
print(resultado_potencia)  

```






