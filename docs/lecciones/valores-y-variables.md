---
layout: default
title: Valores y variables
description: Teoría - Valores y variables
---

# Valores y variables

## ¿Qué es una variable?

Una variable es un almacenamiento para un valor, que puede ser una cadena, un número u otra cosa. Cada variable tiene un *nombre* (o un **identificador**) para distinguirla de otras variables. Puedes acceder a un valor por el nombre de la variable.

Las variables son uno de los elementos más utilizados en los programas; por lo tanto, es importante entender cómo utilizarlas.

## Declaración de variables

Antes de poder comenzar a utilizar una variable, debes declararla. Para ello, Kotlin proporciona dos palabras clave:

- **`val`** (para valor) declara una variable de **solo lectura** (solo un valor nombrado), que no se puede cambiar después de que se haya inicializado, por lo que se puede asignar un valor una vez (en realidad, esto no es del todo cierto, analizaremos este tema con más detalle más adelante);
- **`var`** (para variable) declara una variable mutable, que se puede cambiar (tantas veces como sea necesario).
**`const`** se utiliza para constantes (junto con `val`), para valores que se conocen *en tiempo de compilación*.

¡Las palabras clave `val` y `var` te proporcionan una variable!

Cuando declaras una variable, debes agregar su nombre después cualquiera de una de estas dos palabras clave. Ten cuidado: el nombre de una variable no puede comenzar con un dígito. Generalmente, comienza con una letra. Debes elegir nombres significativos y legibles para las variables para que tu código sea fácil de entender.

Para asignar un valor determinado a una variable, debemos usar el operador de asignación `=`.

Declaremos una variable inmutable llamada `language` y guardaremos en ella la cadena `"Kotlin"`.

```kotlin
val language = "Kotlin"
```

Ahora podemos acceder a esta cadena por el nombre de la variable. ¡Vamos a imprimirla!

```kotlin
println(language) // Imprime "Kotlin" sin comillas
```

Esta variable no se puede modificar después de que se haya dado un valor, porque se declaró como `val`.

Los **identificadores** distinguen entre mayúsculas y minúsculas: `language` no es lo mismo que `Language`.

Ahora, declaremos una variable mutable llamada `dayOfWeek` e imprimamos su valor antes y después de cambiarlo.

```kotlin
var dayOfWeek = "lunes"
println(dayOfWeek) // Imprime lunes

dayOfWeek = "martes"
println(dayOfWeek) // Imprime martes
```

En el ejemplo anterior, declaramos una variable llamada `dayOfWeek` y la inicializamos con el valor `"lunes"`. Luego, accedimos al valor por el nombre de la variable y lo imprimimos. Después de eso, cambiamos su valor a `"martes"` e imprimimos este nuevo valor.

No es necesario que vuelvas a declarar una variable para cambiar su valor. Simplemente asígnale un nuevo valor usando el operador `=`.

También es posible declarar e inicializar una variable con el valor de otra variable:

```kotlin
val cost = 3
val costOfCoffee = cost
println(costOfCoffee) // Imprime 3
```

## Almacenar diferentes tipos de valores

Ya hemos mencionado que las variables pueden almacenar diferentes tipos de valores: cadenas, números, caracteres, booleanes y otros tipos de datos, que veremos más adelante.

Declaremos cuatro variables inmutables para almacenar un número, una cadena, un carácter y un booleano, y luego imprimamos sus valores.

```kotlin
val ten = 10
val greeting = "Hola"
val firstLetter = 'A'
val condition = true

println(ten)         // Imprime 10
println(greeting)    // Imprime Hola
println(firstLetter) // Imprime A
println(condition)   // Imprime true
```

Sin embargo, existe una restricción para las variables mutables (las declaradas con la palabra clave `var`). Al reasignar sus valores, solo puede usar valores nuevos del mismo tipo que el inicial. Por lo tanto, el fragmento de código a continuación no es correcto:

```kotlin
var number = 10
number = 11     // Ok
number = "doce" // ¡Aquí hay un error!
```

>**¡Recuerde esta restricción!**
>
>Los lenguajes que tienen esta restricción, como Koltin, se les conoce como **lenguaje fuertemente tipado**.

## Conclusión

Ahora sabes que hay dos palabras clave que se utilizan para declarar variables. De hecho, en muchos casos, es mejor usar variables inmutables (aquellas declaradas con la palabra clave `val`). Antes de usar `var`, debes asegurarte de que `val` no sea adecuado en ese caso. Si realmente no lo es, usa `var`.

Sin embargo, ten en cuenta que cuantas más variables mutables tengas en tu código, más difícil será leerlo y comprenderlo.

>**Recuerda**, las variables inmutables ayudan a escribir código más legible. Por lo tanto, ¡usa `val` siempre que sea posible! Puedes reemplazarlo fácilmente con `var` cuando sea absolutamente necesario.

[¡Practiquemos!](/lecciones/ejercicio-031)
