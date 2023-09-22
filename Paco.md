### Apuntes de la primera parcial de el tercer semestre 
#### Empezamos con analisis de codigo estatico 
""" mensaje: str = "Hola "
numero : float = 3.1416
otro_numero: int = 15 """

""" num = ""
n = input("Dame un numero entero ")
if n%2 == 0:
    num = "par "
else:
    num = "Impar "
    
    num  """


#### Casting 

num_str = "3 "
num_int = int(num_str)
print(f"num_int: (num_int)")

num_float = 3.14
num_int = int(num_float)
print(f"num_int: (num_int)")

num_str = str(num_float)
print(f"num_str: (num_str)")

### Listas 
#### Colecciones 

def suma (a, b):
    return a+b
def resta (a, b):
    return a-b
def multiplicacion (a, b):
    return a*b
def division (a, b):
    return a/b
operaciones =[ suma, resta, multiplicacion, division]

print(operaciones[0](5, 4))
print(operaciones[1](5, 4))
print(operaciones[2](5, 4))
print(operaciones[3](5, 4))
    
for operacion in operaciones:
    print(operacion(5, 4))

lista = [1, 2, 3, 4, 5 True, 4.5, "Hola ", [1, 2, 3]]

#### Slinces 

print(lista)
print(lista[:])
def suma(a, b):
    pass

print(suma(3, 4))
def operaciones(a, b):
    return [a+b, a-b, a*b, a/b]

respuestas = operaciones(5, 4)
print(respuestas)
w, x, y, z = operaciones(5, 4)
print(w)
res_suma,_,_,_ = operaciones(5, 4)
res_suma


#### Tuplas

tupla_funciones = (suma, resta, multiplicacion, division)
print(tupla_funciones[1](5, 4))

tupla = (1, 2, 3, 4, 5, True, 4.5, "hola ", [1, 2, 3])
lista.append(10)
lista

tupla[0].__mod__(3)

def suma(a: int, b:int ) -> int:
    return a + b
def operacion(a: int, b:int ) -> (int, int):
    return (a+b, a-b)
(a, b) = operacion(5, 6)
a,b = operacion(6 ,5)
print (a,b)

#### Range 

numeros = range(10)
print(numeros)
range (0, 10)

for i in numeros:
    print(i, end=",")

    nuemos = range (5, 10)
numeros


for i in numeros:
    print(i, end= " ")

    numeros_pares = range (2, 11, 2)
for par in numeros_pares:
    print(par, end=" ")

    for item in range(2, 11, 2):
    print (item, end= " ")

    numeros = list(numeros)

    numeros 

    lista = [3, 6, 7, 40, 34, 67, 89]
max(lista)

min(lista)

sum(lista)

sorted(lista)

print(lista.sort())

lista.sort(reverse=True)
lista

#### Set Conjuntos 

mi_set = {1, 2, 3, 3, 3, 3}
mi_set

data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 1, 2, 2, 1, 2, 1, 2, 1]
list(set (data))

data2 = {1, 56, 57, 58}
mi_set.union(data2)

#### Diccionarios 

mi_dict = { "Llave": "Valor "}
mi_dict["Llave"]

mi_dict.keys()

mi_dict.values()

days_of_week ={
    "Monday": 1,
    "Tuesday": 2,
    "Wendneday": 3,
    "Thursday": 4,
    "Friday": 5,
    "Sarturday": 6,
    "Sunday": 7
}
for e in mi_set:
    print(e)
    
for key in days_of_week.keys():
    print(key, end=" ")
    
for value in days_of_week.items():
    print(key, value)
for value in days_of_week.values():
    print(value)
    
    print(days_of_week)

#### Ahora empezamos a usar streamlit para hacer paginas web como la siguiente que es una calculadora en streamlit 

import streamlit as st
 
st.sidebar.title("Calculadora ICI ")

def pedir_Valores():
    name = st.text_input("Nombre")
    n1 = st.number_input("Numero 1")
    n2 = st.number_input("Numero 2")
    
    if st.button("Sumar"):
        st.success(f"Hola {name}")
        st.write(f"{n1} + {n2} = {n1 + n2}")
        

opcion = st.sedebar.selecbox("opciones:", [
    "Suma", "Resta", "Multiplicaciion", "Division", "Acerca de"
])

match opcion:
    case "Suma":
        st.write("Esta es la opcion de suma...")
        pedir_Valores()
    case "Resta":
        st.write("Esta es la opcion de resta...")
    case "Multplicaacion":
        st.write("Esta es la opcion de Multiplicacion ...")
    case "Division ":
        st.write("Esta es la opcion de Division...")
    case "Acerca de":
        st.write("Derechos reservados...")

#### Tambien podemos hacer las opciones por separado como se puede ver aqui importanto desde mi libreria 

import milibreria as lib 

if __name__ == "__main__":
    print(lib.suma(7,8))
    print(lib. resta (8,4))

#### Para la resta 

def resta(a:int, b:int)-> int:
    return a-b

#### Y para la suma de diferentes maneras 

def suma(a: int, b: int) ->int:
    return a + b
def suma2(a: float, b: float)->float:
    return a + b
def suma1(a: int|float, b: int|float)-> int|float:
    return a + b

if __name__ == "__name__":
    print(suma("5," "6.5"))
    print(suma1())
    print(suma("5," "6.5"))
    
