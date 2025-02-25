# 📊 **Business Impact Analysis (BIA) – Vorlage**  

*Systematische Analyse der potenziellen Auswirkungen von Störungen auf Geschäftsprozesse und Ressourcen.*  

---

## 📋 **1. Ziel der Business Impact Analysis (BIA)**  

Die Business Impact Analysis (BIA) identifiziert kritische Geschäftsprozesse und bewertet die Auswirkungen von Unterbrechungen auf diese Prozesse. Ziel ist es, die notwendigen Maßnahmen zur Risikominderung zu definieren und die Geschäftskontinuität sicherzustellen.

---

## 📑 **2. Allgemeine Informationen**  

- **Erstellt von:** ____________________________  
- **Abteilung:** _______________________________  
- **Datum:** _________________________________  
- **Überprüft von:** ___________________________  
- **Überprüfungsdatum:** ______________________  

---

## 🔍 **3. Kritische Geschäftsprozesse**  

| **Prozess-ID** | **Prozessname**                  | **Abteilung**          | **Prozessverantwortlicher** | **Kritikalitätsstufe** | **Beschreibung**                           |  
|---------------|-----------------------------------|------------------------|----------------------------|-----------------------|-------------------------------------------|  
| PROC-001      | Auftragsbearbeitung              | Vertrieb               | Max Mustermann             | Hoch                  | Bearbeitung und Abwicklung von Bestellungen |  
| PROC-002      | Kundenservice                    | Kundenbetreuung        | Sarah Müller               | Mittel                | Unterstützung und Betreuung von Kunden     |  
| PROC-003      | Rechnungsstellung                | Buchhaltung            | Thomas Wagner              | Hoch                  | Erstellung und Versand von Rechnungen      |  
| PROC-004      | Lagerverwaltung                  | Logistik               | Laura Schmidt              | Niedrig               | Verwaltung des Lagerbestands               |  
| PROC-005      | Gehaltsabrechnung                | HR                     | Jonas Becker               | Hoch                  | Abwicklung der Gehaltszahlungen            |  

---

## ⚠️ **4. Auswirkungen einer Unterbrechung**  

| **Prozess-ID** | **Auswirkung auf Geschäftsbetrieb**        | **Finanzielle Verluste (€/Tag)** | **Imageschaden** | **Compliance-Risiko** | **Sicherheitsrisiko** |  
|---------------|--------------------------------------------|-------------------------------|-----------------|----------------------|----------------------|  
| PROC-001      | Verzögerte Auftragsabwicklung              | 15.000                        | Hoch            | Mittel               | Niedrig              |  
| PROC-002      | Unzufriedene Kunden                        | 5.000                         | Mittel          | Niedrig              | Niedrig              |  
| PROC-003      | Zahlungsrückstände                         | 20.000                        | Hoch            | Hoch                 | Niedrig              |  
| PROC-004      | Lagerfehlbestände                          | 2.500                         | Niedrig         | Niedrig              | Niedrig              |  
| PROC-005      | Gehaltszahlungen verspätet                | 10.000                        | Hoch            | Hoch                 | Mittel               |  

---

## ⏱ **5. Wiederanlauf- und Wiederherstellungszeiten**  

| **Prozess-ID** | **Maximal tolerierbare Ausfallzeit (RTO)** | **Maximal tolerierbarer Datenverlust (RPO)** |  
|---------------|--------------------------------------------|---------------------------------------------|  
| PROC-001      | 12 Stunden                                 | 4 Stunden                                   |  
| PROC-002      | 24 Stunden                                 | 8 Stunden                                   |  
| PROC-003      | 8 Stunden                                  | 2 Stunden                                   |  
| PROC-004      | 48 Stunden                                 | 12 Stunden                                  |  
| PROC-005      | 4 Stunden                                  | 1 Stunde                                    |  

- **RTO (Recovery Time Objective):** Maximal akzeptable Ausfallzeit für den Prozess  
- **RPO (Recovery Point Objective):** Maximales Datenverlustintervall in Stunden  

---

## 🛡 **6. Kritische Ressourcen und Abhängigkeiten**  

| **Prozess-ID** | **Benötigte IT-Systeme/Anwendungen**   | **Mitarbeiteranzahl** | **Externe Abhängigkeiten**                |  
|---------------|-----------------------------------------|-----------------------|------------------------------------------|  
| PROC-001      | ERP-System, CRM                         | 10                    | Logistikdienstleister                    |  
| PROC-002      | Helpdesk-Software, Telefonanlage        | 8                     | VoIP-Anbieter                            |  
| PROC-003      | Buchhaltungssoftware, E-Mail-System     | 5                     | Steuerberater                            |  
| PROC-004      | Lagerverwaltungssystem, Barcode-Scanner | 6                     | Lieferanten                              |  
| PROC-005      | Gehaltsabrechnungssoftware              | 3                     | Bankdienstleister                        |  

---

## 🚨 **7. Risikobewertung**  

| **Risiko-ID** | **Risiko**                          | **Wahrscheinlichkeit** | **Auswirkung** | **Risikoniveau** | **Empfohlene Maßnahme**            |  
|--------------|-------------------------------------|------------------------|---------------|-----------------|------------------------------------|  
| RISK-001     | Serverausfall                      | Hoch                   | Katastrophal  | Kritisch        | Implementierung eines Failover-Systems |  
| RISK-002     | Cyberangriff (Ransomware)          | Mittel                 | Hoch          | Hoch            | Stärkung der IT-Sicherheitsmaßnahmen |  
| RISK-003     | Stromausfall im Rechenzentrum      | Niedrig                | Mittel        | Mittel          | Backup-Stromversorgung installieren  |  
| RISK-004     | Ausfall des VoIP-Dienstleisters    | Mittel                 | Mittel        | Mittel          | Backup-Kommunikationskanal einrichten |  
| RISK-005     | Menschliches Versagen              | Hoch                   | Mittel        | Hoch            | Regelmäßige Schulungen für Mitarbeitende |  

---

## 🛠 **8. Maßnahmen zur Risikominderung**  

- Implementierung von Hochverfügbarkeitslösungen für kritische Systeme  
- Regelmäßige Backups mit Überprüfung der Wiederherstellbarkeit  
- Etablierung von Notfallkommunikationsplänen  
- Durchführung regelmäßiger Schulungen und Awareness-Programme  
- Zusammenarbeit mit vertrauenswürdigen Drittanbietern zur Absicherung externer Abhängigkeiten  

---

## 📅 **9. Test und Validierung**  

| **Test-ID** | **Testart**                   | **Datum**       | **Ergebnis**       | **Verbesserungen**                       |  
|------------|-------------------------------|----------------|-------------------|------------------------------------------|  
| TEST-001   | Backup-Wiederherstellung       | 01.03.2024     | Erfolgreich       | Keine                                    |  
| TEST-002   | Notfallkommunikation           | 15.03.2024     | Verbesserungswürdig | Optimierung der Kontaktliste erforderlich |  
| TEST-003   | Failover-Test                  | 20.03.2024     | Fehlgeschlagen    | Konfiguration des Failover-Systems prüfen |  
| TEST-004   | Cyberangriff-Simulation        | 25.03.2024     | Erfolgreich       | Zusätzliche Phishing-Trainings einführen |  

---

## 📊 **10. Abschlussbewertung**  

- [ ] Alle kritischen Geschäftsprozesse wurden identifiziert und bewertet  
- [ ] Wiederherstellungszeiten (RTO/RPO) sind dokumentiert  
- [ ] Maßnahmen zur Risikominderung wurden geplant und implementiert  
- [ ] Test- und Validierungsmaßnahmen wurden durchgeführt  

**Datum der letzten Überprüfung:** ___________________  
**Verantwortlich:** _________________________________  

---

## 📝 **11. Genehmigung**  

**Erstellt von:**  
Name: ____________________________  
Position: _________________________  
Datum: ___________________________  

**Genehmigt von:**  
Name: ____________________________  
Position: _________________________  
Datum: ___________________________  