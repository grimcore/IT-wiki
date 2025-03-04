---
undefined: ""
File: Contents/Prüfungen/LAP/Sicherheit/Firewall.md
sticker: lucide//book-open-check
---

## Erklären Sie den Begriff „Firewall“.

Eine Firewall ist eine Sicherheitsvorrichtung, die den Datenverkehr zwischen einem Netzwerk (z.B. einem Computer oder einem Unternehmensnetzwerk) und dem Internet überwacht und kontrolliert. Sie kann den Zugriff auf bestimmte Daten oder Dienste blockieren oder zulassen, basierend auf festgelegten Regeln. Firewalls schützen vor unbefugtem Zugriff, verhindern Angriffe und können dazu beitragen, Schadsoftware vom Netzwerk fernzuhalten. 

## Welche Arten von Firewalls kennen Sie?

- **Nach Architektur**: Software, Hardware und Cloud basierte Firewalls
- **Nach Funktion**: Paket, Stateful Inspection, Proxy, Next-Gen und Web Application Firewall
- **Nach Einsatzort**: Netzwerk, Host-basierte, Perimeter und Interne Firewalls

## Erklären Sie die Funktionsweise einer „Firewall“.

Eine Firewall ist ein Sicherheitssystem, das den ein- und ausgehenden Datenverkehr in einem Netzwerk überwacht und kontrolliert. Sie dient dazu, unberechtigte Zugriffe zu verhindern und Netzwerkressourcen zu schützen. Sie arbeitet mit definierten Regeln, diese können auf IP-Adressen, Ports, Protokollen oder spezifischen Anwendungen basieren. Pakete die den Regeln nicht entsprechen werden verworfen oder blockiert. 

## Wo wird eine „Firewall“ eingesetzt?

Zwischen internen und externen Netzwerken (LAN -> WAN), innerhalb des internen Netzwerkes um zb. sensible Daten einer Abteilung zu isolieren  
Host-basierte Firewalls laufen direkt auf einzelnen Geräten (PC’s, Laptop, Server, Smartphone und Tablets)  
Zum Schutz von Webservern oder Cloud Diensten (DDoS Attack) 

## Erklären Sie den Unterschied zwischen „IDS“ und „IPS“.

### Intrusion Detection System
Ein IDS ist ein Überwachungssystem, das verdächtigen oder bösartigen Netzwerkverkehr erkennt und meldet. 

Es greift jedoch nicht aktiv ein.  

### Intrusion Prevention System
Ein IPS ist ein Schutzsystem, das nicht nur verdächtigen Datenverkehr erkennt, sondern auch aktiv Maßnahmen ergreift, um Angriffe zu verhindern.  

In vielen modernen Sicherheitssystemen werden IDS und IPS zusammen eingesetzt, um sowohl die Erkennung als auch die Prävention von Bedrohungen zu gewährleisten.

## Erklären Sie die Funktionsweise einer „DMZ“.

Eine DMZ (Demilitarized Zone) ist ein isoliertes Netzwerksegment, das zwischen einem internen Netzwerk und dem öffentlichen Internet eingerichtet wird. Es dient als Pufferzone, in der öffentlich zugängliche Dienste (z. B. Webserver, Mailserver) bereitgestellt werden, ohne das interne Netzwerk direkt zu gefährden.