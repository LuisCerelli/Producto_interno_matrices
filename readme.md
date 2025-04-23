# Producto Interno entre Matrices

![Producto_Interno](Imagenes/A.dot(B).png)

Este repositorio fue creado con el objetivo de **reforzar y consolidar conocimientos** en álgebra lineal, específicamente sobre el concepto del **producto interno entre matrices**. No busca ser una solución profesional ni una guía oficial, sino un recurso personal y didáctico para mantenerme mejor este tema clave.

---

## ¿Cómo se define el producto interno entre matrices?

El producto interno entre matrices es uno de los conceptos más útiles y fascinantes del álgebra lineal. Permite combinar matrices de forma que sus propiedades puedan aprovecharse para cálculos complejos.

El producto interno está **definido cuando el número de columnas de la primera matriz coincide con el número de filas de la segunda**. Es decir, las dimensiones deben estar alineadas adecuadamente.

Esta operación es esencial en computación, donde se utilizan matrices para representar datos y realizar cálculos avanzados.

---

## ¿Cómo aplicamos el producto interno?

### Ejemplo práctico:

Consideremos dos matrices:

```python
import numpy as np

A = np.array([[1, 2, 3],
              [4, 5, 6],
              [7, 8, 9],
              [10, 11, 12]])  # Matriz de 4x3

B = np.array([[2, 3],
              [5, 7],
              [11, 13]])       # Matriz de 3x2

C = np.dot(A, B)
print(C)
```

En este caso:
- A tiene dimensiones **4x3**
- B tiene dimensiones **3x2**

Como el número de columnas de A coincide con el número de filas de B (3), **el producto es posible** y el resultado es una matriz de **4x2**.

### Paso a paso:
Para obtener cada elemento de la matriz resultante:
- Se toma una fila de A y una columna de B
- Se multiplican sus elementos correspondientes
- Se suman los productos obtenidos

Por ejemplo, el primer elemento del resultado es:
```
1*2 + 2*5 + 3*11 = 2 + 10 + 33 = 45
```

Este proceso se repite para cada combinación de filas de A y columnas de B.

---

## ¿Qué pasa si el producto no está definido?

Intentar hacer `B.dot(A)` producirá un error porque:
- B tiene 2 columnas
- A tiene 4 filas

❌ **No coinciden**, por lo tanto **el producto interno no está definido**.

---

## Consejos prácticos

- Verificá siempre las dimensiones antes de hacer una multiplicación
- Usá herramientas como NumPy para evitar errores y simplificar los cálculos
- Asegurate de que la dimensión del resultado tenga sentido dentro del contexto del problema

---

Este repo fue armado de manera libre y experimental para ayudarme a internalizar los conceptos clave del álgebra lineal en un entorno práctico con Python ❤️

¡Gracias por pasar!

