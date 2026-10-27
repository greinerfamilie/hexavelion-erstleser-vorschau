# GitHub-Erstleser-Vorschau V334 — ausdrücklich noch nicht veröffentlicht

**Grundlage:** bestehende Arbeitsfassung V1.00.333, Originalansichten aus der Quelle V1.00.332.

## Zweck
Die echten grafischen Originalansichten der Anmeldung, des Willkommensablaufs und der Erstleser-Startumfrage in einem klar getrennten statischen Test zeigen; ohne Netlify-Login über einen Weiter-Button navigieren und die echte veröffentlichte Tally-Umfrage Gx2Y7Z als eingebettetes Formular testen.

## Was funktioniert und was nicht
- Das Layout der Leser-Anmeldung ist original, aber diese Vorschau deaktiviert die Anmelde- und Registrierungsfelder. Der Netlify-Identity-Quellcode wurde NICHT überschrieben oder gelöscht.
- Die Erstleser-Startumfrage ist das echte Tally-Formular, kein nachgebautes Formular. Es war am 27.10.2026 veröffentlicht und offen.
- Das Formular nutzt KEINE erfundene `leser_id`, KEINEN gefälschten HMAC-Nachweis und KEINE Netlify-Funktionen. Es sendet nur den Hidden-Field-Wert `version=V1.00.334-GITHUB-VORSCHAU-UNBESTAETIGT`.
- Reale Antwortabgabe kann eine Antwort in Tally erzeugen, aber KEINE bestätigte Leser-Einreichung. Testantworten explizit als TEST kennzeichnen. Vor und nach dem Test den Submission-Zähler prüfen. Tally-Eingang und korrekte Antworten sind erst nach Prüfung in Tally bewiesen.
- Der Button zur Leseansicht zeigt ausschließlich einen Platzhalter, nicht den Prolog oder andere Buchtexte. Er prüft NICHT, ob die Umfrage abgesendet wurde.
- KEIN GitHub-Pages-Deployment wurde durchgeführt. Kein GitHub-Commit, kein Netlify-Deploy.

## Sicher veröffentlichen, erst nach ausdrücklicher Freigabe
Dieses Verzeichnis ist ausschließlich die statische Vorschau. NUR diesen Inhalt in eine ausdrücklich dafür bestimmte isolierte GitHub-Pages-Testseite geben, **NICHT** in das mit Netlify verbundene Repository hochladen; sonst könnte dort automatisch ein Netlify-Preview-Build anlaufen. GitHub Pages ist möglicherweise öffentlich: Niemand sollte dort echte Zugangsdaten eingeben. Keine Buchtexte/Schlüssel/geschützten Funktionen hinzufügen.

## Originalgrafiken
Es wurden ausschließlich sechs für die drei Ansichten benötigte Originalgrafiken aus `public/index.html` aus dem Quellarchiv extrahiert. Sie wurden nicht verändert oder neu generiert. Originalansichten sind als abgeleitete Kopien gesichert, die Hauptquelle V333 bleibt unverändert. Die originale Oleo-Schriftdatei ist nicht Bestandteil des Weitergabepakets, wodurch browserabhängig Schriftabweichungen möglich sind.

## Keine Datenbank
Niemals Netlify Database oder eine andere Datenbank automatisch erstellen, aktivieren, provisionieren oder migrieren. Diese statische Vorschau enthält keinerlei Datenbankcode und keinen automatischen Build.
