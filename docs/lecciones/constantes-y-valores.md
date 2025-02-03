---
layout: default
title: Constantes y variables tipo val
description: Teoría - Constantes y variables tipo val
---

# Constantes y variables tipo `val`

A veces, es necesario utilizar una variable que no se debe modificar durante la ejecución del programa. Dichas variables se conocen como constantes o variables `val` en Kotlin, donde se declaran con la palabra clave `val`. La diferencia entre una variable `var` y una variable `val` es, como hemos visto, que no podemos modificar su valor una vez asignada.

## Variables val

El siguiente código presenta dos variables `val`: `pi`, que representa una constante matemática conocida, y `helloMsg`, que representa una cadena de texto.

```kotlin
val pi = 3.1415
val helloMsg = "Hola"

println(pi) // 3.1415
println(helloMsg) // Hola
```

Ambas variables no se pueden modificar, pero se puede acceder a ellas tantas veces como sea necesario.

El compilador producirá un error si intentamos modificar el valor de una variable `val`, si intentas compilar el código siguiente tendrás como resultado un error: Val no se puede reasignar.

```kotlin
val pi = 3.1415
pi = 3.1416 // línea de error
```

Ten en cuenta que el valor de una variable `val` se puede reasignar a una variable `var` sin ninguna restricción y el valor de una variable regular se puede cambiar tantas veces como sea necesario:

```kotlin
val count = 10
var cnt = count
cnt = 20 // Aquí no hay errores, cnt no es una constante
```

### Variables `val` y mutabilidad

Es importante tener en cuenta que `val` no es sinónimo de inmutable. En el siguiente ejemplo, utilizaremos una `MutableList`, que es un conjunto ordenado de elementos del mismo tipo. Puedes avanzar y aprender más sobre `MutableList`, pero no es necesario en este momento.

```kotlin
// Creación de la lista
val myMutableList = mutableListOf(1, 2, 3, 4, 5)
// Intentando actualizar la lista
myMutableList = mutableListOf(1, 2, 3, 4, 5, 6) // Línea de error
```

La segunda línea no se compilará, ya que estamos intentando reasignar una variable val. Sin embargo, hay un punto esencial que recordar.

Siempre es posible cambiar el estado interno de una variable `val`: si bien está prohibido reasignar la variable, su contenido se puede modificar de otras maneras.

Entonces, el siguiente código es correcto:

```kotlin
// creación de la lista
val myMutableList = mutableListOf(1, 2, 3, 4, 5)
// Añadir un nuevo elemento
myMutableList.add(6) // Funciona
// Imprimir lista
println(myMutableList) // [1, 2, 3, 4, 5, 6]
```

Como puedes ver, este código cambió el estado interno de `myMutableList` agregando otro número entero. Cuando invocamos la función add(), no cambiamos la variable en sí, sino la lista que representa.

Si estás familiarizado con el lenguaje de programación Java, puede que te resulte más fácil pensar en las variables `val` de Kotlin como variables `final` de Java. Son bastante similares: ambas prohíben reasignar un valor a la variable, pero permiten cambiar el estado interno del objeto.

## Variables constantes

En Kotlin, también hay un modificador `const`, que se usa antes de la palabra clave `val` para declarar una constante de tiempo de compilación. El valor de una variable constante se conoce en el momento de la compilación y no se modificará en el momento de la ejecución:

```kotlin
const val MY_STRING = "Esta es una cadena constante"
```

El siguiente código te dará un error, ya que el valor es desconocido antes de la ejecución del programa y no es una constante:

```kotlin
const val MY_STRING = readln() // ¡¡¡no es una cadena constante!!!
```

Existen algunas restricciones sobre cuándo se puede aplicar el modificador `const`. En primer lugar, solo se puede utilizar con una variable de tipo `String` o un valor primitivo:

```kotlin
const val CONST_INT = 127
const val CONST_DOUBLE = 3.14
const val CONST_CHAR = 'c'
const val CONST_STRING = "Soy constante"
const val CONST_ARRAY = arrayOf(1, 2, 3) // Error: solo se permiten primitivas y cadenas
```

Además, las variables const deben declararse en el nivel superior, fuera de cualquier función:

```kotlin
const val MY_INT_1 = 1024 // Línea correcta

fun main() {
   const val MY_INT_2 = 2048 // Error: el modificador 'const' no es aplicable a una 'variable local'
}
```

### Cuándo utilizar variables `val`

Esperamos que ahora comprendas cómo funciona la palabra clave `val` para las variables. Es hora de averiguar cuándo utilizarla.

Una buena práctica es utilizar variables val de forma predeterminada. Luego, cuando parezca necesario para el código, cámbielas por variables `var`:

```kotlin
var a = 1024
val b = 256
val c = 128
a += b * c
```

Este enfoque le permite escribir programas con la cantidad mínima de variables mutables, lo que genera menos errores.
