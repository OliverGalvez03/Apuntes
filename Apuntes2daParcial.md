~~~ python
x = 10
id(x)
# Maximo de la lista
# max(1,2,3,4,5)

def a():
    x = "Hola"
    print(f"{x}:{id(x)}")

def b():
    x = "Hola"
    print(f"{x}:{id(x)}")

x = "Hola"
a()
b()
print(f"{x}:{id(x)}")

def c():
    #
    global x
    x = "Bye"
    print(id(x))

c()
print(id(x))
x = 10
print(id(x))

def d():
    print(x)
    d()

def e():
    global y
    print(id(y))

def mi_funcion():
    msg = "Dentro de mi_funcion"
    print(msg)

print("Antes de llamar a mi_funcion")
mi_funcion()
print("Despues de llamar a mi_funcion")
~~~

~~~ python
def suma(a, b):
    """
    This function adds two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The sum of a and b.
    """
    return a + b

def resta(a, b):
    """
    This function subtracts two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The difference between a and b.
    """
    return a - b

def multiplicacion(a, b):
    """
    This function multiplies two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The product of a and b.
    """
    return a * b

def division(a, b):
    """
    This function divides two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    float: The quotient of a and b.
    """
    return a / b
~~~

~~~ python
def suma(a, b):
    """
    This function adds two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The sum of a and b.
    """
    # Check if both a and b are integers
    if not isinstance(a, int) or not isinstance(b, int):
        print("Both a and b should be integers.")
        return None
    
    # Add a and b
    result = a + b
    
    # Print the result
    print(f"The sum of {a} and {b} is {result}.")
    
    return result
~~~

~~~ python

#import unittest


def suma(a, b):
    """
    This function adds two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The sum of a and b.
    """
    return a + b

def resta(a, b):
    """
    This function subtracts two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The difference between a and b.
    """
    return a - b

assert suma(2, 3) == 5.0, "debería ser 5"
assert suma(-2, 3) == 1, "debería ser 1"
assert suma(0, 0) == 0, "debería ser 0"
assert suma(-3,-3) == -6, "debería ser -6"
    
assert resta(2, 3) == -1, "debería ser -1"
assert resta(-2, 3) == -5, "debería ser -5"
assert resta(0, 0) == 0, "debería ser 0"
~~~

~~~ python
def suma(a, b):
    return a + b


def resta(a, b):
    return a - b


def multiplicacion(a, b):
    return a * b


def division(a, b):
    if b == a:
        raise ZeroDivisionError("Division by zero")
    return float(a/b)
''

def cuadrado(a):
    return a ** a


#import Calculadora.calculos as calc #alias
 
#print(calc.suma.__doc__)
#print(calc.suma(2,3))
 
 
#from Calculadora.calculos  import calculos
 
#print(calculos.suma(2, 3))
#print(calculos.resta(2, 3))
#print(calculos.multiplicacion(2, 3))
#print(calculos.division(2, 3))
#print(calculos.cuadrado(2, 3))


#from Calculadora.calculos import * 

#print(suma(2, 3))
#print(resta(2, 3))

#from Calculadora.calculos import suma,resta

#print(suma(2, 3))
#print(resta(2, 3))

#from Calculadora.calculos import suma as sumar #alias aka
#from Calculadora.calculos import suma as restar 

#print(sumar(2, 3))


from Calculadora.calculos import suma as sumar, resta as restar

print(sumar(2, 3))
print(restar(2, 3))
~~~
