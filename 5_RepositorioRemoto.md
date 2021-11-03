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
       
       git push -u github master 
       
        

        
2. Acceder a GitHub y comprobar que se han subido los cambios mostrando el historial de versiones.
        
        
        
    
# Ejercicio 3
    
1. Colaborar en el repositorio remoto libro-git de otro usuario.
        
        git checkout master
        git merge bibliografia
        
        
2. Clonar su repositorio libro-git.
        
        git log --graph --all --oneline
        
        
3. Añadir el fichero autores.txt  que   contenga el nombre del usuario y su correo
electrónico.
        
        git branch -d bibliografia
        
        
4. Añadir los cambios a la zona de intercambio temporal.
        
        git log --graph --all --oneline
        
        
5. Hacer un commit con el mensaje “Añadido autor.



6. Subir los cambios al repositorio remoto.



   
# Ejercicio 4 
    
1. Desde vuestra cuenta de GitHub realizad un «Fork» del repositorio https://github.com/mcuevaseljust/guiaApunts.git.
        
        git branch bibliografia
        
        
2. Modificad el fichero README.md, añadiendo vuestro nombre en la tabla.        
        git checkout bibliografia
        
        
3. Haced un «Pull request» para contribuir en el repositorio de «mcuevaseljust» podéis dejar un comentario.
        
        nano bibliografia.txt
                Scott Chacon and Ben Sarub. Pro Git. Apress Ryan Hodson. Ry's Git Tutorial. Smashwords (2014)

        