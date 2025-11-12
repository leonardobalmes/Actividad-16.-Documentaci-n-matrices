# Tecnológico de Software  
## Materia: Fundamentos de Álgebra  
## Alumno: Leonardo Balmes Solis  
## Actividad #16 - Operaciones con matrices  

---

### Ejercicio 1: Clasificar matrices  

Identifica el tipo de cada matriz:

![matrices](https://latex.codecogs.com/svg.image?A%20=%20\begin{pmatrix}1&0\\0&1\end{pmatrix},\quad%20B%20=%20\begin{pmatrix}3&0&0\\0&-2&0\\0&0&5\end{pmatrix},\quad%20C%20=%20\begin{pmatrix}2&1&4\\1&3&5\\4&5&6\end{pmatrix},\quad%20D%20=%20\begin{pmatrix}1&2&3\\0&4&5\\0&0&6\end{pmatrix})

---

#### Matriz A  
Matriz *identidad* \(I_2\), también es *diagonal, escalar* (\(\lambda = 1\)), *simétrica* y *triangular superior e inferior*.  
Propiedad: \(A = A^T\).

---

#### Matriz B  
Matriz *diagonal* de orden \(3 \times 3\).  
También es *triangular superior e inferior*, y *simétrica*.  
No es escalar porque sus elementos diagonales son diferentes \((3, -2, 5)\).

---

#### Matriz C  
Una **matriz simétrica** de tamaño \(3 \times 3\) es aquella en la que los elementos ubicados de forma opuesta respecto a la diagonal principal son iguales, es decir, \(C_{ij} = C_{ji}\).  
Por ejemplo: \(C_{12} = 1 = C_{21}\), \(C_{13} = 4 = C_{31}\), \(C_{23} = 5 = C_{32}\).  
Esta matriz no es ni diagonal ni triangular.

---

#### Matriz D  
Matriz *triangular superior* de orden \(3 \times 3\).  
No es simétrica ni diagonal.  
Su determinante es:

![detD](https://latex.codecogs.com/svg.image?\det(D)=1\cdot4\cdot6=24\neq0)

Por lo tanto, es *invertible*.

---

### Conclusión del Ejercicio 1  

En este ejercicio se analizaron los diferentes tipos de matrices considerando la disposición de sus elementos y la ubicación de los ceros.  
Se comprendieron las características que diferencian a las matrices identidad, diagonal, simétrica y triangular, las cuales resultan esenciales para el manejo y las operaciones algebraicas con matrices.

---

### Ejercicio 2: Operaciones básicas  

Dadas las matrices:

![matrices2](https://latex.codecogs.com/svg.image?A%20=%20\begin{pmatrix}2&-1\\3&4\end{pmatrix},\quad%20B%20=%20\begin{pmatrix}5&2\\-1&3\end{pmatrix})

Calcula:  
a) \(A + B\)  
b) \(2A - B\)  
c) \(AB\)  
d) \(BA\)  
e) \(A^T\)

---

#### a) Suma de matrices \(A + B\)

![suma](https://latex.codecogs.com/svg.image?A+B=\begin{pmatrix}2+5&-1+2\\3+(-1)&4+3\end{pmatrix}=\begin{pmatrix}7&1\\2&7\end{pmatrix})

---

#### b) Operación \(2A - B\)

![resta](https://latex.codecogs.com/svg.image?2A-B=2\begin{pmatrix}2&-1\\3&4\end{pmatrix}-\begin{pmatrix}5&2\\-1&3\end{pmatrix}=\begin{pmatrix}-1&-4\\7&5\end{pmatrix})

---

#### c) Producto \(AB\)

![AB](https://latex.codecogs.com/svg.image?AB=\begin{pmatrix}2&-1\\3&4\end{pmatrix}\begin{pmatrix}5&2\\-1&3\end{pmatrix}=\begin{pmatrix}11&1\\11&18\end{pmatrix})

---

#### d) Producto \(BA\)

![BA](https://latex.codecogs.com/svg.image?BA=\begin{pmatrix}5&2\\-1&3\end{pmatrix}\begin{pmatrix}2&-1\\3&4\end{pmatrix}=\begin{pmatrix}16&3\\7&13\end{pmatrix})

---

#### e) Transpuesta de \(A\)

![AT](https://latex.codecogs.com/svg.image?A^T=\begin{pmatrix}2&3\\-1&4\end{pmatrix})

---

### Conclusión del Ejercicio 2  

Durante el ejercicio se aplicaron las operaciones básicas del álgebra matricial: suma, resta, multiplicación y transposición.  
Esto permitió comprobar que el orden en la multiplicación de matrices altera el resultado \((AB \neq BA)\) y que la transpuesta transforma las filas en columnas, reforzando la comprensión de estos conceptos fundamentales.

---

### Ejercicio 3: Multiplicación en cadena  

Dadas las matrices:

![matrices3](https://latex.codecogs.com/svg.image?A=\begin{pmatrix}1&2\\3&4\end{pmatrix},\quad%20B=\begin{pmatrix}2&0\\1&3\end{pmatrix},\quad%20C=\begin{pmatrix}1&1\\0&2\end{pmatrix})

Verifica que \((AB)C = A(BC)\)

---

#### Paso 1: Calcular \(AB\)

![AB1](https://latex.codecogs.com/svg.image?AB=\begin{pmatrix}1&2\\3&4\end{pmatrix}\begin{pmatrix}2&0\\1&3\end{pmatrix}=\begin{pmatrix}4&6\\10&12\end{pmatrix})

---

#### Paso 2: Calcular \((AB)C\)

![ABC](https://latex.codecogs.com/svg.image?(AB)C=\begin{pmatrix}4&6\\10&12\end{pmatrix}\begin{pmatrix}1&1\\0&2\end{pmatrix}=\begin{pmatrix}4&16\\10&34\end{pmatrix})

---

#### Paso 3: Calcular \(BC\)

![BC](https://latex.codecogs.com/svg.image?BC=\begin{pmatrix}2&0\\1&3\end{pmatrix}\begin{pmatrix}1&1\\0&2\end{pmatrix}=\begin{pmatrix}2&2\\1&7\end{pmatrix})

---

#### Paso 4: Calcular \(A(BC)\)

![ABC2](https://latex.codecogs.com/svg.image?A(BC)=\begin{pmatrix}1&2\\3&4\end{pmatrix}\begin{pmatrix}2&2\\1&7\end{pmatrix}=\begin{pmatrix}4&16\\10&34\end{pmatrix})

---

#### Verificación

![verificacion](https://latex.codecogs.com/svg.image?(AB)C=\begin{pmatrix}4&16\\10&34\end{pmatrix},\quad%20A(BC)=\begin{pmatrix}4&16\\10&34\end{pmatrix})

Por lo tanto:

![igualdad](https://latex.codecogs.com/svg.image?(AB)C=A(BC))

---

### Conclusión del Ejercicio 3  

Se comprobó la *propiedad asociativa* de la multiplicación de matrices, la cual indica que el modo de agrupar los factores no altera el resultado: \((AB)C = A(BC)\).  
Esta propiedad demuestra que las operaciones encadenadas son coherentes en el álgebra matricial y facilitan la simplificación de cálculos en transformaciones lineales y sistemas de ecuaciones.
