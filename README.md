# COMANDOS GIT
Git es un software que permite llevar un control y gestión sobre nuestro código fuente, su naturaleza es distriuida lo que permite trabajar de forma individual o colaborando con cualquier integrante del equipo que comparta el repositorio.

![Image of Git_Distribuido](https://s3.amazonaws.com/media-p.slid.es/uploads/142575/images/1638371/git-tutorial-basics-clone-repotorepocollaboration.png)

Cuando un usuario desea colaborar con un repositorio GIT, lo que hace es clonar la instancia de repositorio con el siguiente comando

```
git clone url_o_path_repositorio directorio_destino
```
El comando git clone realiza la clonación de toda la historio del proyecto.
Donde __url_o_path_repositorio__: representa el path donde esta ubicado el repositorio, si es un servicio o un servidor se debe especificar en la URL, __directorio_repositorio__: es la carpera donde dejaremos el proyecto, si se omite este parámetro se utilizará el nombre del repo donde se clona.

A continuación una pequeña guía de los comandos utilizados para un flujo de trabajo en GIT.

Inicializa un repositorio, se guardaran todos los cambios nefectuados dentro de la carpeta
```
git init
```
Indica estado de repositorio
```
git status
```

Realiza el registro de la historio en git
```
git commit -m "razon social" archivomodificado
```
Indica diferencias entre un archivo anterior y otro que ha sido modificado, pero que aún no ha sido commitiado.
```
git diff index.html
```
Indica la diferencia entre dos puntos de la historio en un archivo especifico
```
git diff id01..id02 nombreArchivo.extension
```

realiza un commit a todo lo que ha sido modificado
```
git commit -am "Comentario del commit"
```
muestra los cambios y las distintas versiones realizadas en el repositorio.
```
git log
```
Una modificación a este comando podría ser el siguiente
```
git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative
```
Que muestra la historia del proyecto con un formato más prety!

Para descartar cambios usamos
```
git chekout -- nombreArchivo
```
Para cambiar a otra versión de la hostoria del archivo en git usamos
```
git checkout hash_commit nombreArchivo.extension 
```

Para borrar un archivo del proyecto en GIT
```
git rm nombreArchivo.extension
```

Configuraciones extras o generales de cada proyecto.
```
git config --global user.name "Norma Soto"
git config --global user.email "correo@aa.aa"
```


> __Miguel Cantillana__ / miguel[at]ewok[dot]cl



