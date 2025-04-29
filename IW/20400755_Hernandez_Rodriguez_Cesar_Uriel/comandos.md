# 📘 Comandos Esenciales de Git y GitHub

Una lista de 20 comandos esenciales para trabajar con Git y GitHub, con sus descripciones y ejemplos de uso.

| Comando | Descripción | Ejemplo de uso |
|--------|-------------|----------------|
| `git init` | Inicializa un nuevo repositorio Git en el directorio actual. | `git init` |
| `git clone <url>` | Clona un repositorio remoto en tu máquina local. | `git clone https://github.com/usuario/repositorio.git` |
| `git status` | Muestra el estado actual de los archivos del proyecto. | `git status` |
| `git add <archivo>` | Agrega archivos específicos al área de preparación (staging). | `git add index.html` |
| `git add .` | Agrega todos los archivos modificados al área de preparación. | `git add .` |
| `git commit -m "mensaje"` | Guarda los cambios preparados en el repositorio local con un mensaje. | `git commit -m "Agrega nueva funcionalidad"` |
| `git push` | Envía los commits del repositorio local al remoto (GitHub). | `git push origin main` |
| `git pull` | Descarga y fusiona los cambios del repositorio remoto al local. | `git pull origin main` |
| `git fetch` | Descarga cambios del repositorio remoto, pero no los fusiona automáticamente. | `git fetch origin` |
| `git merge <rama>` | Fusiona una rama con la actual. | `git merge develop` |
| `git branch` | Lista todas las ramas del proyecto. | `git branch` |
| `git branch <nombre>` | Crea una nueva rama. | `git branch feature-login` |
| `git checkout <rama>` | Cambia a otra rama existente. | `git checkout main` |
| `git checkout -b <rama>` | Crea y cambia a una nueva rama. | `git checkout -b hotfix` |
| `git log` | Muestra el historial de commits. | `git log` |
| `git remote -v` | Lista las URLs remotas asociadas al repositorio. | `git remote -v` |
| `git remote add origin <url>` | Asocia el repositorio local con uno remoto. | `git remote add origin https://github.com/usuario/repositorio.git` |
| `git reset <archivo>` | Quita un archivo del área de preparación. | `git reset index.html` |
| `git revert <id_commit>` | Crea un nuevo commit que revierte los cambios de uno anterior. | `git revert a1b2c3d` |
| `git stash` | Guarda temporalmente los cambios no confirmados. | `git stash` |

---

> 📝 **Nota:** Asegúrate de tener configurado tu usuario de Git con:
> ```bash
> git config --global user.name "Tu Nombre"
> git config --global user.email "tuemail@example.com"
> ```

