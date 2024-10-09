# Mi proyecto

Primer paso: En este apartado se realiza la creación del repositorio haciendo uso del comando git init "nombre del proyecto". En este caso lo llamamos TALLERDS2.

Segundo paso: Por medio de las congiguraciones globales, aplicamos esto para el usuario y el email correspondiente a nuestra cuenta de Github.

   git config --global user.name Mervid_17 (configuración para el usuario de git)
   git config --global user.email alejandromercadobenitez@gmail.com 
   (Configuracion para el correo asociado)

Tercer paso: Se procede a crear una rama llamada master

 git checkout -b master (se usa este comando para la creación de la rama)

Cuarto paso:  Accedemos a la carpeta que nombramos TALLERDS2
 
 cd TALLERDS2
  ( comando para acceder a la carpeta)

Quinto paso: creamos un redme.md para tener los reportes de todo y en la cabecera del archivo 

ponemos (Mi proyecto)

 echo "# Mi proyecto" > readme.md

 Sexto paso: Añadimos la cabecera al archivo readme.md

 $ git add readme.md

Séptimo paso: Realizamos el primer commit

 git commit -m "Mi primer commit"

 Octavo paso: Creamos una nueva Rama llamada Feature

  git checkout -b feature

Noveno paso: creamos un nuevo documento de texto llamado DOCUMENTO.txt

 echo "PRIMER TEXTO" > DOCUMENTO.txt

Décimo paso: Añadimos todo a DOCUMENTO.txt

 git add DOCUMENTO.txt

 Paso Once: Realizamos un commit dentro de esta rama feature

 git commit -m "first commit"

Paso doce: Añadimos un segundo texto en el segundo renglón del texto llamado DOCUMENTO.txt

echo "SEGUNDO TEXTO" >> DOCUMENTO.txt

paso trece: Realizamos el segundo commit en esta rama

git commit -m "second commit"

Paso catorce: Añadimos un tercer texto al archivo DOCUMENTO.txt

echo "TERCER TEXTO" >> DOCUMENTO.txt

Paso quince: Realizamos en tercer commit en esta rama

git commit -am "THIRD commit

Paso 16: Regresamos a la rama llamada master

git checkout master

Paso 17: Realizamos un merge entre la rama master y la rama feature.

git merge feature

paso 18: desde esta rama, creamos una rama llamada Hotfix

git checkout -b hotfix

paso 19: Añadimos un nuevo texto al DOCUMENTO.txt

echo "Corrección innmediata" >> DOCUMENTO.txt

paso 20: Realizamos un nuevo commit para evidenciar los cambis necesarios.

git commit -am "Hotfix"

paso 21: Regresamos nuevamente a la rama master

git checkout master

paso 22: Realizamos un pick en la rama master con el fin de volver a uno de los commits ya realizados

git cherry-pick hotfix

Paso 22: Enlistamos todo los commits realizados para elegir uno de ellos y revisar los conflictos.

git reflog

Paso 23: Elegimos uno de los commits por medio de su serial

git checkout 6594d70


Paso 24: Revertimos el merge de la rama

 git rebase feature

 Paso 25: volvemos nuevamente a la rama feature

 git checkout feature

 paso 26: creamos un nuevo documento llamado Conflicto.txt y le añadimos un mensaje

 echo "Cambio en feature" > Conflicto.txt


Paso 27: Realizamos un nuevo commit en esta rama

 git commit -am "cambios en FEATURE"

 