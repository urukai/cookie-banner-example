Cookie-Banner-Beispiel
======================

Wir speichern im Browser, ob die Benutzer den Cookie-Banner weggeklickt haben. Je nachdem zeigen wir diesen bei einem Reload wieder an.

Chronologischer Ablauf
----------------------

1. Benutzer rufen die Website auf. Wir gehen davon aus, dass wir den Banner NICHT zeigen müssen. Mit CSS wird der Banner entsprechend versteckt.

2. Ein Skript prüft nun, ob bei dieser Website der Banner schon mal weggeklickt wude. Falls ja, finden wir im LocalStorage des Browsers eine entsprechende Information (z.B. "ja", "banner-done", 1 )

3. Wenn eine solche Information gefunden wird, machen wir nichts weiter. Der Banner erscheint nicht.

4. Wenn wir KEINE solche Information finden, bedeutet das, dass der Banner noch nie weggeklickt wurde. Also müssen wir ihn zeigen. Dazu fügen wir mit Javascript dem Banner eine passende CSS-Klasse hinzu, die ihn einblenden lässt.

5. Der Banner erscheint

6. Die Benutzer lesen die Cookie-Hinweise sehr aufmerksam durch.

7. Da sie damit einverstanden sind, klicken sie auf den Button "Akzeptieren". Dadurch wird jetzt im LocalStorage des Browsers die Information hinterlegt, dass der Banner weggeklickt wurde (besagter Wert oben, z.B. "ja", "banner-done", 1 ). Zusätzlich nehmen wir beim Banner die CSS-Klasse weg, damit er verschwindet.

8. Es beginnt wieder bei Punkt 1


