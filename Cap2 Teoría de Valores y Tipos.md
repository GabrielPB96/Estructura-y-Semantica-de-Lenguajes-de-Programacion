## Valor
datos

## Tipo
>*Es un conjunto de valores que presentan comportamiento uniforme bajo ciertas operaciones.*

Organizar los datos en conjuntos.
1. Cadenas
2. Números Enteros
3. Números Reales
**Información**
| CI | nombre |estatura |
|----|---------|----------|
| 9345678| 'Ale'|1,85|

- ### Tipos Primitivos
>*Valores que no pueden ser descompuestos.*

Algunos lenguajes permiten definir tipos primitivos (enumerados).

```java
public enum Mes {
	ENE, FEB, MAR, ABR, MAY, JUN, JUL, AGO, SEP, OCT, NOV, DIC;
}
```

- ### Tipos Compuestos
>*Valores que pueden decomponerse.*

#### Conceptos Estructurales para tipos Compuestos
- Producto Cartesiano (X)
	>*Sea **S** un tipo*
	>*Sea **T** un tipo*
	>***S x T** = {(x, y) | x € **S** ^ y € **T**}*

	**Ej:**
		**S** = {a, b}
		**T** = {1, 2, 3}
		**S x T** = {(a, 1), (a, 2), ... , (b, 1), (b, 2)}
	*#* cardinalidad de conjunto
	*#*(**S x T**) = *#* S * *#* T
	
```c++
	struct empleado {
		int codigo;
		string nombre;
		float salario;
	}
```

```pascal
	type empleado = record
						codigo : Integer;
						nombre : String;
						salario : Real;
					end
```

- Unión Disyunta (+)
	>*Sea **S** un tipo*
	>*Sea **T** un tipo*
	>***S x T** = {izq x | x € **S**} U {der y | y € **T**}*

	**Ej:**
		**S** = {a, b}
		**T** = {1, 2, 3}
		**S + T** = {izq a, der q, izq b, der 3}
		*#* (S + T) = *#* S + *#* T

```ML
	datatype EntOReal = EsEnt of int | EsReal of real;
```

- Mapeo

	