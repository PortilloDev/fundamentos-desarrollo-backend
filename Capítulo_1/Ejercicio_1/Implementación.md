
## Implementación en pseudocódigo
INICIO contador = 0 suma = 0 LEER numero MIENTRAS numero != 0 HACER suma = suma + numero contador = contador + 1 LEER numero FIN MIENTRAS SI contador > 0 ENTONCES promedio = suma / contador IMPRIMIR "El promedio es: ", promedio SINO IMPRIMIR "No se ingresaron números para calcular el promedio." FIN SI FIN

```
INICIO
    contador=0
    suma=0

    LEER numero

    MIENTRAS numero != 0 Hacer
        suma = suma + numero
        contador = contador + 1
        LEER numero
    FIN MIENTRAS

    SI contador > 0 ENTONCES
        promedio = suma / contador
        IMPRIMIR "El promedio es: ", promedio
    SINO
        IMPRIMIR "No se ingresaron números para calcular el promedio."
    FIN SI
FIN
```



## Implementación en Python

```python
def calcular_promedio():
    contador = 0
    suma = 0.0
    numero = float(input("Ingresa un número (0 para finalizar): "))
    while numero != 0:
        suma += numero
        contador += 1
        numero = float(input("Ingresa otro número (0 para finalizar): "))
    if contador > 0:
        promedio = suma / contador
        print(f"El promedio es: {promedio}")
    else:
        print("No se ingresaron números para calcular el promedio.")

if __name__ == "__main__":
    calcular_promedio()



```
## Entrada de datos

### Caso 1:
````
Ingresa un número (0 para finalizar): 10
Ingresa otro número (0 para finalizar): 20
Ingresa otro número (0 para finalizar): 30
Ingresa otro número (0 para finalizar): 0
````

### Caso 2:
- Entrada:
````
Ingresa un número (0 para finalizar): 5
Ingresa otro número (0 para finalizar): -5
Ingresa otro número (0 para finalizar): 15
Ingresa otro número (0 para finalizar): 0
````

### Caso 3:
````
Ingresa un número (0 para finalizar): 0
````
