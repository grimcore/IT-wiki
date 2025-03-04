---
undefined: ""
File: Contents/Prüfungen/LAP/Sicherheit/Zertifikate.md
sticker: lucide//book-open-check
---
## Wo werden in der IT Zertifikate eingesetzt und wo können diese beschafft werden?

IT-Zertifikate spielen eine entscheidende Rolle in der Absicherung digitaler Kommunikation und Identitäten. Sie basieren auf Public Key Infrastructure (PKI) und dienen zur Authentifizierung, Verschlüsselung und Integritätssicherung.  
Zertifikate werden von Zertifizierungsstellen (CAs) ausgestellt, die als vertrauenswürdige Dritte agieren. Sie prüfen die Identität von Organisationen oder Einzelpersonen, bevor sie ein Zertifikat ausstellen (z.B.: DigiCert, Global Sign, Sectigo) 

## Erklären Sie den Begriff „SSL“.

SSL steht für Secure Sockets Layer und ist ein Verschlüsselungsprotokoll, das entwickelt wurde, um die Kommunikation zwischen zwei Systemen sicher zu machen. Es wird hauptsächlich verwendet, um Daten im Internet vor unbefugtem Zugriff zu schützen. SSL sorgt dafür, dass sensible Informationen wie Passwörter, Kreditkartendaten oder persönliche Daten verschlüsselt übertragen werden.

## Welche Merkmale hat ein Zertifikat?

### Technische Merkmale eines Zertifikats

- Seriennummer
- Aussteller (Issuer)
- Subjekt (Subject)
- Gültigkeitsdauer
- Öffentlicher Schlüssel (Public Key)
- Signatur der Zertifizierungsstelle
- Zertifikatstyp 
- Algorithmus  

### Sicherheitsmerkmale
- Vertrauenswürdigkeit 
- Widerrufstatus  

### Struktur eines Zertifikats (X.509 Standard)

- Version
- Seriennummer
- Signaturalgorithmus
- Issuer
- Validity
- Subject
- Public Key 
- Erweiterungen (Extensions)

## Erklären Sie den Begriff „TLS“

TLS (Transport Layer Security) ist ein kryptografisches Protokoll, das entwickelt wurde, um die Sicherheit der Kommunikation in Computernetzwerken zu gewährleisten. Es bietet Verschlüsselung, Integritätsschutz und Authentifizierung für Daten, die über das Internet oder andere Netzwerke übertragen werden. TLS sorgt dafür, dass die übermittelten Daten nicht von Dritten abgefangen, verändert oder gefälscht werden können.