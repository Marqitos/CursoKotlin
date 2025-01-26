---
layout: playground
title: Literales básicos: Números, cadenas de texto y caractéres
description: Teoría - Literales básicos: Números, cadenas de texto y caractéres
---

# Literales básicos: Números, cadenas de texto y caractéres

Independientemente de su complejidad, todos los programas realizan esencialmente operaciones con números, cadenas y otros valores. Estos valores se denominan literales, es decir, en el sentido o significado más básico del símbolo. 

Antes de comenzar a escribir nuestros primeros programas, aprendamos los literales básicos en Kotlin: números ( enteros y con decimales), caracteres y cadenas. Puedes encontrar estos literales en todas partes en la vida cotidiana.

## Números

### Números enteros

Usamos números enteros para contar cosas en el mundo real. También usaremos a menudo números enteros en Kotlin.

A continuación se muestran varios ejemplos de literales de números enteros válidos separados por comas: `0`, `1`, `2`, `10`, `11`, `100`.

Si un valor entero contiene muchos dígitos, podemos agregar guiones bajos para dividir los dígitos en bloques y hacer que este número sea más legible: por ejemplo, `1_000_000` es mucho más fácil de leer que `1000000`.

Puede agregar tantos guiones bajos como desee: `1__000_000`, `1_2_3`. Pero, recuerde que los guiones bajos no pueden aparecer al principio ni al final del número. Si escribe `_10` o `100_`, obtendrá un error.

### Números con decimales

Además de contar cosas simples, podemos necesitar números con decimales, que se almacenan como otro tipo de dato diferente. Y se comporta de forma diferente en cierto tipo de operaciones.

Pero es muy común en el mundo real, como para representar dinero. O cuentas más especificas, como el area de un círculo, donde necesita el número π.

Para ello escribir utilizando `.` como separador decimal, por ejemplo `3.1415926`.

## Caracteres

Un solo carácter puede representar un dígito, una letra u otro símbolo. Para escribir un solo carácter, envolvemos un símbolo entre comillas simples de la siguiente manera: `'A'`, `'B'`, `'C'`, `'x'`, `'y'`, `'z'`, `'0'`, `'1'`, `'2'`, `'9'`. Los literales de caracteres pueden representar letras del alfabeto, dígitos del `'0'` al `'9'`, espacios en blanco (`' '`) o algunos otros símbolos (por ejemplo, `'$'`).

No confunda los caracteres que representan números (por ejemplo, `'9'`) con los números en sí mismos (por ejemplo, `9`), ya que se tratan de tipos de datos diferentes.

Un carácter no puede incluir dos o más dígitos o letras porque representa un solo símbolo. Los dos ejemplos siguientes son incorrectos: `'abc'`, `'543'` porque estos literales tienen demasiados caracteres.

## Cadenas de texto

Las cadenas de texto representan cualquier texto, como el texto de un anuncio, la dirección de una página web o el inicio de sesión de un sitio web. Una cadena de texto es una secuencia de caracteres individuales.

Para escribir cadenas, envolvemos caracteres entre comillas dobles en lugar de comillas simples. Aquí hay algunos ejemplos válidos: `"texto"`, `"Quiero aprender Kotlin"`, `"123456"`, `"e-mail@gmail.com"`. Por lo tanto, las cadenas pueden incluir letras, dígitos, espacios en blanco y otros caracteres.

Una cadena también puede contener un solo carácter, como `"A"`. No lo confundas con el carácter `'A'`, que no es una cadena.

## Conclusión

En la codificación diaria, dependes en gran medida de literales. A menudo, usarás números enteros como `123` para contar o medir, caracteres como `'A'` o `'1'` para símbolos individuales y cadenas como `"ABC"` para manejar texto. La eficiencia es clave en la programación. Cuando el uso de la memoria sea una preocupación, opta por un carácter como `'A'` en lugar de una cadena como `"A"`, ya que los caracteres suelen utilizar menos memoria.

Esto es solo el comienzo. Kotlin ofrece una amplia gama de otros literales para que explores en los próximos temas.

¡Así que practiquemos para dominar estos tres básicos!
