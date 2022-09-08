# workMasterStorage
Trabajo 1 de maestria clase almacenamiento y datos

#subir archivo

Agregar un archivo a un repositorio utilizando la línea de comando

Puedes cargar un archivo existente a un repositorio en GitHub.com utilizando la línea de comandos.

Sugerencia: También puede agregar un archivo existente a un repositorio desde el sitio web GitHub.

Este procedimiento supone que ya has:

    Creado un repositorio en GitHub, o bien tiene un repositorio existente que es propiedad de alguien más con quien quiere colaborar
    Clonado el repositorio de forma local en el equipo

Advertencia: Nunca git add, commit ni información confidencial de push en un repositorio remoto. La información sensible puede incluir, pero no se limita a:

    Contraseñas
    Claves SSH
    Claves de acceso de AWS
    claves de API
    Números de tarjeta de crédito
    Números PIN

Para más información, vea "Eliminación de datos confidenciales de un repositorio".

    En tu computadora, mueve el archivo que deseas cargar a GitHub en el directorio local que se creó cuando clonaste el repositorio.
    Abra Terminal. 1. Cambia el directorio de trabajo actual por tu repositorio local. 1. Agregue el archivo al "stage" para confirmarlo en el repositorio local.

    $ git add .
    # Adds the file to your local repository and stages it for commit. Para sacar del "stage" un archivo, use "git reset HEAD EL_ARCHIVO".

    Confirme el archivo que ha agregado al "stage" en el repositorio local.

    $ git commit -m "Add existing file"
    # Commits the tracked changes and prepares them to be pushed to a remote repository. Para eliminar esta confirmación y modificar el archivo, usa 'git reset --soft HEAD~1' y confirma y agrega nuevamente el archivo.

    Inserte los cambios en el repositorio local en GitHub.com.

    $ git push origin your-branch
    # Pushes the changes in your local repository up to the remote repository you specified as the origin

https://docs.github.com/es/repositories/working-with-files/managing-files/adding-a-file-to-a-repository