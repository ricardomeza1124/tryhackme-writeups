# Linux Fundamentals Part 2 — TryHackMe

## Objetivo

Seguir aprendiendo Linux, pero ya un poco más en serio.
En esta parte aprendí a conectarme a una máquina remota por SSH, a usar flags y switches
en los comandos, a interactuar más con el sistema de archivos y a entender los permisos.
También vi cuáles son los directorios más importantes del sistema.

---

## Herramientas y comandos que aprendí

- SSH → no es exactamente un comando de Linux, es un protocolo para conectarte a otra máquina de forma remota. Lo usé por primera vez acá y me pareció bastante cool.
- flags y switches (por ej. -l, -a, -h) → son opciones que le agregas a un comando para cambiar cómo funciona. Tipo ls -la te da más info que solo ls.
- touch → crea un archivo vacío. Útil para crear archivos rápido sin abrirlos.
- mkdir → crea una carpeta nueva.
- cp → copia un archivo de un lugar a otro.
- mv → mueve o renombra un archivo.
- rm → borra un archivo. Hay que usarlo con cuidado porque no hay papelera.
- file → te dice qué tipo de archivo es, incluso si no tiene extensión.
- chmod → cambia los permisos de un archivo (quién puede leer, escribir o ejecutarlo).
- su → te permite cambiar de usuario dentro de la terminal.
- ls -la → lista todos los archivos incluyendo los ocultos, con detalles de permisos y dueño.

---

## Cómo fui resolviendo cada task

**Task 1 — Introduction**
La intro de la room, sin preguntas. Solo explica que esta parte va a ser más práctica
y que se va a usar SSH para conectarse a la máquina en lugar del navegador como antes.

**Task 2 — Accessing Your Linux Machine Using SSH**
Aquí aprendí qué es SSH y cómo conectarme a una máquina remota con un comando en la terminal.
Al principio no entendía bien por qué era necesario conectarse "de afuera", pero tiene sentido
cuando piensas en servidores reales. Tuve que usar el comando con usuario, IP y contraseña.
Fue la primera vez que me conecté a algo remoto desde una terminal y se sintió bastante pro jaja.

**Task 3 — Introduction to Flags and Switches**
Esto me aclaró algo que me había confundido en la parte 1: por qué los comandos a veces
tienen guiones y letras después. Resulta que eso son flags o switches que modifican
cómo funciona el comando. Aprendí a usar --help para ver qué opciones tiene cada comando,
lo cual es muy útil cuando no sabes qué hace cada flag.

**Task 4 — Filesystem Interaction Continued**
Acá ya empezamos a hacer cosas más concretas con archivos: crearlos con touch,
hacer carpetas con mkdir, copiarlos con cp, moverlos con mv y borrarlos con rm.
También aprendí el comando file para identificar qué tipo de archivo es algo.
Las preguntas pedían ejecutar estos comandos en la máquina y ver los resultados.

**Task 5 — Permissions 101**
Esta fue la task más difícil para mí. Los permisos en Linux son distintos a Windows
y al principio los números y letras (rwx, 777, etc.) me confundieron bastante.
Pero básicamente es un sistema para controlar quién puede leer, escribir o ejecutar
cada archivo. Aprendí a ver los permisos con ls -la y a cambiarlos con chmod.
También usé su para cambiar de usuario y comprobar qué podía hacer cada uno.

**Task 6 — Common Directories**
Acá aprendí cuáles son las carpetas más importantes de Linux y para qué sirve cada una:
/etc, /var, /tmp, /root, /home... Esto me ayudó a entender mejor la estructura del sistema
porque antes no sabía por qué había tantas carpetas con nombres raros en la raíz.

**Task 7 — Conclusions and Summaries**
Resumen de todo lo visto. Sin preguntas técnicas, solo para cerrar la room.
Me quedé con la idea de que Linux tiene una lógica muy clara si empezás a entender
la estructura base del sistema.

---

## Lecciones aprendidas

1. SSH es fundamental en ciberseguridad. Casi todo en este mundo pasa por conexiones
   remotas y SSH es la herramienta estándar para eso. Ya no me parece magia jaja.

2. Los permisos de Linux son poderosos pero al principio son confusos. Entendí la lógica
   general (lectura, escritura, ejecución para usuario, grupo y otros) pero voy a necesitar
   practicar más para dominarlo.

3. Saber los directorios principales del sistema es clave. En CTFs y en pentesting
   en general siempre se anda buscando cosas en /etc, /var/log, /tmp, etc.
   Ya sé para qué sirve cada uno básicamente.

---

## Próximos pasos

- Seguir con Linux Fundamentals Part 3.
- Practicar más chmod y permisos porque todavía me cuesta leerlos de un vistazo.
- Intentar conectarme por SSH a una VM propia para practicar fuera de TryHackMe.
