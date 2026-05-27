## Aritmética boleana

Objetivo: construir una **ALU** (unidad aritmético lógica).

### Operaciones aritméticas

Las computadoras de propósito general mínimamente tienen que hacer estas operaciones:

- suma
- conversión de signos
- resta
- comparación
- multiplicación
- división

Se pueden construir todas las otras operaciones mediante una sola: la suma.

### Números binarios

Representación de números en sistema decimal, por ej: 6083 es igual a
![[Pasted image 20260505173620.png]]
Siguiendo esta lógica podríamos representar cualquier número pero en su base *decimal* o en base dos, por ej: 10011:
![[Pasted image 20260505173735.png]]
**Fixed word size**: dentro del sistema decimal tenemos una representación numérica infinita, sabemos que un entero x tiene un número superior y otro inferior y así. Las computadoras son finitas y el término comúnmente usado que se usa para referirse a la representación básica de una computadora es *Word size*. Esto nos indica que hay una cantidad física que podemos representar de números (8,16,32,64 bits)
Suponiendo que tenemos 8 bits, esto es : 2^8 = 255 que en binario seria: 11111111.

### Suma binaria

Para sumar binarios se comienza desde los dos primeros bits desde la derecha los llamados **menos significativos**. Siguiente es sumar el número de acarreo al siguiente par de bits mas a la izquierda o los **más significativos**. Si la suma de los bits genera un acarreo de uno se obtiene un **desbordamiento**:
![[Pasted image 20260505175603.png]]
Como vemos, la suma de números de 4 bits de la derecha genera un desbordamiento agregando un quinto bit.

## Números binarios con signo
La manera mas extendida de representar hoy números de distinto signo es usando el *two´s complements method* o también conocido como *radix complement*.
Para un sistema con un tamaño de n bits, los números con signo son representados con 2^n - x.
Ejemplo: en un sistema de 4 bits, el número 7 se representa como 2^4 - 7 = 9 que es 1001