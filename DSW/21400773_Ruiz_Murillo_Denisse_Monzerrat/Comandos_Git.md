# Comandos Básicos de Git

---

## 1. `git clone <url>`
**Descripción**: Crea una copia local de un repositorio remoto completo, incluyendo todo el historial de cambios y todas las ramas. Es el primer comando que se usa para empezar a trabajar con un proyecto existente.
**Ejemplo**:
```bash
git clone https://github.com/usuario/repo.git  # Clona un repositorio usando protocolo HTTPS
git clone git@github.com:usuario/repo.git     # Clona usando SSH (más seguro)
git clone --branch main repo.git           # Clona solo una rama específica (más rápido)
```

## 2. `git init`
**Descripción**: Inicializa un nuevo repositorio Git en el directorio actual, creando la estructura de datos necesaria para el control de versiones. Se usa cuando se comienza un proyecto desde cero.
**Ejemplo**:
```bash
git init              # Crea un repositorio estándar
git init --bare       # Crea un repositorio bare (para servidores)
```

## 3. `git add <archivo>`
**Descripción**: Añade cambios del directorio de trabajo (working directory) al área de preparación (staging area), preparándolos para ser incluidos en el próximo commit. Permite seleccionar cuidadosamente qué cambios se van a guardar.
**Ejemplo**:
```bash
git add archivo.txt          # Añade un archivo específico al staging
git add .                    # Añade todos los archivos modificados y nuevos
git add -p                   # Modo interactivo para seleccionar cambios parciales
```

## 4. `git commit`
**Descripción**: Captura un snapshot de los cambios actuales en el área de preparación (staging area), creando un nuevo commit en el historial del repositorio. Cada commit debe tener un mensaje claro que explique los cambios.
**Ejemplo**:
```bash
git commit -m "Estructura del desarrollo"      # Commit básico con mensaje descriptivo
git commit -am "Actualización de estilos"     # Añade automáticamente cambios y hace commit (solo archivos rastreados)
git commit --amend                 # Modifica el último commit (útil para correcciones)
```

## 5. `git status`
**Descripción**: Muestra el estado actual del directorio de trabajo (working directory) y del área de preparación (staging area), incluyendo qué archivos han sido modificados, cuáles están preparados para commit y cuáles no están siendo rastreados.
**Ejemplo**:
```bash
git status           # Muestra el estado detallado
git status -s        # Versión corta con códigos de estado (M=modificado, A=añadido, etc.)
```

## 6. `git push`
**Descripción**: Sube los commits locales al repositorio remoto, compartiendo tus cambios con otros colaboradores. Es importante especificar la rama destino.
**Ejemplo**:
```bash
git push origin main         # Sube cambios a la rama main del remoto 'origin'
git push -u origin feature   # Sube cambios y establece relación de seguimiento
git push --force-with-lease  # Fuerza push de manera segura (sobrescribe historia remota)
```

## 7. `git pull`
**Descripción**: Obtiene los últimos cambios del repositorio remoto y los fusiona automáticamente con tu rama local. Equivale a hacer git fetch seguido de git merge.
**Ejemplo**:
```bash
git pull origin main         # Descarga cambios y hace merge
git pull --rebase origin main # Descarga cambios y aplica rebase (mantiene historial lineal)
```

## 8. `git branch`
**Descripción**: Permite listar, crear o eliminar ramas en el repositorio. Las ramas permiten trabajar en características aisladas sin afectar el código principal.
**Ejemplo**:
```bash
git branch                  # Lista todas las ramas locales
git branch -a               # Lista todas las ramas (locales y remotas)
git branch -d ramitax        # Elimina una rama local (solo si está fusionada)
```

## 9. `git checkout`
**Descripción**: Permite cambiar entre ramas existentes, crear nuevas ramas o restaurar archivos a su estado en un commit específico. Es una herramienta versátil para navegar el repositorio.
**Ejemplo**:
```bash
git checkout develop        # Cambia a la rama develop
git checkout -b nuevaRama   # Crea y cambia a nueva rama nuevaRama
git checkout HEAD~2 -- doc.txt # Restaura archivo a como estaba hace 2 commits
```

## 10. `git merge`
**Descripción**: Combina los cambios de una rama con la rama actual, creando un nuevo commit de merge cuando es necesario. Es la forma estándar de integrar cambios entre ramas.
**Ejemplo**:
```bash
git merge feature/login     # Fusiona la rama feature/login con la actual
git merge --no-ff release  # Fuerza creación de commit de merge (evita fast-forward)
git merge --abort          # Cancela un merge con conflictos
```

## 11. `git log`
**Descripción**: Muestra el historial de commits de forma detallada, incluyendo autor, fecha y mensaje de cada cambio. Esencial para entender la evolución del proyecto.
**Ejemplo**:
```bash
git log                     # Muestra historial completo
git log --oneline --graph   # Muestra versión compacta con gráfico de ramas
git log -p                  # Muestra diferencias introducidas en cada commit
```

## 12. `git diff`
**Descripción**: Muestra las diferencias entre commits, ramas o el directorio de trabajo (working directory) y el área de preparación (staging area). Muy útil para revisar cambios antes de hacer commit.
**Ejemplo**:
```bash
git diff                    # Cambios no añadidos al staging
git diff --cached           # Cambios entre staging y último commit
git diff main..feature      # Compara dos ramas diferentes
```

## 13. `git reset`
**Descripción**: Permite deshacer cambios moviendo el puntero HEAD a un commit específico. Tiene tres modos principales que afectan al directorio de trabajo (working directory) y área de preparación (staging area) de diferente manera.
**Ejemplo**:
```bash
git reset --soft HEAD~1     # Deshace commit pero mantiene cambios en staging
git reset --mixed HEAD~1    # Deshace commit y saca cambios del staging (default)
git reset --hard HEAD~1     # Deshace commit y descarta todos los cambios (peligroso)
```

## 14. `git stash`
**Descripción**: Guarda temporalmente cambios no commiteados en una pila, permitiendo cambiar de contexto rápidamente. Los cambios pueden recuperarse más tarde.
**Ejemplo**:
```bash
git stash                   # Guarda cambios no commiteados
git stash list              # Muestra todos los stashes guardados
git stash pop               # Aplica y elimina el stash más reciente
```

## 15. `git remote`
**Descripción**: Gestiona las conexiones con repositorios remotos, permitiendo añadir, renombrar o eliminar referencias a otros repositorios Git.
**Ejemplo**:
```bash
git remote -v               # Lista todos los remotos con sus URLs
git remote add upstream URL # Añade un nuevo remoto (para forks)
git remote rename origin primary # Renombra un remoto existente
```

## 16. `git fetch`
**Descripción**: Descarga objetos y referencias de un repositorio remoto sin modificar tu directorio de trabajo (working directory). Permite ver los cambios antes de integrarlos.
**Ejemplo**:
```bash
git fetch origin            # Descarga cambios del remoto 'origin'
git fetch --prune           # Elimina referencias a ramas remotas eliminadas
git fetch --all             # Descarga cambios de todos los remotos configurados
```

## 17. `git rebase`
**Descripción**: Reaplica commits sobre otra rama base, creando un historial lineal. Útil para mantener un historial limpio, pero no debe usarse en commits ya compartidos.
**Ejemplo**:
```bash
git rebase main             # Reaplica commits actuales sobre main
git rebase -i HEAD~3        # Rebase interactivo (permite editar últimos 3 commits)
git rebase --abort          # Cancela un rebase en progreso
```

## 18. `git tag`
**Descripción**: Crea referencias estáticas a puntos específicos en el historial, típicamente usadas para marcar releases (v1.0, v2.0, etc.). Pueden ser ligeras o anotadas.
**Ejemplo**:
```bash
git tag v1.0.0              # Crea tag ligero
git tag -a v1.1.0 -m "Release estable" # Crea tag anotado con mensaje
git tag -d v0.9             # Elimina un tag local
```

## 19. `git config`
**Descripción**: Configura opciones específicas para el repositorio local o globalmente para el usuario. Controla el comportamiento de Git y las preferencias personales.
**Ejemplo**:
```bash
git config --global user.name "Monita"  # Establece nombre para todos tus commits
git config --global core.editor "code --wait" # Configura VS Code como editor
git config --list            # Muestra todas las configuraciones actuales
```

## 20. `git restore`
**Descripción**: Restaura archivos en el directorio de trabajo (working directory) o área de preparación (staging area) a su estado en un commit específico. Alternativa moderna a algunos usos de git checkout/reset.
**Ejemplo**:
```bash
git restore doc.txt         # Descarta cambios en directorio de trabajo (working directory)
git restore --staged doc.txt # Saca archivo del área de preparación (staging area)
git restore --source=HEAD~2 doc.txt # Restaura archivo a como estaba hace 2 commits
```