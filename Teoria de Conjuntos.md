# Teoria de conjuntos

La teoria de conjuntos es un area fundamental de las matematicas que trata sobre las propiedades y relaciones entre conjuntos , que son colecciones bien definidas de objetos. Python, como un lenguaje versatil, ofrece varias formas de trabajar con conjuntos.


```python
A = {1, 2, 3, 4, 5}
```


```python
B = {6, 7, 8, 9}
```


```python
C = {9, 10, 11, 12}
```

## Creacion de conjuntos
En Python se pueden crear conjuntos de la siguiente manera 


```python
lista = [1, 2, 3, 4, 5]
```


```python
lista
```




    [1, 2, 3, 4, 5]




```python
conjunto = set(lista)
```


```python
conjunto
```




    {1, 2, 3, 4, 5}



# Operaciones 
Python proporciona operadores y metodos para realizar operadores y metodos para realizar operaciones basicas de conjuntos como Union, Interseccion, Diferencia y Diferencia simetrica

## Union

Es la formación de un nuevo conjunto creado por dos o más conjuntos que pueden o no tener elementos en común. La simbología utilizada para representar la unión entre conjuntos es ∪.

$$
 C = A \cup B = {x:x \in \quad o \quad x \in B}
$$

En este caso podemos ver que la unión de dos conjuntos A y B forman un conjunto compuesto por los elementos que pertenecen a A y los elementos que pertenecen a B.

Lo anterior se lee de la siguiente manera: A unido a B, está formado por todos los elementos x, tal que x pertenece a A o x pertenece a B.
En python la operacion de union puede realizarse utilizando el operador  | o el metodo union()


```python
union = {A | B}
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[37], line 1
    ----> 1 union = {A | B}
    

    TypeError: unhashable type: 'set'



```python
A.union(B)
```




    {1, 2, 3, 4, 5, 6, 7, 8, 9}



## Interseccion

Llamamos intersección entre conjuntos, al conjunto formado por todos los elementos que pertenecen a ambos conjuntos. La simbología utilizada para representar la unión entre conjuntos es.
$$
A \cap B = \{ x \mid x \in A \text{ y } x \in B \}\$$
]

Por ejemplo: dados los conjuAtos R = {1,2,3,4} y el conjunto S = {3,4,5,6}, podríamos decir que la interseces

$$
A \cap B = \{3, 4\}
$$

En Python, puedes realizar la intersección entre conjuntos utilizando el operador & o el método intersection(). Aquí tienes algunos ejemplos de cómo hacerlo:
$$ria:


```python
interseccion = A & B
```


```python
A.intersection(C)
```




    set()



## Diferencia

La diferencia de conjuntos A y B, denotada como A- B o A\B consiste en todos los elementos que están en A pero no están en B. La fórmula para la diferencia de conjuntos puede expresarse como:

$$
A - B = \{ x \mid x \in A \text{ y } x \notin B \}
$


En Python, puedes calcular la diferencia entre dos conjuntos utilizando el operador de resta - o el método difference(). Aquí tienes algunos ejemplos de cómo hacerlopresentar la diferencia de conjuntos.





```python
diferencia = A - B
```


```python
A.difference(B)
```




    {1, 2, 3, 4, 5}



## Diferencia Exclusiva


La diferencia exclusiva entre dos conjuntos, a menudo denotada comoA�B⊕
�
A⊕B, consiste en los elementos que pertenecen a uno de los conjuntos, pero no a ambos. Es decir, incluye los elementos que están en A pero no en B, así como los elementos que están en B pero no en A.

Matemáticamente, la diferencia exclusiva entre dos conjuntos A y B se puede expresar como la unión de las diferencias entre A y B y entre

$$
A \oplus B = (A - B) \cup (B - A)
$$

En Python, puedes calcular la diferencia exclusiva utilizando el operador ^ o el método symmetric_difference()

$ B y A:


```python

```
