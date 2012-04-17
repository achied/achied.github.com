---
layout: post
title: "Migrando de Blogger a Octopress"
date: 2012-04-17 09:00
comments: true
categories: [blog, ruby, jekyll, octopress, blogger]
---

## Un poco de historia

Hace tiempo emprendí la aventura de escribir un blog, más como pasatiempo y
forma de diversión que como tarea seria. Como resultado... pocas y
desorganizadas entradas.

La cosa empezó con [blogger](http://www.blogger.com/) y poco a poco la
dependencia de tener que tener un cliente específico o tener que estar editando
online hacían que cada vez me costara más. Probé a usar
[scribefire](http://www.scribefire.com/) pero tampoco tuve mucho éxito.

Como siempre, la falta de tiempo y la necesidad de tener una forma más rápida y sencilla de crear los
post, poder revisarlos, poder insertar trozos de cógio fácilmente... eran las
excusas que ivan sumando para abandonar la tarea que había empezado.

Estos días atrás oí hablar de [jekyll](https://github.com/mojombo/jekyll) y
[jekyllbootstrap](http://jekyllbootstrap.com/) pero no terminaba de animarme ni
de obtener un resultado que me convenciera a la primera.

Pero he encontrado el proyecto [octopress](http://octopress.org/), un
framework para [jekyll](https://github.com/mojombo/jekyll) que simplifica la
necesidad de tener que crear tus propios HTML y CSS.

La página del proyecto muestra una documentación sencilla y clara de [cómo
instalar y personalizar el blog](http://octopress.org/help/)

## ¿Y por qué cambiar?

Si escribo poco y apenas le dedico tiempo... ¿por qué cambiar? Básicamente por
tres razones:

<!-- more -->

1. Seguir aprendiendo ruby
2. Seguir aprendiendo Git
3. Seguir divirtiéndome

Existen otra serie de factores que me han animado al cambio.

## Más útil para un desarrollador

La sintáxis de código es más sencilla y automática, con múltiples opciones y
recursos. Desde la inclusión en línea del código,

``` ruby sample
def sample
  puts "Hello World!!!"
end
```

hasta la posibilidad de hacerlo disponible bajo descarga

{% include_code hello_world.rb %}

## Edición del post fácil y cómoda

Con cualquier editor, de forma sencilla, en [markdown](http://daringfireball.net/projects/markdown/syntax)

```
## Edición del post fácil y cómoda

Con cualquier editor, de forma sencilla, en [markdown](http://daringfireball.net/projects/markdown/syntax)
```

## Previsualización del blog offline

Tan sencillo como

```
bundle exec rake generate
bundle exec rake preview
```

y tendré en mi máquina local la versión completa de mi blog.

## Integrado con las páginas y repositorios de github

Al tener el blog dentro del repositorio de [github](https://github.com/) puedo
enlazar las páginas de los proyectos y llevar el control de versiones de todos
los post.

¿Esto hará que escriba más post? No lo sé, pero he pasado un rato divertido y...
he aprendido mucho.
