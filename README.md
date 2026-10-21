# IhrMotor.de Rechnungstool

Eine statische Rechnungsseite für GitLab Pages. Es werden keine Bibliotheken oder Server benötigt.

## Sichere Demo-Vorlage

Die veröffentlichten Absenderdaten sind absichtlich Platzhalter: Inhaber/Firmenname, Adresse, Telefonnummer, Umsatzsteuer-ID (`DExxxx`) und IBAN (`XXXX`). Ersetze sie erst nach Prüfung, bevor du echte Rechnungen erstellst. Die Website und der dort genannte Firmenname sowie veröffentlichte Beispielpreise sind weiterhin sichtbar, wenn das GitLab-Projekt öffentlich ist.

## Lokal verwenden

Öffne `index.html` in einem aktuellen Browser. Rechnungen und Entwürfe werden im lokalen Browser-Speicher dieses Geräts abgelegt; sie werden nicht synchronisiert oder serverseitig gesichert. Nutze **Drucken / als PDF speichern** und wähle im Druckdialog **Als PDF speichern**.

Beim ersten Öffnen ist eine klar markierte Musterrechnung mit fiktiven Kundendaten und einer Beispielposition geladen. Der Druckdialog lässt sich auch mit leeren oder unvollständigen Angaben öffnen; die gedruckte Rechnung zeigt dann einen Hinweis auf die fehlenden Angaben. Die Musterkennzeichnung kann über das Kontrollkästchen ein- und ausgeschaltet werden.

## GitLab Pages

Lege die Dateien in ein GitLab-Projekt und pushe sie auf den Standardbranch. Der Job in `.gitlab-ci.yml` veröffentlicht `index.html` über GitLab Pages.

## Vor dem produktiven Einsatz prüfen

- Absender- und Bankdaten sind absichtlich Platzhalter (`USt-IdNr.: DExxxx`, `IBAN: XXXX`).
- Die Website veröffentlicht nur den Preis für die Motorschadensanalyse; weitere Preise sind manuell einzutragen.
- Steuersätze und Pflichtangaben pro Rechnung mit der zuständigen Buchhaltung oder Steuerberatung abstimmen.
- Rechnungsarchiv und Entwürfe liegen nur im jeweiligen Browserprofil. Browserdaten löschen entfernt auch diese Daten.
