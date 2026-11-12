Konsignationsabgleich – Webversion (für Kamera-Scan am Handy)
=============================================================

Warum eine eigene Webadresse?
Die Kamera im Handy-Browser funktioniert nur über eine verschlüsselte Verbindung (HTTPS).
Die Datei index.html muss deshalb auf einem Webserver mit HTTPS liegen.
Die Claude-Artefakt-Version kann keine Kamera nutzen.

Was ist in diesem Ordner?
- index.html: das komplette Tool in einer Datei. Alle Artikeldaten sind eingebaut,
  es ist keine Installation und kein Internetzugriff auf eigene Daten nötig.

Einrichtung (Beispiel Synology Web Station oder Hostpoint)
1. Bei Synology: Web Station aktivieren, HTTPS mit Zertifikat einrichten
   (z. B. Let's Encrypt in der Systemsteuerung). Bei Hostpoint: Webhosting mit HTTPS verwenden.
2. Ordner anlegen, z. B. konsignation/
3. index.html in diesen Ordner hochladen (Datei-Station bzw. FTP/SFTP-Zugang von Hostpoint).
4. Im Handy-Browser (Safari) öffnen: https://DEINE-ADRESSE/konsignation/
5. Beim ersten Öffnen Kamera-Zugriff erlauben.

Wichtig
- Zugriff nur für dich: Den Ordner mit einem Passwort schützen (Web Station bzw. Hostpoint-Zugriffsschutz),
  da die Seite Bestandsdaten enthält.
- Die Soll-PDF wird bei jedem Durchgang neu ausgewählt. Sie wird nicht gespeichert.
- Der CSV-Export speichert eine Datei auf dem Gerät.
- Ein Test mit einem echten Scan am Handy steht noch aus. Bitte beim ersten Mal eine Position prüfen.
