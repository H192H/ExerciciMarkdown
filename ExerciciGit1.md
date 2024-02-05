# EXERCICI GIT 1: CREACIO I ACTUALITZACIO DE
# REPOSITORIS

## Exercici 1

1. Crea un repositori nou amb el nom llibre i mostrar el seu contingut.
- mkdir libro
- cd libro
 -git init
4. Configura Git definint el nom de l'usuari, el correu electrònic i activar l'exida en color.
Mostrar la configuració final.
git config --global user.name "hajar"
git config --global user.email "hajarbenchauoi34@gmail.com"
git config --global color.ui true
git config --global --list

## Exercici 2

1. Comprova l'estat del repositori.
Git status
2. Crea un fitxer índex.txt amb el següent contingut:
nano índex.txt
3. Comprova de nou l'estat del repositori.
git status
4. Afegeix el fitxer a la zona d'intercanvi temporal.
git add índex.txt
5. Tornar a comprovar una vegada més l'estat del repositori.
git status
Exercici 3 Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i veure
l'estat del repositori.
git commit -m "Afegit índex del llibre."
git status

## Exercici 4

1. Canvia el fitxer índex.txt perquè continga el següent:
nano índex.txt
2. Mostra els canvis respecte a l'última versió guardada al repositori.
git diff
3. Fer un commit dels canvis amb el missatge "Afegit capítol 3 sobre gestió de branques".
4. git commit -m "Afegit capítol 3 sobre gestió de branques."
   
## Exercici 5

1. Mostrar els canvis de l'última versió del repositori respecte a l'anterior.
git diff HEAD~1 HEAD
2. Canviar el missatge de l'últim commit a "Afegit capítol 3 sobre gestió de branques a
l'índex."
git commit --amend -m "Afegit capítol 3 sobre gestió de branques a l'índex."
3. Tornar a mostrar els últims canvis del repositori.
git status
Exercici 6 Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els que tenen
l'extensió out i les imatges (jpg, png, bmp i gif).
nano .gitignore
 Ignorar fitxers que comencen per "daw"
daw*
 Ignorar fitxers amb extensió out
*.out
 Ignorar imatges
*.jpg
*.png
*.bmp
*.gif
git add .gitignore
git commit -m "Afegit .gitignore per ignorar fitxers específics."
