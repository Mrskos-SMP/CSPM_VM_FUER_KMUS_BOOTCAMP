# 🛡 **Security Posture Management (SPM) – Checkliste**  

*Überprüfe regelmäßig den Sicherheitsstatus deines Unternehmens mit dieser umfassenden Checkliste.*  

---

## 📋 **1. Asset-Inventarisierung**  

- [ ] **Alle IT-Assets identifiziert:**  
  - Server, Workstations, Laptops  
  - Netzwerkgeräte (Router, Switches, Firewalls)  
  - Cloud-Ressourcen (IaaS, PaaS, SaaS)  
  - Mobile Geräte (Smartphones, Tablets)  

- [ ] **Asset-Register gepflegt und aktuell:**  
  - Regelmäßige Überprüfung der Asset-Liste  
  - Klassifizierung der Assets nach Kritikalität  

- [ ] **Zugriffsrechte dokumentiert:**  
  - Wer hat Zugriff auf welches System?  
  - Least Privilege Prinzip umgesetzt  

---

## 🔍 **2. Sicherheitsbewertung und Schwachstellenanalyse**  

- [ ] **Regelmäßige Schwachstellenscans durchgeführt:**  
  - Wöchentliche Scans für kritische Systeme  
  - Monatliche Scans für alle anderen Systeme  

- [ ] **Verwendung von Schwachstellenscannern:**  
  - [ ] Nessus  
  - [ ] OpenVAS  
  - [ ] Qualys  

- [ ] **Bewertung der Schwachstellen nach CVSS:**  
  - Kritische Schwachstellen (CVSS >9) innerhalb von 24h behoben  
  - Hohe Schwachstellen (CVSS 7-9) innerhalb von 7 Tagen behoben  

- [ ] **Manuelle Sicherheitsüberprüfungen:**  
  - Penetrationstests für geschäftskritische Anwendungen  
  - Code Reviews zur Schwachstellenanalyse  

---

## ⚙ **3. Konfigurationsmanagement**  

- [ ] **Systemkonfigurationen regelmäßig überprüft:**  
  - Server, Netzwerkgeräte und Anwendungen entsprechen Sicherheitsrichtlinien  
  - Automatisierte Überwachungstools eingesetzt (z. B. Ansible, Puppet)  

- [ ] **Härtung der Systeme gemäß Best Practices:**  
  - CIS-Benchmarks implementiert  
  - Unnötige Dienste und Ports deaktiviert  

- [ ] **Sicherheitsupdates regelmäßig eingespielt:**  
  - Kritische Patches innerhalb von 24h installiert  
  - Standard-Patches innerhalb des Wartungsfensters angewendet  

---

## 📊 **4. Netzwerk- und Zugriffskontrollen**  

- [ ] **Netzwerksegmentierung implementiert:**  
  - Trennung von Produktions-, Entwicklungs- und Testumgebungen  
  - Firewalls und VLANs zur Segmentierung eingesetzt  

- [ ] **Zugriffskontrollen und Authentifizierung:**  
  - Multi-Faktor-Authentifizierung (MFA) aktiviert  
  - Starke Passwortrichtlinien durchgesetzt  

- [ ] **Überwachung des Datenverkehrs:**  
  - Intrusion Detection/Prevention Systeme (IDS/IPS) aktiv  
  - Log-Management und SIEM-Systeme implementiert  

---

## 🛡 **5. Sicherheitsrichtlinien und Compliance**  

- [ ] **Aktuelle Sicherheitsrichtlinien vorhanden:**  
  - Richtlinien für Passwortmanagement, Zugriffskontrolle und Vorfallmanagement  
  - Mitarbeitende regelmäßig geschult  

- [ ] **Einhaltung gesetzlicher Anforderungen:**  
  - DSGVO/GDPR  
  - ISO 27001  
  - PCI-DSS (falls zutreffend)  

- [ ] **Regelmäßige Audits durchgeführt:**  
  - Interne Audits (mindestens halbjährlich)  
  - Externe Audits nach Bedarf  

---

## 🚨 **6. Vorfallmanagement**  

- [ ] **Incident Response Plan vorhanden:**  
  - Schritte zur Reaktion auf Sicherheitsvorfälle definiert  
  - Ansprechpartner und Eskalationsketten dokumentiert  

- [ ] **Sicherheitsvorfälle dokumentiert und analysiert:**  
  - Lessons Learned nach jedem Vorfall  
  - Prozesse zur Vorfallbehebung verbessert  

- [ ] **Notfallpläne und Backups:**  
  - Regelmäßige Backups aller kritischen Systeme  
  - Disaster Recovery Pläne getestet und aktuell  

---

## 📈 **7. Überwachung und Reporting**  

- [ ] **Sicherheitsmetriken regelmäßig ausgewertet:**  
  - Anzahl offener Schwachstellen  
  - Time to Remediate (TTR)  
  - Anzahl der Sicherheitsvorfälle  

- [ ] **Regelmäßige Berichterstattung an das Management:**  
  - Monatliche Sicherheitsberichte  
  - Risikoanalysen und Empfehlungen  

- [ ] **Kontinuierliche Verbesserung:**  
  - Rückmeldungen aus Audits und Vorfällen integriert  
  - SPM-Prozesse regelmäßig überprüft und optimiert  

---

## ✅ **8. Abschlussprüfung**  

- [ ] Alle kritischen Systeme überprüft  
- [ ] Offene Schwachstellen identifiziert und dokumentiert  
- [ ] Sicherheitsrichtlinien aktuell und kommuniziert  
- [ ] Compliance-Anforderungen erfüllt  

**Datum der letzten Überprüfung:** ___________________  
**Verantwortlich:** _________________________________  