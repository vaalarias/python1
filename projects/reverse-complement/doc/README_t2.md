# Tarea 2. Git y GitHub: add y commits
## Valentina Janet Arias Ojeda
###  Introducción.
En este documento se revisarán los temas aprendidos en clase con un ejercicio. Se editaran archivos controlados con git y se compararan las versiones.
También se revisarán los pasos para restaurarlos.
### Procedimiento.
En el archivo de DNA que ya tienes creado, agrega la secuencia del gene araB en formato Fasta.
```
#Estando dentro de la carpeta del proyecto reverse-complement
nano data/secuence.faa
#agrego secuencia
```
Sube los cambios a git y confirmalos.
```
git add sequence.faa
git commit sequence.faa -m "Secuencia del gen araB agregada"
```
Simula que el gene araC ha sufrido 3 mutaciones en su secuencia, cambia 3 nucleótidos.
```
#Realizo 3 modificaciones
nano sequence.faa
```
Agrega los cambios a git y confirmalos.
```
git add sequence.faa
git commit sequence.faa -m "3 Mutaciones simuladas"
```
Haz las siguientes comparaciones del archivo: última vs penútima y última vs antepenúltima.
```
#Comparación de última y penúltima
git diff 27687e1 56e79e6
#Comparación de última y antepenúlma
git diff 27687e1 73dcbe1
```
Restaura la versión del archivo que no tiene las mutaciones.
```
git checkout 56e79e6 data/sequence.faa
git add data/sequence.faa
   16  git commit data/sequence.faa -m "Archivo restaurado a la versión sin mutaciones"
```

### Resultados y conclusiones
En la realización de esta tarea repasé los comandos para administrar las modificaciones en archivos controlados de git y aprendí a hacerlo de manera correcta para no tener problemas al controlar archivos futuros.