# Comandos Básicos de Git :)

```bash
# 1. Inicializar repositorio
git init                         # Ejemplo: inicia Git en tu carpeta actual

# 2. Clonar repositorio remoto
git clone https://github.com/user/repo.git   # Ejemplo: clona un repo remoto

# 3. Agregar archivos al staging
git add archivo.txt              # Ejemplo: agrega solo archivo.txt
git add .                        # Ejemplo: agrega todos los archivos

# 4. Crear commit con mensaje
git commit -m "Agrega login"     # Ejemplo: guarda los cambios con un mensaje

# 5. Ver estado del repositorio
git status                       # Ejemplo: muestra archivos modificados

# 6. Ver historial de commits
git log                          # Ejemplo: historial completo
git log --oneline                # Ejemplo: historial resumido

# 7. Ver ramas locales
git branch                       # Ejemplo: lista ramas locales

# 8. Cambiar a otra rama
git checkout main                # Ejemplo: cambia a la rama 'main'

# 9. Crear y cambiar a nueva rama
git checkout -b nueva-funcionalidad   # Ejemplo: crea y entra a una nueva rama

# 10. Combinar ramas
git merge develop                # Ejemplo: une 'develop' con tu rama actual

# 11. Subir cambios al remoto
git push origin main             # Ejemplo: sube tus commits a GitHub

# 12. Traer cambios del remoto
git pull origin main             # Ejemplo: actualiza tu rama con cambios remotos

# 13. Descargar cambios sin aplicar
git fetch origin                 # Ejemplo: descarga cambios sin mezclarlos

# 14. Ver repositorios remotos
git remote -v                    # Ejemplo: muestra URLs del repositorio remoto

# 15. Eliminar una rama local
git branch -d vieja-rama         # Ejemplo: borra la rama local 'vieja-rama'

# 16. Resetear al commit anterior (borra cambios)
git reset --hard HEAD~1          # Ejemplo: deshace el último commit

# 17. Resetear pero mantener cambios
git reset --soft HEAD~1          # Ejemplo: deshace commit pero conserva los cambios

# 18. Guardar cambios temporalmente
git stash                        # Ejemplo: guarda cambios no comiteados

# 19. Ver lista de stashes
git stash list                   # Ejemplo: muestra los cambios guardados

# 20. Aplicar último stash
git stash apply                  # Ejemplo: recupera los últimos cambios guardados
