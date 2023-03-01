# Tarea 1. Git y GitHub: add y commits
## Valentina Janet Arias Ojeda
###  Introducción.
En este documento se revisarán los temas aprendidos en clase con un ejercicio. Se probará el funcionamiento de un programa dado con un documento a descargar y se permitirá su control por *Git*. Posteriormente se subirá a un repositorio de *GitHub* para su revisión.
### Procedimiento.
- En un archivo de texto, coloca la secuencia de DNA del gene *araC* de *E.coli* en formato fastA obtenida de http://regulondb.ccg.unam.mx/sequence?type=GN&term=ECK120000050&format=fasta 
````
#Copié y pegué la secuencia en un archivo creado en la terminal de git
nano araC.txt
#La moví a la carpeta indicada.
````
- Este archivo guardalo en la carpeta `data` del proyecto `reverse-complement`.
````
mv araC.txt Documents/python1/projects/reverse-complement/data/.
````
- Haz que el archivo sea controlado por git
````
#Estando dentro de la carpeta del proyecto reverse-complement ejecuto el comando git add
git add data/sequence.faa
#Uso el comando git status para verificar que se haya agregado correctamente
git status
#Realizo el commit
git commit -m "Secuencia de gen araC"
#Subir cambios a github
git push origin master
````
### Resultados y conclusiones
En la realización de esta tarea repasé los comandos pricipales de git y aprendí a hacerlo de manera correcta para no tener problemas al controlar archivos futuros.
