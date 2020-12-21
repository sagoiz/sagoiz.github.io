---
layout: post
title:  "Acerca del mundo No-SQL"
date: 2020-12-21 10:45:00 +0300
tags: [blog, No-SQL, MongoDB]
author: Serafin
---

# Algunos comentarios y reflexiones sobre No-SQL

Hablando el otro día sobre desarrollo en JavaScript, bases de datos relacionales y no relacionales surgió el tema de las diferencias a la hora de cómo organizar los datos.

Cómo crear las tablas, o colecciones o lo que sea que vayamos a utilizar para la aplicación.
En el mundo SQL el tema suele tratar siempre de crear tablas, campos, relaciones entre las diferentes tablas, campos únicos, etc.

Todo esto en el mundo No-SQL cambia un poco, *o mucho*.

Primero, las estructuras SQL son ajenas al mundo JavaScript, mientras que **en No-SQL todo son objetos tipo JSON.**

En No-SQL podemos adaptar (y de hecho debemos) el formato de los datos para que sea lo mas cercano posible a la aplicación, a cómo va a utilizar la aplicación los datos.

En cierto modo hay una forma tipo SQL de organizar datos en No-SQL, de manera que podemos crear diferentes colecciones, enlazar unas con otras, crear relaciones entre documentos, etc.

Pero de esta manera estamos perdiendo el verdadero poder del mundo No-SQL.

Para empezar de manera suave y progresiva, tenemos que imaginar que solamente vamos a tener una sola colección y que todos los datos van a estar dentro de los documentos, en forma de objetos y arrays de objetos.

