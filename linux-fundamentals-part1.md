# Linux Fundamentals Part 1 — TryHackMe

## Objetivo

Esta room es para aprender los primeros pasos en Linux.
Nunca había usado Linux antes (bueno casi nada), así que esto fue bastante nuevo para mí.
La idea es aprender a moverte por la terminal y entender por qué Linux es tan importante
en el mundo de la ciberseguridad.

---

## Herramientas y comandos que aprendí

- `echo` → básicamente le dices a la terminal que imprima algo. Como un "hola mundo".
- `whoami` → te dice con qué usuario estás trabajando. Útil cuando no sabes ni dónde estás.
- `ls` → lista lo que hay en la carpeta donde estás. Como ver el contenido de una carpeta en Windows.
- `cd` → para moverte entre carpetas. cd = change directory.
- `cat` → abre y muestra el contenido de un archivo de texto directamente en la terminal.
- `pwd` → te dice exactamente en qué carpeta estás parado en ese momento.
- `find` → busca archivos dentro del sistema. Esto me costó un poco al principio.
- `grep` → busca palabras o texto dentro de archivos. Muy útil cuando el archivo es largo.
- `>` → guarda lo que imprime un comando en un archivo (lo crea o lo sobreescribe).
- `>>` → igual pero en vez de borrar lo que había, agrega al final.
- `&&` → encadena dos comandos, el segundo solo corre si el primero funcionó bien.
- `|` → pasa el resultado de un comando al siguiente. Esto se llama "pipe" y al principio me confundió bastante.

---

## Cómo fui resolviendo cada task

**Task 1 — Introduction**
Esta task no tiene preguntas, solo es leer la intro de la room. Básicamente te explica
de qué va todo y te da contexto. Yo la leí rápido porque quería llegar a la parte
donde puedo escribir comandos jaja.

**Task 2 — A Bit of Background on Linux**
Aquí aprendí un poco de historia de Linux, de dónde vino y por qué hay tantas versiones distintas
(Ubuntu, Kali, etc.). La pregunta fue sobre el año en que salió la primera versión del sistema.
Tuve que leer con atención porque no sabía nada de esto.

**Task 3 — Interacting With Your First Linux Machine (In-Browser)**
Esto estuvo buenísimo porque puedes usar una terminal directamente en el navegador,
sin instalar nada. La primera vez que vi la pantalla negra con el cursor parpadeando
no supe ni qué hacer jaja. Pero bueno, hay que empezar por algún lado.

**Task 4 — Running Your First few Commands**
Aquí escribí mis primeros comandos de verdad: echo y whoami. Se siente raro al principio
escribir algo y que la terminal te responda, pero también es emocionante. La pregunta
era sobre el output de uno de esos comandos al correrlo en la máquina.

**Task 5 — Interacting With the Filesystem!**
Esta fue la task que más me gustó. Aprendí a navegar carpetas con cd, ver qué hay
con ls y leer archivos con cat. Fue como explorar un sistema de archivos pero
sin interfaz gráfica. Hubo una pregunta donde tenía que buscar el contenido de un archivo
específico, y para eso usé cat después de navegar hasta la carpeta correcta.

**Task 6 — Searching for Files**
Aquí me costó más. El comando find tiene muchas opciones y al principio no entendía
bien la sintaxis. Tuve que releer la explicación varias veces. grep también lo usé
para buscar texto dentro de archivos. Las preguntas pedían encontrar archivos escondidos
en el sistema, así que fue como un mini juego de exploración.

**Task 7 — An Introduction to Shell Operators**
Los operadores me volaron la cabeza un poco. Lo del pipe (|) especialmente, porque
no entendía bien cómo un comando le "pasa" info a otro. Pero con los ejemplos de la room
lo fui entendiendo de a poco. Creo que esto lo voy a entender mejor con la práctica.

**Task 8 — Conclusions & Summaries**
Solo un resumen de todo lo que se vio. Nada técnico, solo para cerrar la room.
Me sirvió para repasar mentalmente lo que había aprendido.

---

## Lecciones aprendidas

1. La terminal da miedo al principio pero en realidad los comandos básicos son pocos
   y bastante lógicos. ls lista, cd mueve, cat muestra. No es tan caótico como pensaba.

2. find y grep son más poderosos de lo que parecen. Todavía no los domino,
   pero entendí para qué sirven y eso ya es algo.

3. Los operadores como pipe y && son los que hacen que la terminal sea realmente útil,
   pero también son los que más cuesta entender al principio. Paciencia.

---

## Próximos pasos

- Seguir con Linux Fundamentals Part 2.
- Practicar los comandos en mi propia máquina para no depender solo del entorno de TryHackMe.
- Entender mejor cómo funciona find con diferentes opciones porque todavía lo uso
  a medias nomás.
