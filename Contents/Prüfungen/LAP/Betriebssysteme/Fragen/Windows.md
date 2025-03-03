---
undefined: ""
File: Contents/Prüfungen/LAP/Betriebssysteme/Windows.md
---

## Was ist ein „Betriebssystem“?

Ein Betriebssystem ist eine grundlegende Software, die als Schnittstelle zwischen der Hardware und der Anwendungssoftware eines Computers fungiert.

### Hauptaufgaben

- **Ressourcenverwaltung**: Verwaltet Arbeitsspeicher, Festplatten und andere Hardware-Komponenten
- **Prozessverwaltung**: Steuert die Ausführung von Programmen und verteilt Prozessorzeit
- **Dateiverwaltung**: Organisiert das Speichern und Abrufen von Daten
- **Geräteverwaltung**: Koordiniert die Kommunikation mit Ein- und Ausgabegeräten

### Funktionsweise

Das Betriebssystem ist hierarchisch in Schichten aufgebaut.

- Der Kernel bildet die unterste Schicht und kommuniziert direkt mit der Hardware
- Darüber liegen weitere Verwaltungsschichten
- Die Benutzeroberfläche bildet die oberste Schicht zur Interaktion mit dem Benutzer

### Bedeutung

Ohne Betriebssystem wäre ein Computer praktisch nutzlos. Es ermöglicht:

- Die Ausführung von Programmen
- Den Zugriff auf Daten
- Die Kommunikation zwischen verschiedenen Hardwarekomponenten
- Eine benutzerfreundliche Bedienung des Computers

### Sicherheitsaspekte

Moderne Betriebssysteme bieten wichtige Schutzfunktionen:

- Speicherschutz
- Begrenzte Benutzerrechte
- Schutz vor Systemabstürzen
- Abwehr von externen Angriffen

## Welche Windows Client-Betriebssysteme kennen Sie?

### Windows 9x-Serie

- Windows 95 (1995)
- Windows 98 (1998)
- Windows ME (1999)

### Windows NT-basierte Systeme

- Windows 2000 (2000)
- Windows XP (2001)
- Windows Vista (2007)
- Windows 7 (2009)
- Windows 8 (2012)
- Windows 8.1 (2013)
- Windows 10 (2015)
- Windows 11 (2021)

### Besondere Merkmale

- Ab Windows XP bis Windows 10 waren alle Systeme als 32-Bit- und 64-Bit-Version verfügbar
- Windows 11 ist nur noch als 64-Bit-Version erhältlich
- Windows RT war eine spezielle Version für ARM-Prozessoren, wurde aber 2015 eingestellt

## Was sind die größten Unterschiede zwischen den Client-Betriebssystemen?**

### Windows-Entwicklung: Zwei Hauptlinien

#### 9x-Serie (Windows 95-ME)

- Erste eigenständige Betriebssysteme
- Einführung langer Dateinamen und USB
- Multimedia-Erweiterungen

#### NT-basierte Systeme

##### Entwicklungsphasen

- Windows NT 3.1 - 4.0: Modularer Aufbau
- Windows 2000/XP: Vereinigung Consumer/Business
- Windows Vista - 7: Sicherheit und Benutzeroberfläche
- Windows 8: Touch-orientiert
- Windows 10: Vereinigung klassischer/moderner Funktionen
- Windows 11: Modernes Design, höhere Sicherheitsanforderungen

##### Technische Entwicklung

- Von 16/32-Bit zu 64-Bit
- Steigende Hardware-Anforderungen
- Verbesserte Stabilität und Sicherheit
- Cloud- und Sicherheitsintegration

## Welche Unterschiede gibt es zwischen 32 und 64 Bit Betriebssystemen?

| **Aspekt**             | **32-Bit**                                                          | **64-Bit**                                                           |
| ---------------------- | ------------------------------------------------------------------- | -------------------------------------------------------------------- |
| Speicherverwaltung     | - Max. 4 GB RAM  <br>- Pro Programm max. 2 GB RAM                   | - Bis zu 16 Exbibyte RAM  <br>- Größere Speicherverwaltung           |
| Leistung               | - Langsamere Datenverarbeitung  <br>- Mehrere Verarbeitungszyklen   | - Schnellere Datenverarbeitung  <br>- Effizienteres Multitasking     |
| Kompatibilität         | - Läuft auf älteren Systemen                                        | - 32-Bit Programme kompatibel  <br>- 64-Bit Programme nur auf 64-Bit |
| Hardware-Anforderungen | - Geringere Systemanforderungen  <br>- Für ältere Computer geeignet | - Benötigt 64-Bit Prozessor  <br>- Für moderne Hardware optimiert    |
| Sicherheit             | - Grundlegende Sicherheitsfunktionen                                | - Verbesserte Sicherheitsfeatures  <br>- Bessere Fehlererkennung     |

## Welche Windows Server-Betriebssysteme kennen Sie?

### Moderne Server-Versionen

- Windows Server 2012 (2012)
- Windows Server 2012 R2
- Windows Server 2016
- Windows Server 2019
- Windows Server 2022 (2021)
- Windows Server 2025 (kommend)

### Typische Editionen pro Version

- Standard Edition
- Enterprise Edition (bei älteren Versionen)
- Datacenter Edition
- Essentials Edition (bei neueren Versionen)

> [!note]
Die aktuelle Version ist Windows Server 2022, während Windows Server 2025 als nächste Version in Entwicklung ist und auf Windows 11 basieren wird.

## Wozu dient die Registry und welche Informationen werden dort gespeichert?

Die Windows Registry ist eine zentrale hierarchische Datenbank, die kritische Einstellungen und Konfigurationen für das Betriebssystem verwaltet.

### Hauptfunktionen

- Speicherung von Systemkonfigurationen und Einstellungen
- Verwaltung von Benutzereinstellungen und -profilen
- Speicherung von Hardware- und Softwarekonfigurationen
- Zentrale Ablage für Programmeinstellungen

### Gespeicherte Informationen

- Systemeinstellungen: Grundlegende Windows-Konfigurationen
- Benutzerprofile: Individuelle Einstellungen für jeden Benutzer
- Programmeinstellungen: Konfigurationen installierter Software
- Hardware-Informationen: Gerätetreiber und Hardware-Konfigurationen
- Sicherheitseinstellungen: Zugriffsrechte und Berechtigungen

### Struktur

Die Registry ist hierarchisch in Schlüssel (Keys) und Werte (Values) organisiert:

- **Schlüssel**: Funktionieren wie Ordner zur Organisation
- **Unterschlüssel**: Weitere Unterteilung der Hauptschlüssel
- **Werte**: Enthalten die eigentlichen Konfigurationsdaten

**Hauptzweige (Hives)**

- **HKEY_LOCAL_MACHINE**: Systemweite Einstellungen
- **HKEY_CURRENT_USER**: Einstellungen des aktuellen Benutzers
- **HKEY_CLASSES_ROOT**: Dateizuordnungen und COM-Objekte
- **HKEY_USERS**: Alle Benutzerprofile
- **HKEY_CURRENT_CONFIG**: Aktuelle Hardware-Konfiguration