TEMA 3
CREACIÓ I ACTUALITZACIÓ DE REPOSITORIS
------------------------------------------------------
##-- Exercici 4 GIT 4:Gestió de branques --
Indica els comandaments amb els quals resoldries els escenaris plantejats en els diferents
exercicis.
##Exercici 1
>1.Crea una nova branca bibliografia i mostrar les branques del repositori.
*git branch bibliografia
*git branch
##Exercici 2
>1.Crear el fitxer capítols/capitol4.txt i afegir el següent text
*git checkout master
echo «Afegir els canvis a la zona d’intercanvi temporal» capitols/capitol4.txt
>2.Afegir els canvis a la zona d'intercanvi temporal.
*git add capitols/capitol4.txt
>3.Fer un commit amb el missatge "Afegit capítol 4."
*git commit -m «Afegit capitol 4»
>4.Mostrar la història del repositori incloent totes les branques
*git log –all –oneline --graph
##Exercici 3:
>1. Canvia a la branca bibliografia.
*git checkout bibliografia
>2. Crea el fitxer bibliografia.txt i afegir la següent referència:
*echo «Afegir els canvis a la zona d’intercanvi temporal» > bibliografia.txt
>3. Afegeix els canvis a la zona d'intercanvi temporal.
*git add bibliografia.txt
>4. Fes un commit amb el missatge "Afegida primera referència bibliogràfica."
*git commit -m «Afegida primera refréncia blibliogràfica»
>5. Mostra la història del repositori incloent totes les branques.
*git log –all –oneline --graph
##Exercici 4
>1.Fusiona la branca bibliografia amb la branca master.
*git checkout master
>2.Mostra la història del repositori incloent totes les branques.
*git merge bibliografia
>3.Elimina la branca bibliografia.
*git branch -d bibliografia
>4.Mostra de nou la història del repositori incloent totes les branques.
*git log –all –oneline --graph
##Exercici 5
>1.Crea la branca bibliografia.
*git branch bibliografia
>2.Canvia a la branca bibliografia.
*git checkout bibliografia
>3.Canvia el fitxer bibliografia.txt perquè continga les següents referències:
*echo «Nova referència bibliogràfica» > bibliografia.txt
>4.Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge
"Afegida nova referència bibliogràfica."
*git add bibliografia.txt
*git commit -m «Afegida nova referencia bibliogràfica»
>5.Canvia a la branca master.
*git checkout master
>6.Canvia el fitxer bibliografia.txt perquè continga les següents referències:
*echo «Nova referència bibliogràfica» > bibliografia.txt
>7.Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge
"Afegida nova referència bibliogràfica."
*git add bibliografia.txt
*git commit -m «Afegida nova referència bibliogràfica»
>8.Fusiona la branca bibliografia amb la branca master.
*git merge bibliografia
>9.Resol el conflicte deixant el fitxer bibliografia.txt amb les referències:
>10.Afegeix els canvis a la zona d'intercanvi temporal i fes un commit amb el
missatge "Resolt conflicte de bibliografia."
*git add bibliografia
*git commit -m «Resolt conflicte de bibliografia»
>11.Mostra la història del repositori incloent totes les branques.
*git log –all –oneline --graph
