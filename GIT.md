COMANDOS GIT
------------

- inicializa un repositorio, se guardaran todos los cambios nefectuados dentro de la carpeta

>>git init
```
git init
```


#indica estado de repositorio
>>git status

>>git commit -m "razon social" archivomodificado

#indica diferencias entre un archivo anterior y otro que ha sido modificado, pero que uan no ha sido commitiado
>>git diff index.html
>>git diff id01..id02 nombreArchivo.extension

#realiza un commit a todo lo que ha sido modificado
>>git commit -am "razon social"

#muestra los cambios y las distintas versiones realizadas en el repositorio.
>>git log

#descartar cambios
>>git chekout -- nombreArchivo

#cambiar a otra version
>>git checkout id nombreArchivo.extension

#comando para borrar archivo
>>git rm nombreArchivo.extension

#configuraciones extras
>>git config --global user.name "Norma Soto"

>>git config --global user.email "correo@aa.aa"

