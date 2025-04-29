# 📘 Comandos de Git

Lista de 20 comandos básicos de Git, su descripción y un ejemplo de uso.

---

1. **`git init`**  
   Inicializa un nuevo repositorio Git en la carpeta actual.  
   Ejemplo: `git init`

2. **`git clone <URL>`**  
   Clona un repositorio remoto en tu computadora.  
   Ejemplo: `git clone https://github.com/usuario/repositorio.git`

3. **`git status`**  
   Muestra el estado actual del repositorio (archivos modificados, nuevos, etc.).  
   Ejemplo: `git status`

4. **`git add .`**  
   Agrega todos los archivos al área de preparación (staging).  
   Ejemplo: `git add .`

5. **`git add <archivo>`**  
   Agrega un archivo específico al área de preparación.  
   Ejemplo: `git add index.html`

6. **`git commit -m "mensaje"`**  
   Guarda los cambios preparados en el historial con un mensaje.  
   Ejemplo: `git commit -m "Agregué el login"`

7. **`git push`**  
   Sube los cambios confirmados al repositorio remoto.  
   Ejemplo: `git push origin main`

8. **`git pull`**  
   Descarga y fusiona los cambios del repositorio remoto.  
   Ejemplo: `git pull origin main`

9. **`git branch`**  
   Muestra las ramas locales disponibles.  
   Ejemplo: `git branch`

10. **`git branch <nombre>`**  
    Crea una nueva rama.  
    Ejemplo: `git branch nueva-funcionalidad`

11. **`git checkout <rama>`**  
    Cambia a otra rama existente.  
    Ejemplo: `git checkout develop`

12. **`git checkout -b <rama>`**  
    Crea y cambia a una nueva rama en un solo paso.  
    Ejemplo: `git checkout -b feature-login`

13. **`git merge <rama>`**  
    Fusiona una rama en la rama actual.  
    Ejemplo: `git merge develop`

14. **`git log`**  
    Muestra el historial de commits del repositorio.  
    Ejemplo: `git log`

15. **`git remote -v`**  
    Muestra las direcciones de los remotos configurados.  
    Ejemplo: `git remote -v`

16. **`git remote add origin <URL>`**  
    Agrega un repositorio remoto como `origin`.  
    Ejemplo: `git remote add origin https://github.com/usuario/repositorio.git`

17. **`git reset --hard HEAD`**  
    Revierte todos los cambios locales no confirmados.  
    Ejemplo: `git reset --hard HEAD`

18. **`git rm <archivo>`**  
    Elimina un archivo del proyecto y del control de versiones.  
    Ejemplo: `git rm archivo.txt`

19. **`git stash`**  
    Guarda temporalmente los cambios sin confirmar.  
    Ejemplo: `git stash`

20. **`git stash pop`**  
    Recupera los cambios guardados con `git stash`.  
    Ejemplo: `git stash pop`
