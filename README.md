ejemplo
=======

Ejemplo práctico para tarea "Llevando git un paso más allá"

## Resumen de comandos
* `git init`, para inicializar un repositorio nuevo en el directorio actual.
* `git clone ruta_repo`, para copiar un repositorio existente dentro del directorio actual. Creará un directorio nuevo para el repo.
* `git status`, para ver el estado de nuestro directorio de trabajo, y el stash. Nos permite ver qué se está por commitear, o qué falta agregar a stash.
* `git add nombre_de_archivos`, para agregar uno o más archivos al próximo commit. Se dice que luego del add se han pasado a stash.
* `git commit -m un_comentario`, para realizar efectivamente un commit con todo lo guardado en el área de stash. Dejará el stash limpio.
* `git log`, para tener un listado de los commits, ordenados en forma inversa según la fecha de captura.
* `gitk`, para acceder a un inspector gráfico de la evolución del proyecto.
* `git lol`, un alias para el comando `git log` con muchas opciones y argumentos. Es necesario [configurarlo](http://uberblo.gs/2010/12/git-lol-the-other-git-log).
* `git reset --hard id_commit`, para volver atrás descartando los cambios realizados luego del commit especificado, eliminándolos definitivamente.
* `git reset --soft id_commit`, para volver atrás descartando los cambios realizados luego del commit especificado, dejándolos en el directorio de trabajo.
* `git checkout -b nombre_rama`, para crear una nueva rama desde el punto actual.
* `git checkout nombre_rama`, para pasar de la rama actual hacia otra.
* `git branch`, para ver las ramas actuales.
* `git branch -D nombre_rama`, para eliminar una rama. Es necesario estar posicionado en *otra rama*.
* `git merge nombre_rama`, para mezclar el contenido de la rama especificada dentro de la rama actual.
* `git mergetool`, para mezclar en forma asistida el contenido de archivos conflictuados al hacer un `git merge`. Son aquellos archivos sobre los que no se ha podido hacer una mezcla automática.
* `git tag nombre_tag sha_del_commit`, para etiquetar cierto commit con un identificador de elección propia. Sirve para marcar versiones, entregas o hitos remarcables en el proyecto.
* `git tag -l`, para listar todos los tags del proyecto.
* `git remote add origin direccion_repo_remoto`, para agregar un repositorio remoto al proyecto, llamándolo "origin".
* `git push -u origin master`, para subir el repositorio local en el repositorio remoto. No debe haber conflictos entre ambos para que la operación se resuelva correctamente. De haberlos, deberá resolverse en forma local.
* `git pull origin master`, para bajar una copia del repositorio remoto dentro del branch especificado, en este caso 'master', al repositorio local. Puede haber conflictos de merge, que se resolverán del modo indicado anteriormente.



* `conflicto` linea generada en branch segundaRama



* `conflicto2` linea generada desde branch master