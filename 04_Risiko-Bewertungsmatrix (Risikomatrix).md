# ⚖ **Risiko-Bewertungsmatrix (Risikomatrix)**  

*Strukturierte Bewertung von Risiken basierend auf Wahrscheinlichkeit und Auswirkung.*  

---

## 📋 **1. Ziel der Risikomatrix**  

Die Risikomatrix dient der standardisierten Bewertung von Sicherheitsrisiken. Durch die Kategorisierung nach Wahrscheinlichkeit und Auswirkung können Risiken effektiv priorisiert und entsprechende Maßnahmen zur Risikominderung ergriffen werden.

---

## 📑 **2. Risikobewertungs-Kriterien**  

### **2.1 Wahrscheinlichkeit (Likelihood)**  

| **Wahrscheinlichkeit** | **Bewertung** | **Beschreibung**                                               |  
|------------------------|---------------|-----------------------------------------------------------------|  
| Sehr hoch (5)          | 5             | Tritt fast sicher ein, mehrmals im Jahr                         |  
| Hoch (4)               | 4             | Tritt häufig ein, mindestens einmal pro Jahr                    |  
| Mittel (3)             | 3             | Könnte eintreten, einmal in 2-3 Jahren                          |  
| Niedrig (2)            | 2             | Seltenes Eintreten, einmal in 5 Jahren                          |  
| Sehr niedrig (1)       | 1             | Sehr unwahrscheinlich, tritt kaum ein                           |  

---

### **2.2 Auswirkung (Impact)**  

| **Auswirkung**         | **Bewertung** | **Beschreibung**                                               |  
|------------------------|---------------|-----------------------------------------------------------------|  
| Katastrophal (5)       | 5             | Kritische Geschäftsunterbrechung, erheblicher finanzieller Schaden |  
| Hoch (4)               | 4             | Große Unterbrechung, Datenverlust, erheblicher Imageschaden     |  
| Mittel (3)             | 3             | Moderate Auswirkungen, reduzierte Serviceverfügbarkeit         |  
| Niedrig (2)            | 2             | Geringfügige Störungen, schnell behebbare Vorfälle             |  
| Sehr niedrig (1)       | 1             | Keine nennenswerten Auswirkungen                               |  

---

## 📊 **3. Risikomatrix**  

Die Kombination von Wahrscheinlichkeit und Auswirkung ergibt das Risikoniveau:

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

## 🛡 **4. Risikoanalyse und Bewertung**  

| **Risiko-ID** | **Beschreibung**                   | **Wahrscheinlichkeit** | **Auswirkung** | **Risikoniveau** | **Empfohlene Maßnahme**              |  
|--------------|------------------------------------|------------------------|---------------|-----------------|--------------------------------------|  
| RISK-001     | Ungepatchte kritische Schwachstelle | Hoch (4)               | Katastrophal (5) | Kritisch        | Sofortiges Patching                  |  
| RISK-002     | Veraltete Zugriffskontrollen       | Mittel (3)             | Hoch (4)      | Hoch            | Zugriffskontrollen aktualisieren    |  
| RISK-003     | Fehlende Netzwerkssegmentierung    | Niedrig (2)            | Mittel (3)    | Mittel          | Einführung von VLANs                |  
| RISK-004     | Unzureichende Passwort-Policy      | Hoch (4)               | Niedrig (2)   | Mittel          | Durchsetzung starker Passwörter     |  
| RISK-005     | Veraltetes SSL/TLS-Zertifikat      | Sehr hoch (5)          | Mittel (3)    | Hoch            | Zertifikat aktualisieren            |  

---

## ⚙ **5. Risikobehandlungsoptionen**  

- ✅ **Akzeptieren:** Risiko ist bekannt, aber akzeptabel.  
- 🛡 **Mildern:** Maßnahmen zur Risikominderung umsetzen.  
- 🔁 **Übertragen:** Risiko an Dritte abgeben (z. B. Versicherung).  
- 🚫 **Vermeiden:** Risikoverursachende Aktivität einstellen oder ändern.  

---

## 📅 **6. Risikomanagement-Zyklus**  

1. **Identifikation:** Alle potenziellen Risiken erkennen.  
2. **Bewertung:** Risiken bewerten und priorisieren (Mithilfe der Matrix).  
3. **Behandlung:** Maßnahmen zur Risikominimierung umsetzen.  
4. **Überwachung:** Risiken regelmäßig überwachen und neu bewerten.  
5. **Berichterstattung:** Management über aktuelle Risiken informieren.  

---

## ✅ **7. Abschluss**  

- [ ] Alle identifizierten Risiken bewertet und dokumentiert.  
- [ ] Maßnahmen zur Risikominderung geplant und eingeleitet.  
- [ ] Regelmäßige Überprüfung und Aktualisierung der Risikomatrix eingeplant.  

**Datum der letzten Überprüfung:** ___________________  
**Verantwortlich:** _________________________________  