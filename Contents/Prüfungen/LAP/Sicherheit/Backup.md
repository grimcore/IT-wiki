---
undefined: ""
File: Contents/Prüfungen/LAP/Sicherheit/Backup.md
sticker: lucide//book-open-check
---

## Welche Aufbewahrungsfristen für Backups gibt es in Österreich?

Für steuerlich relevante Dokumente und Unterlagen und Unternehmen, die dem Unternehmensgesetzbuch (UGB) (Unternehmensdokumente, Geschäftsbriefe und Verträge) unterliegen gilt eine 7 jährige Aufbewahrungsfrist. Gemäß der DSGVO dürfen Daten nur so lange wie nötig aufbewahrt werden. Branchenintern werden Fristen von 3-12 Monaten empfohlen. 

## Erklären Sie den Zweck eines Backups.

Der Zweck eines Backups ist es, eine Sicherheitskopie von wichtigen Daten zu erstellen, um diese im Falle von Datenverlust, Beschädigung oder Diebstahl wiederherstellen zu können. Es dient der Datenwiederherstellung und dem Schutz vor technischen Ausfällen, Cyberangriffen oder Fehlern.

## Welche Sicherungskonzepte kennen Sie?

- **Vollbackup**: Eine vollständige Sicherung aller Daten.
- **Inkrementelles** Backup: Sichert nur die Änderungen seit dem letzten Backup.
- **Differenzielles** Backup: Sichert alle Änderungen seit dem letzten Vollbackup.
- **Spiegel-Backup**: Erzeugt eine exakte Kopie der Daten in Echtzeit.
- **Wöchentliche/Monatliche Backups**: Regelmäßige, zeitlich festgelegte Sicherungen.

## Welche Sicherungsmedien für Backups kennen Sie?

- Externe Festplatten
- Magnetbänder (z. B. LTO)
- USB-Sticks
- Netzwerkspeicher (NAS)
- Cloud-Speicher
- Optische Medien (z. B. DVDs, Blu-ray)

## Nennen Sie Beispiele für Software, mit welcher Backups erstellt werden können.

Acronis True Image, Veeam Backup & Replication und Macrium Reflect, EaseUS Todo Backup, Clonezilla, Windows-Backup, Carbonite (Cloudlösung) und Crash Plan (Cloudlösung)

## Was muss bei einem Datenbankbackup beachtet werden?

Bei einem Datenbank-Backup muss darauf geachtet werden, dass die Datenbank entweder in einem konsistenten Zustand gesichert wird, um Datenverlust oder -korruption zu vermeiden. Dies kann durch konsistente Snapshots oder durch die Verwendung von Transaktionslogs erreicht werden, die alle Änderungen protokollieren. Es ist auch wichtig, dass während des Backups keine Schreibvorgänge auf der Datenbank erfolgen (außer bei sogenannten Online-Backups). Zusätzlich sollten regelmäßige Testwiederherstellungen durchgeführt werden, um die Integrität der Backups sicherzustellen.

## Was sind möglichst ideale Orte um Datenträger von Backups aufzubewahren?

Ideale Orte zur Aufbewahrung von Datenträgern für Backups sind sichere, gut klimatisierte Räume wie ein Datenzentrum oder ein Serverraum, um Schäden durch extreme Temperaturen oder Feuchtigkeit zu vermeiden. Zusätzlich sollten Backups an einem externen, geografisch getrennten Standort (z. B. in der Cloud oder in einem offsite Storage-Bereich) aufbewahrt werden, um sie vor lokalen Katastrophen wie Bränden oder Überschwemmungen zu schützen.

## Was muss bei einem Cloud-Backup beachtet werden?

Bei einem Cloud-Backup muss auf Sicherheit geachtet werden, insbesondere auf Verschlüsselung der Daten sowohl während der Übertragung als auch im Ruhezustand. Es ist wichtig, einen vertrauenswürdigen Anbieter zu wählen, der Datenschutzrichtlinien einhält und idealerweise auch ein Datenspeicherort im gewünschten geografischen Bereich bietet. Zudem sollte die Wiederherstellbarkeit regelmäßig getestet und die Backup-Strategie für die Cloud angepasst werden, um eine effiziente Nutzung und schnelle Wiederherstellung zu gewährleisten.

## Erklären Sie mögliche Ursachen für Datenverlust.

- Hardwarefehler (z. B. Festplattenausfall)
- Softwarefehler (z. B. Bugs oder Programmabstürze)
- Benutzerfehler (z. B. versehentliches Löschen von Dateien)
- Virens oder Malware-Angriffe
- Naturkatastrophen (z. B. Brände, Überschwemmungen)
- Stromausfälle oder unsachgemäße Handhabung von Datenträgern

> [!note]
Auch Fehler bei der Datensicherung oder unzureichende Backup-Strategien können zu Datenverlust führen.