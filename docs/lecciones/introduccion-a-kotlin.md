---
layout: playground
title: Introducción a Kotlin
description: Teoría - Introducción a Kotlin
---

# Introducción a Kotlin

## ¿Qué es Kotlin?

Kotlin es un lenguaje de programación moderno y muy eficaz desarrollado por [JetBrains](https://jetbrains.com).
Tiene una [sintaxis](/glosario#sintaxis) clara y concisa,
lo que hace que su código sea fácil de leer.

Kotlin se utiliza ampliamente en todo el mundo y su popularidad entre los desarrolladores crece constantemente.
Muchos desarrolladores que utilizan Kotlin señalan que hace que su trabajo sea más rápido y productivo,
ya que escriben sobre un 40% menos de código que en [Java](/glosario#java), para hacer lo mismo. 😀

![Logo Kotlin](/img/logoKotlin.svg)

La sintaxis básica de Kotlin es similar a la de Java, pero tiene numerosas ventajas.
Una de estas características son las funciones de extensión,
que ofrecen a los desarrolladores la capacidad de ampliar la funcionalidad de las clases sin tener que utilizar la herencia.
 Además, Kotlin ofrece [inferencia de tipos](/glosario#inferencia-de-tipos),
lo que permite al compilador determinar el tipo de variable en función del contexto,
lo que simplifica la codificación y reduce la cantidad de errores en programas complejos.

## Breve historia de Kotlin

En julio de 2011, JetBrains presentó el Proyecto Kotlin, un nuevo lenguaje para la plataforma Java,
que había estado en desarrollo durante un año.
El nombre proviene de la isla Kotlin cerca de San Petersburgo, Rusia.
El objetivo principal de este proyecto era proporcionar una alternativa más segura
y concisa a Java en todos los contextos en los que Java se utiliza actualmente.

En 2016, se lanzó la primera versión estable oficial (Kotlin v1.0).
 La comunidad de desarrolladores ya estaba interesada en utilizar este lenguaje, especialmente en Android.

En la conferencia Google I/O 2017, Google anunció un soporte de primera clase para Kotlin en Android.
Chet Haase, uno de los mayores responsables de Android, dijo:

> Entendemos que no todo el mundo está usando Kotlin ahora mismo, pero creemos que llegará ese momento

En este momento, Kotlin se considera un lenguaje de propósito general para muchas plataformas, no solo para Android.
El lenguaje se actualiza con varias versiones al año. La última versión se puede encontrar en el [sitio oficial](https://kotlinlang.org).
Este curso está basado en la versión v2.1,
pero intentaré ir actualizándolo si se producen cambios en el lenguaje en versiones posteriores.

## Una función de Kotlin de muestra

A continuación, se muestra una muestra de un programa simple en el lenguaje de programación Kotlin que imprime `¡Hola, Kotlin!`.

Si conoces otros lenguajes de programación, posiblemente veas cosas en común con ellos.
Pero, por ahora, no necesitas entender cómo funciona este código.

```kotlin
fun main() {
    println("¡Hola, Kotlin!")
}
```

## Plataformas de aplicación para Kotlin: JVM, Android, JS, Nativo

Kotlin se puede utilizar en una variedad de plataformas de aplicaciones,
como JVM (Java Virtual Machine), Android, JavaScript y Native.
Es conocido por su flexibilidad y facilidad de uso cuando se trata de desarrollar software para diferentes plataformas.

Por ejemplo,
los desarrolladores que están familiarizados con Java pueden aprender fácilmente a usar Kotlin en dispositivos Android.
Lo mismo es cierto para los desarrolladores que están familiarizados con JavaScript
y desean desarrollar aplicaciones para la web utilizando Kotlin.

![Destinos de uso de Kotlin](/img/KotlinMultilang.png)

- [JVM](https://docs.oracle.com/javase/specs/jvms/se8/html):
Kotlin es completamente interoperable con Java,
lo que significa que Kotlin funciona muy bien con todo el [código fuente](/glosario#codigo-fuente)
y las bibliotecas de Java existentes.
También permite a las empresas realizar una migración gradual de Java a Kotlin
porque el código Java también puede acceder al código Kotlin.
Al mismo tiempo, los desarrolladores pueden usar Kotlin como el único lenguaje del proyecto,
para ser ejecutado en cualquier dispositivo con soporte JVM.
- [Android](https://www.android.com):
Utilizando el lenguaje Kotlin, puede crear aplicaciones móviles para Android, el sistema operativo más utilizado en el mundo.
- JS:
Kotlin también es compatible con JavaScript,
lo que le permite desarrollar aplicaciones web del lado del cliente y jecutarlas en un navegador.
- [Nativo](https://kotlinlang.org/docs/native-overview.html):
Kotlin/Native es una tecnología para compilar código Kotlin en ejecutables nativos
que se pueden ejecutar en cualquier sistema operativo, como Windows, Linux, iOS y macOS.
- [Multiplataforma](https://kotlinlang.org/docs/multiplatform.html#kotlin-multiplatform-use-cases):
Con Kotlin Multiplatform, puede crear aplicaciones móviles multiplataforma que comparten código
entre proyectos Android e iOS para implementar redes,
almacenamiento de datos y validación de datos, análisis, cálculos y otra lógica de aplicación.

Entre todas estas oportunidades, los programadores modernos prefieren el desarrollo móvil y del lado del servidor,
pero el lenguaje también está ganando popularidad en otras áreas.

## Características: Programación funcional, programación orientada a objetos y más

Kotlin está diseñado como un lenguaje pragmático,
lo que significa que su propósito principal es resolver problemas del mundo real en lugar de cumplir propósitos concretos.

También es importante que Kotlin admita múltiples paradigmas de programación, como programación imperativa,
programación orientada a objetos, programación genérica, programación funcional y más.
Kotlin también ofrece herramientas como funciones anónimas y funciones de orden superior,
que permiten a los desarrolladores crear fácilmente abstracciones sobre el código existente.

Por último, pero no menos importante, Kotlin es un lenguaje compatible con herramientas de desarrollo,
lo que significa que los entornos de desarrollo más populares;
como IntelliJ IDEA, Eclipse y Android Studio; son compatibles con él.

## Conclusión

¡Felicitaciones!

Ya tienes una idea de lo que es Kotlin, origen, diversas aplicaciones y características únicas.
Ahora te estás uniendo a una comunidad global de creadores que dan forma al futuro de la tecnología.

Usa tus nuevos conocimientos para completar este paso inicial de tu emocionante viaje.

[¡Es hora de comprobar lo aprendído!](/lecciones/ejercicio-001)
