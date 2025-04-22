1. git init

        Descripción: Inicializa un nuevo repositorio Git en el directorio actual, creando una estructura de archivos oculta que Git usa para gestionar versiones.

        Ejemplo de uso:

        Imagina que estás comenzando un nuevo proyecto y quieres usar Git para gestionarlo. Abres la terminal, navegas a la carpeta del proyecto y ejecutas el siguiente comando:
        git init

        Esto crea una carpeta oculta llamada .git dentro del directorio actual, convirtiéndolo en un repositorio Git. A partir de aquí, puedes empezar a realizar seguimiento de tus cambios.

2. git clone

        Descripción: Clona un repositorio remoto (por ejemplo, desde GitHub) a tu máquina local, creando una copia exacta del proyecto.

        Ejemplo de uso:

        Si encuentras un repositorio en GitHub que te interesa y quieres trabajar en él en tu máquina local, usas el comando git clone. Por ejemplo:
        git clone https://github.com/usuario/mi-proyecto.git

        Este comando descargará todo el contenido del repositorio remoto y lo almacenará en una nueva carpeta llamada mi-proyecto en tu computadora.

3. git status

        Descripción: Muestra el estado de los archivos en tu repositorio, indicando si están modificados, no rastreados, listos para ser confirmados, etc.

        Ejemplo de uso:

        Has realizado cambios en varios archivos, pero no sabes si ya los agregaste para confirmar. Para averiguarlo, ejecutas:
        git status

        El resultado te dirá qué archivos están modificados, cuáles están preparados para el commit y cuáles no han sido agregados aún al área de staging.

4. git add

        Descripción: Agrega archivos al área de staging, lo que indica que estos archivos están listos para ser confirmados (committed).

        Ejemplo de uso:

        Después de hacer cambios en el archivo index.html y style.css, decides que estos cambios están listos para ser confirmados. Ejecutas:
        git add index.html style.css

        Esto moverá esos archivos al área de staging. Ahora puedes confirmar esos cambios con git commit.

5. git commit -m

        Descripción: Guarda los cambios en el repositorio con un mensaje descriptivo sobre lo que se ha hecho.

        Ejemplo de uso:

        Después de haber agregado los archivos al área de staging, confirmas los cambios con un mensaje. Por ejemplo:
        git commit -m "Agrega nueva funcionalidad de búsqueda"

        Esto registra los cambios de los archivos que agregaste a la zona de staging, y el mensaje te ayuda a identificar ese commit en el futuro.

6. git log

        Descripción: Muestra un historial de todos los commits realizados en el repositorio, incluyendo la fecha, el autor y el mensaje del commit.

        Ejemplo de uso:

        Quieres revisar los cambios previos realizados en el proyecto. Ejecutas el siguiente comando para ver el historial:
        git log

        Esto te mostrará una lista de commits con detalles como el autor, la fecha y el mensaje. Por ejemplo:

        commit a3c5e89  
        Author: Jorge Ismael <correo@ejemplo.com>  
        Date: Tue Apr 10 10:00 2025  
        Mensaje: Agrega nueva funcionalidad de búsqueda

7. git diff

        Descripción: Muestra las diferencias entre la versión actual del archivo y la versión más reciente confirmada en el repositorio.

        Ejemplo de uso:

        Has hecho modificaciones en el archivo app.js pero no estás seguro de qué exactamente has cambiado. Para ver las diferencias con la última versión confirmada, ejecutas:
        git diff app.js

        Este comando te mostrará las líneas que has agregado o eliminado en el archivo, para que puedas revisarlas antes de confirmar los cambios.

8. git branch

        Descripción: Muestra las ramas existentes en tu repositorio o permite crear una nueva rama para trabajar en una nueva característica sin afectar la rama principal.

        Ejemplo de uso:

        Si quieres trabajar en una nueva funcionalidad sin modificar la rama principal (main), primero creas una nueva rama. Ejecutas:
        git branch nueva-funcionalidad

        Esto crea una rama llamada nueva-funcionalidad, que ahora puedes usar para hacer cambios sin afectar el código principal.

9. git checkout

        Descripción: Cambia de una rama a otra, o restaura archivos específicos a su última versión confirmada.

        Ejemplo de uso:

        Después de haber creado la rama nueva-funcionalidad, decides cambiarte a esa rama para comenzar a trabajar en ella. Ejecutas:
        git checkout nueva-funcionalidad

        Ahora estás en la rama nueva-funcionalidad, y puedes comenzar a hacer cambios sin afectar la rama principal.

10. git merge

        Descripción: Fusiona los cambios de una rama específica con la rama actual.

        Ejemplo de uso:

        Después de terminar de trabajar en la rama nueva-funcionalidad, quieres unir esos cambios a la rama main. Estando en la rama main, ejecutas:
        git merge nueva-funcionalidad

        Esto incorpora todos los cambios realizados en nueva-funcionalidad a la rama main.

11. git pull

        Descripción: Descarga los últimos cambios del repositorio remoto y los fusiona con tu rama local.

        Ejemplo de uso:

        Quieres asegurarte de tener la versión más reciente del repositorio remoto antes de continuar trabajando. Ejecutas:
        git pull origin main

        Este comando descargará cualquier cambio nuevo desde el repositorio remoto (origin) y lo fusionará con tu rama local main.

12. git push

        Descripción: Sube los cambios confirmados (commits) en tu repositorio local al repositorio remoto.

        Ejemplo de uso:

        Después de confirmar tus cambios localmente, deseas que estos se reflejen en el repositorio remoto (por ejemplo, en GitHub). Ejecutas:
        git push origin main

        Esto sube los cambios de tu rama main al repositorio remoto.

13. git remote -v

        Descripción: Muestra las URL de los repositorios remotos configurados en tu repositorio local.

        Ejemplo de uso:

        Si quieres ver qué repositorios remotos están configurados para tu repositorio local, ejecutas:
        git remote -v

        Esto mostrará una lista de los repositorios remotos, como:

        origin https://github.com/usuario/mi-proyecto.git (fetch)
        origin https://github.com/usuario/mi-proyecto.git (push)

14. git reset --hard

        Descripción: Restaura el repositorio a un estado anterior, eliminando los cambios no confirmados.

        Ejemplo de uso:

        Si cometiste un error y quieres volver a un commit anterior, puedes ejecutar:
        git reset --hard HEAD~1

        Esto restaurará tu repositorio al estado en el commit anterior, descartando los cambios realizados después de ese commit.

15. git rm

        Descripción: Elimina archivos del repositorio y del sistema de archivos.

        Ejemplo de uso:

        Si deseas eliminar un archivo llamado prueba.txt tanto del repositorio como de tu carpeta local, ejecutas:
        git rm prueba.txt

        Luego, necesitas confirmar este cambio con un commit.

16. git stash

        Descripción: Guarda temporalmente los cambios no confirmados para poder trabajar en otra cosa.

        Ejemplo de uso:

        Si estás trabajando en algo, pero necesitas cambiar de contexto sin perder tus avances, puedes hacer un stash. Ejecutas:
        git stash

        Esto guarda tu trabajo no confirmado y limpia tu área de trabajo.

17. git stash pop

        Descripción: Recupera los cambios guardados con git stash.

        Ejemplo de uso:

        Después de haber terminado con el trabajo urgente, puedes recuperar los cambios guardados previamente con:
        git stash pop

        Esto restaurará tus cambios guardados en el stash y podrás continuar trabajando.

18. git rebase

        Descripción: Reaplica los commits de una rama sobre otra base, generalmente para mantener un historial de commits más limpio.

        Ejemplo de uso:

        Estás trabajando en una rama feature y quieres actualizarla con los últimos cambios de main. Ejecutas:
        git rebase main

        Esto moverá tus commits de la rama feature encima de la última versión de main.

19. git tag

        Descripción: Marca un commit con una etiqueta, que generalmente se usa para marcar versiones o hitos importantes.

        Ejemplo de uso:

        Después de lanzar una nueva versión de tu proyecto, puedes etiquetar el commit correspondiente con:
        git tag v1.0

        Esto crea una etiqueta llamada v1.0 para el commit actual, indicándolo como una versión estable.

20. git config

        Descripción: Configura diversas opciones de Git, como el nombre de usuario, correo electrónico, editor de texto, entre otros.

        Ejemplo de uso:

        Si es la primera vez que usas Git, debes configurar tu nombre de usuario y correo electrónico. Ejecutas:

        git config --global user.name "Tu Nombre"
        git config --global user.email "tu@email.com"