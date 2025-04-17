# Comandos GitHub

**NOTAS:** 

- *Todo lo que se encuentre en verde hay que reemplazarlo*
- *Lo que se encuentre después de **!** son comentarios*

## Configuración básica

---

**Establecer el nombre de usuario que aparecerá cuando se realice un commit**

```
git config --global user.name "NombreUsuario"
git config --gloabl user.name "Nano"
```

---

**Establecer el correo que se usará para subir los cambios**

```
git config --global user.email correo@que_queremos_usar.com
git config --global user.email Nano@example.com
```

---

**Activar colores para palabras reservadas**

```
git config --global color.ui true/false
git config --global color.ui true
```

## Iniciar repositorio

---

**Inicializar el proyecto en GIT de manera local** 

Necesitamos estar dentro de una carpeta del proyecto. Este se utiliza cuando nosotros creamos el proyecto, es decir no hay un repositorio existente.

```
git init
```

---

**Clonar un repositorio existente**

Este comando nos permitirá bajar una copia de un proyecto en la nube, ya sea de GitHub o BitBucket.

```
git clone url
git clone https://github/PRACTICA.git
```

---

## Subir archivos

---

### Zona de preparación, comentarios y subida de archivos

---

Para subir archivos hay una serie de comandos que hay que ejecutar, como explicación breve al momento de utilizar ***git add .*** indicamos que todos los archivos con cambios serán enviados  a la zona de preparación; También podemos seleccionar los archivos que nosotros deseemos mandar con ***git add archivo.extensión, archivo2.extension*** en el caso de que algunos se encuentren incompletos.

```
*! Agregar los archivos a la "Zona de preparación"*
git add .  
*! Agregar un titulo a la actualización que se desea envíar* 
git commit -m "Mensaje de la actualización envíada"
*! Enviar la nueva información al repositorio online*
git push origin master

*! Nota: Algunos repositorios utilizan master y otro main
! Origin hace referencia al proyecto local mientras que 
! Master a la rama principal en la nube*

git add .  
git commit -m "Corrección de errores en la consulta de API Get"
git push origin master
```

---

**Subir archivos en concreto**

```
git add archivoUno.txt, ArchivoDos.txt   
git commit -m "Mensaje de la actualización envíada"
git push origin master

git add userController.js, userRoutes.js, userSchema.js
git commit -m "API Usuarios"
git push origin master
```

---

**Enviar a zona de preparación todos los archivos con una extensión**

Este comando envía a la zona de preparación a todos los archivos del proyecto con la extensión especificada.

```
git add *.extensión
git add *.txt

*! Después de estos comandos hay que incluir el comentario y push*
```

---

**Enviar a zona de preparación todos de una carpeta con la misma extensión**

```
git add directorio/*.extensión
git add controladores/*.js

*! Después de estos comandos hay que incluir el comentario y push*
```

---

**Enviar una carpeta completa a preparación**

```
git add directorio/
git add controladores/

*! Después de estos comandos hay que incluir el comentario y push*
```

---

## Tags

---

Las etiquetas son mensajes en commit que sirven para resaltar una versión específica del proyecto

---

**Listar los tags existentes**

```
git tag
```

---

**Crear Tag**

```
git tag -a version -m "mensaje"
git tag -a v1.0.0 -m "Primera versión estable"
```

---

## Branch (Ramas)

---

**Listar ramas del proyecto**

```
git branch
```

---

**Crear una rama**

```
git branch nombreRama
git branch baNano
```

---

**Eliminar ramas**

Al eliminar una rama la consola nos devolverá un mensaje de confirmación; El segundo comando salta la confirmación.

```
*! Suponiendo que tenemos las ramas: Nano, Swaggy, Jhova, Azaral y Comic*
git branch -d nombreRama
git branch -d Swaggy
```

```
*! Al colocar la 'd' en mayúscula saltamos la confirmación de eliminación*
git branch -D nombreRama
git branch -D Swaggy
```

---

## Git rebase

---

Rebase hace que la  rama actual del proyecto se pongan al día con la rama principal. Es recomendable usarlo cuando se llega a una versión estable, así todos los miembros podrán seguir trabajando con todos los agregados hechos hasta la fecha.

---

 **Clonar el contenido de la rama principal en la rama actual**

```
git rebase
```

---

**Hacer rebase a una rama que no es la actual**

```
git rebase nombreRama
git rebase Swaggy
```

---

**Conflictos**

Si llegará a haber un conflicto los efectos de **REBASE** se detendrán y tendremos las siguientes opciones

```
*! Al resolver los conflictos generados con el siguiente comando continuaremos el proceso
! de rebase*
git rebase --continue

*! Abortar la ejecución del comando volviendo la rama al estado antes de ejecutarlo*
git rebase --abort

*! Omitir los conflictos y continuar **Ni voltees a ver este comando***
git rebase --skip
```