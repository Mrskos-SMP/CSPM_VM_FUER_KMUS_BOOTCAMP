# 📊 **Metriken-Definitionsdokument**  

*Dokumentation der wichtigsten Metriken zur Überwachung der IT-Sicherheit und des Risikomanagements.*  

---

## 📋 **1. Allgemeine Informationen**  

- **Projektname:** ____________________________  
- **Erstellt von:** ___________________________  
- **Datum:** _________________________________  
- **Abteilung:** _____________________________  
- **Version:** _______________________________  

---

## 🎯 **2. Ziel des Dokuments**  

Dieses Dokument definiert die wichtigsten Kennzahlen (KPIs und Metriken) zur Überwachung und Bewertung der IT-Sicherheit und des Risikomanagements im Unternehmen. Es dient als Leitfaden für die Erhebung, Analyse und Interpretation der Metriken zur kontinuierlichen Verbesserung der Sicherheitslage.

---

## 📑 **3. Übersicht der Metriken**  

| **Metrik**                           | **Beschreibung**                                                  | **Zielwert** | **Messintervall** | **Verantwortlich** |  
|-------------------------------------|------------------------------------------------------------------|-------------|-------------------|--------------------|  
| Anzahl offener Schwachstellen       | Aktuell nicht behobene Schwachstellen im System                   | < 50        | Wöchentlich       | IT-Sicherheitsteam |  
| Kritische Schwachstellen (%)        | Anteil der kritischen Schwachstellen an allen offenen Schwachstellen | 0%       | Wöchentlich       | IT-Sicherheitsteam |  
| Time to Remediate (TTR)             | Durchschnittliche Zeit zur Behebung von Schwachstellen            | < 30 Tage   | Monatlich         | IT-Sicherheitsteam |  
| Patch Compliance Rate (%)           | Anteil der Systeme mit aktuellen Sicherheitspatches               | > 95%       | Monatlich         | IT-Abteilung       |  
| Mean Time to Detect (MTTD)          | Durchschnittliche Zeit zur Erkennung eines Sicherheitsvorfalls    | < 5 Stunden | Monatlich         | SOC-Team           |  
| Mean Time to Respond (MTTR)         | Durchschnittliche Zeit zur Reaktion auf Sicherheitsvorfälle       | < 24 Stunden| Monatlich         | Incident Response Team |  
| Anzahl erfolgreicher Angriffe       | Verzeichnete Sicherheitsvorfälle im Berichtszeitraum              | 0           | Monatlich         | IT-Sicherheitsteam |  
| Phishing-Erkennungsrate (%)         | Erkennungsrate bei Phishing-Simulationen                          | > 90%       | Quartalsweise     | HR/IT              |  
| Anzahl durchgeführter Pentests      | Anzahl der durchgeführten Penetrationstests                       | ≥ 2/Jahr    | Halbjährlich      | Externer Dienstleister |  
| Benutzer mit starken Passwörtern (%)| Anteil der Benutzer mit sicheren Passwörtern                      | > 98%       | Quartalsweise     | IT-Abteilung       |  

---

## 🔍 **4. Detaillierte Definition der Metriken**  

### 4.1 **Anzahl offener Schwachstellen**  
- **Definition:** Gesamtanzahl der derzeit bekannten, aber nicht behobenen Schwachstellen.  
- **Zielwert:** < 50  
- **Messintervall:** Wöchentlich  
- **Datenquelle:** Schwachstellenmanagement-Tool (z. B. Nessus, Qualys)  

---

### 4.2 **Kritische Schwachstellen (%)**  
- **Definition:** Prozentsatz der offenen Schwachstellen, die als kritisch eingestuft sind.  
- **Formel:** (Anzahl kritischer Schwachstellen / Gesamtanzahl offener Schwachstellen) * 100  
- **Zielwert:** 0%  
- **Messintervall:** Wöchentlich  
- **Datenquelle:** Schwachstellenmanagement-Tool  

---

### 4.3 **Time to Remediate (TTR)**  
- **Definition:** Durchschnittliche Zeit (in Tagen), die benötigt wird, um identifizierte Schwachstellen zu beheben.  
- **Formel:** Summe aller Remediation-Zeiten / Anzahl der behobenen Schwachstellen  
- **Zielwert:** < 30 Tage  
- **Messintervall:** Monatlich  
- **Datenquelle:** Schwachstellenmanagement- und Ticketsystem  

---

### 4.4 **Patch Compliance Rate (%)**  
- **Definition:** Anteil der Systeme, die mit den neuesten Sicherheitspatches aktualisiert sind.  
- **Formel:** (Anzahl gepatchter Systeme / Gesamtanzahl der Systeme) * 100  
- **Zielwert:** > 95%  
- **Messintervall:** Monatlich  
- **Datenquelle:** Patch-Management-System  

---

### 4.5 **Mean Time to Detect (MTTD)**  
- **Definition:** Durchschnittliche Zeit, die benötigt wird, um einen Sicherheitsvorfall zu erkennen.  
- **Formel:** Summe aller Erkennungszeiten / Anzahl der Vorfälle  
- **Zielwert:** < 5 Stunden  
- **Messintervall:** Monatlich  
- **Datenquelle:** SIEM-System (z. B. Splunk, ELK)  

---

### 4.6 **Mean Time to Respond (MTTR)**  
- **Definition:** Durchschnittliche Zeit, die benötigt wird, um auf einen Sicherheitsvorfall zu reagieren und ihn zu beheben.  
- **Formel:** Summe aller Reaktionszeiten / Anzahl der Vorfälle  
- **Zielwert:** < 24 Stunden  
- **Messintervall:** Monatlich  
- **Datenquelle:** Incident-Management-System  

---

### 4.7 **Anzahl erfolgreicher Angriffe**  
- **Definition:** Anzahl der im Berichtszeitraum erfolgreichen Angriffe auf die IT-Systeme.  
- **Zielwert:** 0  
- **Messintervall:** Monatlich  
- **Datenquelle:** SIEM-System, Incident-Response-Logs  

---

### 4.8 **Phishing-Erkennungsrate (%)**  
- **Definition:** Prozentsatz der korrekt identifizierten Phishing-E-Mails während einer Phishing-Simulation.  
- **Formel:** (Anzahl erkannter Phishing-E-Mails / Anzahl gesendeter Phishing-E-Mails) * 100  
- **Zielwert:** > 90%  
- **Messintervall:** Quartalsweise  
- **Datenquelle:** Phishing-Simulations-Tool  

---

### 4.9 **Anzahl durchgeführter Pentests**  
- **Definition:** Anzahl der im Berichtszeitraum durchgeführten Penetrationstests.  
- **Zielwert:** ≥ 2/Jahr  
- **Messintervall:** Halbjährlich  
- **Datenquelle:** Pentest-Berichte  

---

### 4.10 **Benutzer mit starken Passwörtern (%)**  
- **Definition:** Anteil der Benutzerkonten mit Passwörtern, die den Sicherheitsrichtlinien entsprechen.  
- **Formel:** (Anzahl der Konten mit starken Passwörtern / Gesamtanzahl der Benutzerkonten) * 100  
- **Zielwert:** > 98%  
- **Messintervall:** Quartalsweise  
- **Datenquelle:** Active Directory, Passwort-Management-Tool  

---

## 📊 **5. Visualisierung und Reporting**  

- **Dashboards:**  
  - [ ] KPI-Dashboard im SIEM-System  
  - [ ] Schwachstellen-Heatmap  
  - [ ] Zeitreihen-Analyse von MTTD und MTTR  

- **Berichte:**  
  - [ ] Monatlicher IT-Sicherheitsbericht  
  - [ ] Quartalsweise Risikoberichte für das Management  
  - [ ] Ad-hoc-Berichte bei kritischen Vorfällen  

---

## 🛠 **6. Verantwortlichkeiten**  

| **Metrik**                           | **Verantwortliche Abteilung**   | **Primärer Kontakt**        |  
|-------------------------------------|---------------------------------|-----------------------------|  
| Schwachstellenmanagement            | IT-Sicherheitsteam             | Max Mustermann              |  
| Patch Compliance                    | IT-Abteilung                   | Sarah Müller                |  
| Incident Detection and Response     | SOC-Team                       | Jonas Becker                |  
| Phishing-Simulationen               | HR/IT                          | Laura Schmidt               |  
| Penetrationstests                   | Externer Dienstleister         | Thomas Wagner               |  

---

## 📅 **7. Überprüfung und Aktualisierung**  

- **Überprüfungsintervall:** Quartalsweise  
- **Letzte Überprüfung:** ___________________________  
- **Nächste geplante Überprüfung:** ___________________  
- **Verantwortlich für die Überprüfung:** ____________________  

---

## 📝 **8. Genehmigung**  

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