# ⚖ **Risk Register (Risikoregister)**  

*Zentrale Dokumentation zur Erfassung, Bewertung und Verwaltung von Risiken im Unternehmen.*  

---

## 📋 **1. Ziel des Risikoregisters**  

Das Risikoregister dient als zentrales Instrument zur Identifikation, Bewertung, Überwachung und Behandlung von Risiken, die den Geschäftsbetrieb oder die IT-Infrastruktur beeinträchtigen könnten. Es ermöglicht eine strukturierte Vorgehensweise zur Risikominderung und fördert die Einhaltung von Compliance-Anforderungen.

---

## 📑 **2. Risikoinventar**  

| **Risiko-ID** | **Beschreibung**                           | **Ursache**                      | **Auswirkung**                         | **Wahrscheinlichkeit** | **Auswirkungsgrad** | **Risikoniveau** | **Status**       | **Verantwortlich** | **Frist**     |  
|--------------|--------------------------------------------|----------------------------------|----------------------------------------|------------------------|--------------------|-----------------|------------------|--------------------|--------------|  
| RISK-001     | Ungepatchte kritische Schwachstellen       | Fehlendes Patch-Management      | Systemkompromittierung, Datenverlust   | Hoch                   | Katastrophal       | Kritisch        | Offen            | Max Mustermann     | 05.04.2024   |  
| RISK-002     | Veraltete Zugriffskontrollen               | Fehlende Richtlinien            | Unbefugter Zugriff auf Systeme         | Mittel                 | Hoch               | Hoch            | In Bearbeitung   | Sarah Müller       | 10.04.2024   |  
| RISK-003     | Fehlende Netzwerksicherheit                | Unzureichende Segmentierung     | Ausbreitung von Malware im Netzwerk    | Niedrig                | Mittel             | Mittel          | Offen            | Thomas Wagner      | 15.04.2024   |  
| RISK-004     | Unzureichende Passwort-Policy              | Schwache Passwörter             | Erhöhte Wahrscheinlichkeit von Angriffen | Hoch                 | Niedrig            | Mittel          | Offen            | Jonas Becker       | 07.04.2024   |  
| RISK-005     | Veraltetes SSL/TLS-Zertifikat              | Abgelaufenes Zertifikat         | Sicherheitswarnungen, Vertrauensverlust | Sehr hoch            | Mittel             | Hoch            | Behoben          | Laura Schmidt      | 01.04.2024   |  

---

## 🔍 **3. Risikobewertung**  

### **3.1 Wahrscheinlichkeit (Likelihood)**  

| **Bewertung**        | **Wahrscheinlichkeit** | **Beschreibung**                                         |  
|----------------------|------------------------|---------------------------------------------------------|  
| Sehr hoch (5)        | 5                      | Tritt fast sicher ein, mehrmals pro Jahr                |  
| Hoch (4)             | 4                      | Tritt häufig ein, mindestens einmal pro Jahr            |  
| Mittel (3)           | 3                      | Könnte eintreten, einmal in 2-3 Jahren                  |  
| Niedrig (2)          | 2                      | Seltenes Eintreten, einmal in 5 Jahren                  |  
| Sehr niedrig (1)     | 1                      | Sehr unwahrscheinlich, tritt kaum ein                   |  

---

### **3.2 Auswirkung (Impact)**  

| **Bewertung**        | **Auswirkungsgrad**    | **Beschreibung**                                         |  
|----------------------|------------------------|---------------------------------------------------------|  
| Katastrophal (5)     | 5                      | Kritische Geschäftsunterbrechung, erheblicher finanzieller Schaden |  
| Hoch (4)             | 4                      | Große Unterbrechung, Datenverlust, erheblicher Imageschaden |  
| Mittel (3)           | 3                      | Moderate Auswirkungen, reduzierte Serviceverfügbarkeit |  
| Niedrig (2)          | 2                      | Geringfügige Störungen, schnell behebbare Vorfälle     |  
| Sehr niedrig (1)     | 1                      | Keine nennenswerten Auswirkungen                        |  

---

### **3.3 Risikomatrix**  

| **Auswirkung** / **Wahrscheinlichkeit** | **Sehr niedrig (1)** | **Niedrig (2)** | **Mittel (3)** | **Hoch (4)** | **Sehr hoch (5)** |  
|-----------------------------------------|----------------------|----------------|---------------|-------------|-------------------|  
| **Katastrophal (5)**                    | Mittel               | Hoch           | Hoch          | Kritisch    | Kritisch          |  
| **Hoch (4)**                            | Mittel               | Mittel         | Hoch          | Hoch        | Kritisch          |  
| **Mittel (3)**                          | Niedrig              | Mittel         | Mittel        | Hoch        | Hoch              |  
| **Niedrig (2)**                         | Niedrig              | Niedrig        | Mittel        | Mittel      | Hoch              |  
| **Sehr niedrig (1)**                    | Niedrig              | Niedrig        | Niedrig       | Mittel      | Mittel            |  

**Legende:**  
- 🟥 **Kritisch:** Sofortige Maßnahmen erforderlich  
- 🟧 **Hoch:** Maßnahmen zeitnah umsetzen  
- 🟨 **Mittel:** Beobachten und mittelfristig beheben  
- 🟩 **Niedrig:** Keine unmittelbaren Maßnahmen erforderlich  

---

## 🛠 **4. Risikobehandlungsmaßnahmen**  

| **Risiko-ID** | **Maßnahme**                              | **Verantwortlich** | **Frist**     | **Status**       | **Kommentar**                     |  
|--------------|-------------------------------------------|--------------------|--------------|------------------|-----------------------------------|  
| RISK-001     | Patch-Management einführen               | Max Mustermann     | 05.04.2024   | Offen            | Kritische Schwachstellen vorhanden |  
| RISK-002     | Zugriffskontrollrichtlinien aktualisieren | Sarah Müller       | 10.04.2024   | In Bearbeitung   | Neue Richtlinien in Entwicklung   |  
| RISK-003     | Netzwerksegmentierung implementieren     | Thomas Wagner      | 15.04.2024   | Offen            | VLAN-Konfiguration geplant        |  
| RISK-004     | Starke Passwort-Policy umsetzen          | Jonas Becker       | 07.04.2024   | Offen            | Benutzer müssen Passwörter ändern |  
| RISK-005     | SSL/TLS-Zertifikat erneuern              | Laura Schmidt      | 01.04.2024   | Behoben          | Zertifikat wurde aktualisiert     |  

---

## 📊 **5. Metriken und KPIs**  

| **Metrik**                            | **Wert**    | **Zielwert** |  
|---------------------------------------|------------|--------------|  
| Anzahl offener Risiken                | X          | < 50         |  
| Anzahl kritischer Risiken             | X          | 0            |  
| Durchschnittliche Zeit zur Behebung   | X Tage     | < 30 Tage    |  
| Risikoakzeptanzquote (%)              | X %        | < 10 %       |  
| Anzahl abgeschlossener Maßnahmen      | X          | > 90 %       |  

---

## 🚨 **6. Eskalationsprozess**  

1. **Stufe 1:** Kritische Risiken werden innerhalb von 24 Stunden gemeldet.  
2. **Stufe 2:** Nach 48 Stunden ohne Maßnahmen erfolgt eine Eskalation an den IT-Leiter.  
3. **Stufe 3:** Nach 72 Stunden wird die Geschäftsleitung informiert.  

---

## 📅 **7. Überwachung und Aktualisierung**  

- Monatliche Überprüfung des Risikoregisters auf neue oder geänderte Risiken  
- Quartalsweise Aktualisierung der Risikobewertung und Maßnahmen  
- Jährliche Überprüfung der Risikomanagement-Strategie  

---

## ✅ **8. Abschluss und Freigabe**  

- [ ] Alle identifizierten Risiken wurden bewertet und dokumentiert.  
- [ ] Maßnahmen zur Risikominderung wurden geplant und eingeleitet.  
- [ ] Das Risikoregister wurde an relevante Stakeholder weitergeleitet.  

**Datum der letzten Überprüfung:** ___________________  
**Verantwortlich:** _________________________________  