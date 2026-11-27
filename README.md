# Mi primer Repositorio

Este repositorio nacio en el curso de Git y GitHub.

Editado desde la web GitHub.

Actualizado en una sesion de clase.

Listado de comandos : 
git init # Iniciar un repositorio en el directorio actual (crea /.git)

ls -la # Lista el contenido del directorio actual (tanto visibles como invisibles, all)

git status # Nos da informacion , como la rama en que nos encontramos , si hay archivos no trackeados , si hay archivos en el staging area para hacer commit

git add <nombre.extension> # Agrega una archivo al staging area

git commit -m "mensaje" # Hace commit a lo que este en el staging area

git diff # Muestra los cambios exactos (añadidos con + y eliminados con -) entre distintos archivos del directorio de trabajo
git diff --staged # Muestra los cambios ya preparados que iran en el siguiente commit 

git log # Lista el historial de los commits ordenados por fecha; se muestra autor, fecha, ,mensaje ,hash del commit
git log --oneline # Lista resumida de los commits ordenados por fecha ; se muestra hash y mensaje del commit 

git show # Muestra informacion del ultimo commit realizado ; hash, autor, fecha, mensaje, diff del commit 

git commit --amend -m "mensaje" # Modifica el mensaje del ultimo commit realizado

# .gitignore : Todo lo que se encuentre dentro de esa carpepta, git no los trackeara

git restore <archivo.ext> # Deshace el ultimo cambio hecho en el archivo del directorio de trabajo
git restore --staged <archivo.ext> # Deshace el comando git add <archivo.ext>

git remote add origin <direccion> # Conectar mi repo local con GitHub
git remote -v # Verifica que el repositorio en GitHub quedo registrado

git push -u origin main # Sube los archivos del repo local al repositorio remoto (-u origin main , vincula la rama local main con origin/main para que afuturo baste con git push)

git fetch # Descarga los cambios del repo remoto sin aplicarlos
git merge # Combina los cambios y los aplicarlos
# git pull = git fetch + git merge
