# Comandos más usados de Git
Kevin José Pérez Delgadillo - 21400750
### 1. `git init`  
**Descripción:** Inicializa un nuevo repositorio Git.  
**Ejemplo:**  
```bash
git init
```
*Caso de uso:* Comenzar el control de versiones en un nuevo proyecto local.

---

### 2. `git clone`  
**Descripción:** Clona un repositorio remoto en tu máquina local.  
**Ejemplo:**  
```bash
git clone https://github.com/usuario/repositorio.git
```
*Caso de uso:* Descargar una copia de un repositorio desde GitHub.

---

### 3. `git status`  
**Descripción:** Muestra los archivos modificados y el estado del repositorio.  
**Ejemplo:**  
```bash
git status
```
*Caso de uso:* Verificar qué archivos han sido modificados antes de hacer commit.

---

### 4. `git add`  
**Descripción:** Añade archivos al área de preparación (staging).  
**Ejemplo:**  
```bash
git add archivo.txt
```
*Caso de uso:* Preparar archivos para el próximo commit.

---

### 5. `git commit`  
**Descripción:** Guarda los cambios en el historial del repositorio.  
**Ejemplo:**  
```bash
git commit -m "Mensaje del commit"
```
*Caso de uso:* Confirmar los cambios preparados y añadir un mensaje descriptivo.

---

### 6. `git push`  
**Descripción:** Envía los commits locales al repositorio remoto.  
**Ejemplo:**  
```bash
git push origin main
```
*Caso de uso:* Subir tus cambios a GitHub.

---

### 7. `git pull`  
**Descripción:** Descarga y fusiona los cambios del repositorio remoto.  
**Ejemplo:**  
```bash
git pull origin main
```
*Caso de uso:* Actualizar tu repositorio local con los últimos cambios remotos.

---

### 8. `git fetch`  
**Descripción:** Descarga cambios del repositorio remoto sin fusionarlos.  
**Ejemplo:**  
```bash
git fetch origin
```
*Caso de uso:* Verificar los cambios remotos antes de hacer merge.

---

### 9. `git merge`  
**Descripción:** Fusiona una rama en la rama actual.  
**Ejemplo:**  
```bash
git merge rama-desarrollo
```
*Caso de uso:* Unir los cambios de una rama secundaria a la rama principal.

---

### 10. `git branch`  
**Descripción:** Lista, crea o elimina ramas.  
**Ejemplo:**  
```bash
git branch nueva-rama
```
*Caso de uso:* Crear una nueva rama para una característica.

---

### 11. `git checkout`  
**Descripción:** Cambia de rama o restaura archivos.  
**Ejemplo:**  
```bash
git checkout main
```
*Caso de uso:* Cambiar a la rama principal.

---

### 12. `git switch`  
**Descripción:** Cambia entre ramas (más moderno que `checkout`).  
**Ejemplo:**  
```bash
git switch desarrollo
```
*Caso de uso:* Navegar entre ramas de manera más clara.

---

### 13. `git log`  
**Descripción:** Muestra el historial de commits.  
**Ejemplo:**  
```bash
git log --oneline
```
*Caso de uso:* Ver una lista resumida de los commits anteriores.

---

### 14. `git remote`  
**Descripción:** Administra repositorios remotos.  
**Ejemplo:**  
```bash
git remote add origin https://github.com/usuario/repo.git
```
*Caso de uso:* Enlazar tu repositorio local a uno en GitHub.

---

### 15. `git reset`  
**Descripción:** Deshace cambios en el área de staging o historial.  
**Ejemplo:**  
```bash
git reset archivo.txt
```
*Caso de uso:* Quitar un archivo del staging antes del commit.

---

### 16. `git revert`  
**Descripción:** Crea un nuevo commit que revierte los cambios de uno anterior.  
**Ejemplo:**  
```bash
git revert abc1234
```
*Caso de uso:* Deshacer un commit sin alterar el historial.

---

### 17. `git stash`  
**Descripción:** Guarda temporalmente cambios sin hacer commit.  
**Ejemplo:**  
```bash
git stash
```
*Caso de uso:* Guardar cambios sin confirmar cuando necesitas cambiar de rama rápidamente.

---

### 18. `git rebase`  
**Descripción:** Reescribe el historial para aplicar commits sobre una nueva base.  
**Ejemplo:**  
```bash
git rebase main
```
*Caso de uso:* Limpiar el historial antes de fusionar ramas.

---

### 19. `git tag`  
**Descripción:** Crea marcas en commits específicos (por ejemplo, versiones).  
**Ejemplo:**  
```bash
git tag v1.0
```
*Caso de uso:* Marcar una versión estable del proyecto.

---

### 20. `git config`  
**Descripción:** Configura opciones de Git como el usuario y el editor.  
**Ejemplo:**  
```bash
git config --global user.name "Kevin"
```
*Caso de uso:* Establecer tu identidad en todos tus repositorios.
