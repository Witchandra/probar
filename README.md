	# Lenguaje de programación en Jypiter - Python

## 1. Tipos de objetos
Aquí resumo las secuencias de ADN de orquídeas que he analizado, junto con un comando simple para procesarlas:

| Tipo                 |   Definición       | Comando             |
|----------------------|--------------------|---------------------------|
| *String* | Letras           | str |
| *Integer* | Número enteros        | int |
| *Float*   | Decimales           | float |
|*Lista*       | Conjunto de elementos, Variados,  Ordenado |list |
|*Diccionario*       | Sirve para buscar cosas |dict |

## 2. Herramientas

### Type
 - Determinar el tipo de un objeto. Incluso en funciones avanzadas crear un nuevo tipo.
Ejemplo:
```python
print(type(42))
# Salida: <class 'int'>
print(type("ACGATCGACTGACTAGCTACTT"))
# Salida: <class 'str'>
print(type([1, 2, 3]))
# Salida: <class 'list'>
print(type((1, 2, 3)))
# Salida: <class 'tuple'>
```

### Len
 - Cuenta cuántos elementos hay en ese objeto y devuelve un entero que representa esa cantidad. (cadena de texto, una lista, una tupla o un diccionario)
Ejemplo:
```python
len("Hola")
# Out 4 (la longitud de la cadena "Hola"). 

len([1, 2, 3]) 
# Out 3 (la longitud de la lista).

len((1, 2, 3)) 
# Out 3 (la longitud de la tupla (1, 2, 3)). 

len({"a": 1, "b": 2}) 
# Out 2 (la longitud del diccionario, que son las claves).
```

### Concatenar
 - Unir str
 - NO se puede concantenar un int + str
Ejemplo:
```python
'7'+'6'
# Out '76'
'a'+'b'
# Out 'ab'
```

### Poner en mayusculas y remplazar
Ejemplo:
```python
DNA = DNA.upper().replace(' ','')
# Out "ACGTACGATCGTACG"
```

### Cuando inicia con:
Ejemplo:
```python
DNA = "ATGCAGTTGAC"
if DNAseq.startswith('ATG'):
    print('eureka, se expresa')
elif DNAseq.startswith('ATA'):
    print('se expresa! en la mitocondria')
elif DNAseq.startswith('ATT'):
    print('se expresa! en la mitocondria')
else:
    print('no se expresa')
# Out 'eureka, se expresa'
```

### Contar un elemento de una str
 - Unir str
 - NO se puede concantenar un int + str
Ejemplo:
```python
DNA = "ACCGAGA"
print(DNA.count('T'))
# Out 0
print(DNA.count('T'),DNA.count('A'))
# Out 0 3
```

### Calcular porcentaje de un elemento de una str
Ejemplo:
```python
DNA = "ACGATCGACTGACTAGCTACTT"
longitud = len(DNA)
NumA = DNA.count('A')
print('Porcentaje de A:',NumA/longitud*100)
# Out: 27.27272727
```

### Redonder
1. Primera opcion
Ejemplo:
```python
round(24.568484354354646846,2)
# Out 24.57
```
2. Segunda opción
```python
print('A: %.3f' %(24.568484354354646846))
# Out 24.568
```

### Imprimir reemplazando
```python
print('A: %s' %'32')
# Out A: 32
print('A: %d' %4456)
# Out A: 4456
print('A: %.3f' %(100*NumberT/SeqLength))
# Out A: 17.391
```

### Condicionales
```python
x=10
if x!=10:
    x=x+2
else:
    x+=5
print(x)
# Out 15

x=13
if x == 10:
	x=x+2
elif x != 11:
	x=x+3
elif x >= 12:
	x=x+4
else:
	x=x+5
print(x)
# Out 16
```

### Posiciones
- Recuerda que las posiciones inician desde 0. Si quieres un seleccionar una posicion entonces pones en corchetes el primero numero es la posicion, el final es "stop".
```python
DNA = "ACGATCGACTGACTAGCTACTT"
print(DNA [0:3])
# Out "ACG"
```

### Diccionario
- Formado por llaves y valores. Sirve para que busques cosas.
- Ejemplo: Taxa={'Peces':3,'Monotreas':6,'Reptiles':15,'Lepidoptera':50}

	- # Crear un diccionario a partir de listas
	```python
	Keys = ['Peces','Monotreas','Reptiles','Lepidoptera']
	Values = [3,6,15,50]
	Taxa = dict(zip(Keys,Values))
	print(Taxa)
	# Out {'Peces': 3, 'Monotreas': 6, 'Reptiles': 15, 'Lepidoptera': 50}
	```
 	
