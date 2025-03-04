---
undefined: ""
File: Contents/Prüfungen/LAP/Netzwerktechnik/Hardware.md
sticker: lucide//book-open-check
---

## **Erklären Sie den Begriff „Switch“**

Ein **Switch** ist ein Netzwerkgerät, das Datenpakete gezielt an den richtigen Empfänger weiterleitet. Er arbeitet auf **Schicht 2 (Sicherungsschicht)** und nutzt MAC-Adressen, um den Datenverkehr effizient zu steuern. Im Gegensatz zu einem Hub sendet er Daten nicht an alle, sondern nur an das Zielgerät, was die **Netzwerkperformance verbessert** und **Kollisionen vermeidet**. Manche Switches arbeiten auch auf **Schicht 3 (Routing-Switch)** und können IP-Adressen verarbeiten.

## **Erklären Sie den Begriff „Hub“.**

Ein **Hub** ist ein einfaches Netzwerkgerät, das eingehende Datenpakete **an alle angeschlossenen Geräte** weiterleitet, unabhängig vom Empfänger. Er arbeitet auf **Schicht 1 (Bitübertragungsschicht)** und besitzt **keine Intelligenz zur Steuerung des Datenverkehrs**. Dadurch entstehen **mehr Kollisionen**, was die Netzwerkperformance verringert. Hubs werden heute kaum noch genutzt und sind durch **Switches** ersetzt worden.

## **Erklären Sie den Begriff „Repeater“.**

Ein **Repeater** ist ein Netzwerkgerät auf **Schicht 1 (Bitübertragungsschicht)**, das **Signale verstärkt und weiterleitet**, um größere Entfernungen zu überbrücken. Er nimmt schwache oder verzerrte Signale auf, regeneriert sie und sendet sie weiter, ohne die Daten zu analysieren. Repeater werden häufig in **Ethernet- und WLAN-Netzwerken** eingesetzt, um die Reichweite zu erhöhen. 

## **Erklären Sie den Begriff „Router“.**

Ein **Router** ist ein Netzwerkgerät auf **Schicht 3 (Vermittlungsschicht)**, das **Netzwerke miteinander verbindet und den Datenverkehr zwischen ihnen steuert**. Er verwendet **IP-Adressen**, um Datenpakete über das effizienteste Routing weiterzuleiten. Router ermöglichen die **Verbindung zum Internet** und können zusätzliche Funktionen wie **NAT (Network Address Translation), Firewall-Schutz und WLAN** bieten.

### Hauptfunktionen

- Verbindung von Netzwerken
- Weiterleitung von Datenpaketen
- Optimale Pfadauswahl
- Netzwerksicherheit
- NAT-Übersetzung

### Kernaufgabe

- Intelligente Weiterleitung von Daten basierend auf IP-Adressen zwischen verschiedenen Netzwerken.

## **Erklären Sie den Begriff „Bridge“.**

Eine **Bridge** ist ein Netzwerkgerät auf **Schicht 2 (Sicherungsschicht)**, das **zwei oder mehr Netzwerke mit gleicher Protokollstruktur verbindet**. Sie analysiert MAC-Adressen und entscheidet, ob Daten weitergeleitet oder gefiltert werden.

### Arten von Bridges

- **Lokale Bridge:** Verbindet zwei Netzwerke innerhalb eines Standorts.
- **Remote Bridge:** Verbindet Netzwerke über größere Distanzen, z. B. über WAN.
- **Transparent Bridge:** Arbeitet unauffällig und benötigt keine Konfiguration.

Bridges werden oft durch **Switches** ersetzt, finden aber noch Anwendung in spezialisierten Netzwerken.

  

## **Erklären Sie den Begriff „asymmetrisches Switching“.**

**Asymmetrisches Switching** ist eine Methode in Netzwerkswitches, bei der **Ports mit unterschiedlichen Bandbreiten** miteinander verbunden werden. 
Dadurch können Geräte mit **verschiedenen Geschwindigkeiten effizient kommunizieren**.

### Beispiel

Ein Switch hat:

- **Fast-Ethernet-Ports (100 Mbit/s)** für Clients
- **Gigabit-Ethernet-Ports (1 Gbit/s)** für Server

Ein asymmetrischer Switch stellt sicher, dass ein **hohes Datenaufkommen von Clients zum Server** flüssig läuft, ohne den Server auszubremsen.

### Vorteil

- Optimiert den Datenfluss zwischen langsamen und schnellen Netzwerken.

### Nachteil

- Kann zu Engpässen führen, wenn viele langsame Geräte gleichzeitig senden.

> [!note]
Wird oft in Unternehmensnetzwerken genutzt, um Server und Workstations effizient zu verbinden.

  

## **Was bedeutet der Begriff „PoE“ bzw. „FPoE“ und wo wird er es eingesetzt?**

### PoE
steht für "Power over Ethernet" und bezeichnet eine Technologie, die Daten und elektrische Energie über ein einziges Ethernet-Kabel überträgt. 

#### Haupteinsatzgebiete 

- Drahtlose Zugangspunkte
- IP-Kameras
- VoIP-Telefone
- Andere netzwerkfähige Geräte

#### Vorteile von PoE

- Vereinfachte Installation (nur ein Kabel nötig)
- Kosteneinsparungen
- Flexible Geräteplatzierung
- Intelligente Leistungssteuerung

PoE ermöglicht die Stromversorgung von Geräten an schwer zugänglichen Orten ohne zusätzliche Stromverkabelung.

### FPoE (Fiber Power over Ethernet)

**Fiber Power over Ethernet (FPoE)** ist eine Technologie, die **Daten und Strom über Glasfaserkabel** überträgt. Während herkömmliches **PoE (Power over Ethernet)** nur mit Kupferkabeln funktioniert, ermöglicht **FPoE die Energieversorgung über Glasfaser** durch spezielle Adapter oder hybride Kabel.

#### Wie funktioniert es?

- Daten werden **über Glasfaser** transportiert.
- Strom wird **parallel über separate Kupferadern** oder durch spezielle Wandler (z. B. PoE-zu-Glasfaser-Adapter) übertragen.
- Am Endgerät wird der Strom wieder in ein nutzbares Format umgewandelt.

#### Vorteile

- **Größere Reichweite** als PoE (bis zu mehreren Kilometern statt nur 100 m).
- **Keine elektromagnetischen Störungen (EMI)** durch Glasfaser.
- **Geringerer Energieverlust** über lange Strecken.

#### Einsatzbereiche

- IP-Kameras oder WLAN-Access-Points an weit entfernten Standorten.
- Industrielle Netzwerke oder smarte Städte.
- Telekommunikations- und Rechenzentrumsumgebungen.

> [!note]
FPoE ist noch nicht weit verbreitet, aber eine vielversprechende Lösung für Netzwerke, die hohe Reichweite mit Stromversorgung kombinieren müssen.  

## **Für was wird ein „Gateway“ benötigt und auf welchen Geräten wird dieses konfiguriert?**

Ein Gateway wird benötigt, um verschiedene Netzwerke mit unterschiedlichen Protokollen oder Datenformaten miteinander zu verbinden und die Kommunikation zwischen ihnen zu ermöglichen. Es dient als Brücke zwischen Netzwerken.

### Hauptfunktionen

- Datenrouting
- Protokollumwandlung
- Sicherheitsfunktionen
- Netzwerkverwaltung

### Gateway typische Geräte

- Router (oft als Kombination aus Router und Modem)
- Spezielle Gateway-Geräte (z.B. IoT-Edge-Geräte)
- Computer oder Server, die als Gateway fungieren
- Netzwerk-Switches mit Gateway-Funktionalität

> [!note]
Die Konfiguration erfolgt je nach Gerät über die Systemsteuerung, spezielle Apps oder Web-Interfaces

## **In welcher OSI-Schicht arbeitet üblicherweise ein Switch?**

### Layer 2 (die Datenverbindungsschicht)  
Layer 2-Switches arbeiten mit den Data-Link Layer-Adressen (MAC). Link-Layer-, Hardware- oder MAC-Layer-Adressen bezeichnen einzelne Geräte. Den meisten Hardware-Geräten wird diese Nummer bei der Herstellung fest zugewiesen.

> [!note]
Switches, die auf Layer 2 arbeiten, sind sehr schnell, weil sie die Pakete lediglich nach MAC-Adressen sortieren und ihre Layer 3-Daten nicht auf weitere Informationen untersuchen. 

### Layer 3 (die Vermittlungsschicht)  
Layer 3-Switches nutzen Netzwerk- oder IP-Adressen, die Standorte im Netzwerk bezeichnen. Ein solcher Standort kann eine Workstation, die Speicherposition eines Computers oder ein anderes Datenpaket sein, das in einem Netzwerk übertragen wird.

> [!note]
Layer 3 Switches benötigen mehr Zeit für die Untersuchung von Paketen als Layer 2-Geräte und nutzen Routing-Funktionen, um die besten Übertragungswege der Pakete an ihr Ziel aktiv zu berechnen.

  

## **In welcher OSI-Schicht arbeitet üblicherweise ein Router?**

Ein Router arbeitet in der **Schicht 3 (Vermittlungsschicht) des OSI-Modells** und leitet Datenpakete anhand der **Ziel-IP-Adresse** im Paket-Header weiter. Er ermöglicht die Verbindung zwischen Netzwerken mit **unterschiedlichen Topologien** und sorgt für eine effiziente Datenübertragung.