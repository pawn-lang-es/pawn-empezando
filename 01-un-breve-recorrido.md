# Un breve recorrido

Sea cual sea el lenguaje o la herramienta, la programación es un proceso que 
requiere una forma particular de resolver los problemas —o incluso una forma
particular de pensar sobre las actividades y la información. Se centra alrededor
del *analisis*: "lo que se tiene que hacer bajo ciertas condiciones", del 
*reduccionismo*: subdividir una tarea larga en una jerarquía de tareas más 
pequeñas, y de la *síntesis*: unir todo de forma adecuada.

Antes de empezar a crear un programa, debes entender el problema que se te 
presenta. Una vez tengas una idea clara de lo que el programa debe hacer, tienes
que pensar una solución en pequeños pasos *deterministas* y *discretos*. Cada paso
podría tener entradas y salidas, y debes ser capaz de describir la función de
dicho paso en términos únicamente de sus entradas y salidas —esto es lo que el 
término *discreto* significa. Si no eres capaz de explicar un paso sin referirte
a otros "pasos" en el programa, o tienes una entrada oculta o asumes algo que no 
deberías, por lo que debes reconsiderar tu análisis. El término *determinista*
significa que el funcionamiento de los pasos o una sequencia de pasos no deberían
depender de la interpretación (humana) o suposiciones.

Muchos programadores principantes encuentran útil escribir estos pasos en un 
diagrama de flujo (o de otra forma). Durante el análisis del programa y su 
solución, encontrarás frecuentemente que algunos pasos son más grandes —o 
demasiado grandes para ser anotados en una pequeña caja de una diagrama. Dichos 
pasos más grandes deben ser subdivididos, tal vés en otro diagrama. [...] Los 
diagramas de flujo son la semántica más antigua de un programa. No obstante, 
muchos otros tipos de diagramas y gráficos existen hoy en día.

![Este es un diagrama de flujo](./images/flow-chart.PNG)

Lo que la mayoría de personas perciben como "programación", el acto de escribir
código en un lenguaje de programación, solo comienza después de  que el análisis
anterior se haya realizado. Existen muchos lenguajes de programación, y lo
que todos ellos tiene en común es una "gramática" estricta y rígida (llamada sintaxis)
y la habilidad de inventar nuevas "palabras" de un vocabulario pequeño.
Sin embargo, la gran diferencia entre los lenguajes de programación y los 
lenguajes naturales, es que los lenguajes de programación son diseñados para 
permitir la comunicación con una *máquina*. Una máquina, u otro dispositivo
programable, hace *exactamente* lo que se le instruye —ni un poquito más ni menos.
Una máquina no asume nada sobre su entorno; tampoco anticipa cualquier instrucción
futura, ni tampoco recuerda lo que hizo hace un milisegundo. Los "pasos pequeños, 
deterministas y discretos" que se mencionaron en el párrafo anterior deben,
por tanto, también ser *precisos* y de fácil *comprensión*. 

Los diagramas de flujo, u otro tipo de diagramas, pueden ser creados a mano y en
papel, pero construir un programa que un computador pueda ejecutar requiere
herramientas especiales —con nombres como *compilador*, *enlazador/localizador*,
*editor* y *debugger*. También, la mayoría de los programadores son usuarios 
con "permisos administrativos" en sus computadores y las herramientas que usan
son frecuentemente menos limpias que tu suite de ofimática favorita. Por otro lado, 
las herramientas hechas para los programadores buscan que trabajes eficientemente,
en lugar de hacerte perder el tiempo con animaciones, soniditos innecesarios y
otros intentos de lucir *cool*. Brevemente: no seas despectivo con las interfaces
rudimentarias de las herramientas de los programadores.

![La herramienta de un programador: el IDE de Pawn](./images/ide-quincy.PNG)

Una vez que hayas atravezado todo esto —cuando el análisis de los requerimientos
y la descomposición en pasos pequeños sea completada, y después de haber escrito
el código, podemos (finalmente) ejecutar el programa y mirar sus salidas.
Frecuentemente, el programa no se comporta como se esperaba o incluso podría no
ejecutarse en su primera versión. Esto podría ser debido a simples errores de escritura,
los cuales son simples de corregir; pero también podría ser debido a que el 
programador no entendió correctamente el problema. Naturalmente, ahora tenemos 
que encontrar y solucionar los errores en el programa, lo cual es un ciclo muy 
similar al usado en el desarrollo inicial:

- entender el comportamiento del programa y lo que el programa *debería* estar
haciendo,
- encontrar una solución en pequeños pasos discretos,
- escribir estos pasos en el lenguaje de programación,
- y, revisar y probar el programa.

Básicamente, no hay mucha diferencia entre el proceso del desarrollo inicial de 
un programa y el de la correción/mantenimiento de un programa existente. El autor 
de este manual tiene mucho más que decir sobre encontrar y corregir errores, 
pero solo dirá que probar y debuguear (el proceso de corregir errores en un programa)
es parte integral del ciclo de desarrollo.

> [Regresar a la página anterior](00-introduccion-a-la-programacion.md) (Introducción a la programación)
>
> [Ir a la siguiente página](02-un-lenguaje-de-programacion.md) (Un lenguaje de programación ...)
>
> <sub>[Subir al principio de esta página](#un-breve-recorrido)</sub>