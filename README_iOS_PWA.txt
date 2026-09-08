CREMERCE – iOS-PWA
==================

Inhalt
------
- dist/index.html: CREMERCE-App
- dist/manifest.webmanifest: App-Name, Farben und Icons
- dist/service-worker.js: Offline-Cache und Aktualisierung
- dist/offline.html: verständliche Offline-Seite
- dist/icons/: Icons für iPhone, iPad und andere Geräte
- docs/: Importvorlage und direkt nutzbare Beispieldaten

Wichtig
-------
Eine PWA benötigt HTTPS. Das direkte Öffnen der index.html aus dem ZIP-Ordner
reicht für Service Worker und iOS-Installation nicht. Den Inhalt des Ordners
"dist" auf einem HTTPS-Webspace veröffentlichen.

Installation auf iPhone oder iPad
---------------------------------
1. Die veröffentlichte CREMERCE-Adresse in Safari öffnen.
2. Auf "Teilen" tippen.
3. "Zum Home-Bildschirm" auswählen.
4. Mit "Hinzufügen" bestätigen.

Datenübernahme
--------------
Die Datei docs/CREMERCE_Importvorlage.csv kann in Excel bearbeitet werden.
Sie verwendet dieselben Feldnamen wie der Export in CREMERCE. Deshalb kann
eine exportierte CSV später ohne Spaltenumbau wieder importiert werden.

Beim Import gilt Marke + Asset-ID als eindeutige Kombination:
- bereits vorhanden: Datensatz wird aktualisiert
- noch nicht vorhanden: Datensatz wird ergänzt

Der HTML-Prototyp speichert Datensätze lokal auf dem jeweiligen Gerät.
Für einen gemeinsamen Echtbetrieb werden Backend, Anmeldung, Rollen,
zentrale Datenbank, Backups und serverseitige TikTok-Verbindungen benötigt.
