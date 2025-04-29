1.- git init
    Inicializa un nuevo repositorio Git en la carpeta actual.
 Ejemplo: git init

2.- git clone
    Crea una copia local de un repositorio remoto.
 Ejemplo: git clone https://github.com/yaairnaavaa/DSW-IW-2025 

3.- git config --global user.name " Nombre "
    Establece tu nombre de usuario para los commits.
 Ejemplo: git config --global user.name LAGL99

4.- git config --global user.email " email "
    Establece tu dirección de correo electrónico para los commits. 
 Ejemplo: git config --global user.email "luangomezlo@ittepic.edu.mx"

5.- git add archivo
    Añade un archivo a la lista de cambios a confirmar.
 Ejemplo: git add Perfil.md

6.- git add .
    Añade todos los archivos modificados en el directorio actual al área de staging.
Ejemplo: git add . 

7.- git commit -m "Mensaje"
    Guarda los cambios en el área de staging con un mensaje descriptivo.
 Ejemplo: git commit -m "Carpeta Gomez Lopez"

8.-git diff 
    Muestra las diferencias entre el directorio de trabajo y el área de staging.
 Ejemplo: git diff  MAIN BRANCH

9.- git remote add nombre url
    Añade un nuevo repositorio remoto. 
 Ejemplo: git remote add IW https://github.com/LAGL99

10.- git remote -v
    Muestra las URLs de los repositorios remotos. 
 Ejemplo: git remote -v 
    origin  https://github.com/yaairnaavaa/DSW-IW-2025 (fetch)
    origin  https://github.com/yaairnaavaa/DSW-IW-2025 (push)     

11.- git push nombre rama
    Envía los cambios a un repositorio remoto. 
Ejemplo: origin main

12.- git pull nombre rama
    Obtiene y fusiona los cambios de un repositorio remoto. 
Ejemplo: gut pull origin main

13.- git fetch nombre 
    Descarga los cambios de un repositorio remoto sin fusionarlos. 
Ejemplo: git fetch main 

14.- git branch
    Muestra las ramas disponibles.
Ejemplo: git branch
        main
15.- git branch nombre_de_rama
    Crea una nueva rama.
Ejemplo: git branch Antonio

16.- git checkout nombre_de_rama
    Cambia a una rama existente.
Ejemplo: git checkout Antonio

17.- git checkout -b nombre_de_rama
    Crea y cambia a una nueva rama.
Ejemplo: git checkout Antonio2

18.- git merge nombre_de_rama
    Fusiona una rama con la rama actual.
Ejemplo: git merge main

19.- git branch -d nombre_de_rama
    Borra una rama.
Ejemplo: git branch -d Antonio2

20.- git rebase nombre_de_rama
    Reimplanta los cambios de la rama actual sobre una rama especificada. 
Ejemplo: git rebase Antonio main 