# Laboratorio Git

Creo una carpeta con el nombre del repositorio e incializo el repositorio con el comando git init

Creo un nuevo repositorio en GitHub y lo conecto a mi repositorio local con git remote add origin git@github.com:angelarera/laboratorio-git.git , que es la clave SSH de mi repositorio en la nube. 
Añado mis archivos al staging con git add . , hago un commit con el comando git commit -m "verificando la conexión" y con git push -u origin master lo subo a mi repositorio en la nube. Refresco mi ventana con GitHub y compruebo que se ha subido correctamente para verificar la conexión entre mi repositorio local y mi repositorio en la nube. 

Creo un nuevo archivo en mi repositorio local, al que he llamado fichero.js y lo añado al staging con git add .
Creo un commit con git commit -m "añadiendo un nuevo archivo" y lo subo a GitHub con git push

Creo una nueva rama llamada development con git branch development y cambio a ella con git checkout development
Hago cambios en fichero.js (he cambiado el contenido del console.log, que decía anteriormente soy un fichero nuevo, por soy un fichero modificado)
Lo añado a staging con git add . , hago git commit -m "modificando mi archivo" y lo subo a GitHub con git push --set-upstream origin development

Vuelvo a mi rama master con git checkout master, y hago un merge de la misma con la rama development con el comando git merge development
Hago git add . , git commit -m "fusionando mis ramas" y lo subo a GitHub con git push