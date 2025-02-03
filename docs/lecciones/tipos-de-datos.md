# Tipos de datos

Todos sabemos que un número y un fragmento de texto son muy diferentes. ¿Cómo lo sabemos? Bueno, se pueden realizar operaciones aritméticas (como la multiplicación) con números, pero no con textos. Kotlin también lo sabe. Por eso, cada variable tiene un tipo que determina qué operaciones posibles se pueden realizar con esa variable y qué valores se pueden almacenar en ella.

## Tipos de variables

El tipo de una variable se establece cuando se declara la variable:

```kotlin
val text = "Hola, ahora estoy estudiando Kotlin."
val n = 1
val firstLetter = 'A'
val condition = true
```

En este caso, Kotlin sabe que `text` es una cadena, `n` es un número, `firstLetter` es un carácter y `condition` es un booleano. Kotlin determina los tipos de ambas variables automáticamente. Este mecanismo se llama **inferencia de tipos**.

Por favor, observa el siguiente fragmento de código. Así es como declaramos una variable con inferencia de tipos:

```kotlin
val/var identificador = valor
```

También puedes especificar el tipo de una variable al declararla:

```kotlin
val/var identificador: Tipo = valor
```

Ten en cuenta que el nombre del tipo siempre comienza con una letra mayúscula.
Declaremos las mismas variables que en el ejemplo anterior y especifiquemos sus tipos:

```kotlin
val text: String = "Hola, ahora estoy estudiando Kotlin."
val n: Int = 1
val firstLetter: Char = 'A'
val condition: Boolean = true
```

El tipo `Int` indica que la variable almacena un número entero (`0`, `1`, `2`, `100_000_000`, ...). El tipo `String` indica que la variable almacena una cadena (`"Hola"`, `"John Smith"`). Más adelante, aprenderás más sobre estos y otros tipos de datos.

Ves que se pueden usar estas dos formas de declaración de variables en la práctica. Cuando usa la inferencia de tipos, hace que su código sea más conciso y legible, pero en algunos casos, puede ser mejor especificar el tipo.

No es necesario asignarle el valor a una variable en el momento de definirla, podemos hacerlo más tarde. Pero en este caso el compilador no puede inferir el tipo de dato que se le va asignar, y tenemos que decirselo.

```kotlin
val saludo // error
greeting = "hola"
```

El ejemplo anterior producirá un error de compilación (`La variable 'saludo' debe inicializarse`), ya que Kotlin no puede inferir el tipo de la variable cuando simplemente se declara. Por el contrario, el ejemplo siguiente sí funciona porque el tipo lo especifica el programador:

```kotlin
val greeting: String // ok
greeting = "hola"
```

## Tipos de datos para números

## Otros tipos de datos

### Clasificación básica de tipos de datos
