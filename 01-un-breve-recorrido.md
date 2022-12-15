# Un breve recorrido

Sea cual sea el lenguaje o la herramienta, la programación es un [craft] que 
requiere una forma particular de resolver los problemas —o incluso una forma
particular de pensar sobre las actividades y la información. Se centra alrededor
del *analisis*: "lo que se tiene que hacer bajo ciertas condiciones", *reduccionismo*:
subdividir una tarea larga en una herarquía de tareas más pequeñas, y de la
*sintesis*: unir todo de forma adecuada.

Antes de empezar a crear un programa, debes entender el problema que se te 
presenta. Una vez tengas una idea clara de lo que el programa debe hacer, tienes
que pensar una solución en pequeños pasos deterministas y discretos. Cada paso
podría tener entradas y salidas, y debes ser capaz de describir la función de
dicho paso en términos únicamente de sus entradas y salidas —esto es lo que el 
término *discreto* significa. Si no eres capaz de explicar un paso sin referirte
a otros "pasos" en el programa, tienes una entrada oculta o asumes algo que no 
deberías, por lo que debes reconsiderar tu análisis. El término *determinista*
significa que el funcionamiento de los pasos o una sequencia de pasos no deberían
depender de la interpretación (humana) o suposiciones.

Muchos programadores principantes encuentran útil escribir estos pasos en un 
diagrama de flujo (o de otra forma). Durante el análisis del programa y su 
solución, encontrarás frecuentemente que algunos pasos son más grandes —o 
demasiado grandes para ser anotados en una pequeña caja de una diagrama. Dichos 
pasos más grandes deben ser subdivididos, tal vés en otro diagrama. [...] Los 
diagramas de flujo son la semántica más antigua de software. No obstante, muchos 
otros tipos de diagramas y gráficos existen hoy en día.

Lo que la mayoría de personas perciben como "programación", el acto de escribir
código en un lenguaje de programación, solo comienza después de  que el análisis
anterior se haya realizado. Existen muchos lenguajes de programación, y lo
que todos ellos tiene en común es una "gramática" estricta y rígida (llamada sintaxis)
y la habilidad de inventar nuevas "palabras" de un vocabulario pequeño.
Sin embargo, la gran diferencia entre los lenguajes de programación y los 
lenguajes naturales, es que los lenguajes de programación son diseñados para 
permitir la comunicación con una *máquina*. Una máquina, o otro dispositivo
programable, hace *exactamente* lo que se le isntruye —ni un poquito más ni menos.
Una máquina no asume nada sobre su entorno; tampoco anticipa cualquier instrucción
futura, ni tampoco recuerda lo que hizo hace un milisegundo. Los "pasos pequeños, 
deterministicas y discretos" que se mencionaron en el párrafo anterior deben,
por tanto, también ser *precisos* y *comprensivos*. 

Los diagramas de flujo, o otro tipo de diagramas, pueden ser creados a mano y a
papel, pero construir un programa que un computador puede ejecutar requiere
herramientas especiales —con nombres como *compilador*, *enlazador/localizador*,
*editor* y *debugger*. También, la mayoría de los programdores son usuarios 
con "permisos administrativos" en sus computadores y las herramientas que usan
son frecuentemente menos limpias que tu suite de ofimática favorita. Por otro lado, 
las herramientas hechas para los programadores buscan que trabajes eficientemente,
en lugar de hacerte perder el tiempo con animaciones, soniditos innecesarios y
otros intentos de lucir *cool*. Brevemente: no seas despectivo con las interfaces
rudimentarias de las herramientas de los programadores.

Una vez que hayas atravezado todo esto —cuando el análisis de los requerimientos
y la descomposición en pasos pequeños sea completada, y después de haber escrito
el código, podemos (finalmente) ejecutar el programa y mirar sus saldias.
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
- y, revisar y pobrar el programa.

Básicamente, no hay mucha diferencia entre el proceso del desarrollo inicial de 
un programa y el de la correción/mantenimiento de un programa existente. El autor 
tiene mucho más que decir sobre encontrar y corregir errores, pero solo dirá 
que probar y debuguear (el proceso de corregir errores en un programa) es parte 
integral del ciclo de desarrollo.