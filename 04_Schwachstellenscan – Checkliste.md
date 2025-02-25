# 🛡 **Schwachstellenscan – Checkliste**  

*Systematische Vorgehensweise zur Durchführung eines umfassenden Schwachstellenscans.*  

---

## 📋 **1. Vorbereitungen des Schwachstellenscans**  

- [ ] **Zieldefinition:**  
  - [ ] Welche Systeme, Anwendungen und Netzwerke sollen gescannt werden?  
  - [ ] Umfang und Grenzen des Scans klar definieren (IP-Bereiche, Hosts, Ports).  

- [ ] **Freigaben und Genehmigungen:**  
  - [ ] Schriftliche Genehmigung vom IT-Sicherheitsbeauftragten einholen.  
  - [ ] Benachrichtigung der betroffenen Teams und Stakeholder.  

- [ ] **Tool-Auswahl:**  
  - [ ] Auswahl eines geeigneten Schwachstellenscanners:  
    - [ ] Nessus  
    - [ ] OpenVAS  
    - [ ] Qualys  
    - [ ] Burp Suite (für Webanwendungen)  

- [ ] **Scan-Profile und Einstellungen:**  
  - [ ] Authentifizierte Scans einrichten (wo möglich).  
  - [ ] Auswahl des Scantyps:  
    - [ ] Netzwerk-Scan  
    - [ ] Webanwendungsscan  
    - [ ] Datenbank-Scan  
    - [ ] Cloud-Umgebungsscan  

- [ ] **Backup und Notfallplanung:**  
  - [ ] Backup der zu scannenden Systeme erstellen.  
  - [ ] Notfallplan für den Fall von Systemausfällen während des Scans bereitstellen.  

---

## 🔍 **2. Durchführung des Schwachstellenscans**  

- [ ] **Netzwerkscan:**  
  - [ ] Überprüfung auf offene Ports und Dienste.  
  - [ ] Erkennung von veralteten Protokollen (z. B. Telnet, FTP).  
  - [ ] Identifikation von Netzwerkgeräten (Router, Switches, Firewalls).  

- [ ] **Betriebssystem- und Serverscan:**  
  - [ ] Überprüfung auf fehlende Sicherheitsupdates und Patches.  
  - [ ] Erkennung von Standardpasswörtern und unsicheren Konfigurationen.  

- [ ] **Webanwendungsscan:**  
  - [ ] Überprüfung auf häufige Schwachstellen (OWASP Top 10):  
    - [ ] SQL Injection  
    - [ ] Cross-Site Scripting (XSS)  
    - [ ] Insecure Direct Object References  
  - [ ] Prüfung auf unsichere Cookies und Header.  

- [ ] **Datenbanksicherheit:**  
  - [ ] Überprüfung auf SQL-Injections.  
  - [ ] Überprüfung auf ungesicherte Backup-Dateien.  

- [ ] **Cloud-Sicherheit:**  
  - [ ] Prüfung der Konfigurationen von Cloud-Ressourcen (S3-Buckets, Azure Blobs).  
  - [ ] Überprüfung der IAM-Rollen und Zugriffsberechtigungen.  

- [ ] **Mobile und IoT-Geräte:**  
  - [ ] Überprüfung auf unsichere Standardkonfigurationen.  
  - [ ] Prüfung auf Schwachstellen in der Firmware.  

---

## ⚙ **3. Nachbearbeitung des Scans**  

- [ ] **Ergebnisanalyse:**  
  - [ ] Überprüfung und Validierung der Scan-Ergebnisse.  
  - [ ] Entfernen von Fehlalarmen (False Positives).  

- [ ] **Bewertung der Schwachstellen:**  
  - [ ] Einordnung der Schwachstellen nach CVSS-Score:  

| **Schweregrad** | **CVSS-Score** | **Beschreibung**                         |  
|-----------------|----------------|------------------------------------------|  
| Kritisch        | 9.0 – 10.0     | Sofortige Behebung erforderlich          |  
| Hoch            | 7.0 – 8.9      | Schnelle Behebung empfohlen              |  
| Mittel          | 4.0 – 6.9      | Zeitnahe Behebung                        |  
| Niedrig         | 0.1 – 3.9      | Nach Verfügbarkeit beheben               |  

- [ ] **Risikobewertung:**  
  - [ ] Wahrscheinlichkeit der Ausnutzung der Schwachstelle.  
  - [ ] Potenzielle Auswirkungen auf Verfügbarkeit, Integrität und Vertraulichkeit.  

---

## 🛠 **4. Behebung der Schwachstellen**  

- [ ] **Patch-Management:**  
  - [ ] Einspielen von Sicherheitsupdates und Patches.  
  - [ ] Vorab-Tests der Patches in einer Staging-Umgebung.  

- [ ] **Konfigurationsänderungen:**  
  - [ ] Härtung der Systeme gemäß Best Practices (z. B. CIS-Benchmarks).  
  - [ ] Entfernen oder Deaktivieren unnötiger Dienste und Ports.  

- [ ] **Code-Änderungen:**  
  - [ ] Behebung von Schwachstellen im Anwendungscode.  
  - [ ] Durchführung von Code-Reviews.  

- [ ] **Mitigation bei fehlenden Patches:**  
  - [ ] Einsatz von Workarounds zur Risikominderung.  
  - [ ] Erhöhung der Überwachung für anfällige Systeme.  

---

## 🔄 **5. Verifizierung und Retesting**  

- [ ] **Durchführung eines erneuten Scans:**  
  - [ ] Überprüfung, ob alle Schwachstellen erfolgreich behoben wurden.  
  - [ ] Validierung der getroffenen Maßnahmen.  

- [ ] **Dokumentation:**  
  - [ ] Alle behobenen und offenen Schwachstellen dokumentiert.  
  - [ ] Ergebnisse des Retests im Schwachstellenregister aktualisiert.  

---

## 📊 **6. Reporting**  

- [ ] **Erstellung eines detaillierten Berichts:**  
  - [ ] Zusammenfassung der Scan-Ergebnisse.  
  - [ ] Übersicht der gefundenen Schwachstellen mit Risikobewertung.  
  - [ ] Handlungsempfehlungen zur Behebung der Schwachstellen.  

- [ ] **Reporting an das Management:**  
  - [ ] Monatliche oder quartalsweise Berichte zu offenen und behobenen Schwachstellen.  
  - [ ] Metriken wie Time to Remediate (TTR) und Anzahl kritischer Schwachstellen.  

---

## ✅ **7. Abschlussprüfung**  

- [ ] Alle identifizierten Schwachstellen wurden überprüft.  
- [ ] Kritische Schwachstellen wurden behoben oder mitigiert.  
- [ ] Der Schwachstellenscan wurde vollständig dokumentiert.  
- [ ] Die Ergebnisse wurden an relevante Stakeholder kommuniziert.  

**Datum des letzten Scans:** ___________________  
**Verantwortlich:** ____________________________  