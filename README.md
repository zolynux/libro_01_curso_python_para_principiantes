# Curso Python Para Principiantes

## Entorno de desarrollo

Comenzaremos a saber instalado todo nuestro sistema,
para crear un entorno de desarrollo propicio, trabajar con Python.

1. Sistema operativo GNU/Linux, Windows, MacOs
2. Python 2.7
3. VS-code, PyCharm o NeoVim

## Estructura y elementos del lenguaje

Los lenguajes informáticos, Python, pertenece al grupo de los lenguajes de programación
y un lenguaje interpretado, de alto nivel, multiplataforma, de tipado dinámico
y multiparadigma.

### Glosario

**lenguaje informático:** es un idioma artificial, utilizado por ordenadores, cuyo fin es transmitir
información de algo son:

- **Lenguaje de programación**: Python, PHP, Java, C, etc.
- **Lenguajes de especificación**: UML
- **Lenguajes de consulta**: SQL, NoSQL
- **Lenguajes de marcas**: HTML, XML
- **Lenguajes de transformación**: XSLT
- **Protocolos de comunicaciones**: HTTP, FTP
- **Entre otros**

**Lenguaje de programación:** es un lenguaje informático, diseñado para expresar órdenes e instrucciones precisas, que deben ser llevadas a cabo por una computador.

**Lenguajes de alto nivel:** son aquellos cuyas característica principal, consiste en una estructura sintáctica y semántica legible, acorde a las capacidades cognitivas humanas.

**Lenguajes interpretados:** a diferencia de los compilados, no requieren de un compilador para ser ejecutados sino de un intérprete.

**Tipado dinámico:** un lenguaje de tipado dinámico es aquel cuyas variables, no requieren ser definidas asignando su tipo de datos, sino que éste, se auto-asigna en tiempo de ejecución, según el valor declarado.

**Multiplataforma:** significa que puede ser interpretado en diversos Sistemas Operativos (OS) como GNU/Linux, Windows, MacOS, Solaris, entre otros.

**Multiparadigma:** acepta diferentes paradigmas (técnicas) de programación, tales como la orientación a objetos, aspectos, la programación imperativa y funcional.

**Código fuente:** es un conjunto de instrucciones y órdenes lógicas, compuestos de algoritmos que se encuentran escritos en un determinado lenguaje de programación, las cuales deben ser interpretadas o compiladas, para permitir la ejecución del programa informático.

## Elementos del lenguajes

Como en la mayoría de los lenguajes de programación de alto nivel, en Python se compone de una  serie de elementos que alimentan su estructura. Entre ellos, podremos encontrar los siguientes:

### Variables

Una variable es un espacio para almacenar datos modificables, en la memoria de de un ordenador.

~~~py
nombre_de_la_variable = valor_de_la_variable
~~~

**Variables:** Utilizar nombres descriptivos y en minúsculas. Para nombres compuestos, separar las parabras por guiones bajos.

- **Correcto:** `mi_variable = 12`
- **Incorrecto:** `MiVariable = 12`, `mivariable = 12`, `mi_variable=12`, `mi_variable  =   12`.

**Constantes:** Utilizar nombres descriptivos y en mayúsculas separando palabras por guiones bajos. Para nombres compuestos, separar las parabras por guiones bajos.

- **Ejemplo:** `MI_CONSTANTE = 12`.

Para **imprimir un valor en pantalla**, en Python, se utiliza la palabra clave `print`:

~~~py
mi_variable = 15
print mi_variable
~~~

### Tipos de datos

Los tipos de datos son los tipos de datos que se pueden asignar a una variable. En Python, existen varios tipos de datos, los cuales se pueden ver en la siguiente tabla:

| Tipo de datos | Descripción |
| ------------- | ----------- |
| int           | Entero      |
| float         | Flotante    |
| str           | Cadena      |
| bool          | Booleano    |
| list          | Lista       |
| tuple         | Tupla       |
| dict          | Diccionario |

Para **asignar un valor a una variable**, se utiliza la **asignación** `=`:

**Cadena de texto (string):**

~~~py
mi_cadena = "Hola Mundo"

mi_cadena_multilinea = """
Hola Mundo
esta es una cadena
de varias lineas
"""
~~~

**Número entero (int):**

~~~py
mi_entero = 12

mi_entero_hexa = 0x12

mi_entero_octal = 0o12

mi_entero_decimal = 12

mi_entero_binario = 0b1010

mi_entero_bin = 0b1010
~~~

**Número flotante (float):**

~~~py
mi_flotante = 12.12

mi_flotante_decimal = 12.12

mi_flotante_hexa = 0x12.12

mi_flotante_octal = 0o12.12

mi_flotante_binario = 0b1010.12
~~~

**Booleano (bool):**

~~~py
mi_booleano = True
mi_booleano = False
~~~

Existen además, otros tipos de datos más complejos, que veremos más adelante.

### Operadores Aritméticos

Los operadores aritméticos son operadores que se utilizan para realizar operaciones matemáticas.

|Símbolo|Significado| Ejemplo| Resultado|
|-------|-----------|--------|----------|
|+|Suma|a = 10 + 4 |5|
|-|Resta|a = 10 - 4 |6|
|*|Multiplicación|a = 10 * 4 |40|
|/|División|a = 10 / 4 |2.5|
|//|División entera|a = 10 // 4 |2|
|%|Módulo|a = 10 % 4 |2|

nota: Siempre colocar un espacio entre los operadores y los valores

**Un ejemplo sencillo con variables y operadores aritméticos:**

~~~py
monto_bruto = 175
tasa_interes = 12
monto_interes = monto_bruto * tasa_interes / 100
tasa_bonificacion = 5
importe_bonificacion = monto_bruto * tasa_bonificacion / 100
monto_neto = (monto_bruto - importe_bonificacion) + mononeto_interes
~~~

## Comentarios

Un archivo, no solo puede contner código, sino también comentarios (notas que como el código, no se ejecutan, para poder comprender a apuntar la nota).

Los comentarios pueden ser de dos tipos: de una sola linea o de varias lineas.

~~~py
# Este es un comentario de una sola linea

"""
Este es un comentario de varias lineas
Este es un comentario de varias lineas
Este es un comentario de varias lineas
"""

mi_variable = 15   # Este es un comentario de una sola linea
~~~

En los comentarios, pueden incluirse palabras clave que nos ayuden a identificar además, el subtipo de comentario:

~~~py
# TODO esto es algo por hacer
# FIXME esto es algo que debe arreglarse
# XXX esto es algo que no sabemos como solucionar
~~~

Comentarios en la misma línea del código deben separarse con dos espacios. Luego del signo de hash `#`.

**Correcto:** `a = 15  # Edad de Maria`
**Inorrecto:** `a = 15 # Edad de Maria`

## Tipos de datos complejos

Python, posse ademas de los tipos ya vistos, 3 tipos de datos complejos:

- Tuplas
- Listas
- Diccionarios

### Tuplas

Una tupla es una secuencia de elementos, que pueden ser de diferentes tipos.

Para crear una tupla, se utiliza la palabra clave `tuple`:

~~~py
mi_tupla = (1, 2, 3)

mi_tupla = ("Hola", "Mundo")

mi_tupla = ("Hola", "Mundo", "Python")

mi_tupla = ("Hola", "Mundo", "Python", 12)

mi_tupla = ("Hola", "Mundo", "Python", 12, True)
~~~

Para **imprimir una tupla**, se utiliza la palabra clave `print`:

~~~py
print mi_tupla

# (1, 2, 3)
# (1, 2, 3)
# ('Hola', 'Mundo', 'Python')
# ('Hola', 'Mundo', 'Python', 12)
# ('Hola', 'Mundo', 'Python', 12, True)
~~~

También se puede acceder a una porción de la tupla:

~~~py
print mi_tupla[0]  # Imprime el primer elemento de la tupla

print mi_tupla[1:4]  # Imprime una porción de la tupla
print mi_tupla[3:]  # Imprime una porción de la tupla
print mi_tupla[:2]  # Imprime una porción de la tupla
~~~

### Listas

Una lista es una secuencia de elementos, que pueden ser de diferentes tipos.

Para crear una lista, se utiliza la palabra clave `list`:

~~~py
mi_lista = [1, 2, 3]

mi_lista = ["Hola", "Mundo"]

mi_lista = ["Hola", "Mundo", "Python"]

mi_lista = ["Hola", "Mundo", "Python", 12]

mi_lista = ["Hola", "Mundo", "Python", 12, True]
~~~

Para **imprimir una lista**, se utiliza la palabra clave `print`:

~~~py
print mi_lista

# [1, 2, 3]
# [1, 2, 3]
# ['Hola', 'Mundo', 'Python']
# ['Hola', 'Mundo', 'Python', 12]
# ['Hola', 'Mundo', 'Python', 12, True]
~~~

### Diccionarios

Un diccionario es un contenedor de pares clave-valor, donde cada pareja es una tupla de dos elementos.

~~~py
mi_diccionario = {'clave_1': valor_1, 'clave_2': valor_2, 'clave_7': valor_7}

print mi_diccionario['clave_2']  # Salida: valor_2
~~~

Un diccionario permite eliminar cualquier entrada: `del(mi_diccionario['clave_2'])`.

Al igual que las listas, el diccionario permite modificar los valores: `mi_diccionario['clave_1'] = 'nuevo valor'`
