---
undefined: ""
File: Contents/Prüfungen/LAP/Netzwerktechnik/OSI-Schichtenmodell.md
---
## **Wie viele Schichten enthält das OSI-Schichtenmodell?**

Sieben, manchmal auch 8 XD 

## **Nennen Sie die Namen der einzelnen Schichten und welche Funktionen sie erfüllen.**

### 1. Physical Layer (Bitübertragungsschicht): WLAN IEEE 802.11

- Umwandlung von Bits in physikalische Signale
- Physikalische Übertragung der Daten

### 2. Data Link Layer (Sicherungsschicht): ARP,STP

- Segmentierung der Daten in Frames
- Fehlerbehandlung und Hinzufügen von Prüfsummen

### 3. Network Layer (Vermittlungsschicht): IP, ICMP,RIP

- Routing der Datenpakete zum nächsten Knoten
- Adressierung und Wegewahl im Netzwerk

### 4. Transport Layer (Transportschicht): TCP, UDP

- Zuordnung der Datenpakete zu Anwendungen
- Flusskontrolle und Fehlerbehandlung

### 5. Session Layer (Sitzungsschicht): NetBIOS, RPC

- Steuerung der Verbindungen und des Datenaustauschs
- Verwaltung von Kommunikationssitzungen

### 6. Presentation Layer (Darstellungsschicht): SSL,TLS

- Umwandlung systemabhängiger Daten in ein unabhängiges Format
- Datenkompression und Verschlüsselung

### 7. Application Layer (Anwendungsschicht): HTTP, SMTP, DNS

- Bereitstellung von Funktionen für Anwendungen
- Schnittstelle zwischen Netzwerk und Benutzer

## **Erklären Sie das TCP/IP-Schichtenmodell im Vergleich zum OSI-Schichtenmodell.**  

Das **TCP/IP-Schichtenmodell** und das **OSI-Schichtenmodell** sind zwei Referenzmodelle für Netzwerkkommunikation. Während das OSI-Modell ein theoretisches Modell mit sieben Schichten ist, ist das TCP/IP-Modell praxisnaher und besteht aus vier Schichten.
### 1. OSI-Modell (7 Schichten)

 **Konzeptionelles Modell**, detailliert, selten in der Praxis genutzt.

| **Schicht**           | **Funktion**                   | **Beispiele**  |
| --------------------- | ------------------------------ | -------------- |
| **7. Anwendung**      | Netzwerkdienste für Apps       | HTTP, FTP, DNS |
| **6. Darstellung**    | Verschlüsselung, Kompression   | SSL/TLS, JPEG  |
| **5. Sitzung**        | Sitzungsverwaltung             | NetBIOS, RPC   |
| **4. Transport**      | Verbindung & Fehlerkontrolle   | TCP, UDP       |
| **3. Vermittlung**    | Routing, IP-Adressen           | IP, ICMP, ARP  |
| **2. Sicherung**      | MAC-Adressen, Fehlererkennung  | Ethernet, WLAN |
| **1. Bitübertragung** | Physikalische Datenübertragung | Kabel, Funk    |

### 2. TCP/IP-Modell (4 Schichten)

 **Praxisnah, für das Internet entwickelt**.

| **Schicht**    | **Entspricht OSI** | **Funktion**                            |
| -------------- | ------------------ | --------------------------------------- |
| **Anwendung**  | 7 - 5              | Dienste für Apps (HTTP, DNS)            |
| **Transport**  | 4                  | Verbindung & Fehlerkorrektur (TCP, UDP) |
| **Internet**   | 3                  | Routing & IP-Adressen (IP, ICMP)        |
| **Netzzugang** | 2 - 1              | Physische Übertragung (Ethernet, WLAN)  |

###  Kurz gesagt

- **OSI-Modell**: Theoretisch, 7 Schichten, detailliert.
- **TCP/IP-Modell**: Praxisnah, 4 Schichten, Internet-Standard.
- **Unterschied**: OSI ist feingliedriger, TCP/IP fasst Schichten zusammen.