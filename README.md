🧩 Guía Completa de Git con Comandos Explicados

Este README contiene todos los comandos principales de Git, acompañados de explicaciones claras para ayudarte a trabajar de forma profesional y resolver dudas rápidamente.

🔧 1. Configuración inicial
git config --global user.name "Tu Nombre"      
# Configura tu nombre de usuario global en Git

git config --global user.email "tuemail@example.com"
# Configura tu correo global en Git

git config --list
# Muestra toda la configuración activa en Git

--------------------------------------------------------
--------------------------------------------------------

📁 2. Crear o clonar repositorios
git init
# Crea un repositorio vacío en la carpeta actual

git clone URL_DEL_REPO
# Descarga un repositorio remoto y lo copia a tu computadora

--------------------------------------------------------
--------------------------------------------------------

🔄 3. Ciclo básico de trabajo
git status
# Muestra los archivos modificados, agregados o pendientes

git add archivo.ext
# Envía un archivo al área de preparación (staging)

git add .
# Agrega TODOS los archivos modificados al staging

git commit -m "mensaje"
# Guarda los cambios de forma permanente en el historial

git log
# Muestra la lista completa de commits con detalles

git log --oneline --graph --decorate
# Muestra el historial de manera resumida con ramas y estructura visual

--------------------------------------------------------
--------------------------------------------------------

🌿 4. Ramas (Branches)
git branch nombre_rama
# Crea una nueva rama

git checkout nombre_rama
# Cambia a una rama existente

git checkout -b nombre_rama
# Crea una nueva rama y cambia a ella de inmediato

git branch
# Lista todas las ramas locales

git branch -d nombre_rama
# Elimina una rama que ya fue fusionada

--------------------------------------------------------
--------------------------------------------------------

🔀 5. Merge (Fusión de ramas)
git checkout main
# Cambia a la rama donde quieres recibir cambios

git merge nombre_rama
# Fusiona los cambios de otra rama hacia la rama actual

--------------------------------------------------------
--------------------------------------------------------

🌎 6. Repositorios remotos
git remote -v
# Muestra los repositorios remotos configurados

git remote add origin URL
# Enlaza tu repositorio local con uno remoto (GitHub por ejemplo)

git remote set-url origin URL
# Cambia la URL del repositorio remoto

--------------------------------------------------------
--------------------------------------------------------

⬆️⬇️ 7. Push y Pull
git push origin nombre_rama
# Sube los commits a la rama remota

git push -u origin nombre_rama
# Sube la rama por primera vez y la deja enlazada

git pull
# Descarga y fusiona cambios desde el repositorio remoto

git pull origin main
# Descarga los cambios específicamente desde la rama main

--------------------------------------------------------
--------------------------------------------------------

📦 8. Stash (Guardar cambios temporalmente)
git stash
# Guarda tus cambios temporalmente sin hacer commit

git stash list
# Muestra la lista de cambios guardados

git stash apply
# Recupera los cambios del stash sin eliminarlo

git stash drop
# Elimina el stash más reciente

--------------------------------------------------------
--------------------------------------------------------

♻️ 9. Restaurar / Reset
git restore archivo
# Revierte los cambios no agregados (antes del git add)

git restore --stage archivo
# Quita el archivo del staging sin borrar los cambios

git reset --soft HEAD~1
# Deshace el último commit pero deja los cambios en el directorio

git reset --hard HEAD~1
# Borra el último commit y los cambios (¡PELIGRO!)

--------------------------------------------------------
--------------------------------------------------------

🚫 10. Archivo .gitignore

Ejemplo de contenido:

__pycache__/
*.log
node_modules/
.env
*.pyc

--------------------------------------------------------
--------------------------------------------------------

🚀 11. Subir un proyecto a GitHub por primera vez
git init
# Inicializa el repositorio

git add .
# Agrega todos los archivos

git commit -m "Primer commit"
# Crea el primer commit

git branch -M main
# Configura la rama principal como main

git remote add origin URL
# Conecta con el repositorio de GitHub

git push -u origin main
# Sube todo al repositorio remoto

--------------------------------------------------------
--------------------------------------------------------

🤝 12. Trabajo colaborativo
git pull origin main
# Actualiza tu repositorio local antes de trabajar

git checkout -b feature/nueva-funcion
# Crea una rama para trabajar en una nueva función

git push origin feature/nueva-funcion
# Sube la rama al repositorio remoto

--------------------------------------------------------
--------------------------------------------------------

🏷️ 13. Tags (Versiones)
git tag v1.0
# Crea un tag llamado v1.0

git push --tags
# Sube todos los tags al remoto

--------------------------------------------------------
--------------------------------------------------------

🧠 14. Flujo profesional recomendado
git checkout main
# Cambia a la rama principal

git pull
# Descarga los cambios más recientes

git checkout -b feature/nueva-funcion
# Crea una nueva rama de desarrollo

git add .
# Prepara los archivos modificados

git commit -m "Descripción del cambio"
# Guarda cambios

git push -u origin feature/nueva-funcion
# Sube la rama

--------------------------------------------------------
--------------------------------------------------------

⭐ 15. Comandos que más vas a usar siempre
git status     # Ver estado
git add .      # Agregar cambios
git commit -m "mensaje"    # Crear commit
git push       # Subir cambios
git pull       # Descargar cambios
git checkout -b rama       # Crear nueva rama
git merge rama             # Fusionar ramas
git log --oneline --graph  # Historial visual
