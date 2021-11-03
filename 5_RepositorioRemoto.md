---   
title: Ejercicios de repositorios remotos
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
1. Crear un nuevo repositorio público en GitHub con el nombre libro-git.
        
    ~~~
       
    ~~~

2. Añadirlo al repositorio local del libro
       
    
        git remote add github "https://github.com/JonathanGranell/libro-git.git"
       

3. Mostrar todos los repositorios remotos configurados.       
        
         git remote -v
        
    
# Ejercicio 2
    
1. Añadir los cambios del repositorio local al repositorio remoto de GitHub
       
       git push https://github.com/JonathanGranell/libro-git.git master
       
        

        
2. Acceder a GitHub y comprobar que se han subido los cambios mostrando el historial de versiones.
        
        
        
    
# Ejercicio 3
    
1. Colaborar en el repositorio remoto libro-git de otro usuario.
        
        git checkout master
        git merge bibliografia
        
        
2. Clonar su repositorio libro-git.
        
        git clone https://github.com/4tomyc/libro-git.git
        
        
3. Añadir el fichero autores.txt  que   contenga el nombre del usuario y su correo
electrónico.
        
        nano autores.txt
        
        
4. Añadir los cambios a la zona de intercambio temporal.
        
        git add .
        
        
5. Hacer un commit con el mensaje “Añadido autor.

        git commit -m "Añadido autores.txt"

6. Subir los cambios al repositorio remoto.

        https://github.com/JonathanGranell/libro-git.git

   
# Ejercicio 4 
    
1. Desde vuestra cuenta de GitHub realizad un «Fork» del repositorio https://github.com/mcuevaseljust/guiaApunts.git.
        
        Esta añadido en mi repositorio cuando le mande mi enlace al profesor el lo podrá ver
        
        
2. Modificad el fichero README.md, añadiendo vuestro nombre en la tabla.        
        Nombre añadido a la tabla
        
        
3. Haced un «Pull request» para contribuir en el repositorio de «mcuevaseljust» podéis dejar un comentario.
        
       Pull rquest creado que vera el profesor mcuevas en su usuario
        