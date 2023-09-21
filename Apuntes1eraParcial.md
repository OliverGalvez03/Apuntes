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
~~~

~~~ python
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

### Streamlit
~~~ python
streamlit run main.py

import streamlit as st
st.slidebar.title("Calculadora")
opcion = st.sidebar.selectbox("Opciones",[
       "Suma,"Resta","Multiplicacion","Division"])

def pedir_variables()
    name = st.text.input
    n1 = st.number.input
    n2 = st.number.input

match option
  case "Sumar"
  if st.button("Sumar")
     st.success
     st.write(f"{n1}+{n2} = (n1 + n2)")
~~~

~~~ python
#dataclass #decoradora
   Class user:
      id: str
      name: str
      age: int

def show_data(self):
    return f"ID:(id)\n Nombre: {name}\nEdad:(age)"

if _name_ == "_main_":
   usuario = user("1","Hugo",25)
   usuario = [usuario1,usuario2,usuario3,usuario4]
   for usuario in usuarios,
       print(usuario.show_data())
~~~

#### Calculadora 
~~~ python
def suma(num1, num2):
    return num1 + num2

def resta(num1, num2):
    return num1 - num2

def multiplicacion(num1, num2):
    return num1 * num2

def division(num1, num2):
    return num1 / num2

print("Por favor, elige una operación:")
print("1. Suma")
print("2. Resta")
print("3. Multiplicación")
print("4. División")

opcion = input("Ingresa una opción (1/2/3/4): ")

num1 = float(input("Ingresa el primer número: "))
num2 = float(input("Ingresa el segundo número: "))

if opcion == '1':
    print(num1, "+", num2, "=", suma(num1, num2))

elif opcion == '2':
    print(num1, "-", num2, "=", resta(num1, num2))

elif opcion == '3':
    print(num1, "*", num2, "=", multiplicacion(num1, num2))

elif opcion == '4':
    print(num1, "/", num2, "=", division(num1, num2))

else:
    print("Opción inválida")
~~~
