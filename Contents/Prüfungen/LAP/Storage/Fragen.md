---
undefined: ""
File: Contents/Prüfungen/LAP/Storage/Fragen.md
sticker: lucide//book-open-check
---
## Was ist eine Storage? 

Storage ist ein System zur digitalen Speicherung von Daten, z. B. Festplatten, NAS, SAN oder Cloud.

## Erklären Sie den Begriff „Shared Storage“. 

Shared Storage ist ein Speicher, der von mehreren Geräten oder Servern gleichzeitig genutzt wird, z. B. NAS oder SAN.

## Welche Anschlüsse für Festplatten kennen Sie? 

- SATA
- SAS
- NVMe
- USB
- IDE
- SCSI
- eSATA

## Was ist der Unterschied von einer HDD zu einer SSD? 

HDDs nutzen magnetische Scheiben, sind langsamer und mechanisch. SSDs nutzen Flash-Speicher, sind schneller und ohne bewegliche Teile.

## Erklären Sie den Unterschied von SAS zu SATA. 

SAS ist schneller, zuverlässiger und für Server ausgelegt. SATA ist günstiger, langsamer und für Endgeräte geeignet.

## Wie funktionieren Bandlaufwerke? 

Bandlaufwerke speichern Daten sequenziell auf magnetischem Band, ideal für Archivierung und große Datenmengen.

## Wie funktionieren optische Speichermedien? 

Daten werden mit einem Laser auf eine reflektierende Schicht geschrieben und durch Lichtreflexion gelesen.

## Was ist eine SAN? 

Storage Area Network ist ein Hochgeschwindigkeitsnetzwerk, das Server mit Speichersystemen verbindet und blockbasierten Speicher bereitstellt.

## Was ist ein HBA? 

Host Bus Adapter verbindet Server mit Speichersystemen, z. B. in SANs, und steuert den Datentransfer.

## Was bedeutet Fibre Channel (FC)? 

Ein Hochgeschwindigkeitsprotokoll für den Datentransfer in SANs, meist über Glasfaser.

## Was ist ein Fibre Channel Switch? 

Ein Fibre Channel Switch verbindet Geräte in einem SAN und leitet Datenpakete zwischen Servern und Speichersystemen über das Fibre Channel-Protokoll. Er ermöglicht schnelle, zuverlässige und skalierbare Verbindungen.

## Was ist eine NAS? 

Network Attached Storage ist ein netzwerkgebundener Speicher, der Dateien für mehrere Geräte bereitstellt.

## Erklären Sie den Begriff „WORM“. 

Write Once, Read Many beschreibt Speichermedien, auf die Daten einmalig geschrieben und danach nur gelesen werden können.

## Wo und Weshalb wird „WORM“ eingesetzt? 

WORM wird in Archivierungssystemen eingesetzt, um Daten vor Manipulation zu schützen, z. B. in der Buchhaltung oder bei rechtlich relevanten Dokumenten.

## Was bedeutet „RAID“?

Redundant Array of Independent Disks kombiniert mehrere Festplatten für höhere Leistung, Ausfallsicherheit oder beides.

## Welche Arten von „RAID“ kennen Sie und beschreiben Sie diese näher? 

### RAID 0

Aufteilung

- hohe Leistung
- keine Redundanz

### RAID 1

Spiegelung

- hohe Redundanz
- geringere Kapazität

### RAID 5

Kombination aus Aufteilung mit Parität

- Redundanz 
- Effizienz

### RAID 10

Kombination aus RAID 1 / 0 

- hohe Leistung 
- Redundanz

## Erklären Sie den Unterschied von Brutto- und Nettospeicher bei RAID. 

### Bruttospeicher

ist die Gesamtkapazität aller Festplatten. 

### Nettospeicher

ist die nutzbare Kapazität nach Abzug für Redundanz (z. B. Parität bei RAID).

Neben Parität können Overhead durch Metadaten, Dateisysteme und RAID-Level-Implementierung den Nettospeicher reduzieren.
Overhead durch Metadaten entsteht, wenn RAID- oder Dateisysteme Informationen wie Dateistrukturen, Speicherzuweisungen oder Fehlerkorrekturdaten auf den Laufwerken speichern, wodurch weniger Speicher für Nutzdaten verfügbar bleibt.

#### Systeme mit Overhead durch Metadaten

- **RAID 1, 5, 6, 10**: Speichern Redundanzinformationen oder Paritätsdaten.
- **Dateisysteme wie NTFS, ext4, Btrfs**: Speichern Dateistrukturen, Zugriffsrechte, Journaling.

#### Systeme ohne signifikanten Metadaten-Overhead:

- **RAID 0**: Keine Redundanz oder Parität, minimaler Overhead.
- **RAW-Datenträger**: Keine Dateisystemstrukturen, nur reine Daten.

## Was bedeutet „Hot-Swap“? 

Hot-Swap bedeutet, dass Komponenten wie Festplatten während des laufenden Betriebs ausgetauscht werden können, ohne das System herunterzufahren.

## Was bedeutet „Hot-Standby“? 

Hot-Standby bedeutet, dass ein Ersatzsystem oder eine Komponente bereitsteht, um bei einem Ausfall automatisch aktiv zu werden.

## Was bedeutet „BBU“ im Zusammenhang mit RAID? 

BBU (Battery Backup Unit) sichert den RAID-Controller bei Stromausfall, um zwischengespeicherte Daten zu schützen.

## Was bedeutet „FBU“ im Zusammenhang mit RAID? 

Flash Backup Unit ist ein Modul, das bei Stromausfall die Daten im RAID-Controller-Cache auf einen nichtflüchtigen Speicher (z. B. Flash) sichert.

## Erklären Sie den Begriff „FAT“. 

*File Allocation Table Dateizuordnungstabelle*

### Varianten

- **FAT12**: Für sehr kleine Medien, z. B. Disketten.
- **FAT16**: Unterstützt größere Speichermedien bis zu 2 GB.
- **FAT32**: Unterstützt Medien bis zu 2 TB mit kleineren Clustergrößen, was Speicher effizienter macht.

### Aufbau

- **Bootsektor**: Enthält Informationen über das Dateisystem und Startcode.
- **FAT-Tabellen**: Verfolgen die Belegung und Zuordnung von Speicherblöcken.
- **Datenbereich**: Speichert die tatsächlichen Dateien.

### Eigenschaften

Einfach und weit verbreitet.
Unterstützt keine erweiterten Berechtigungen oder Journaling.
Begrenzt Dateigrößen (z. B. 4 GB bei FAT32).

## Erklären Sie den Begriff „NTFS“. 

New Technology File System ist ein Dateisystem von Microsoft 
NTFS wurde 1993 mit Windows NT 3.1 eingeführt.

### Funktionen

- **Journaling**: Verhindert Datenverlust bei Abstürzen.
- **Berechtigungen**: Unterstützt Zugriffskontrollen und Sicherheitsrichtlinien.
- **Kompression**: Ermöglicht effiziente Speichernutzung.
- **Dateigrößen**: Unterstützt Dateien bis 16 Exabyte.
- **Verschlüsselung**: Bietet integrierte Verschlüsselung (EFS).

### Vorteile
- Stabil
- sicher 
- ideal für moderne Systeme
- Unterstützt große Laufwerke und komplexe Datenstrukturen

## Erklären Sie den Begriff „EXT“. 

Extended File System ist ein Dateisystem für Linux, entwickelt als erstes speziell für Unix-basierte Systeme. 
EXT wurde 1992 mit dem Linux-Kernel 0.96c eingeführt.

### Versionen

- **EXT (1992)**: Einfaches Dateisystem mit begrenzten Funktionen.
- **EXT2 (1993)**: Unterstützt größere Dateien und Speichermedien.
- **EXT3 (2001)**: Fügt Journaling für Datensicherheit hinzu.
- **EXT4 (2008)**: Verbessert Leistung, unterstützt größere Dateien und Datenträger.

>[!note]
EXT ist effizient und speziell für Linux optimiert.

## Erklären Sie den Begriff „ReFS“. 

Resilient File System ist ein Dateisystem von Microsoft, entwickelt für hohe Zuverlässigkeit, Skalierbarkeit und Datenintegrität.
ReFS wurde 2012 mit Windows Server 2012 eingeführt.

### Eigenschaften

- **Datenintegrität**: Erkennung und automatische Korrektur von Datenfehlern.
- **Hohe Skalierbarkeit**: Unterstützt große Dateien, Volumes und Metadaten.
- **Optimierung**: Für Virtualisierung und Speicherpools (z. B. mit Storage Spaces).
- **Kein Journaling**: Nutzt stattdessen Metadatenintegrität.

ReFS wird heute vor allem in Windows Server-Umgebungen genutzt, insbesondere für Storage Spaces, Virtualisierung (z. B. Hyper-V) und Workloads, die hohe Skalierbarkeit und Datenintegrität erfordern.

### Relevanz

In Server- und Cloud-Szenarien hoch relevant.
Im Consumer-Bereich weniger verbreitet, da NTFS dort weiterhin dominiert.
Stetige Weiterentwicklung, aber keine vollständige Ablösung von NTFS.