#  **********************************************************************
#  ***********************     📘 COMANDOS GIT     *********************

## 1️⃣. `git stash` 
Guarda temporalmente los cambios sin tener que hacer commit. Muy útil si necesitas cambiar de rama rápidamente.

**Ejemplo de uso:**
Estás trabajando en un nuevo feature, pero te piden urgentemente corregir 
un bug en otra rama. Guardas tu trabajo actual así:

```bash
git stash
```
---------------------------------------------------------------

## 2️⃣. `git stash pop` 
Recupera y aplica el último stash al directorio de trabajo actual.

**Ejemplo de uso:**
Después de corregir el bug en la otra rama, vuelves a tu rama original y aplicas tu trabajo anterior:

```bash
git stash pop
```
----------------------------------------------------------------

## 3️⃣. `git reflog` 
Muestra un historial de todas las acciones recientes (incluidos commits eliminados).

¿Para qué sirve?
Recuperar commits "perdidos", ver lo que hiciste recientemente, incluso si los commits ya no están en ninguna rama.

**Ejemplo de uso:**
Accidentalmente hiciste git reset --hard y perdiste un commit importante. Puedes recuperarlo:

```bash
git reflog
```
-------------------------------------------------------------------------

## 4️⃣. `git cherry-pick <hash>` 
Aplica un commit específico de otra rama al historial actual.

**Ejemplo de uso:**
Hiciste un commit útil en "inicio-x" que también necesitas en main, sin hacer un merge completo:

```bash
git cherry-pick 2a4b7cd
```
------------------------------------------------------------------------------

## 5️⃣. `git bisect` 
Permite encontrar el commit que introdujo un error utilizando búsqueda binaria.

**Ejemplo de uso:**
Tu aplicación dejó de funcionar, pero no sabes en qué commit comenzó. y vas probando versiones 
hasta encontrar el commit culpable. Usas bisect:

```bash
git bisect start
```
-------------------------------------------------------------------------------

## 6️⃣. `git shortlog` 
Sirve para ver quién ha hecho cuántos commits. Útil para reportes o créditos.

**Ejemplo de uso:**
Al final de un  sprint, quieres ver quién contribuyó más:

```bash
git shortlog -sn
```
-------------------------------------------------------------------------------

## 7️⃣. `git clean -fd` 
Elimina archivos y carpetas que no están siendo rastreados por Git.

**Ejemplo de uso:**
Después de compilar, quedaron carpetas dist/ o .log que no quieres:

```bash
git clean -fd
```
-----------------------------------------------------------------------------

## 8️⃣. `git grep` 
Busca texto dentro de los archivos versionados por Git.

**Ejemplo de uso:**
Quieres saber en qué archivo usaste una función llamada login:

```bash
git grep 'function login'
```
----------------------------------------------------------------------------

## 9️⃣. `git blame` 
Sirve para ver quién fue el autor de cada línea de un archivo, ideal para rastrear
 bugs o preguntar por lógica.

**Ejemplo de uso:**
Una función parece estar mal, y quieres saber quién la escribió para preguntarle: 

```bash
git blame utils.js
```
------------------------------------------------------------------------------

## 🔟. `git show <hash>` 
Muestra toda la información de un commit específico (autor, fecha, cambios).

**Ejemplo de uso:**
Te dan el hash de un commit para revisarlo. Y ves qué archivos modificó y qué líneas cambió:

```bash
git show abc1234
```
-----------------------------------------------------------------------------

## 1️⃣1️⃣. `git tag` 
Permite listar, crear o eliminar etiquetas (tags) en commits.

**Ejemplo de uso:**
Has terminado la versión 1.0 de tu app y quieres marcar ese commit:

```bash
git tag v1.0.0
```
-----------------------------------------------------------------------------

## 1️⃣2️⃣. `git remote -v`
Muestra todas las URLs de los repositorios remotos configurados.

**Ejemplo de uso:**
Estás trabajando en equipo y quieres confirmar que el repositorio remoto apunta al proyecto correcto:

```bash
git remote -v
```
-------------------------------------------------------------------------------

## 1️⃣3️⃣. `git log --graph` 
Muestra el historial de commits como un gráfico de ramas.

**Ejemplo de uso:**
Quieres ver cómo se han unido diferentes ramas al proyecto y su relación:

```bash
git log --oneline --graph --all
```
--------------------------------------------------------------------------

## 1️⃣4️⃣. `git archive` 
Crea un archivo comprimido del contenido de una rama o commit.

**Ejemplo de uso:**
Te piden enviar una copia del código fuente de la rama actual en ZIP:

```bash
git archive -o app.zip HEAD
```
--------------------------------------------------------------------------

## 1️⃣5️⃣. `git apply` 
Aplica un parche creado previamente (por ejemplo, con `git diff`).

**Ejemplo de uso:**
Recibiste un parche de un compañero que arregla un bug:

```bash
git apply fix.patch
```
---------------------------------------------------------------------------

## 1️⃣6️⃣. `git diff --staged` 
Muestra diferencias de archivos ya añadidos al área de preparación (staged) antes de hacer commit.

**Ejemplo de uso:**
Ya hiciste git add, pero quieres revisar qué exactamente será parte del commit:

```bash
git diff --staged
```
---------------------------------------------------------------------------

## 1️⃣7️⃣. `git config --list` 
Muestra toda la configuración activa de Git (nombre, email, alias, editor, etc.).

**Ejemplo de uso:**
No estás segura de qué usuario está configurado para hacer commits en tu máquina:

```bash
git config --list
```
-------------------------------------------------------------------------

## 1️⃣8️⃣. `git rm --cached <archivo>` 
Elimina un archivo del índice (staging area) pero lo deja en el disco.

**Ejemplo de uso:**
Sin querer agregaste .env al repo y quieres quitarlo sin borrarlo del proyecto local:

```bash
git rm --cached .env
```
------------------------------------------------------------------------------

## 1️⃣9️⃣. `git commit --amend` 
Modifica el último commit (ya sea su mensaje o los archivos).

**Ejemplo de uso:**
Hiciste commit pero olvidaste incluir un archivo o cometiste un error en el mensaje:

```bash
git commit --amend -m "Corrige error en función de login"
```
------------------------------------------------------------------------------

## 2️⃣0️⃣. `git rev-parse --abbrev-ref HEAD` 
Devuelve el nombre de la rama en la que estás actualmente.

**Ejemplo de uso:**
Vas a hacer un push y no recuerdas el nombre de la rama actual:

```bash
git rev-parse --abbrev-ref HEAD
```
