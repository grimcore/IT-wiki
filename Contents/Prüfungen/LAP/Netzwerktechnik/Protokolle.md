---
undefined: ""
File: Contents/Prüfungen/LAP/Netzwerktechnik/Protokolle.md
---
# Schichten 1 und 2

## Erklären Sie das Zugriffsverfahren „Token Passing“.

Token Passing ist ein deterministisches Medienzugriffsverfahren für Rechnernetze, das auf einer logischen Ringtopologie basiert. Die Hauptmerkmale sind: 

### Funktionsweise
Ein spezielles Datenpaket, das Token genannt wird, zirkuliert zwischen den Netzwerkstationen. 

#### 1. Sendeerlaubnis
Nur die Station, die das Token besitzt, darf Daten senden. 

#### 2. Token-Weitergabe
Nach der Datenübertragung oder wenn keine Daten zu senden sind, wird das Token an die nächste Station weitergegeben. 
#### 3. Kollisionsvermeidung
Da immer nur eine Station sendet, werden Datenkollisionen vermieden. 

### Realisierungsformen

- Token Ring (IEEE 802.5): Der Nachbar ist die physisch nächste Station.
- Token Bus (IEEE 802.4): Der Nachbar ist die logisch nächste Station.

### Einsatzgebiete
Token Passing eignet sich besonders für Netzwerke mit hoher Last und Echtzeitanwendungen. 

> [!note]
Token Passing gewährleistet eine faire Verteilung der Sendezeit und eine deterministische Übertragung, was es für bestimmte industrielle Anwendungen attraktiv macht.

## **Erklären Sie das Zugriffsverfahren „CSMA/CD“.**

CSMA/CD (Carrier Sense Multiple Access with Collision Detection) ist ein Medienzugriffsverfahren, das in Ethernet-Netzwerken verwendet wird, um den Zugriff mehrerer Stationen auf ein gemeinsames Übertragungsmedium zu regeln. 

### Funktion 

#### 1. Carrier Sense
Eine Station, die Daten senden möchte, prüft zunächst, ob das Übertragungsmedium frei ist

#### 2. Multiple Access
Wenn das Medium frei ist, beginnt die Station mit der Datenübertragung 

#### 3. Collision Detection
Während der Übertragung überwacht die sendende Station weiterhin das Medium, um mögliche Kollisionen zu erkennen 

### Bei einer Kollision 

1. Die sendenden Stationen erkennen die Kollision durch eine Spannungsänderung auf dem Kabel 
2. Ein spezielles Kollisionssignal (jam signal) wird gesendet, um alle Stationen zu informieren 
3. Alle sendenden Stationen stoppen die Übertragung und warten eine zufällige Zeitspanne, bevor sie einen erneuten Sendeversuch unternehmen 

> [!note]
CSMA/CD wird hauptsächlich in der Datenverbindungsschicht (Schicht 2 des OSI-Modells) implementiert und war besonders in älteren Ethernet-Netzwerken mit Bus-Topologie relevant. In modernen Netzwerken mit Switches und Vollduplex-Verbindungen ist CSMA/CD weniger bedeutend, da Kollisionen dort seltener auftreten

## Erklären Sie den Begriff „100baseT“.

100BaseT, auch als Fast Ethernet bekannt, ist ein Ethernet-Standard für lokale Netzwerke (LANs), der eine Datenübertragungsrate von 100 Mbit/s ermöglicht. Es ist die Weiterentwicklung des älteren 10BaseT-Standards und bietet somit eine zehnfach höhere Geschwindigkeit. 

### Hauptmerkmale von 100BaseT

1. **Übertragungsrate**: 100 Mbit/s
2. **Kabeltyp**: Twisted-Pair-Kabel
3. **Maximale Kabellänge**: 100 Meter
4. **Topologie**: Stern-Topologie mit einem zentralen Switch oder Hub

### Varianten von 100BaseT

1. **100Base-TX**: Die am häufigsten verwendete Variante, die zwei Paare von Kategorie-5-Kabeln oder höher verwendet.
2. **100Base-T4**: Verwendet vier Paare von Kategorie-3-Kabeln oder höher (veraltet).
3. **100Base-FX**: Nutzt Glasfaserkabel für längere Distanzen.

> [!note]
100BaseT verwendet, wie sein Vorgänger 10BaseT, das CSMA/CD-Zugriffsverfahren, was es zu einem "echten" Ethernet macht. Es ist abwärtskompatibel, sodass 100BaseT-Geräte in der Regel auch mit 10BaseT-Netzwerken arbeiten können. Heute sind die meisten modernen Ethernet-Geräte 10/100/1000-fähig, was bedeutet, dass sie 10BaseT, 100BaseT und 1000BaseT (Gigabit Ethernet) unterstützen

## Erklären Sie den Begriff „1000baseTX“.

### 1000Base-TX – Bedeutung und Erklärung**

**1000Base-TX** ist ein **Gigabit-Ethernet-Standard** (IEEE 802.3ab), der eine Übertragungsrate von **1 Gbit/s (1000 Mbit/s)** über **Twisted-Pair-Kupferkabel** ermöglicht.

### Merkmale

- **1000** → 1 Gbit/s Geschwindigkeit
- **Base** → Basisband-Übertragung (kein Frequenzmultiplex)
- **TX** → Twisted-Pair-Kabel (Kategorie 6 oder höher, max. 100 m)

**Unterschied zu 1000Base-T:**

- 1000Base-TX nutzt **nur zwei Aderpaare**, während 1000Base-T **vier Aderpaare** benötigt.
- **Weniger Signalverarbeitung**, aber teurere Kabel und Hardware.

**Einsatz:**

- Wird selten genutzt, da **1000Base-T günstiger** und flexibler ist.

## Erklären Sie den Begriff „1000baseSX“.

1000BASE-SX ist ein Gigabit-Ethernet-Standard für Glasfaserkabel. 

### Eigenschaften

- **Übertragungsgeschwindigkeit**: 1 Gbit/s
- **Wellenlänge**: 850 nm
- **Kabeltyp**: Multimode-Glasfaser
- **Maximale Länge**: 220-550 Meter

### Einsatzgebiete 

- Verbindungen in Bürogebäuden
- Netzwerkverbindungen zwischen Switches
- Rechenzentren

### Besonderheiten

- "SX" steht für "short wavelength"
- Kosteneffektiv für kurze Distanzen
- Verwendet LC-Steckverbinder

## Erklären Sie den Begriff „1000baseLX“.

1000BASE-LX ist ein Gigabit-Ethernet-Standard für Glasfaserkabel

### Eigenschaften 

- **Übertragungsgeschwindigkeit**: 1 Gbit/s
- **Wellenlänge**: 1270 bis 1355 nm (typischerweise 1310 nm)
- **Kabeltyp**: Singlemode-Glasfaser (SMF) oder Multimode-Glasfaser (MMF)
- **Maximale Kabellänge**: 10 km über Singlemode-Faser


### Besonderheiten

- "LX" steht für "long wavelength" und "long reach"
- Geeignet für längere Strecken als 1000BASE-SX
- Weit verbreitet in Unternehmensnetzwerken aufgrund der Reichweite und Kosteneffizienz
- Einige Hersteller bieten erweiterte Reichweiten von bis zu 20 km an

> [!note]
1000BASE-LX wird häufig für Verbindungen zwischen Gebäuden oder in größeren Netzwerkinfrastrukturen eingesetzt

## Wozu dient das „Spanning-Tree“ Protokoll?

Das Spanning-Tree-Protokoll (STP) dient hauptsächlich dazu, Schleifen in Ethernet-Netzwerken zu verhindern und eine schleifenfreie Baumstruktur zu bilden. 

### Funktionen

1. Vermeidung von Netzwerkschleifen in Switch-Infrastrukturen
2. Sicherstellung einer eindeutigen Weiterleitung von Datenpaketen
3. Verhinderung von Broadcast-Stürmen und Überlastung von Netzwerkressourcen
4. Schaffung einer effizienten und fehlertoleranten Baumtopologie
5. Ermöglichung von Netzwerkredundanz ohne deren negative Auswirkungen

> [!note]
STP arbeitet auf Layer 2 des OSI-Modells und tauscht Informationen zwischen Switches mittels Bridge Protocol Data Units (BPDUs) aus. Bei Ausfällen oder Unterbrechungen reorganisiert das Protokoll automatisch die Netzwerkstruktur, um neue optimale Verbindungspfade zu ermitteln

  

## Was bedeutet „Root Bridge“ im Spanning-Tree Protokoll?

Die Root Bridge ist ein zentrales Konzept im Spanning-Tree-Protokoll (STP)

### Übersicht

- Sie dient als Referenzpunkt für alle anderen Switches im Netzwerk
- Es ist der Switch mit der niedrigsten Bridge-ID
- Die Bridge-ID setzt sich aus der Bridge-Priorität und der MAC-Adresse zusammen
- Standardmäßig haben alle Switches eine Bridge-Priorität von 32768
- Bei gleicher Priorität wird die MAC-Adresse als Tiebreaker verwendet

### Funktionen der Root Bridge

- Bildet die Wurzel der Baumstruktur im Netzwerk
- Alle anderen Switches berechnen den kürzesten Pfad zur Root Bridge
- Dient zur Vermeidung von Schleifen im Netzwerk

> [!note]
Die Auswahl der Root Bridge erfolgt automatisch durch den Vergleich der Bridge-IDs zwischen den Switches. Netzwerkadministratoren können die Wahl beeinflussen, indem sie einem gewünschten Switch eine niedrigere Priorität zuweisen

## Was definiert die Norm 802.1q?

Die Norm IEEE 802.1Q definiert den Standard für Virtual Local Area Networks (VLANs) in Ethernet-Netzwerken. 

### Hauptmerkmale

- Unterstützung von bis zu **4.096 VLANs** durch ein 12-Bit VLAN-ID-Feld
- Einfügen eines **4-Byte-Tags** in den Ethernet-Frame **zwischen Quelladresse und Typ/Länge-Feld**
- Ermöglicht paketbasierte Tagged VLANs statt nur portbasierter VLANs
- Beinhaltet auch eine Priorisierungsmöglichkeit für Datenverkehr (Class of Service)

### 802.1Q-Tag

- 16 Bit Tag Protocol Identifier (TPID)
- 16 Bit Tag Control Information (TCI) mit VLAN-ID, Prioritätsinformationen und Canonical Format Indicator

> [!note]
802.1Q ermöglicht die effiziente Segmentierung von Netzwerken und verbessert die Sicherheit, da Datenpakete nur zwischen Mitgliedern desselben VLANs übermittelt werden können

## Was versteht man unter einem Tagged Ethernet Frame?

Ein Tagged Ethernet Frame ist ein erweiterter Ethernet-Frame, der zusätzliche Informationen für Virtual Local Area Networks (VLANs) enthält.

### Hauptmerkmale

- Ein 4-Byte (32-Bit) VLAN-Tag wird nach den Quell- und Ziel-MAC-Adressen eingefügt
- Das Tag enthält die VLAN-ID und Prioritätsinformationen.
- Es ermöglicht die Zuordnung des Frames zu einem bestimmten VLAN.
- Basiert auf dem IEEE 802.1Q-Standard

### Bestandteile 

- Tag Protocol Identifier (TPI): 2 Bytes, Wert 0x8100 für 802.1Q
- 3 Bits für Priorität
- 1 Bit für den Canonical Format Identifier (CFI)
- 12 Bits für die VLAN-ID, ermöglicht bis zu 4.096 verschiedene VLANs

### Tagged Frames ermöglichen

- Dynamische VLAN-Zuweisung
- Trennung und Priorisierung von Netzwerkverkehr
- Erhöhte Flexibilität und Skalierbarkeit in Netzwerken

> [!note]
Tagged Ethernet Frames werden hauptsächlich zwischen VLAN-fähigen Switches verwendet, um VLANs über mehrere Switches hinweg zu unterstützen.

# Schichten 3 und 4

## Nennen Sie verschiedene Netzwerkprotokolle der Schichten 3 und 4.

### Netzwerkprotokolle der Schicht 3 (Vermittlungsschicht)

- IP (Internet Protocol) - sowohl IPv4 als auch IPv6
- ICMP (Internet Control Message Protocol)
- IPsec
- X.25

### Netzwerkprotokolle der Schicht 4 (Transportschicht)

- TCP (Transmission Control Protocol)
- UDP (User Datagram Protocol)
- SCTP (Stream Control Transmission Protocol)
- DCCP (Datagram Congestion Control Protocol)

> [!note]
Diese Protokolle erfüllen unterschiedliche Aufgaben in den jeweiligen Schichten. Während Schicht-3-Protokolle wie IP sich um Adressierung und Routing kümmern, sind Schicht-4-Protokolle wie TCP und UDP für die zuverlässige Ende-zu-Ende-Datenübertragung zuständig

## Nennen Sie die Protokolle und Funktionen der TCP/IP Familie.

### Wichtige Protokolle

- **IP (Internet Protocol)**: Logische Adressierung und Routing von Datenpaketen
- **TCP (Transmission Control Protocol)**: Zuverlässige, verbindungsorientierte Datenübertragung
- **UDP (User Datagram Protocol)**: Schnelle, verbindungslose Datenübertragung
- **ICMP (Internet Control Message Protocol)**: Fehlerbehandlung und Diagnose
- **HTTP/HTTPS**: Übertragung von Webinhalten
- **DNS (Domain Name System)**: Namensauflösung
- **DHCP (Dynamic Host Configuration Protocol)**: Automatische IP-Konfiguration
- **FTP (File Transfer Protocol)**: Dateiübertragung
- **SMTP (Simple Mail Transfer Protocol)**: E-Mail-Versand

## Wie gliedert sich der TCP/IP Protokollstack in das OSI-Schichtenmodell ein?
 
### Einordnung des TCP/IP-Protokollstacks in das OSI-Schichtenmodell

Das **TCP/IP-Modell** besteht aus **vier Schichten** und wird in das **siebenstufige OSI-Modell** eingeordnet, indem mehrere OSI-Schichten zusammengefasst werden.

| **OSI-Modell (7 Schichten)** | **TCP/IP-Modell (4 Schichten)** | **Beispiele für Protokolle** |
| ---------------------------- | ------------------------------- | ---------------------------- |
| **Anwendung (7)**            | Anwendung                       | HTTP, FTP, SMTP, DNS         |
| **Darstellung (6)**          | Anwendung                       | SSL/TLS, JPEG                |
| **Sitzung (5)**              | Anwendung                       | RPC, NetBIOS                 |
| **Transport (4)**            | Transport                       | TCP, UDP                     |
| **Vermittlung (3)**          | Internet                        | IP, ICMP, ARP                |
| **Sicherung (2)**            | Netzzugang                      | Ethernet, WLAN, PPP          |
| **Bitübertragung (1)**       | Netzzugang                      | Kabel, Funktechnologien      |

### **Zusammenfassung:**

- Das **TCP/IP-Modell ist praxisnaher** und fasst die OSI-Schichten 5–7 in einer **Anwendungsschicht** zusammen.
- Die **Transportschicht bleibt gleich** (TCP, UDP).
- Die **Internetschicht entspricht der OSI-Vermittlungsschicht** (IP, ICMP).
- Die **Netzzugangsschicht kombiniert die OSI-Sicherungs- und Bitübertragungsschicht**.

Das TCP/IP-Modell ist kompakter und wurde speziell für die Internetkommunikation entwickelt, während das OSI-Modell detaillierter, aber eher theoretisch ist.

## Erklären Sie den Unterschied zwischen TCP und UDP.

### Unterschied zwischen TCP und UDP

**TCP (Transmission Control Protocol)** und **UDP (User Datagram Protocol)** sind **Transportprotokolle** im **TCP/IP-Modell** und haben unterschiedliche Eigenschaften und Einsatzzwecke.

|**Merkmal**|**TCP** (Verbindungsorientiert)|**UDP** (Verbindungslos)|
|---|---|---|
|**Verbindungsaufbau**|Ja, mit Handshake (drei Schritte)|Nein, direktes Senden|
|**Fehlersicherung**|Ja, mit Bestätigung und erneuter Übertragung|Nein, keine Bestätigung|
|**Datenreihenfolge**|Ja, Pakete werden in der richtigen Reihenfolge wiederhergestellt|Nein, Reihenfolge kann variieren|
|**Geschwindigkeit**|Langsamer durch Fehlerkorrektur|Schneller, da ohne Kontrolle|
|**Typische Anwendungen**|Web (HTTP, HTTPS), E-Mail (SMTP, IMAP), Dateiübertragung (FTP)|VoIP, Videostreaming, Online-Gaming, DNS|

### Zusammenfassung

- **TCP bietet Zuverlässigkeit**, aber ist langsamer.
- **UDP ist schnell und effizient**, aber ohne Fehlerkorrektur.
- **Einsatz hängt vom Anwendungsfall ab**: TCP für **sichere Übertragungen**, UDP für **zeitkritische Daten**.

> [!note]
> Auch wenn UDP selbst über keine Fehlerkorrektur oder Datenchecks verfügt, haben viele Programme solche Mechanismen schon selbst eingebaut. 
> Und in so einem Fall würde man nur Chaos mit TCP verursachen.

## Erklären Sie den Aufbau eines TCP Headers.

Ein TCP-Header besteht aus mehreren Feldern und hat eine Standardgröße von 20 Byte, kann aber durch optionale Felder auf bis zu 60 Byte erweitert werden. 

### Hauptkomponenten

1. **Quell-Port (16 Bit)**: Gibt die Portnummer des Senders an
2. **Ziel-Port (16 Bit)**: Gibt die Portnummer des Empfängers an
3. **Sequenznummer (32 Bit)**: Zur Validierung und Sortierung der Segmente
4. **Bestätigungsnummer (32 Bit)**: Gibt die nächste erwartete Sequenznummer an
5. **Data Offset (4 Bit)**: Zeigt die Länge des TCP-Headers in 32-Bit-Blöcken an
6. **Reserviert (4 Bit)**: Für zukünftige Verwendung, normalerweise auf Null gesetzt
7. **Flags (8 Bit)**: Kennzeichnen bestimmte Zustände (z.B. URG, ACK, PSH, RST, SYN, FIN)
8. **Fenstergröße (16 Bit)**: Für Flusskontrolle
9. **Prüfsumme (16 Bit)**: Zur Fehlererkennung
10. **Urgent Pointer (16 Bit)**: Zeigt dringende Daten an, wenn URG-Flag gesetzt ist

> [!note]
Optionale Felder können zusätzliche Informationen wie die maximale Segmentgröße (MSS) enthalten

## Erklären Sie den Aufbau eines UDP Headers.

Ein UDP-Header besteht aus vier Feldern, die jeweils 16 Bit (2 Byte) groß sind, und hat eine Gesamtgröße von 8 Byte. 

### Felder 

1. **Quell-Port**: Gibt die Portnummer des Senders an. Dieses Feld ist optional und kann auf '0' gesetzt werden, wenn keine Antwort erwartet wird. 
2. **Ziel-Port**: Gibt die Portnummer des Empfängers an. Dieses Feld ist obligatorisch für die korrekte Zuordnung des Datagramms. 
3. **Länge**: Gibt die Gesamtlänge des UDP-Datagramms in Oktetten (Bytes) an, einschließlich Header und Nutzdaten. Der Mindestwert beträgt 8 Byte. 
4. **Prüfsumme**: Dient zur Fehlererkennung. Sie wird über den Header und die Daten gebildet. 

> [!note]
Der UDP-Header ist sehr kompakt und effizient, was zu einer schnellen Verarbeitung mit wenig Rechenleistung führt

## Was ist „NAT“?

NAT (Network Address Translation) ist ein Verfahren zur Übersetzung von IP-Adressen in Computernetzwerken. Es ermöglicht mehreren Geräten in einem lokalen Netzwerk, eine einzige öffentliche IP-Adresse für den Internetzugang zu teilen. 

### Hauptmerkmale von NAT

1. **Adressübersetzung**: NAT ändert die Header von IP-Paketen, um private IP-Adressen in öffentliche umzuwandeln und umgekehrt. 
2. **Einsparung von IP-Adressen**: Es hilft, die begrenzte Anzahl öffentlicher IPv4-Adressen effizienter zu nutzen. 
3. **Sicherheit**: NAT bietet eine zusätzliche Schutzebene, indem es die interne Netzwerkstruktur verbirgt. 
4. **Implementierung**: NAT wird typischerweise in Routern oder Firewalls eingesetzt. 
5. **Arten**: Es gibt verschiedene NAT-Techniken, darunter statisches NAT (SNAT) und dynamisches NAT (DNAT). 

> [!note]
NAT spielt eine wichtige Rolle bei der Verbindung privater Netzwerke mit dem Internet und hat dazu beigetragen, die Lebensdauer von IPv4 zu verlängern

## Was ist „PAT“?

PAT (Port Address Translation) ist eine spezielle Form der Netzwerkadressübersetzung (NAT), die es ermöglicht, mehrere Geräte in einem privaten Netzwerk über eine einzige öffentliche IP-Adresse mit dem Internet zu verbinden. 

### Die Hauptmerkmale von PAT sind

- Übersetzung von privaten IP-Adressen und Portnummern in eine öffentliche IP-Adresse mit eindeutigen Portnummern
- Ermöglicht vielen Geräten die gemeinsame Nutzung einer öffentlichen IP-Adresse
- Hilft bei der Einsparung von IPv4-Adressen
- Erhöht die Sicherheit durch Verbergen der internen Netzwerkstruktur

### PAT Funktion

1. Die private IP-Adresse des sendenden Geräts durch seine eigene öffentliche IP-Adresse ersetzt
2. Die ursprüngliche Portnummer durch eine eindeutige Portnummer austauscht
3. Diese Zuordnungen in einer Übersetzungstabelle speichert

> [!note]
PAT wird häufig in Heimnetzwerken und Unternehmensumgebungen eingesetzt, um mehreren Geräten den Internetzugang über eine einzige öffentliche IP-Adresse zu ermöglichen

## Erklären Sie den Begriff „IPSEC“.

IPsec (Internet Protocol Security) ist ein Protokoll-Framework zur Sicherung von IP-Kommunikationen durch Authentifizierung und Verschlüsselung von IP-Paketen. Es wurde entwickelt, um vertrauliche Daten sicher über unsichere Netzwerke wie das Internet zu übertragen. 

### Hauptmerkmale von IPsec

- Arbeitet auf der Vermittlungsschicht (Layer 3) des OSI-Modells
- Bietet Vertraulichkeit, Integrität und Authentifizierung für IP-Pakete
- Unterstützt zwei Modi: Transport- und Tunnelmodus
- Verwendet verschiedene Protokolle wie AH (Authentication Header) und ESP (Encapsulating Security Payload)

### Kernkomponenten

1. **AH**: Bietet Authentifizierung und Integritätsschutz, aber keine Verschlüsselung
2. **ESP**: Bietet Verschlüsselung und optional Authentifizierung
3. **IKE (Internet Key Exchange)**: Verwaltet Schlüsselaustausch und Authentifizierung

### Anwendungsbereiche

- Aufbau von VPNs (Virtual Private Networks)
- Sichere Verbindungen zwischen Unternehmensstandorten
- Sicherer Fernzugriff für Remote-Mitarbeiter
- Schutz sensibler Daten in öffentlichen Netzwerken

> [!note]
IPsec ist ein wesentlicher Bestandteil moderner Netzwerksicherheit und wird in IPv6 integriert, kann aber auch mit IPv4 verwendet werden.

## Erklären Sie den Begriff „ICMP“.

ICMP (Internet Control Message Protocol) ist ein Netzwerkprotokoll, das zur Übermittlung von Kontroll- und Fehlermeldungen in IP-Netzwerken dient. Es ist Bestandteil der Internet Protocol Suite und arbeitet auf der Vermittlungsschicht (Layer 3) des OSI-Modells. 

### Hauptfunktionen von ICMP

1. **Fehlerberichterstattung**: ICMP sendet Fehlermeldungen zurück zum Absender, wenn Probleme bei der Paketübertragung auftreten.
2. **Netzwerkdiagnose**: Tools wie "Ping" nutzen ICMP-Echo-Request und -Reply-Nachrichten, um die Konnektivität zu testen.
3. **Statusinformationen**: ICMP ermöglicht den Austausch von Informationen über den Netzwerkzustand zwischen Geräten.

### Wichtige Eigenschaften

- ICMP-Nachrichten werden in IP-Datagrammen gekapselt.
- Jede ICMP-Nachricht enthält einen Typ und einen Code zur Identifikation des Problems.
- ICMP ist ein unzuverlässiges Protokoll, da Nachrichten ohne Bestätigung gesendet werden.
- Es verwendet keine Ports wie TCP oder UDP, sondern Typ- und Code-Werte.

> [!note]
ICMP spielt eine wichtige Rolle bei der Aufrechterhaltung und Fehlerbehebung in Netzwerken, indem es die Kommunikation von Problemen und Statusinformationen zwischen Netzwerkgeräten ermöglicht

## Erklären Sie den Begriff „MTU“.

MTU (Maximum Transmission Unit) bezeichnet die maximale Größe eines Datenpakets, das über ein Netzwerk übertragen werden kann, ohne fragmentiert zu werden.

### Hauptmerkmale der MTU 

- Gemessen in Bytes oder Oktetten
- Definiert die größte Paketgröße auf der Vermittlungsschicht (Layer 3) des OSI-Modells
- Variiert je nach Netzwerktechnologie und -protokoll

### Typische MTU-Werte 

- Ethernet: 1500 Bytes
- WLAN: Etwa 1500 Bytes
- PPPoE: 1492 Bytes

### MTU-Einstellungen

- Zu große MTU kann zu Paketfragmentierung und Leistungseinbußen führen
- Zu kleine MTU erhöht den Overhead durch mehr Header-Informationen

> [! note]
Eine optimale MTU-Konfiguration hilft, die Netzwerkleistung zu verbessern, indem sie die Anzahl der Pakete für eine Datenübertragung minimiert und gleichzeitig unnötige Fragmentierung vermeidet

  

## Erklären Sie den Windows Befehl „ping“.

Der Windows-Befehl "ping" ist ein Diagnose-Werkzeug zur Überprüfung der Netzwerkkonnektivität.

### Hauptfunktionen

- Testen der Erreichbarkeit eines Hosts im Netzwerk
- Messen der Antwortzeit (Latenz) zwischen zwei Geräten

### Funktionsweise

1. Sendet ICMP-Echo-Request-Pakete an eine Zieladresse
2. Wartet auf ICMP-Echo-Reply-Pakete vom Ziel
3. Standardmäßig werden in Windows vier Anfragen gesendet

## Erklären Sie den Windows Befehl „netstat“.

Der Windows-Befehl "netstat" (Network Statistics) ist ein Kommandozeilentool zur Netzwerkdiagnose und -analyse.

### Hauptfunktionen

- Anzeige aktiver TCP-Verbindungen
- Auflistung von Ports, die auf Verbindungen warten
- Darstellung von Ethernet-Statistiken
- Anzeige der IP-Routingtabelle
- Bereitstellung von Statistiken für verschiedene Netzwerkprotokolle

### Wichtige Parameter von netstat: 

- -a: Zeigt alle aktiven Verbindungen und lauschenden Ports
- -b: Zeigt die ausführbaren Programme für jede Verbindung
- -n: Stellt Adressen und Portnummern numerisch dar
- -o: Zeigt die Prozess-ID (PID) für jede Verbindung
- -p: Filtert Verbindungen nach Protokoll (z.B. TCP, UDP)
- -r: Zeigt die Routing-Tabelle an
- -s: Liefert Statistiken für verschiedene Protokolle

  

### Erklären Sie den Windows Befehl „ipconfig“.

Der Windows-Befehl "ipconfig" ist ein Kommandozeilentool zur Anzeige und Verwaltung von Netzwerkkonfigurationen.

### Hauptfunktionen

#### Anzeige von Netzwerkinformationen

- IP-Adressen (IPv4 und IPv6)
- Subnetzmaske
- Standardgateway
- DNS-Server

#### Erweiterter Informationsabruf mit "ipconfig /all": 

- MAC-Adresse (physische Adresse)
- DHCP-Status
- Hostname
- DNS-Suffix

#### Netzwerkdiagnose und -verwaltung: 

- "ipconfig /release": Gibt die aktuelle IP-Adresse frei
- "ipconfig /renew": Fordert eine neue IP-Adresse vom DHCP-Server an
- "ipconfig /flushdns": Löscht den DNS-Cache

#### DNS-bezogene Funktionen: 

- "ipconfig /displaydns": Zeigt den Inhalt des DNS-Caches an

> [!note]
Der Befehl wird in der Windows-Eingabeaufforderung (CMD) ausgeführt und ist besonders nützlich für Netzwerkadministratoren und zur Fehlerbehebung bei Netzwerkprobleme

## Erklären Sie den Windows Befehl „tracert“.

Der Windows-Befehl "tracert" (Abkürzung für Trace Route) ist ein Kommandozeilen-Tool zur Netzwerkdiagnose und -analyse.

### Hauptfunktionen

- Verfolgung des Weges von Datenpaketen durch das Netzwerk
- Anzeige der Zwischenstationen (Hops) auf dem Weg zum Ziel
- Messung der Übertragungszeiten für jeden Hop

### Funktionsweise

1. Sendet speziell präparierte Datagramme mit begrenzter Time-to-Live (TTL)
2. Jeder Router auf dem Weg reduziert die TTL um 1
3. Bei TTL 0 sendet der Router eine ICMP-Nachricht zurück
4. Tracert erhöht die TTL schrittweise, um alle Hops zu erfassen

### Verwendung

1. Öffnen der Eingabeaufforderung (CMD)
2. Eingabe: "tracert [Zieladresse]" (z.B. "tracert [www.example.com](http://www.example.com)")

### Nützliche Optionen

- -h [Zahl]: Begrenzt die maximale Anzahl der Hops
- -d: Deaktiviert die DNS-Namensauflösung für schnellere Ergebnisse
- -4 oder -6: Erzwingt die Verwendung von IPv4 oder IPv6

> [!note]
Tracert ist besonders hilfreich bei der Diagnose von Netzwerkproblemen, der Identifizierung von Engpässen und der Analyse von Routing-Pfaden

## Erklären Sie den Linux Befehl „ifconfig“.

Der Linux-Befehl "ifconfig" (Interface Configuration) ist ein Kommandozeilentool zur Konfiguration und Anzeige von Netzwerkschnittstellen. 

### Hauptfunktionen

#### Anzeige von Netzwerkinformationen

- IP-Adressen
- MAC-Adressen
- Netzmasken
- Broadcast-Adressen

#### Konfiguration von Netzwerkschnittstellen: 

- Aktivieren/Deaktivieren von Interfaces
- Ändern von IP-Adressen und Netzmasken
- Setzen von Flags

#### Verwendung

- Ohne Argumente: Zeigt Informationen aller aktiven Schnittstellen
- Mit Schnittstellenname: Zeigt Informationen der spezifischen Schnittstelle
- Mit -a Option: Zeigt alle Schnittstellen, auch inaktive

#### Beispiele

- Anzeigen aller aktiven Schnittstellen: ifconfig
- Aktivieren einer Schnittstelle: ifconfig eth0 up
- Deaktivieren einer Schnittstelle: ifconfig eth0 down
- Setzen einer IP-Adresse: ifconfig eth0 192.168.0.25 netmask 255.255.255.0

> [!note]
Obwohl ifconfig weit verbreitet ist, wird es in neueren Linux-Distributionen zunehmend durch den "ip" Befehl ersetzt. Dennoch bleibt ifconfig ein wichtiges Werkzeug für Netzwerkadministratoren zur Diagnose und Konfiguration von Netzwerkschnittstellen.

## Erklären Sie den Linux Befehl „traceroute“.

Der Linux-Befehl "traceroute" ist ein Netzwerkdiagnose-Tool, das den Weg von Datenpaketen durch ein IP-Netzwerk zu einem bestimmten Ziel verfolgt. 

### Hauptfunktionen 

- Identifizierung der Router (Hops) auf dem Weg zum Ziel
- Messung der Übertragungszeiten zwischen den Hops
- Erkennung von Netzwerkproblemen und Engpässen

### Funktionsweise

1. Sendet UDP-Pakete mit steigender Time-to-Live (TTL) 
2. Jeder Router reduziert die TTL um 1 und leitet das Paket weiter
3. Bei TTL 0 sendet der Router eine ICMP TIME_EXCEEDED Nachricht zurück
4. Traceroute erhöht die TTL schrittweise, um alle Hops zu erfassen

### Verwendung
```bash
traceroute [Optionen] [Zieladresse]
```

### Beispiel 
```bash
traceroute www.google.de
```

### Nützliche Optionen

- -n: Unterdrückt die Namensauflösung für schnellere Ergebnisse
- -q [Zahl]: Ändert die Anzahl der gesendeten Pakete pro Hop
- -i: Verwendet ICMP-Pakete statt UDP

> [!note]
Traceroute ist besonders hilfreich bei der Diagnose von Netzwerkproblemen, der Identifizierung von Routing-Pfaden und der Analyse von Netzwerkleistung

## Erklären Sie den Linux Befehl „ip“.

Der Linux-Befehl "ip" ist ein vielseitiges Kommandozeilentool zur Konfiguration und Anzeige von Netzwerkeinstellungen. Es ist Teil der iproute2-Toolsammlung und wurde als moderner Ersatz für ältere Befehle wie ifconfig entwickelt. 

### Hauptfunktionen des ip-Befehls

1. Anzeige und Konfiguration von Netzwerkschnittstellen
2. Verwaltung von IP-Adressen
3. Manipulation der Routing-Tabelle
4. Konfiguration von Tunneln und VPNs

### Syntax
```bash
ip [Optionen] Objekt {Kommando | help}  
```

### Wichtige Objekte

- **addr**: IP-Adressen verwalten
- **link**: Netzwerkschnittstellen konfigurieren
- **route**: Routing-Tabelle anzeigen und ändern

### Häufig verwendete Befehle

- **ip addr show**: Zeigt alle IP-Adressen an
- **ip link show**: Listet alle Netzwerkschnittstellen auf
- **ip route show**: Zeigt die Routing-Tabelle an

### Beispiele

- IP-Adresse anzeigen: ip addr show dev eth0
- IP-Adresse hinzufügen: ip addr add 192.168.1.10/24 dev eth0
- Schnittstelle aktivieren: ip link set eth0 up

> [!note]
Der ip-Befehl bietet mehr Flexibilität und Funktionen als ältere Tools und nutzt netlink sockets für eine effizientere Kommunikation mit dem Kernel

## Erklären Sie den Befehl „nslookup“.

Der Befehl "nslookup" (Name Server Lookup) ist ein Netzwerkdiagnosetool, das unter macOS, Windows und Unix verwendet wird, um DNS-Informationen abzufragen. 

### Hauptfunktionen

1. Auflösen von Domainnamen in IP-Adressen und umgekehrt (Reverse Lookup) 
2. Anzeigen verschiedener DNS-Einträge wie MX- oder NS-Records
3. Überprüfen und Debuggen von DNS-Problemen

### Verwendung

- **Ohne Parameter**: Startet den interaktiven Modus
- **Mit Domainname oder IP-Adresse**: Führt eine einfache Abfrage durch
- **Mit zusätzlichen Optionen**: Ermöglicht spezifische DNS-Abfragen

### Beispiele 

- Einfache Abfrage: nslookup [www.example.com](http://www.example.com)
- MX-Record Abfrage: nslookup -q=mx example.com
- Verwendung eines bestimmten DNS-Servers: nslookup example.com 8.8.8.8

> [!note]
Obwohl nslookup weit verbreitet ist, wird es zunehmend durch modernere Alternativen wie den "dig" Befehl ersetzt

# Schichten 5 bis 7

## Erklären Sie das DHCP-Protokoll.

Das DHCP-Protokoll (Dynamic Host Configuration Protocol) ist ein Netzwerkprotokoll zur automatischen Zuweisung von IP-Adressen und anderen Netzwerkkonfigurationsparametern in TCP/IP-Netzwerken. Es wurde 1993 entwickelt, um die manuelle Konfiguration von Netzwerkgeräten zu ersetzen und die Verwaltung großer Netzwerke zu vereinfachen. 

### Funktionsweise

DHCP arbeitet nach dem Client-Server-Modell und verwendet den sogenannten DORA-Prozess: 

1. **Discover**: Der Client sendet eine Broadcast-Nachricht, um DHCP-Server zu finden.
2. **Offer**: DHCP-Server antworten mit Angeboten für IP-Adressen und Konfigurationen.
3. **Request**: Der Client wählt ein Angebot aus und sendet eine Anfrage zurück.
4. **Acknowledge**: Der Server bestätigt die Zuweisung der IP-Adresse.

### Vorteile von DHCP

- Automatische und zentralisierte Verwaltung von IP-Adressen
- Vereinfachte Netzwerkkonfiguration für Endbenutzer
- Effiziente Nutzung des IP-Adressraums
- Einfache Aktualisierung von Netzwerkkonfigurationen

### DHCP-Server

Ein DHCP-Server ist ein Hintergrundprozess, der auf UDP-Port 67 auf Anfragen von Clients wartet. Er kann in verschiedenen Modi betrieben werden: 

- **Manuelle Zuordnung**: Feste Zuweisung von IP-Adressen zu MAC-Adressen
- **Automatische Zuordnung**: Zuweisung aus einem festgelegten Adressbereich
- **Dynamische Zuordnung**: Zeitlich begrenzte Zuweisung von IP-Adressen

> [!note]
DHCP ermöglicht eine effiziente und flexible Verwaltung von Netzwerken, indem es die manuelle Konfiguration einzelner Geräte überflüssig macht und eine zentrale Kontrolle über die Netzwerkressourcen bietet.

## Erklären Sie das DNS bzw. WINS-Protokoll.

Das Domain Name System (DNS) und der Windows Internet Naming Service (WINS) sind beide Protokolle zur Namensauflösung in Netzwerken, haben aber unterschiedliche Funktionen und Einsatzbereiche.

### DNS (Domain Name System)

DNS ist ein globales, hierarchisches Verzeichnissystem für die Zuordnung von Domainnamen zu IP-Adressen im Internet.  

#### Funktion

- Wenn ein Benutzer eine URL eingibt, sendet der Browser eine Anfrage an einen DNS-Resolver.
- Der Resolver kontaktiert verschiedene DNS-Server in einer hierarchischen Struktur, bis er die entsprechende IP-Adresse findet.
- Die IP-Adresse wird an den Browser zurückgegeben, der dann die Website aufrufen kann.

> [!note]
DNS ist essentiell für das moderne Internet und wird weltweit verwendet.

### WINS (Windows Internet Naming Service)

WINS ist ein veraltetes, proprietäres Microsoft-Protokoll für lokale Netzwerke. 

#### Funktion

- Es dient zur Registrierung und Auflösung von NetBIOS-Namen in IP-Adressen.
- WINS-Clients melden sich beim Start beim WINS-Server an und teilen ihren Namen und ihre IP-Adresse mit.
- Der WINS-Server verwaltet diese Informationen in einer Datenbank.

> [!note]
WINS wird heute als veraltet betrachtet und Microsoft empfiehlt, stattdessen DNS zu verwenden. 


### Hauptunterschiede

- **Einsatzbereich**: DNS ist global, WINS nur für lokale Netzwerke.
- **Hierarchie**: DNS kann Hierarchien abbilden, WINS nicht.
- **Aktualität**: DNS ist moderner und unterstützt IPv6, WINS nicht.
- **Verwaltung**: DNS erfordert manuelle Konfiguration, WINS ist dynamischer.

> [!note]
Heute wird in den meisten Netzwerken ausschließlich DNS verwendet, während WINS nur noch in älteren Systemen oder speziellen Umgebungen zum Einsatz kommt.

## Erklären Sie das http bzw. HTTPS-Protokoll.

HTTP (Hypertext Transfer Protocol) und HTTPS (HTTP Secure) sind Internetprotokolle zur Datenübertragung zwischen Client und Server. 

### HTTP

- Entwickelt 1989-1991 am CERN
- Ermöglicht Abruf und Anzeige von Webseiten
- Arbeitet nach dem Client-Server-Prinzip
- Verwendet standardmäßig Port 80
- Kommunikation erfolgt im Klartext

#### Funktionsweise

1. Client sendet HTTP-Request an Server (z.B. GET-Anfrage)
2. Server verarbeitet Anfrage
3. Server sendet HTTP-Response mit Statuscode und angefragten Daten
4. Verbindung wird beendet (zustandsloses Protokoll)

### HTTPS

- Sichere Erweiterung von HTTP
- Verschlüsselt Datenübertragung mittels TLS/SSL
- Verwendet standardmäßig Port 443
- Bietet Schutz vor Abhören und Manipulation der Daten

#### Vorteile von HTTPS: 

- Erhöhte Sicherheit für sensible Daten
- Bevorzugte Behandlung durch Suchmaschinen
- Vertrauenswürdigkeit für Nutzer (Browseranzeige)

> [!note]
HTTPS ist heute der empfohlene Standard für Websites, insbesondere für solche, die sensible Informationen verarbeiten

## Erklären Sie das SMTP / POP3 / IMAP-Protokoll.

Die E-Mail-Protokolle SMTP, POP3 und IMAP dienen der Übertragung und Verwaltung von E-Mails.

### SMTP (Simple Mail Transfer Protocol)

Protokoll zum Versenden von E-Mails

#### Funktionsweise

1. Client lädt E-Mail auf SMTP-Server des Providers
2. SMTP-Server kontaktiert DNS-Server zur Ermittlung des Ziel-SMTP-Servers
3. E-Mail wird über Mail Transfer Agents (MTAs) zum Zielserver übertragen

- Verwendet standardmäßig Port 25, für verschlüsselte Varianten auch 465 oder 587
- Sendet Statusmeldungen während des Übertragungsprozesses

### POP3 (Post Office Protocol Version 3)

Protokoll zum Abrufen von E-Mails vom Server

#### Funktionsweise

1. Client baut TCP-Verbindung zum Server (Port 110) auf
2. Authentifizierung des Benutzers
3. E-Mails werden heruntergeladen und lokal gespeichert
4. E-Mails werden standardmäßig vom Server gelöscht

- Ermöglicht Offline-Verarbeitung der E-Mails
- Begrenzte Funktionalität (Abholen, Auflisten, Löschen von E-Mails) 

### IMAP (Internet Message Access Protocol)

Protokoll zum Zugriff und Verwalten von E-Mails auf dem Server

#### Funktionsweise

- E-Mails bleiben auf dem Server gespeichert
- Ermöglicht Synchronisation zwischen mehreren Geräten
- Bietet erweiterte Funktionen wie Ordnerverwaltung und Suche
- Unverschlüsselt auf Port 143 und verschlüsselt auf Port 993

> [!note]
IMAP ist flexibler als POP3 und besser für die Nutzung auf mehreren Geräten geeignet, während POP3 einfacher ist und sich für die Offline-Nutzung eignet. SMTP hingegen ist für den Versand von E-Mails zuständig und arbeitet mit POP3 oder IMAP zusammen, um den gesamten E-Mail-Prozess abzudecken

  

## Erklären Sie das TELNET bzw. SSH-Protokoll.

TELNET und SSH sind Netzwerkprotokolle zur Fernsteuerung von Computern, unterscheiden sich aber grundlegend in ihrer Sicherheit.

### TELNET (Teletype Network)

- Unverschlüsseltes Protokoll zur Fernsteuerung von Computern
- Verwendet standardmäßig TCP-Port 23
- Überträgt Daten im Klartext, einschließlich Passwörter

#### Funktionsweise

1. Client startet Verbindung mit "telnet" Befehl und Zieladresse
2. Authentifizierung erfolgt unverschlüsselt
3. Textbasierte Kommandos werden ausgetauscht

### SSH (Secure Shell)

- Verschlüsseltes Protokoll für sichere Netzwerkdienste
- Verwendet standardmäßig TCP-Port 22
- Bietet Verschlüsselung, Authentifizierung und Integrität

#### Funktionsweise

1. Server- und Client-Authentifizierung mittels Zertifikaten
2. Verschlüsselte Datenübertragung
3. Unterstützt zusätzliche Funktionen wie SFTP

> [!note]
SSH hat TELNET weitgehend ersetzt, da es wesentlich sicherer ist und Man-in-the-Middle-Angriffe sowie Abhören verhindert

  

## Erklären Sie das FTP bzw. SCP-Protokoll.

FTP (File Transfer Protocol) und SCP (Secure Copy Protocol) sind Netzwerkprotokolle zur Dateiübertragung, unterscheiden sich jedoch in Sicherheit und Funktionsweise.

### FTP (File Transfer Protocol)

- Arbeitet auf der Anwendungsebene des TCP/IP-Stacks
- Verwendet zwei separate Kanäle: 
	1. **Steuerkanal (Port 21)**: Für Befehle und Statuscodes
	2. **Datenkanal**: Für die eigentliche Dateiübertragung

#### Funktionsweise

1. Client stellt Verbindung zum Server her (Port 21)
2. Authentifizierung mit Benutzername und Passwort
3. Dateien können hoch- oder heruntergeladen werden

Überträgt Daten **unverschlüsselt**, was ein Sicherheitsrisiko darstellt

### SCP (Secure Copy Protocol)

- Basiert auf dem SSH-Protokoll für sichere Datenübertragung
- Verwendet Verschlüsselung und Authentifizierung wie SSH

#### Funktionsweise

1. Aufbau einer SSH-Verbindung zwischen Hosts
2. Authentifizierung mittels Passwort oder Public-Key
3. Sichere Dateiübertragung in zwei Modi: 

- **Source-Modus**: Lesen von Dateien vom Zielsystem
- **Sink-Modus**: Schreiben von Dateien auf das Zielsystem

- Bietet **verschlüsselte** und damit sicherere Datenübertragung als FTP

> [!note]
SCP hat FTP in vielen Anwendungsfällen ersetzt, da es eine sicherere Alternative für die Dateiübertragung bietet, insbesondere wenn sensible Daten übertragen werden müssen.

## Erklären Sie das SMB bzw. CIFS-Protokoll.

SMB (Server Message Block) und CIFS (Common Internet File System) sind Netzwerkprotokolle für den Dateizugriff und die Dateifreigabe.

### SMB

- Entwickelt von Microsoft für Datei- und Druckerfreigabe in Windows-Netzwerken
- Arbeitet nach dem Client-Server-Modell
- Ermöglicht Zugriff auf freigegebene Ordner, Dateien und Drucker
- Aktuellste Version ist SMB 3.0 (seit Windows Server 2012 R2)

### CIFS

- Öffentliche Variante und Erweiterung von SMB
- Basiert auf dem TCP/IP-Protokoll
- Ermöglicht Fernzugriff auf Dateien über Netzwerkverbindungen

### Hauptfunktionen

- Datei- und Druckerfreigabe
- Authentifizierung und Zugriffskontrolle
- Datei- und Verzeichnissperren
- Caching und Leistungsoptimierung

> [!note]
Beide Protokolle werden häufig synonym verwendet, wobei CIFS technisch gesehen eine spezifische Implementierung von SMB darstellt[1](https://www.storage-insider.de/cifs-netzwerkprotokoll-einfach-erklaert-a-517742/)[3](https://learn.microsoft.com/de-de/windows/win32/fileio/microsoft-smb-protocol-and-cifs-protocol-overview). SMB/CIFS hat sich über die Jahre weiterentwickelt: 
>
>- SMB 1.0 (auch als CIFS bekannt): Ursprüngliche Version
>- SMB 2.0 und höher: Verbesserte Leistung und Sicherheit
>
SMB/CIFS wird hauptsächlich in Windows-Umgebungen eingesetzt, ist aber auch auf anderen Betriebssystemen wie Unix und Linux (über Samba) verfügbar
