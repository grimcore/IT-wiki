---
undefined: ""
File: Contents/Prüfungen/LAP/Netzwerktechnik/LAN, WAN, WLAN, VLAN.md
---

## **Erklären Sie die Begriffe LAN und WAN inklusive ihrer Unterschiede.**

LAN (Local Area Network) und WAN (Wide Area Network) sind zwei Arten von Computernetzwerken, die sich in Größe und Reichweite unterscheiden.

### LAN

- Verbindet Geräte in einem begrenzten Bereich (z.B. Büro, Haus)
- Hohe Datenübertragungsraten
- Geringe Latenz
- Einfachere Einrichtung und Wartung
- Meist in Privatbesitz

### WAN

- Verbindet mehrere LANs über große Entfernungen
- Niedrigere Datenübertragungsraten als LANs
- Höhere Latenz
- Komplexere Einrichtung und Wartung
- Kann öffentlich oder privat sein

### Hauptunterschiede

**Reichweite**
LAN lokal begrenzt, WAN über große Distanzen

**Geschwindigkeit**
LAN schneller als WAN

**Latenz**
LAN geringer als WAN

**Kosten**
LAN günstiger als WAN

**Technologie**
LAN nutzt Ethernet, WAN verschiedene Technologien wie MPLS, VPN

**Verwaltung**
LAN einfacher zu verwalten als WAN

> [!note]
WANs ermöglichen die Verbindung von Unternehmensstandorten weltweit, während LANs für lokale Netzwerke in Gebäuden oder auf Campussen genutzt werden

## **Erklären Sie den Begriff WLAN.**

WLAN steht für Wireless Local Area Network (drahtloses lokales Netzwerk). Es ist eine Technologie zur kabellosen Verbindung von Geräten mit einem Netzwerk und dem Internet

### Hauptmerkmale von WLAN

- Nutzt Funkwellen zur Datenübertragung
- Arbeitet auf Frequenzen zwischen 2,4 und 5,7 GHz
- Ermöglicht drahtlosen Internetzugang für mehrere Geräte
- Basiert auf IEEE 802.11 Standards

> [!note]
WLAN-Netzwerke bestehen typischerweise aus einem Router als zentralem Element und verbundenen Endgeräten wie Smartphones, Laptops und Tablets[1](https://it-service.network/it-lexikon/wlan/). Die Technologie wird sowohl in privaten Haushalten als auch in Unternehmen und öffentlichen Bereichen eingesetzt. Im Gegensatz zu kabelgebundenen Netzwerken bietet WLAN mehr Flexibilität, kann aber anfälliger für Störungen und Sicherheitsrisiken sein

## **Erklären Sie den Begriff VLAN.**

VLAN steht für Virtual Local Area Network und bezeichnet ein logisches Teilnetzwerk innerhalb eines physischen Local Area Networks (LAN). 

### Hauptmerkmale 

- Unterteilung eines physischen Netzwerks in mehrere logische Segmente
- Bildung eigener Broadcast-Domänen für jedes VLAN
- Arbeitet auf Schicht 2 (Sicherungsschicht) des OSI-Modells
- Basiert auf IEEE 802.1Q Standard

### Arten von VLAN implementierung

#### Portbasiert (Untagged)
Jedem Switch-Port wird ein VLAN zugewiesen
#### Tagged (Trunk Port)
Mehrere VLANs können einen Switch-Port nutzen, Frames erhalten VLAN-Tags

### Vorteile von VLANs

- Verbesserte Netzwerksicherheit durch Segmentierung
- Erhöhte Effizienz durch Reduzierung von Broadcast-Verkehr
- Flexiblere Netzwerkorganisation ohne physische Umverkabelung
- Möglichkeit zur Priorisierung von Datenverkehr

> [!note]
VLANs ermöglichen die logische Gruppierung von Geräten unabhängig von ihrer physischen Position im Netzwerk, was besonders in größeren Unternehmensnetzwerken nützlich ist

## **Ist ein WLAN einem LAN oder einem WAN zuzuordnen? Begründen Sie.**

Ein WLAN (Wireless Local Area Network) ist einem LAN (Local Area Network) zuzuordnen. 

### Begründung

#### Reichweite
WLAN deckt, wie ein LAN, einen begrenzten lokalen Bereich ab, typischerweise innerhalb eines Gebäudes oder Campus. 

#### Funktionalität
WLAN erfüllt die gleiche Funktion wie ein LAN, nämlich die Verbindung von Geräten in einem begrenzten Bereich für den lokalen Datenaustausch. 

#### Definition
WLAN steht für "Wireless Local Area Network", was bereits in der Bezeichnung die Zugehörigkeit zum LAN-Konzept verdeutlicht. 

#### Technologie
WLAN ist im Grunde eine drahtlose Variante des LAN, die die gleichen Netzwerkprinzipien verwendet, nur ohne Kabel. 

#### Anwendungsbereich
WLANs werden, wie LANs, hauptsächlich in Heimnetzwerken, Büros oder auf Campusgeländen eingesetzt.

> [!note]
Der Hauptunterschied zu einem kabelgebundenen LAN liegt lediglich in der Übertragungsmethode (Funk statt Kabel), nicht in der grundlegenden Netzwerkstruktur oder dem Einsatzbereich

## **Ist ein VLAN einem LAN oder einem WAN zuzuordnen? Begründen Sie.**

Ein VLAN (Virtual Local Area Network) ist einem LAN (Local Area Network) zuzuordnen. 

### Begründung

#### Definition
VLAN ist eine Technologie zur Unterteilung eines physischen LANs in mehrere logische Netzwerke. 

#### Funktionsweise
VLANs arbeiten auf der gleichen Netzwerkebene wie LANs und nutzen ähnliche Technologien und Protokolle. 

#### Reichweite
VLANs operieren typischerweise innerhalb der gleichen begrenzten geografischen Reichweite wie LANs, oft innerhalb eines Gebäudes oder Campus. 

#### Zweck
VLANs dienen der Optimierung und Segmentierung von LANs, nicht der Verbindung weit entfernter Netzwerke wie WANs. 

#### Verwaltung
VLANs werden mit LAN-Geräten wie Switches verwaltet, nicht mit WAN-spezifischen Technologien.

> [!note]
Obwohl VLANs die Flexibilität von LANs erweitern, bleiben sie in ihrem Wesen und ihrer Funktionalität eng mit dem LAN-Konzept verbunden.

## **Erklären Sie den Netzwerkdienst „MPLS“ welcher von Providern zur Verfügung gestellt wird.**

MPLS (Multiprotocol Label Switching) ist ein Netzwerkdienst, der von Providern angeboten wird, um Datenverkehr effizienter und schneller durch ihr Netzwerk zu leiten. 

### Hauptmerkmale 

#### Funktionsweise
MPLS weist Datenpaketen beim Eintritt ins Netzwerk Labels zu, die Informationen über die Route enthalten. Router lesen nur diese Labels, nicht die vollständigen IP-Header, was die Weiterleitung beschleunigt. 

#### Effizienz
Durch die Label-basierte Weiterleitung werden Datenpakete schneller durch das Netzwerk geleitet, da die Routenberechnung nur einmal am Eingang erfolgt. 

#### Flexibilität
MPLS ermöglicht die Übertragung verschiedener Datentypen (z.B. Telefonie, Internet) über dieselbe Infrastruktur. 

#### Priorisierung
MPLS kann Datenpakete priorisieren und bestimmten Anwendungen garantierte Bandbreiten zuweisen. 

#### Sicherheit
MPLS-Netze bieten hohe Sicherheit, da sie als private Netzwerke betrieben werden. 

#### Anwendungsbereich
MPLS eignet sich besonders für die Kopplung großer Netze und die Erstellung von Unternehmens-VPNs.

> [!note]
MPLS verbindet die Vorteile von Switching und Routing und arbeitet zwischen den OSI-Schichten 2 und 3, weshalb es oft als "Layer 2.5"-Technologie bezeichnet wird

## **Erklären Sie den Netzwerkdienst „Leased Line“ welcher von Providern zur Verfügung gestellt wird.**

Eine Leased Line ist eine dedizierte, symmetrische Datenverbindung zwischen zwei Punkten, die von Providern für Unternehmen bereitgestellt wird.

### Hauptmerkmale

#### Exklusivität
Die Verbindung wird nicht mit anderen Nutzern geteilt. 

#### Symmetrische Geschwindigkeit
Upload und Download haben die gleiche Bandbreite. 

#### Hohe Zuverlässigkeit
Garantierte Verfügbarkeit durch Service Level Agreements (SLAs) von bis zu 99,99%. 

#### Skalierbarkeit
Bandbreiten von wenigen Mbit/s bis zu 100 Gbit/s möglich. 

#### Ständige Verfügbarkeit
Die Verbindung ist permanent aktiv. 

#### Geringe Latenz
Ideal für zeitkritische Anwendungen.

> [!note] 
Leased Lines eignen sich besonders für Unternehmen mit hohem Bandbreitenbedarf, die eine stabile und sichere Verbindung zwischen Standorten oder zum Internet benötigen

## **Welche Bandbreiten und Normen im Bereich WLAN kennen Sie?**

### Wichtigste WLAN-Standards und ihre Bandbreiten 

#### IEEE 802.11b

- 2,4 GHz Band, bis zu 11 Mbit/s

#### IEEE 802.11a/g 

- 802.11a: 5 GHz Band
- 802.11g: 2,4 GHz Band  

> [!note]
Beide bis zu 54 Mbit/s

#### IEEE 802.11n (Wi-Fi 4): 

- 2,4 GHz und 5 GHz Bänder
- Bis zu 600 Mbit/s (mit 4 Antennen)

#### IEEE 802.11ac (Wi-Fi 5): 

- 5 GHz Band
- Bis zu 6,93 Gbit/s (theoretisch)

#### IEEE 802.11ax (Wi-Fi 6): 

- 2,4 GHz, 5 GHz und 6 GHz Bänder
- Bis zu 9,6 Gbit/s (theoretisch)

#### IEEE 802.11ad: 

- 60 GHz Band
- Bis zu 7 Gbit/s auf kurze Distanzen

#### IEEE 802.11be (Wi-Fi 7, in Entwicklung):

- 2,4 GHz, 5 GHz und 6 GHz Bänder
- Theoretisch bis zu 46,1 Gbit/s

> [!note]
Diese Standards nutzen verschiedene Modulationsverfahren und Antennentechnologien wie MIMO, um höhere Datenraten zu erreichen. Die tatsächlichen Geschwindigkeiten sind in der Praxis oft niedriger als die theoretischen Maximalwerte

## **Was ist eine SSID?**

Eine SSID (Service Set Identifier) ist der eindeutige Name eines drahtlosen Netzwerks (WLAN). Hauptmerkmale der SSID sind:

- Dient zur Identifikation und Unterscheidung von WLAN-Netzwerken
- Besteht aus bis zu 32 Zeichen (Buchstaben, Zahlen, Sonderzeichen) 
- Wird bei der Einrichtung eines WLAN-Routers festgelegt
- Ermöglicht Geräten, verfügbare Netzwerke zu erkennen und sich zu verbinden
- Wird unverschlüsselt bei der Datenübertragung vorangestellt
- Kann sichtbar oder versteckt sein

> [!note]
Die SSID spielt eine wichtige Rolle für die Funktionalität und grundlegende Sicherheit von WLAN-Netzwerken, indem sie Benutzern erlaubt, das gewünschte Netzwerk auszuwählen und sich damit zu verbinden

## **Welche Authentifizierungsmethoden gibt es im Bereich WLAN?**

Es gibt mehrere Authentifizierungsmethoden für WLAN-Netzwerke: 

### Open System
Keine Authentifizierung, jeder Client kann sich verbinden. 

### Pre-Shared Key (PSK)
Ein gemeinsames Passwort für alle Clients, verwendet in WPA und WPA2 Personal Mode. 

### WPA3 Personal
Verwendet Simultaneous Authentication of Equals (SAE) für verbesserte Sicherheit. 

### Enterprise Mode
Nutzt individuelle Zugangsdaten (Benutzername und Passwort) für jeden Client. 

### IEEE 802.1X
Verwendet das Extensible Authentication Protocol (EAP) mit verschiedenen Methoden: 

### PEAP (Protected EAP)
Authentifizierung mit Benutzername und Passwort

### EAP-TLS
Zertifikatsbasierte Authentifizierung

### Wi-Fi Protected Setup (WPS)
Vereinfachte Authentifizierung per Knopfdruck oder PIN. 

> [!note]
Die sichersten Methoden sind derzeit WPA3 und WPA2 Enterprise mit 802.1X. Ältere Methoden wie WEP und WPA gelten als unsicher und sollten nicht mehr verwendet werden

## **Welche Möglichkeiten zur Verschlüsselung von einem WLAN gibt es?**

Es gibt mehrere Möglichkeiten zur Verschlüsselung eines WLAN-Netzwerks, die sich im Laufe der Zeit entwickelt haben.

### WEP (Wired Equivalent Privacy): 

- Ältestes Verfahren
- Gilt als unsicher und veraltet
- Verwendet statische Schlüssel mit 64, 128 oder 256 Bit Länge

### WPA (Wi-Fi Protected Access): 

- Weiterentwicklung von WEP
- Nutzt TKIP (Temporal Key Integrity Protocol)
- Ebenfalls als unsicher eingestuft

### WPA2 (Wi-Fi Protected Access 2): 

- Aktuell am weitesten verbreitet
- Verwendet AES (Advanced Encryption Standard)
- 128-Bit-Verschlüsselung
- Gilt als sicher, hat aber bekannte Schwachstellen

### WPA3 (Wi-Fi Protected Access 3): 

- Neuester Standard (seit 2018)
- Verwendet SAE (Simultaneous Authentication of Equals)
- Bietet 192-Bit-Verschlüsselung für Unternehmen
- Individuelle Datenverschlüsselung für jedes Gerät
- Stärkerer Schutz gegen Brute-Force-Angriffe

> [!note]
WPA2 und WPA3 sind die derzeit empfohlenen Verschlüsselungsmethoden, wobei WPA3 als die sicherste gilt. WEP und WPA sollten aufgrund ihrer Sicherheitsmängel nicht mehr verwendet werden

## **Was ist „Richtfunk“ und wo wird es eingesetzt?**

Richtfunk ist eine drahtlose Nachrichtenübertragung mittels Radiowellen, die von einem Ausgangspunkt auf einen definierten Zielpunkt gerichtet ist. Diese Technologie verwendet energiebündelnde Antennen, um elektromagnetische Wellen in eine bestimmte Richtung zu konzentrieren. 

### Telekommunikation
Für Hochgeschwindigkeitsverbindungen in Regionen ohne Kabelinfrastruktur und als Backup-Lösung. 

### Unternehmen und Kommunen 
Zur Verbindung von Standorten für sichere Datenkommunikation. 

### Breitbandversorgung
Für den Ausbau in nicht erschlossenen Gebieten. 

### Mobilfunk
Als Zugangs- und Transportnetz. 

### Notfallkommunikation
Als temporäre Lösung in Katastrophensituationen. 

### Rundfunkübertragung
Übertragung des Rundfunks 

### Medizin
In Krankenhäusern für die Übertragung von Röntgenbildern und Patientenakten. 

### Veranstaltungen
Zur schnellen und flexiblen Internetversorgung bei Messen oder Großveranstaltungen. 

> [!note]
Richtfunk bietet Vorteile wie hohe Übertragungsgeschwindigkeiten, geringe Störanfälligkeit und die Möglichkeit, große Distanzen zu überbrücken

## **Warum wird z.b. bei einen Hotel / Produktionsfirma ein VLAN eingerichtet?**

### Sicherheit
VLANs ermöglichen die Trennung von Gäste- und Mitarbeiternetzwerken, was den Schutz sensibler Unternehmensdaten erhöht. 

### Flexibilität
Mitarbeiter können an verschiedenen Standorten arbeiten und trotzdem im gleichen Netzwerk bleiben. 

### Effizienz
Durch die Segmentierung wird der Netzwerkverkehr reduziert, was die Gesamtleistung verbessert. 

### Priorisierung
Kritischer Datenverkehr (z.B. Buchungssysteme, Produktionssteuerung) kann priorisiert werden. 

### Kosteneinsparung
VLANs reduzieren den Bedarf an physischer Hardware. 

### Anpassungsfähigkeit
Die Netzwerkstruktur kann leicht an Änderungen in der Unternehmensorganisation angepasst werden. 

### Trennung von Diensten
In Hotels können Gäste-WLAN, Hotelmanagement und IoT-Geräte getrennt werden. In Produktionsfirmen können Büro-, Produktions- und IoT-Netzwerke isoliert werden. 

> [!note]
Diese Vorteile machen VLANs zu einer effizienten Lösung für die komplexen Netzwerkanforderungen in Hotels und Produktionsfirmen.
