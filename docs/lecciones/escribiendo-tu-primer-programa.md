---
layout: playground
title: Escribiendo tu primer programa
description: Teoría - Escribiendo tu primer programa
---

# Escribiendo tu primer programa

En esta lección, escribirás tu primer programa Kotlin, que imprime **"¡Hola, mundo!"**. Este es el primer paso que todo principiante debe dar. Aunque el programa en sí es muy simple, sigue siendo un programa funcional y muestra la sintaxis básica del lenguaje de programación.

## Hola, mundo

Aquí viene. A continuación se muestra el código fuente de este programa:

```kotlin
fun main() {
    println("¡Hola, mundo!")
}
```

### Explicación del código

Si ya has instalado un entorno de programación en tu computadora, puedes ejecutar el programa allí. Si no, tienes la opción de ver como funciona, haciendo click en ▶️. Y ya veremos como instalar un entorno de programación más adelante.

### Terminología básica

Ahora, aprendamos la terminología básica y luego intentemos comprender nuestro programa.

- Un **programa** es una secuencia de instrucciones (llamadas sentencias), que se ejecutan una tras otra de manera predecible.
El flujo secuencial es la situación más común y sencilla cuando las sentencias se ejecutan en el orden en que están escritas, es decir, de arriba hacia abajo, una tras otra;
- Una **sentencia** (o una declaración de programación) es un comando único que se debe ejecutar (como imprimir un texto);
- Una **expresión** es un fragmento de código que produce un único valor (por ejemplo, 2*2 es una expresión);
- Un **bloque** es un grupo de cero o más declaraciones encerradas en un par de llaves {...}; nuestro programa consta de un solo bloque;
- Una **palabra clave** es una palabra que tiene un significado especial en el lenguaje de programación. Los nombres de las palabras clave no se pueden cambiar;
- Un **identificador** (o un nombre) es una palabra escrita por el programador para identificar algo;
- Un **comentario** es un fragmento de texto que se ignora al ejecutar el programa; solo explica una parte del código. Los comentarios comienzan con `//`
- **El espacio en blanco** es un área en blanco, una tabulación o una nueva línea; se utiliza para separar palabras en el programa y para mejorar la legibilidad.

### El programa Hola Mundo bajo el microscopio

El programa **Hola Mundo** ilustra el uso de los elementos básicos de cualquier programa Kotlin. En este momento, consideraremos solo los más importantes.

**El punto de entrada**. La palabra clave `fun` define una función que contiene un fragmento de código para ejecutar. Esta función tiene un nombre especial `main`. Indica el punto de entrada de un programa Kotlin. La función tiene un cuerpo entre llaves {...}.

```kotlin
fun main() {
   // ...
}
```

### Explicar el código

Hablaremos de las funciones más adelante. El nombre de esta función debe ser siempre el mismo: `main`. Si la nombra `Main` o `MAIN` o cualquier otro, el programa no se iniciará.

>**Nota**: El texto después de `//` es solo un comentario, no una parte del código. Además, aprenderemos a escribir comentarios.

**Imprimir "¡Hola, mundo!"**. El cuerpo de esta función consta de instrucciones de programación que definen lo que debe hacer el programa. Nuestro programa imprime la cadena **"¡Hola, mundo!"** utilizando la siguiente instrucción:

`println("¡Hola, mundo!")`

Esta es una de las cosas más importantes que hay que entender sobre el programa **Hola mundo**. Llamamos a la función `println` para mostrar una cadena seguida de una nueva línea en la pantalla. A menudo utilizaremos esta forma para imprimir algo.

>**Recuerda** que `"Hola, mundo!"` no es una palabra clave ni un nombre, es solo una cadena literal que se imprime en la pantalla.

## Programas con múltiples declaraciones

Como regla, un programa contiene múltiples declaraciones. Debes comenzar una nueva línea para escribir cada declaración. Por ejemplo, el programa a continuación tiene dos declaraciones:

```kotlin
fun main() {
    println("Hola")
    println("Mundo")
}
```

Si ejecutas el programa, verás que muestra esto:

```DOS
Hola
Mundo
```

## Conclusión

¡Felicitaciones! Hemos escrito nuestro primer programa, que imprime **"¡Hola, mundo!"** Tiene una función llamada `main`, que representa el punto de entrada de este programa. No te preocupes por todos esos términos (**sintaxis**, **declaración**, **bloque**) por ahora; los explicaremos a lo largo de este curso.

No olvides que puedes usar tu primer código como plantilla para tus futuros programas.

[¡Practiquemos!](/lecciones/ejercicio-021)
