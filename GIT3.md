TEMA 3
CREACIÓ I ACTUALITZACIÓ DE REPOSITORIS
=====================================================
##-- Exercici 3 GIT 3:Desfer canvis --
Indica els comandaments amb els quals resoldries els escenaris plantejats en esl diferents
exercicis.
##Exercici 1
>1.Elimina l'última línia del fitxer índex.txt i guarda-ho.
*nano index.txt
>2.Comprova l'estat del repositori.
*git status
>3.Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del
fitxer.
*git checkout – index.txt
>4.Torna a comprovar l'estat del repositori.
*git status
##Exercici 2
>1.Elimina l'última línia del fitxer índex.txt i guarda-ho.
*nano index.txt
>2.Afegeix els canvis a la zona d'intercanvi temporal.
*git add index.txt
>3.Comprova de nou l'estat del repositori.
*git status
>4.Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de
treball.
*git reset HEAD index.txt
>5.Comprova de nou l'estat del repositori.
*git status
>6.Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del
fitxer.
*git checkout -- index.txt
>7.Torna a comprovar l'estat del repositori.
*git status
##Exercici 3:
>1. Elimina l'última línia del fitxer índex.txt i guardar-ho.
*nano index.txt
>2. Elimina el fitxer capítols/capitol3.txt.
*rm capitols/capitol3.txt
>3. Afegeix un fitxer nou capítols/capitol4.txt buit.
*touch capitols/capitol4.txt
>4. Afegeix els canvis a la zona d'intercanvi temporal.
*git add index.txt capitols/capitol3.txt capitols/capitol4.txt
>5. Comprova de nou l'estat del repositori.
*git status
>6. Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de
treball.
*git reset HEAD index.txt capitols/capitol3.txt capitols/capitol4.txt
>7. Comprova de nou l'estat del repositori.
*git status
>8. Desfés els canvis realitzats per tornar a la versió del repositori.
*git checkout --.
>9. Torna a comprovar l'estat del repositori.
*git status
##Exercici 4
>1.Elimina l'última línia del fitxer índex.txt i guardar-ho.
*nano index.txt
>2.Elimina el fitxer capítols/capitol3.txt.
*rm capitols/capitol.txt
>3.Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge
"Borrat accidental."
*git add index.txt
*git commit -m «Borrar accidental»
>4.Comprova l'historial del repositori.
*git log
>5.Desfés l'últim commit, però mantin els canvis anteriors al directori de treball i a la
zona d'intercanvi temporal.
*git reset HEAD
>6.Comprova l'historial i l'estat del repositori.
*git log
>7.Torna a fer el commit amb el mateix missatge d'abans.
*git commit -c ORIG_HEAD
>8.Desfés l'últim commit i els canvis anteriors al directori de treball, tornant a la
versió anterior del repositori.
*git reset –hard ORIG_HEAD
>9.Comprova de nou l'historial i l'estat del repositori.
*git log
*git status
