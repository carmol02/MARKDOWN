TEMA 3
CREACIÓ I ACTUALITZACIÓ DE REPOSITORIS
---------------------------------------------------------
##-- Exercici 2 GIT 2: Ús de l’historial de canvis--
Indica els comandaments amb els quals resoldries els escenaris plantejats en esl diferents
exercicis.
##Exercici 1
>1.Mostra l'historial de canvis del repositori.
*git log
>2.Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb el següent text:
*nano capitol1.txt
>3.Afegeix els canvis a la zona d'intercanvi temporal (staging area)
*git add capitol1.txt
>4.Fes un commit dels canvis amb el missatge "Afegit capítol 1."
*git commit -m "Afegit capitol 1"
>5.Torna a mostrar l'historial de canvis del repositori.
*git log
##Exercici 2
>1.Crea el fitxer capitol2.txt a la carpeta capítols amb el següent text:
*nano capitol2.txt
>2.Afegeix els canvis a la zona d'intercanvi temporal.
*git add capitols/capitol2.txt
>3.Fes un commit dels canvis amb el missatge "Afegit capítol 2."
*git commit -m "Afegit capitol 2"
>4.Mostra les diferències entre l'última versió i les dues versions anteriors.
*git diff HEAD HEAD HEAD
##Exercici 3:
>1.Crea el fitxer capitol3.txt a la carpeta capítols amb el següent text:
*nano capitol3.txt
>2.Afegeix els canvis a la zona d'intercanvi temporal.
*git add capitols/capitol3.txt
>3.Fes un commit dels canvis amb el missatge "Afegit capítol 3."
*git commit -m "Afegit capitol 2"
>4.Mostra les diferències entre la primera i l'última versió del repositori.
git diff HEAD HEAD HEAD
##Exercici 4
>1.Afegir al final del fitxer índex.txt la següent línia:
*nano index.txt
>2.Afegir els canvis a la zona d'intercanvi temporal.
git add index.txt
>3.Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex
*git commit -m "Afegit capitol 5 a l'index"
>4.Mostrar qui ha fet canvis sobre el fitxer índex.txt.
*git blame index.txt
