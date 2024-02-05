
# xeercici GIT 3: Desfer canvis
## Exercici 1
1. Elimina l'última línia del fitxer índex.txt i guarda-ho.
nano índex.txt
2. Comprova l'estat del repositori
git status
3. Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.
git checkout índex.txt
4. Torna a comprovar l'estat del repositori.
git status
Exercici 2
1. Elimina l'última línia del fitxer índex.txt i guarda-ho.
nano índex.txt
2. Afegeix els canvis a la zona d'intercanvi temporal.
git add índex.txt
3. Comprova de nou l'estat del repositori.
git status
4. Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.
git reset HEAD índex.txt
5. Comprova de nou l'estat del repositori.
git status
6. Desfés els canvis realitzats al fitxer índex.txt per tornar a la versió anterior del fitxer.
git checkout índex.txt
7. Torna a comprovar l'estat del repositori.
git status
Exercici 3
1. Elimina l'última línia del fitxer índex.txt i guardar-ho.
nano índex.txt
2. Elimina el fitxer capítols/capitol3.txt.
rm capítols/capitol3.txt
3. Afegeix un fitxer nou capítols/capitol4.txt buit.
nano capítols/capitol4.txt
4. Afegeix els canvis a la zona d'intercanvi temporal.
git add índex.txt capítols/capitol4.txt
5. Comprova de nou l'estat del repositori.
git status
6. Treu els canvis de la zona d'intercanvi temporal, però mantin-los al directori de treball.
git reset HEAD índex.txt capítols/capitol4.txt
7. Comprova de nou l'estat del repositori.
git status
8. Desfés els canvis realitzats per tornar a la versió del repositori.
git checkout índex.txt capítols/capitol4.txt
9. Torna a comprovar l'estat del repositori.
Git status
Exercici 4
1. Elimina l'última línia del fitxer índex.txt i guardar-ho.
nano índex.txt
2. Elimina el fitxer capítol
rm capítols/capitol3.txt
3. Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Borrat
accidental."
git add índex.txt capítols/capitol3.txt
git commit -m "Borrat accidental."
4. Comprova l'historial del repositori.
Git log
5. Desfés l'últim commit, però mantin els canvis anteriors al directori de treball i a la zona
d'intercanvi temporal.
git reset HEAD~1
6. Comprova l'historial i l'estat del repositori.
git log
7. Torna a fer el commit amb el mateix missatge d'abans.
git commit -m "Borrat accidental."
8. Desfés l'últim commit i els canvis anteriors al directori de treball, tornant a la versió anterior
del repositori.git reset HEAD~1
git checkout índex.txt capítols/capitol3.txt
9. Comprova de nou l'historial i l'estat del repositori.
git log
git status
