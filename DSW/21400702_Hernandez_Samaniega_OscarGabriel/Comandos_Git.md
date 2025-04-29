# Actividad B 20 comandos de Github

## git init
**Descripción:** Inicializa un repositorio Git vacío en el directorio actual. Se crea una carpeta oculta llamada `.git` que contiene toda la información necesaria del repositorio.

**Uso:** Se usa cuando comienzas un proyecto desde cero y quieres que sea gestionado por Git.

**Ejemplo de uso:**
```bash
- `git init` → Crea un repositorio Git local en la carpeta actual.
```

## git show
**Descripción:** Muestra información detallada de un objeto Git, como un commit específico, incluyendo cambios realizados, autor y fecha.

**Uso:** Para inspeccionar el contenido de un commit o etiqueta.

**Ejemplo de uso:**
```bash
- `git show 1a2b3c4d` → Muestra el detalle del commit con ID 1a2b3c4d.
```


## git clone
**Descripción:** Copia todo el contenido de un repositorio remoto a tu máquina local, incluyendo historial, ramas y archivos.

**Uso:** Se usa para obtener una copia local de un repositorio existente.

**Ejemplo de uso:**
```bash
- `git clone https://github.com/usuario/proyecto.git` → Clona el repositorio llamado "proyecto" en una nueva carpeta.
```

## git status
**Descripción:** Muestra los archivos modificados, los que están listos para el próximo commit, los que aún no están siendo rastreados y los que están en staging.

**Uso:** Para saber qué archivos han sido cambiados, agregados o están listos para hacer commit.

**Ejemplo de uso:**
```bash
- `git status` → Lista los archivos modificados, agregados o sin seguimiento.
```

## git add
**Descripción:** Mueve los archivos al área de staging (preparación). Git solo registra en el próximo commit los archivos que han sido añadidos con este comando.

**Uso:** Puedes elegir qué archivos quieres guardar en el commit, lo cual te permite controlar el historial y agrupar cambios de forma lógica.

**Ejemplo de uso:**
```bash
- `git add archivo.html` → Prepara solo ese archivo para commit.
- `git add .` → Prepara todos los cambios detectados para commit.
```

## git commit
**Descripción:** Guarda los cambios del área de staging en el historial de versiones del repositorio.

**Uso:** Después de usar git add, este comando registra de forma permanente esos cambios usando un mensaje descriptivo. Es como un punto de restauración del proyecto.

**Ejemplo de uso:**
```bash
- `git commit -m "Agrega nuevo formulario de contacto"` → Crea un commit con ese mensaje explicando los cambios.
```

## git push
**Descripción:** Envía los commits de tu repositorio local al repositorio remoto. Esto hace que otros puedan ver y colaborar con tus cambios.

**Uso:** Para compartir los cambios realizados en tu código con otros.

**Ejemplo de uso:**
```bash
- `git push origin main` → Sube los commits de la rama "main" al servidor remoto llamado "origin".
```

## git pull
**Descripción:** Combina git fetch (traer) y git merge (fusionar). Descarga e integra los cambios del repositorio remoto con tu copia local.

**Uso:** Se utiliza para mantener tu proyecto actualizado con los cambios hechos por otros.

**Ejemplo de uso:**
```bash
- `git pull origin main` → Trae los últimos cambios de la rama "main" y los fusiona en tu repositorio local.
```

## git fetch
**Descripción:** Recupera los últimos cambios del repositorio remoto sin fusionarlos. Es útil para ver qué hay de nuevo sin modificar tu trabajo actual.

**Uso:** Permite comparar los cambios antes de integrarlos manualmente, es útil cuando deseas tener mayor control del proceso.

**Ejemplo de uso:**
```bash
- `git fetch origin` → Trae los cambios del repositorio remoto llamado "origin".
```

## git blame
**Descripción**: Muestra quién hizo cada cambio línea por línea en un archivo.

**Uso**: Para identificar qué usuario modificó una línea específica y en qué commit lo hizo.

**Ejemplo de uso:**
```bash
- `git blame archivo.js` → Muestra la autoría línea por línea de "archivo.js".
```

## git branch
**Descripción:**  Sirve para listar todas las ramas, crear nuevas o eliminar ramas. Las ramas permiten trabajar en características de forma paralela sin afectar la principal.

**Uso:** Para trabajar en nuevas funcionalidades de forma separada.

**Ejemplo de uso:**
```bash
- `git branch` → Lista todas las ramas.
- `git branch nueva-funcionalidad` → Crea una nueva rama llamada "nueva-funcionalidad".
```

## git cherry-pick
**Descripción:** Aplica uno o varios commits específicos de otra rama a la rama actual.

**Uso:** Para traer cambios puntuales sin hacer un merge completo.

**Ejemplo de uso:**
```bash
- `git cherry-pick 1a2b3c4d` → Aplica el commit identificado como 1a2b3c4d en la rama actual.
```

## git log
**Descripción:** Muestra un historial completo de todos los commits realizados, incluyendo autor, fecha, identificador del commit y mensaje.

**Uso:** Para revisar los cambios hechos a lo largo del tiempo. Útil para rastrear cuándo y por qué se hicieron ciertos cambios. También puedes usar git log --oneline para ver una versión más compacta.

**Ejemplo de uso:**
```bash
- `git log` → Muestra todos los commits, con autor, fecha y mensaje.
```

## git archive
**Descripción:** Crea un archivo comprimido (como .zip o .tar) de los archivos de una rama o commit.

**Uso:**  Para generar una versión empaquetada del proyecto.

**Ejemplo de uso:**
```bash
- `git archive --format=zip HEAD > proyecto.zip` → Crea un archivo ZIP del último commit.
```

## git reset
**Descripción:** Revierte cambios moviendo archivos fuera del área de staging o eliminando commits recientes.

**Uso:** Para deshacer errores o limpiar cambios no deseados.

**Ejemplo de uso:**
```bash
- `git reset archivo.html` → Quita ese archivo del staging.
- `git reset --hard HEAD~1` → Elimina el último commit.
```

## git clean
**Descripción:** Elimina archivos no rastreados del directorio de trabajo, como archivos temporales o generados.

**Uso:**  Para limpiar el área de trabajo de archivos no deseados.

**Ejemplo de uso:**
```bash
- `git clean -f` → Elimina archivos no rastreados.
- `git clean -fd` → Elimina archivos y carpetas no rastreados.
```

## git stash
**Descripción:** Guarda cambios temporales que no están listos para commit y deja el área de trabajo limpia para cambiar de rama o resolver problemas urgentes.

**Uso:** Para guardar progreso sin hacer commit.

**Ejemplo de uso:**
```bash
- `git stash` → Guarda los cambios actuales.
- `git stash pop` → Recupera los cambios guardados.
```

## git rebase
**Descripción:**  Aplica los commits de una rama sobre otra, reescribiendo el historial. Ayuda a mantener un historial más lineal y claro.

**Uso:** Para mantener un historial limpio. Recomendado para sincronizar ramas personales antes de hacer un merge con la rama principal.

**Ejemplo de uso:**
```bash
- `git rebase main` → Aplica tus commits actuales encima de la rama "main".
```

## git tag
**Descripción:** Crea una etiqueta fija en un commit para para identificar versiones específicas del proyecto (por ejemplo: v1.0, v2.1).

**Uso:** Para marcar pruebas o versiones importantes.

**Ejemplo de uso:**
```bash
- `git tag v1.0` → Crea una etiqueta llamada "v1.0".
```

## git show
**Descripción:** Muestra información detallada de un objeto Git, como un commit específico, incluyendo cambios realizados, autor y fecha.

**Uso:** Para inspeccionar el contenido de un commit o etiqueta.

**Ejemplo de uso:**
```bash
- `git show 1a2b3c4d` → Muestra el detalle del commit con ID 1a2b3c4d.