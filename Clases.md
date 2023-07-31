<h1>Introducción a la IA</h1>
_______________________________________________________________________________
<p>La inteligencia artificial o IA, se refiere a la simulación de la inteligencia humana en maquinas que están programadas para pensar como humanos y replicar sus acciones.</p>

![[Pasted image 20230727111307.png]]

<p>En el núcleo de la IA están los algoritmos de aprendizaje automático, que son instrucciones para que las computadoras aprendan por sí mismas. Los datos de entrenamiento se utilizan para enseñar a estos algoritmos cómo hacer predicciones o tomar decisiones basándose en datos de entrada.</p>
<h3>Alpha go</h3>
<p>Un buen ejemplo de estos algoritmos seria el mas conocido siendo el Alpha go, donde Lee Sedol se enfrento a esta misma IA, donde solo pudo obtener una sola victoria después de varias derrotas, esto fue posible ya que la inteligencia fue programada como un sistema neuronal, y donde se enfrento a otro sistema similar, donde solo tenían las reglas básicas del juego, pero después de cientos de partidas lograron aprender las mejores estrategias.</p>

![[Pasted image 20230727111443.png]]

<h3>Diferentes Tecnologias</h3>
<p>IA débil o estrecha: Este tipo de IA es el que más comúnmente encontramos en el mundo hoy en día. Es una IA diseñada y entrenada para realizar una tarea específica, como reconocimiento de voz, recomendaciones de productos, clasificación de correos electrónicos como spam, o jugar ajedrez. No tiene conciencia, ni puede comprender o aprender cualquier cosa más allá de su campo de entrenamiento.</p>
<p>IA general: También conocida como IA fuerte, esta categoría incluye AI que puede entender, aprender y aplicar el conocimiento en una gama de tareas al mismo nivel que un humano. Podría entender el contexto, tomar decisiones y resolver problemas incluso en áreas que nunca ha encontrado antes.</p>
<p>IA superinteligente: Es una IA que supera la capacidad de los humanos en casi todas las actividades económicamente valiosas. En otras palabras, podría superar a los humanos en la mayoría de las tareas que son útiles y valiosas para nosotros.</p>
<h3>Sesgo de la inteligencia artificial en el sistema de seguridad</h3>
<p>Esto ocurrió cuando los datos que se utilizo para el entrenamiento del sistema contenía mas gente de color, esto causo que el sistema aprendiera que las personas de raza tienen la mayor posibilidad de cometer un delito.</p>
<h3>ChatGPT</h3>
<p>El ChatGPT es una serie de modelos de lenguaje desarrollados por OpenIA, estos modelos utilizan inteligencia artificial para generar texto que es similar a las personas, ya que se basan en una técnica de aprendizaje profundo llamada Transformers, que utilizan el procesamiento de lenguaje natural para entrenarse en enormes cantidades de texto y luego generar sus propias respuestas a las solicitudes de los usuarios.</p>
<h3>Medicina Personalizada</h3>
<p>La medicina personalizada, la cual también es conocida como medicina de precisión, se refiere a la personalización del ciudad medico para adaptarlo a las características individuales de cada paciente.</p>
<p>Un buen ejemplo de este tema serian los médicos en la India, donde lo médicos de la zona no son suficientes para todas las personas, por ellos han programado una IA donde reconoce los síntomas para encontrar el tipo de enfermedad que padece, una de estas IA seria la que analiza tus ojos y puede concluir si tienes diabetes o no.</p>

<h1>Python</h1>
_______________________________________________________________________________
<p>Es un lenguaje de programación fácil de leer que permite asignación de variables, operaciones matemáticas, condicionales y manipulaciones de cadenas, entre otros</p>
<p>Ejemplo 1</p>

```python
def suma(num1, num2):
    return num1 + num2

numero1 = float(input("Ingrese el primer número: "))
numero2 = float(input("Ingrese el segundo número: "))

resultado = suma(numero1, numero2)

print(f"el resultado es {resultado} final")
```

<p>Ejemplo 2</p>

```python
 def multiply_by_two(x):
  """This function multiplies
  an input number by 2"""
  return x * 2

help(multiply_by_two)
```

<p>Si se quiere aplicar Python para hacer aplicaciones se tiene que usar el Pycham, para realizar los BackEnds</p>
<h3>Funciones y Ayuda</h3>
<p>Una función en python es un bloque de código reutilizable que realiza una acción especifica</p>
<p>Ejemplo 1</p>

```python
def apply_func_twice(func, arg):
  """This function applies 'func' twice to 'arg'"""
  return func(func(arg))

def add_five(x):
  return x + 5
  
print(apply_func_twice(add_five, 10))
```

<p>Ejemplo 2</p>

```python
def greet(person):
  return f"Hello, {person}!"

def repeat(func, times, arg):
  for _ in range(times):
    print(func(arg))

repeat(greet, 3, 'OpenAI')
```

<h3>Boléanos</h3>
<p>Python utiliza los valores boléanos para determinar una variante true o false.</p>

```python
esta_encendido = True
es_visible = False

if esta_encendido:
    print("El dispositivo está encendido.")
else:
    print("El dispositivo está apagado.")

numero = 10
es_mayor_que_cinco = numero > 5
print(es_mayor_que_cinco)

resultado = esta_encendido and es_visible
print(resultado) 

resultado = esta_encendido or es_visible
print(resultado)

resultado = not esta_encendido
print(resultado)
```

<h3>Listas</h3>
<p>Son secuencias ordenadas de valores que pueden ser modificadas e indexadas, también pueden modificarse.</p>

```python
fruits = ['apple', 'banana', 'cherry', 'eldeberry']

print(fruits[1:3])

fruits[0] = 'apricot'

fruits.append('date')

print(fruits)

print(fruits[-1])
```

<h3>Ejercicios</h3>
<p>Ejercicio: Preguntar sobre un signo zodiacal especifico y que con su respuesta dar su suerte.</p>

```python
ask = input("¿Que signo zodiacal eres? ")

zodiacal = ['picis', 'aries', 'tauro', 'acuario']

mensaje = ['Se enamora', 'Terminará con la tóxica', 'Ganará la lotería', 'Comerá bien rico']

if ask.lower() in zodiacal:
    print(mensaje[zodiacal.index(ask.lower())])
else:
    print("No se ha encontrado nigun Signo")
```


<h3>Bucles y comprensión de listas</h3>
<p>Los bucles en Python (for, while) repiten código determinado. las comprensiones de listas permiten condensar bucles y condicionales en una sola.</p>
<p>Ejemplo 1</p>

```Python
even_squares = [i**2 for i in range(10) if i % 2 == 0]
print(even_squares)
```

<p>Ejemplo 2</p>

```Python
num = 5
factorial = 1
while num > 0:
  factorial *= num
  num -= 1
print(factorial)
```

<h3>Strings y Diccionarios</h3>
<p>Las cadenas son flexibles e inmutables, soportando múltiples métodos de manipulación. las listas y diccionarios también son útiles para organizar datos</p>
<p>Ejemplo 1</p>

```Python
s = "Hello, Mars!"
print(s.lower())
print(s.upper())
print(s.split(", "))
```

<p>Ejemplo 2</p>

```Python
planets = [
    'Mercury', 'Venus', 'Earth',
    'Mars', 'Jupiter', 'Saturn',
    'Uranus', 'Neptune'
]
planet_initials = {
    planet: planet[0]
    for planet in planets
}
print(planet_initials)
```

<h3>Trabajando con librerías externas</h3>
<p>Python permite la importación de librerías ya sea estándar o personalizadas, a través de importaciones. Las librerías contienen módulos que son colecciones de funciones valores</p>

```Python
from math import sqrt

print("Square root of 16 is", sqrt(16))
```

<h1>Nestjs</h1>
_______________________________________________________________________________
<p>Tiene el lenguaje TypeScript por defecto, pero tambien permite vanilla JavaScript.</p>
<p>Instalación</p>

``` cmd
npm i -g @nestjs/cli
```

``` cmd
nest new project-name
```

<h3>Node HTTP Frameword</h3>
<p>Express</p>
<p>Fastify</p>
<h3>Controladores</h3>
<p>Los Controladores son los encargados de escuchar solicitud y emite respuestas</p>