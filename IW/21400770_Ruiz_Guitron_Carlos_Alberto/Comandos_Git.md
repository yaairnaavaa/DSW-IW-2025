- 20 comandos mas usados

1.
- Comando: Git init
- Descripción: crea un repositorio Git nuevo o reinicia uno existente. Es un paso fundamental en la configuración inicial de un     proyecto.
- Ejemplo de uso: Estoy empezando un nuevo proyecto y quiero que este en git, entonces, al crear la carpeta del proyecto, coloco git init para inicializar el proyecto en git y coloco git init

2.
- Comando: git clone
- Descripción: Crea una copia local de un repositorio remoto.
- Ejemplo de uso: en esta tarea, tuve que clonar este repositorio y coloque en terminal: git clone https://github.comIrving/DSW-IW-2025.git para poder usarlo.

3.
- Comando: git add
- Descripción: Agrega cambios al área de preparación (staging area) para su posterior commit.
- Ejemplo de uso: git add DSW/21400770_Ruiz_Guitron_Carlos_Alberto/Perfil.md para añadir la tarea para su posterior commit.

4.
- Comando: git commit
- Descripción: Guarda los cambios en el repositorio local con un mensaje que describe los cambios.
- Ejemplo de uso: git commit -m "Agregado archivo de configuración" Realiza un commit con el mensaje de descripción de los cambios.

5.
- Comando: git status
- Descripción: Muestra el estado actual del repositorio, incluyendo archivos modificados, archivos en el área de preparación, etc.
- Ejemplo de uso: si coloc git status me dira que me falta agregar Comandos_Git.md porque estara en rojo, pero el Perfil.md estara en verde porque ya hice el git add

6.
- Comando: git push
- Descripción: Sube los cambios locales a un repositorio remoto.
- Ejemplo de uso: si colocara git push origin main se mandaran los cambios de la rama main al repositorio remoto, pero, me falta agregar Comandos_Git.md.

7.
- Comando: git pull
- Descripción: Descarga cambios del repositorio remoto y los fusiona con la rama local.
- Ejemplo de uso: si coloco git pull origin main, me traera los nuevos cambios que hay y los fusionara.

8.
- Comando: git branch
- Descripción: Muestra las ramas disponibles en el repositorio. También se puede usar para crear nuevas ramas.
- Ejemplo de uso: git branch Carlos Creara una nueva rama llamada Carlos o si quiero solo ver las ramas existentes coloco git branch.

9.
- Comando: git checkout
- Descripción: Cambia a una rama específica o restablece archivos a su estado anterior.
- Ejemplo de uso: git checkout Carlos Cambia a la rama Carlos.

10.
- Comando: git merge
- Descripción: Combina los cambios de una rama a otra.
- Ejemplo de uso: git merge Carlos Fusiona los cambios de Carlos en la rama actual main.

11.
- Comando: git remote
- Descripción: Gestiona las conexiones a repositorios remotos.
- Ejemplo de uso: git remote add origin https://github.com/usuario/repo.git Agrega un repositorio remoto con el nombre origin.

12.
- Comando: git log
- Descripción: Muestra el historial de commits del repositorio.
- Ejemplo de uso: si quiero ver los commits que hay pongo git log y mostrara una lista de los commits recientes.

13.
- Comando: git diff
- Descripción: Muestra las diferencias entre los archivos modificados y el último commit.
- Ejemplo de uso: si estoy en un archivo que sufrio cambios coloco git diff para ver las diferencias en los archivos no comprometidos.

14.
- Comando: git reset
- Descripción: Deshace los cambios realizados en el área de preparación o incluso un commit.
- Ejemplo de uso: si alguien se equivoco en un archivo colocamos git reset archivo.txt para deshacer los cambios en archivo.txt del área de preparación.

15.
- Comando: git rm
- Descripción: Elimina archivos del repositorio y del sistema de archivos.
- Ejemplo de uso: si esta mal un archivo podemos eliminarlo con git rm archivo.txt para eliminar archivo.txt tanto del repositorio como del directorio local.

16.
- Comando: git stash
- Descripción: Guarda temporalmente los cambios no comprometidos sin hacer commit.
- Ejemplo de uso: si no se si esta bien mi trabajo coloco git stash Guarda los cambios actuales para poder cambiar de rama sin perder el trabajo en curso.

17.
- Comando: git stash pop
- Descripción: Recupera los cambios guardados con git stash y los aplica al directorio de trabajo.
- Ejemplo de uso: git stash pop para recuperar los cambios guardados previamente con git stash y los aplica.

18.
- Comando: git fetch
- Descripción: Obtiene los cambios del repositorio remoto sin fusionarlos con la rama actual.
- Ejemplo de uso: si quiero saber si sufrio cambios el repositorio coloco git fetch origin para bbtiener los cambios del repositorio remoto origin.

19.
- Comando: git tag
- Descripción: Crea una etiqueta (tag) en un commit específico.
- Ejemplo de uso: git tag v1.0 para crear una etiqueta llamada v1.0 en el commit actual.

20
- Comando: git rebase
- Descripción: Aplica los commits de una rama sobre otra, reescribiendo el historial de la rama.
- Ejemplo de uso: git rebase main Aplica los cambios de la rama actual sobre la rama main.