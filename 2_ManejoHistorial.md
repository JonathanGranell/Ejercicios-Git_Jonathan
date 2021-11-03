---   
title: EJERCICIOS DE MANEJO DEL HISTORIAL DE CAMBIOS
titlepage: true
titlepage-rule-height: 0
titlepage-rule-color: 653097
toc-own-page: true
toc-title: Contenidos
header-left: EDD
header-right: GIT
lang: es-ES
footer-left: IES Jaume II el Just
footer-right: \thepage
titlepage-background: ./GIT.png
---
# Ejercicio 1

1. Mostrar el historial de cambios del repositorio.
~~~
    git log
~~~

2. Crear   la   carpeta  capitulos  y   crear   dentro   de   ella   el   fichero  capitulo1.txt  con   el
siguiente texto:
~~~
    mkdir capitulos
    nano capitulos/capitulo1.txt
    Git es un sistema de control de versiones ideado por Linus Torvalds.
~~~

4. Añadir los cambios a la zona de intercambio temporal.
~~~
    git add .
~~~

5. Hacer un commit de los cambios con el mensaje “Añadido capítulo 1.”
~~~    
    git commit -m "Añadidio capítulo 1."
~~~

6. Volver a mostrar el historial de cambios del repositorio.
~~~
    git log
    git show
~~~

# Ejercicio 2

1. Crear el fichero capitulo2.txt en la carpeta capitulos con el siguiente texto.
~~~
    nano capitulos/capitulo2.txt
    El flujo de trabajo básico con Git consiste en: 1-Hacer cambios en el repositorio. 2-Añadir los cambios a la xona de intercambio temporal. 3-Hacer un commit de los cambios.
~~~

2. Añadir los cambios a la zona de intercambio temporal.
~~~
    git add .
~~~

3. Hacer un commit de los cambios con el mensaje “Añadido capítulo 2.”
~~~
    git commit -m "Añadido capítulo 2."
~~~

4. Mostrar las diferencias entre la última versión y dos versiones anteriores.
~~~
    git diff HEAD~2..HEAD
~~~

# Ejercicio 3

1. Crear el fichero capitulo3.txt en la carpeta capitulos con el siguiente texto.
~~~
    nano capitulos/capitulo3.txt
    Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.
~~~

2. Añadir los cambios a la zona de intercambio temporal.
~~~
    git add .
~~~

3. Hacer un commit de los cambios con el mensaje “Añadido capítulo 3.”
~~~
    git commit -m "Añadido capítulo 3."
~~~

4. Mostrar las diferencias entre la primera y la última versión del repositorio.
~~~
    git diff HEAD~1..HEAD
~~~

# Ejercicio 4

1. Añadir al final del fichero indice.txt la siguiente línea:
IES JAUME II EL JUST - EDD Página 1 de 2
EJERCICIOS GIT Curso 2021-2022
~~~
    nano indice.txt
        Capítulo 5: Conceptos avanzados
~~~
1. Añadir los cambios a la zona de intercambio temporal.
~~~
    git add .
~~~
3. Hacer un commit de los cambios con el mensaje “Añadido capítulo 5 al índice.”
~~~
     git commit -m "Añadido capítulo 5 al índice."
~~~

4. Mostrar quién ha hecho cambios sobre el fichero indice.txt.
~~~
    git annotate indice.txt
~~~