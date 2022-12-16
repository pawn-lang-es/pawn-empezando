# Un lenguaje de programación ...

El lenguaje de programación es aspecto más notable de cada cosa relacionada a la
programación. Muchos cursos que enseñan programación se enfocan en uno o más
lenguajes de programación, y esta introducción no es la excepción. Para propósitos
 de ilustrar cómo un lenguaje de programación luce, veamos un programa simple 
 (en lenguaje PAWN): un programa que suma dos números.

```cpp
main()
    {
        new a, b, total

        a = 24
        b = 32
        total = a + b

        printf "%d", total
    }
```

La primera linea dice `main()`. Este es la definición del punto de entrada para 
el programa. El programa empieza aquí, y ejecutará todas las instrucciones que 
estén encerradas entre las llaves. Desde este punto en adelante, el computador 
correrá a través del programa hacia abajo, una instrucción a la vez. Más adelante
aprenderás que existen instrucciones específicas en un lenguaje de programación
que cambian el *flujo* de control, pero el flujo básico es secuencialmente hacia
abajo.

La primera instrucciones seguida de la llave de apertura (`{`), es una declaración
de tres *variables*. Una variable puede ser vista como una caja (o contenedor): la
mayoría de las variables contienen un único valor, o incluso contienen una colección 
de valores u otra información. El programa puede guardar algo en una variable, y 
obtener dicho valor más adelante. El contenido de una variable no cambia por sí 
misma; la única forma de que una variable pueda recibir nueva información es porque 
un programa almacena algo diferente en la variable. Es importante mecionar que una 
variable toma espacio en la memoria (RAM) del computador y por tanto debe ser *creada*.

Las siguientes tres sentencias en el programa son `asignaciones`. Una asignacón 
almacena un valor (o alguna otra cosa) en una variable. Para los que están 
acostumbrados a la matemática, el uso del símbolo `=` podría ser confuso a 
primera vista, porque este símbolo no denota igualdad. Sino, que lo que está 
en la derecha del = debe ser almacenado en la variable que está en la izquierda. 
La parte derecha podría ser una exprensión aritmética, tal como la instrucción 
que suma `a`y `b` y lo almacena en la variable `total`; la parte izquierda del 
símbolo = debe ser siempre una única variable.

Hay una sentencia más antes de la llave de cierre: `printf "%d", total`. En esta 
línea que parece encriptada, la primera palabra, `printf` indica la acción: enviar 
algo a la termina o a una pantalla (del computador); la última palabra, `total`, 
es la variable cuyo valor queremos mostrar, y en el medio hay un código que controla 
*como* el valor es mostrado. La palabra `printf` es una función del sistema, está 
documentada en la Referencia del programador, junto con otros códigos de control. 
El código `%d` significa: mostrar un valor con base decimal y sin una parte fraccionaria.

Lo anterior completa el programa. Cuando el programa "corre", ejecuta todas las 
sentencias entre las llaves de apertura y cierre (`{` y `}`), y luego finaliza. 
Córrelo otra vez, y hará la misma secuencia de pasos, sin siquiera agotarse o 
sin darse cuenta que ya es la segunda (o tercera, cuarta, ...) vez que corre.

Las variables en este programa tienen los nombres `a`, `b` y `total`. Tu puedes 
escoger los nombres de las variables, pero hay algunas reglas a las que debes 
obedecer. Por ejemplo, solo podrías usar letras, números y el carácter `_` en 
el nombre de una variable, y el primer caracter no puede ser un número. Además, 
a pesar de que las mayúsculas y minúsculas son válidas, ellas indicarán variables 
diferentes. Por ejemplo, puedes tener dos variables distintas en tu programa 
que se llamen `manzana` y `Manzana`, respectivamente. Otra forma de explicar 
esto es decir que el lenguaje de programación PAWN es sensitivo a las mayúsculas 
y minúsculas (o *case sensitive* en inglés). No todos los plenguajes de programació
n son sensitivos a las mayúsculas y minúsculas.

El propósito de una asignación es guardar un valor o alguna pedazo de "información" 
para su uso posterior. El valor puede ser cualquier cosa: número de cuentas, nombres, 
total de caminatas, o cualquier elementos que necesitas que el programa recuerde 
durante un momento. Un programa no tiene más memoria que la que esté en sus variables. 
Cuando un programa se ejecuta paso por paso a través de las sentencias, no recuerda 
nada acerca de la(s) sentencia(s) anterior(es). Si el resultado de la actual sentencia 
es importante para otra más abajo en el programa, el resultado debe ser almacenado 
en una variable. Por otro lado, si tu programa no usa el contenido de una variable en
algún otro momento, la asignación es redundante: tu programa podría haber funcionado 
exactamente igual si no tuviera la asignación —solo un poquito más rápido.

Es perfectamente normal cambiar el valor de una variable mientras se ejecuta el programa.
Por ejemplo, cuando quieres contar el número de segundos que tu programa está 
ejecutándose, podrías usar una variable que empiece en cero y se incremente cada 
segundo —como en la siguiente expresión: `tiempoDeEjecucion = tiempoDeEjecucion + 1`. 
En álgebra, esto sería una falsedad: un valor no puede ser igual a sí mismo más uno; 
pero en la programación simplemente significa que el nuevo valor de la variable se 
convertirá en su valor actual más uno.

El orden de las tres sentencias de asignación en el ejemplo es importante. Lo que el 
programa hace (después de la declaración de las variables), es poner un valor en `a`, 
luego otro en `b`, y finalmente la suma que calcula en `total` —donde usa los valores 
previamente almacenados en `a` y `b`. Si tu te acercas a tu vecino y le dices que 
gastaste tu dinero en un sombrero que costaba $ 24 y un libro, y luego recordaste que 
el libro costó $ 32, tu vecino no tendrá ninguna problema en descubrir tu gasto total. 
Pero si lo dices en un programa como las lineas siguientes, estás destinado a obtener 
una respuesta incorrecta:
```cpp
sombrero = 24
total = sombrero + libro
libro = 32
```
La primera asignación, `sombrero = 24` está bien. Cuando el computado mira la segunda 
segunda asignación, todavía no sabe que valor podría tener `libro`. Sin embargo, el 
computador solo se enfocará en esa única instrucción: `total = sombrero + libro`; no 
mirará más adelante ni tampoco recordará que sucedió en el pasado reciente. Y como 
resultado, el computador simplemente asumirá un valor para `libro`. Normalmente podría 
ser asumido como cero en la secuencia anterior, por lo que la asignación establece 
`total = 24 + 0`, lo cual es 24. La última asignación está bien para lo que el 
computador le concierne, pero será inútil en este punto.

> [Regresar a la página anterior](01-un-breve-recorrido.md) (Un breve recorrido)
>
> [Ir a la siguiente página](03-las-herramientas-para-hacerlo.md) (... las herramientas para hacerlo ...)
>
> <sub>[Subir al principio de esta página](#un-lenguaje-de-programación)</sub>