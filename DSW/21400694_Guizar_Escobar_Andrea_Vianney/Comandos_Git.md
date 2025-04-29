# Actividad 1 b. 20 comandos de Github

## 1. git init
**Descripción:** Inicializa un repositorio Git vacío en el directorio actual. Se crea una carpeta oculta llamada `.git` que contiene toda la información necesaria del repositorio.

**Uso:** Se usa cuando comienzas un proyecto desde cero y quieres que sea gestionado por Git.

**Ejemplo de uso:**
```bash
- `git init` → Crea un repositorio Git local en la carpeta actual.
```

## 2. git config
**Descripción:** Permite configurar variables importantes para tu entorno Git, como el nombre del usuario y su correo electrónico. Puedes hacerlo a nivel global (para todos los repositorios del sistema) o local (solo para el proyecto actual).

**Uso:** Ayuda a que Git registre correctamente identidad correcta del autor. También puedes configurar el editor predeterminado, alias, colores, entre otros parámetros. 

**Ejemplo de uso:**
```bash
- `git config --global user.name "Andrea Guizar"` → Define el nombre del usuario.
- `git config --global user.email "andrea@ejemplo.com"` → Define el correo del usuario.
```

## 3. git clone
**Descripción:** Copia todo el contenido de un repositorio remoto a tu máquina local, incluyendo historial, ramas y archivos.

**Uso:** Se usa para obtener una copia local de un repositorio existente.

**Ejemplo de uso:**
```bash
- `git clone https://github.com/usuario/proyecto.git` → Clona el repositorio llamado "proyecto" en una nueva carpeta.
```

## 4. git status
**Descripción:** Muestra los archivos modificados, los que están listos para el próximo commit, los que aún no están siendo rastreados y los que están en staging.

**Uso:** Para saber qué archivos han sido cambiados, agregados o están listos para hacer commit.

**Ejemplo de uso:**
```bash
- `git status` → Lista los archivos modificados, agregados o sin seguimiento.
```

## 5. git add
**Descripción:** Mueve los archivos al área de staging (preparación). Git solo registra en el próximo commit los archivos que han sido añadidos con este comando.

**Uso:** Puedes elegir qué archivos quieres guardar en el commit, lo cual te permite controlar el historial y agrupar cambios de forma lógica.

**Ejemplo de uso:**
```bash
- `git add archivo.html` → Prepara solo ese archivo para commit.
- `git add .` → Prepara todos los cambios detectados para commit.
```

## 6. git commit
**Descripción:** Guarda los cambios del área de staging en el historial de versiones del repositorio.

**Uso:** Después de usar git add, este comando registra de forma permanente esos cambios usando un mensaje descriptivo. Es como un punto de restauración del proyecto.

**Ejemplo de uso:**
```bash
- `git commit -m "Agrega nuevo formulario de contacto"` → Crea un commit con ese mensaje explicando los cambios.
```

## 7. git push
**Descripción:** Envía los commits de tu repositorio local al repositorio remoto. Esto hace que otros puedan ver y colaborar con tus cambios.

**Uso:** Para compartir los cambios realizados en tu código con otros.

**Ejemplo de uso:**
```bash
- `git push origin main` → Sube los commits de la rama "main" al servidor remoto llamado "origin".
```

## 8. git pull
**Descripción:** Combina git fetch (traer) y git merge (fusionar). Descarga e integra los cambios del repositorio remoto con tu copia local.

**Uso:** Se utiliza para mantener tu proyecto actualizado con los cambios hechos por otros.

**Ejemplo de uso:**
```bash
- `git pull origin main` → Trae los últimos cambios de la rama "main" y los fusiona en tu repositorio local.
```

## 9. git fetch
**Descripción:** Recupera los últimos cambios del repositorio remoto sin fusionarlos. Es útil para ver qué hay de nuevo sin modificar tu trabajo actual.

**Uso:** Permite comparar los cambios antes de integrarlos manualmente, es útil cuando deseas tener mayor control del proceso.

**Ejemplo de uso:**
```bash
- `git fetch origin` → Trae los cambios del repositorio remoto llamado "origin".
```

## 10. git merge
**Descripción:** Combina los cambios de una rama con la rama actual. Es una forma común de integrar el trabajo de distintas funcionalidades.

**Uso:** Para combinar el trabajo hecho en distintas ramas. Se utiliza al finalizar el trabajo en una rama secundaria para integrarla con la principal (por ejemplo, integrar una rama feature con main).

**Ejemplo de uso:**
```bash
- `git merge desarrollo` → Une la rama "desarrollo" con la rama actual.
```

## 11. git branch
**Descripción:**  Sirve para listar todas las ramas, crear nuevas o eliminar ramas. Las ramas permiten trabajar en características de forma paralela sin afectar la principal.

**Uso:** Para trabajar en nuevas funcionalidades de forma separada.

**Ejemplo de uso:**
```bash
- `git branch` → Lista todas las ramas.
- `git branch nueva-funcionalidad` → Crea una nueva rama llamada "nueva-funcionalidad".
```

## 12. git checkout
**Descripción:** Permite moverse entre ramas o versiones anteriores del proyecto. También puede usarse para recuperar archivos específicos.

**Uso:** Para moverse entre diferentes ramas o restaurar archivos. Es común para revisar código anterior, probar ramas nuevas o hacer cambios rápidos sin afectar la rama principal.

**Ejemplo de uso:**
```bash
- `git checkout main` → Cambia a la rama "main".
```

## 13. git log
**Descripción:** Muestra un historial completo de todos los commits realizados, incluyendo autor, fecha, identificador del commit y mensaje.

**Uso:** Para revisar los cambios hechos a lo largo del tiempo. Útil para rastrear cuándo y por qué se hicieron ciertos cambios. También puedes usar git log --oneline para ver una versión más compacta.

**Ejemplo de uso:**
```bash
- `git log` → Muestra todos los commits, con autor, fecha y mensaje.
```

## 14. git diff
**Descripción:** Muestra las diferencias entre archivos modificados y los que están en el último commit.

**Uso:** Para revisar qué ha cambiado antes de hacer commit o usarse para comparar ramas.

**Ejemplo de uso:**
```bash
- `git diff` → Muestra los cambios pendientes.
```

## 15. git reset
**Descripción:** Revierte cambios moviendo archivos fuera del área de staging o eliminando commits recientes.

**Uso:** Para deshacer errores o limpiar cambios no deseados.

**Ejemplo de uso:**
```bash
- `git reset archivo.html` → Quita ese archivo del staging.
- `git reset --hard HEAD~1` → Elimina el último commit.
```

## 16. git rm
**Descripción:** Elimina archivos tanto del área de trabajo como del control de 
versiones.

**Uso:**  Se usa cuando quieres borrar archivos del proyecto de forma controlada y que se mantengan el historial.

**Ejemplo de uso:**
```bash
- `git rm archivo.txt` → Borra el archivo y lo marca para commit.
```

## 17. git stash
**Descripción:** Guarda cambios temporales que no están listos para commit y deja el área de trabajo limpia para cambiar de rama o resolver problemas urgentes.

**Uso:** Para guardar progreso sin hacer commit.

**Ejemplo de uso:**
```bash
- `git stash` → Guarda los cambios actuales.
- `git stash pop` → Recupera los cambios guardados.
```

## 18. git rebase
**Descripción:**  Aplica los commits de una rama sobre otra, reescribiendo el historial. Ayuda a mantener un historial más lineal y claro.

**Uso:** Para mantener un historial limpio. Recomendado para sincronizar ramas personales antes de hacer un merge con la rama principal.

**Ejemplo de uso:**
```bash
- `git rebase main` → Aplica tus commits actuales encima de la rama "main".
```

## 19. git tag
**Descripción:** Crea una etiqueta fija en un commit para para identificar versiones específicas del proyecto (por ejemplo: v1.0, v2.1).

**Uso:** Para marcar pruebas o versiones importantes.

**Ejemplo de uso:**
```bash
- `git tag v1.0` → Crea una etiqueta llamada "v1.0".
```

## 20. git remote
**Descripción:** Permite gestionar las conexiones a repositorios remotos desde tu repositorio local

**Uso:** Para conectar tu repositorio local con uno remoto, se puede usar para agregar, eliminar o listar las conexiones remotas.

**Ejemplo de uso:**
```bash
- `git remote -v` → Muestra las URLs de los repositorios remotos.
- `git remote add origin https://github.com/usuario/repo.git` → Agrega un repositorio remoto llamado "origin".
```

# 21400694 - Guizar Escobar Andrea Vianney