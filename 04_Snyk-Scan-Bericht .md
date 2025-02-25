# 🛡 **Snyk-Scan-Bericht**  

*Detaillierter Bericht über Sicherheits- und Schwachstellenanalysen von Abhängigkeiten und Code mit Snyk.*  

---

## 📋 **1. Allgemeine Informationen**  

- **Projektname:** ____________________________  
- **Repository/Codebase:** ____________________  
- **Programmiersprache(n):** __________________  
- **Scan durchgeführt von:** __________________  
- **Scan-Datum:** _____________________________  
- **Verwendete Snyk-Tools:**  
  - [ ] Snyk Open Source  
  - [ ] Snyk Code (SAST)  
  - [ ] Snyk Container  
  - [ ] Snyk Infrastructure as Code (IaC)  

---

## 🎯 **2. Zielsetzung des Scans**  

Der Snyk-Scan dient der Identifikation von Sicherheitslücken, fehlerhaften Konfigurationen und potenziellen Schwachstellen in Open-Source-Bibliotheken, Quellcode, Containern und Infrastruktur-Templates.  

**Ziele des Scans:**  
- Aufdeckung von Schwachstellen in Abhängigkeiten (z. B. CVEs)  
- Überprüfung des Quellcodes auf Sicherheitslücken  
- Erkennung von Schwachstellen in Container-Images  
- Sicherstellung sicherer Infrastruktur-Konfigurationen  

---

## 📑 **3. Zusammenfassung der Ergebnisse**  

- **Gesamtzahl gefundener Schwachstellen:** ___  
- **Kritische Schwachstellen:** ___  
- **Hohe Schwachstellen:** ___  
- **Mittlere Schwachstellen:** ___  
- **Niedrige Schwachstellen:** ___  

**Verteilung nach Kategorien:**  
- **Open-Source-Abhängigkeiten:** ___ Schwachstellen  
- **Quellcode (SAST):** ___ Schwachstellen  
- **Container:** ___ Schwachstellen  
- **Infrastructure as Code (IaC):** ___ Fehlkonfigurationen  

---

## 🔍 **4. Detaillierte Schwachstellenanalyse**  

### **4.1 Open Source Abhängigkeiten**  

| **ID**   | **Bibliothek/Abhängigkeit**     | **Version** | **CVE**          | **Schweregrad** | **Empfohlene Version** |  
|----------|---------------------------------|------------|-----------------|----------------|------------------------|  
| DEP-001  | lodash                         | 4.17.11    | CVE-2019-10744  | Hoch           | 4.17.21                |  
| DEP-002  | jackson-databind               | 2.9.5      | CVE-2018-7489   | Kritisch       | 2.9.10.8               |  
| DEP-003  | moment                         | 2.18.1     | CVE-2020-15168  | Mittel         | 2.29.1                 |  

---

### **4.2 Quellcode-Sicherheitsanalyse (SAST)**  

| **ID**   | **Dateipfad**                     | **Schwachstelle**               | **Schweregrad** | **Zeile** | **Empfohlene Maßnahme**                    |  
|----------|-----------------------------------|---------------------------------|----------------|----------|---------------------------------------------|  
| CODE-001 | /src/auth/login.js               | SQL Injection                  | Kritisch       | 45       | Prepared Statements verwenden               |  
| CODE-002 | /src/api/userController.js       | Cross-Site Scripting (XSS)     | Hoch           | 88       | Eingaben escapen und validieren             |  
| CODE-003 | /src/utils/fileHandler.js        | Path Traversal                 | Mittel         | 102      | Pfadvalidierung implementieren              |  

---

### **4.3 Container-Sicherheitsanalyse**  

| **ID**   | **Image**                      | **Tag**     | **CVE**          | **Schweregrad** | **Fix verfügbar** |  
|----------|-------------------------------|------------|-----------------|----------------|-------------------|  
| CONT-001 | node                          | 12.16.1    | CVE-2020-8116   | Hoch           | Ja                |  
| CONT-002 | ubuntu                        | 18.04      | CVE-2019-3462   | Mittel         | Ja                |  
| CONT-003 | nginx                         | 1.17.1     | CVE-2021-23017  | Kritisch       | Ja                |  

---

### **4.4 Infrastructure as Code (IaC)**  

| **ID**   | **Datei**                    | **Ressource**     | **Fehlkonfiguration**                   | **Schweregrad** | **Empfohlene Maßnahme**               |  
|----------|------------------------------|------------------|-----------------------------------------|----------------|---------------------------------------|  
| IAC-001  | terraform/aws_s3.tf          | aws_s3_bucket    | Public-Read aktiviert                  | Kritisch       | Deaktiviere öffentliche Berechtigungen |  
| IAC-002  | kubernetes/deployment.yaml   | pod/deployment   | Container läuft als Root               | Hoch           | Setze runAsNonRoot auf true           |  
| IAC-003  | azure/main.tf                | azurerm_sql_server | SSL/TLS deaktiviert                  | Mittel         | Aktiviere SSL/TLS                     |  

---

## ⚖ **5. Risikobewertung**  

**Wahrscheinlichkeit:**  
- Sehr hoch (5): Tritt fast sicher ein  
- Hoch (4): Tritt wahrscheinlich ein  
- Mittel (3): Möglicher Eintritt  
- Niedrig (2): Seltenes Eintreten  
- Sehr niedrig (1): Sehr unwahrscheinlich  

**Auswirkung:**  
- Katastrophal (5): Kritische Geschäftsunterbrechung  
- Hoch (4): Bedeutende Beeinträchtigung  
- Mittel (3): Moderate Beeinträchtigung  
- Niedrig (2): Geringe Auswirkungen  
- Sehr niedrig (1): Keine nennenswerten Auswirkungen  

---

## 🛠 **6. Handlungsempfehlungen**  

| **Schwachstelle**                  | **Schweregrad** | **Empfohlene Maßnahme**               | **Verantwortlich**   | **Frist**     |  
|------------------------------------|----------------|---------------------------------------|----------------------|--------------|  
| lodash (CVE-2019-10744)            | Hoch           | Upgrade auf Version 4.17.21          | Max Mustermann       | 10.04.2024   |  
| SQL Injection im Login-Formular    | Kritisch       | Prepared Statements verwenden        | Sarah Müller         | 12.04.2024   |  
| Container nginx (CVE-2021-23017)   | Kritisch       | Update des Images                    | Jonas Becker         | 15.04.2024   |  
| S3 Bucket public-read              | Kritisch       | Deaktiviere öffentliche Berechtigungen| Laura Schmidt       | 20.04.2024   |  

---

## 📅 **7. Zeitplan für die Behebung**  

| **Phase**                         | **Startdatum**   | **Enddatum**     | **Verantwortlich**   |  
|-----------------------------------|------------------|------------------|----------------------|  
| Schwachstellenbehebung starten    | ________________ | ________________ | ____________________ |  
| Code-Review nach Behebung         | ________________ | ________________ | ____________________ |  
| Verifizierung und Retest          | ________________ | ________________ | ____________________ |  
| Abschlussbericht und Review       | ________________ | ________________ | ____________________ |  

---

## 🚨 **8. Lessons Learned**  

- [ ] Welche häufigen Fehler wurden in den Abhängigkeiten gefunden?  
- [ ] Welche Sicherheitsstandards wurden nicht eingehalten?  
- [ ] Welche Verbesserungen sollten in den Entwicklungsprozess integriert werden?  
- [ ] Empfehlungen für zukünftige Sicherheits-Scans und Audits?  

---

## 📝 **9. Genehmigung**  

**Erstellt von:**  
Name: ____________________________  
Position: _________________________  
Datum: ___________________________  

**Geprüft von:**  
Name: ____________________________  
Position: _________________________  
Datum: ___________________________  

**Genehmigt von:**  
Name: ____________________________  
Position: _________________________  
Datum: ___________________________  