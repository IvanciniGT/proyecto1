# Este el el primero proyecto del curso

## Creación de repo:
git init

## Añadir un fichero
git add <nombre_fichero>   # Añadir un fichero
git add *                  # Añadir todos los ficheros del directorio. NO AÑADE OCULTOS
git add .                  # Añadir todos los ficheros del directorio. SI AÑADE OCULTOS
Empezar a controlar el fichero...
Pasar el fichero al área de STAGING


# Que guarda GIT?
Git solo guarda ficheros
NO GUARDA DIRECTORIOS !!!!!!!


# OBJETOS EN GIT:
## Workspace
La carpeta en la que tengo mi proyecto, en la que trabajo
## Staging
Es un fichero que se guarda dentro de la carpeta .git, que va anotando los cambios 
que se van a mandar al REPO desde el área de STAGING
## Repo
La carpeta .git

## Información del estado del proyecto
git status

## Qué es un commit?
Un >>>paquete de cambios<<< que se registra en el repo

## Sacar un fichero del área de STAGING
git rm --cached <NOMBRE_DE_FICHERO>


## Borra el fichero
De donde? De todos los sitios
- del WORKSPACE
- En el staging se le dice que en el proximo paquete de cambios, se elimine el fichero

git rm <NOMBRE_DE_FICHERO>


-----
F1v1 ---> Repo  ----> Mod F1v2 ---->   Repo                       REPO
F2v1 --->  C1                           C2   -----> rm F2v1 --->   C3

                                            ^^^ FOTO :                ^^^ FOTO:
                                                    F1v2                      F1v2  
                                                    F2v1
                                                    
Los commits (paquetes de cambios) se aplican de forma INCREMENTAL
C1:
    Alta F1v1
    Alta F2v1
C2: 
    Mod  F1v2
C3: 
    Elimino F2v1