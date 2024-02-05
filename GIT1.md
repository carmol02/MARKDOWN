TEMA 3
CREACIÓ I ACTUALITZACIÓ DE REPOSITORIS
==============================================
##Exercici 1
>1.Crea un repositori nou amb el nom llibre i mostrar el seu contingut.
*git init
>2.Configura Git definint el nom de l'usuari, el correu electrònic i activar l'exida en
color. Mostrar la configuració final.
*git config --golbal user.name "Carles"
*git config --golbal user.email "carlesmolina03@gmail.com"
*git config --global color.ui auto
*git config --list
##Exercici 2
>1.Comprova l'estat del repositori.
*git status
>2.Crea un fitxer índex.txt amb el següent contingut:
*nano index.txt
>3.Comprova de nou l'estat del repositori.
*git status
>4.Afegeix el fitxer a la zona d'intercanvi temporal.
*git add index.txt
>5.Tornar a comprovar una vegada més l'estat del repositori.
*git status
##Exercici 3:Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre."
i veure l'estat del repositori.
*git commit -m "Afegit index del llibre"
##Exercici 4
>1.Canvia el fitxer índex.txt perquè continga el següent:
*nano index.txt
>2.Mostra els canvis respecte a l'última versió guardada al repositori.
*git diff
>3.Fer un commit dels canvis amb el missatge "Afegit capítol 3 sobre gestió de
branques".
*git commit -m
##Exercici 5
>1.Mostrar els canvis de l'última versió del repositori respecte a l'anterior.
*git log -p -1
>2.Canviar el missatge de l'últim commit a "Afegit capítol 3 sobre gestió de branques
a l'índex."
*git commit --amend -m
>3.Tornar a mostrar els últims canvis del repositori.
*git log -p -1
##Exercici 6: Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els
que tenen l'extensió out i les imatges (jpg, png, bmp i gif).
*echo "daw*" > .gitignore
