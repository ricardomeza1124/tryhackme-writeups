# Linux Fundamentals Part 3 — TryHackMe

## Objetivo

La tercera y última parte de la serie de Linux en TryHackMe.
Acá ya se pone más técnico: editores de texto en la terminal, utilidades del sistema,
cómo funcionan los procesos, automatización de tareas, gestión de paquetes y logs.
Básicamente aprender a "mantener" un sistema Linux además de solo usarlo.

---

## Herramientas y comandos que aprendí

- nano → editor de texto que funciona directamente en la terminal. Mucho más fácil que vim para empezar.
- vim → otro editor de texto en terminal, más potente pero más difícil. Lo vi por encima nomás.
- wget → descarga archivos desde internet directamente en la terminal, sin navegador.
- scp → copia archivos entre máquinas de forma segura usando SSH. Útil para mover archivos a/desde una máquina remota.
- python3 -m http.server → levanta un servidor web simple desde cualquier carpeta. Lo usé para transferir archivos.
- ps → muestra los procesos que están corriendo en el sistema en ese momento.
- top → como el administrador de tareas de Windows pero en la terminal. Muestra procesos en tiempo real.
- kill → termina un proceso usando su ID (PID).
- systemctl → controla servicios del sistema (iniciarlos, pararlos, ver su estado).
- crontab → programa tareas para que se ejecuten automáticamente en horarios específicos.
- apt → el gestor de paquetes de Ubuntu/Debian para instalar o eliminar programas.
- ls /var/log → directorio donde Linux guarda los archivos de log del sistema.

---

## Cómo fui resolviendo cada task

**Task 1 — Introduction**
La intro de siempre. Sin preguntas. Esta parte promete ser la más completa de las tres
y con solo leer el índice ya me di cuenta que iba a aprender cosas más "reales" del sistema.

**Task 2 — Deploy Your Linux Machine**
Igual que en la parte 2, hay que conectarse por SSH a la máquina desplegada.
Ya me salió sin problemas porque lo practiqué en la parte anterior. Pequeña victoria jaja.

**Task 3 — Terminal Text Editors**
Aprendí a usar nano para editar archivos de texto directamente en la terminal.
Crear un archivo, escribir, guardarlo con Ctrl+O y salir con Ctrl+X. También vi vim
pero es bastante más complicado, tiene modos distintos y al principio no sabes ni cómo salir.
Las preguntas pedían crear y editar archivos con estos editores.

**Task 4 — General/Useful Utilities**
Esta task estuvo muy buena. Aprendí a descargar cosas con wget solo poniendo una URL,
y a copiar archivos entre máquinas con scp. También vi cómo levantar un servidor HTTP
rápido con Python, que sirve para pasar archivos de una máquina a otra. Eso se usa
bastante en CTFs y en pentesting según entendí.

**Task 5 — Processes 101**
Los procesos me parecieron interesantes. Cada programa que corre en Linux es un proceso
con un número de identificación (PID). Con ps y top podés verlos, y con kill podés
terminarlos. También aprendí sobre servicios del sistema y cómo controlarlos con systemctl.
Las preguntas pedían encontrar PIDs específicos y trabajar con procesos en la máquina.

**Task 6 — Maintaining Your System: Automation**
Acá aprendí sobre crontab, que es básicamente un sistema para programar tareas.
Podés decirle al sistema "ejecutá este script todos los días a las 3am" y lo hace solo.
La sintaxis del crontab al principio parece un jeroglífico (esos cinco asteriscos),
pero con la explicación de la room lo entendí más o menos.

**Task 7 — Maintaining Your System: Package Management**
Aprendí cómo se instalan programas en Linux con apt. Es como una tienda de aplicaciones
pero desde la terminal. También vi cómo funcionan los repositorios, que son básicamente
las fuentes desde donde se descargan los paquetes. Fue interesante compararlo con
instalar cosas en Windows donde siempre buscás el .exe en internet.

**Task 8 — Maintaining Your System: Logs**
Los logs son archivos donde el sistema registra todo lo que pasa. Están en /var/log
y sirven para saber qué pasó en el sistema, detectar errores o ver actividad sospechosa.
En ciberseguridad esto es clave porque los logs son evidencia. Las preguntas pedían
leer distintos archivos de log y encontrar información dentro de ellos.

**Task 9 — Conclusions & Summaries**
El cierre de toda la serie de Linux Fundamentals. Repaso general, sin preguntas técnicas.
Se siente bien haber llegado hasta acá desde cero.

---

## Lecciones aprendidas

1. nano es tu amigo al principio. No hace falta aprender vim de entrada, con nano
   podés hacer todo lo básico sin volverte loco intentando salir del editor jaja.

2. Los procesos, servicios y crontab son la base de entender cómo "vive" un sistema Linux.
   No es solo archivos y carpetas, hay cosas corriendo todo el tiempo en el fondo.

3. Los logs son oro en ciberseguridad. Saber leerlos y saber dónde están es
   algo que voy a usar mucho más adelante, tanto en defensa como en análisis forense.

---

## Próximos pasos

- Explorar más a fondo vim porque sé que en el mundo real lo voy a necesitar.
- Practicar crontab con ejemplos reales en una VM propia.
- Empezar a ver rooms más avanzadas ahora que ya tengo la base de Linux.
- Repasar permisos, procesos y logs porque son temas que van a aparecer siempre.
