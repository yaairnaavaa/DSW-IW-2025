
# Comandos de Git

---

## 1. git init
Inicializa un nuevo repositorio Git en el directorio actual.

```bash
git init
```

---

## 2. git clone
Clona un repositorio remoto.

```bash
git clone https://github.com/usuario/repositorio.git
```

---

## 3. git status
Muestra el estado del repositorio (archivos modificados, no seguidos, etc.).

```bash
git status
```

---

## 4. git add
Agrega archivos al área de staging.

```bash
git add archivo.txt
git add .
```

---

## 5. git commit
Guarda los cambios en el historial del repositorio.

```bash
git commit -m "Mensaje del commit"
```

---

## 6. git log
Muestra el historial de commits.

```bash
git log
```

---

## 7. git diff
Muestra las diferencias entre archivos.

```bash
git diff
```

---

## 8. git branch
Lista las ramas existentes o crea una nueva.

```bash
git branch
git branch nueva-rama
```

---

## 9. git checkout
Cambia de rama o revierte archivos.

```bash
git checkout main
git checkout archivo.txt
```

---

## 10. git merge
Fusiona una rama en la rama actual.

```bash
git merge feature-x
```

---

## 11. git pull
Trae cambios del repositorio remoto y los fusiona.

```bash
git pull origin main
```

---

## 12. git push
Envía commits al repositorio remoto.

```bash
git push origin main
```

---

## 13. git remote
Administra conexiones a repositorios remotos.

```bash
git remote -v
git remote add origin https://github.com/usuario/repositorio.git
```

---

## 14. git reset
Revierte cambios o elimina commits del historial.

```bash
git reset --hard HEAD~1
git reset archivo.txt
```

---

## 15. git rm
Elimina archivos del repositorio.

```bash
git rm archivo.txt
```

---

## 16. git mv
Mueve o renombra archivos.

```bash
git mv viejo.txt nuevo.txt
```

---

## 17. git stash
Guarda cambios no confirmados para más tarde.

```bash
git stash
git stash pop
```

---

## 18. git tag
Crea etiquetas para versiones específicas.

```bash
git tag v1.0
git tag -a v1.0 -m "Versión 1.0"
```

---

## 19. git fetch
Descarga los cambios del repositorio remoto sin fusionarlos.

```bash
git fetch origin
```

---

## 20. git rebase
Reaplica commits sobre una nueva base.

```bash
git rebase main
```