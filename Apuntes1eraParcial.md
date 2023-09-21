## Apuntes 1era Parcial
### Agosto-Septiembre

~~~ python
#Operadores
print(5+4)
print(5-4)
print(5*4)
print(5/4) #Division
print(5//4) #Division entera
print(5&4) # Residuo
print(5**4) #x a la y

#Logicos
print(True and False)
print(True or False)
print(not False)

#Condicionales
n1: int = 30
n2: int = 20
if n1 > n2: 
    print(f"(n1)>(n2)")



def suma(a, b):
   pass
print(suma(3,4))

def operaciones(a, b):
    return[a+b, a-b, a*b, a/b]
respuestas = operaciones(5, 4)
print(respuestas)

##Tupla

numeros_pares = range(2,11,2)
for i in numeros_pares:
    print(par, end "")

# Set Conjuntos
mi_set = [1,2,3,3,3,3,3]

#Diccionario
mi_dict = ("llave",  "valor")
~~~
