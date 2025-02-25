# 🛡 **Source Code Audit-Checkliste**  

*Strukturierte Checkliste zur Überprüfung des Quellcodes auf Sicherheitslücken und Best Practices.*  

---

## 📋 **1. Allgemeine Informationen**  

- **Projektname:** ____________________________  
- **Repository/Codebase:** ____________________  
- **Programmiersprache(n):** __________________  
- **Audit durchgeführt von:** __________________  
- **Auditzeitraum:** __________________________  

---

## 🔍 **2. Vorbereitungen des Audits**  

### 2.1 **Zugriff und Einrichtung**  
- [ ] Zugriff auf das vollständige Repository gewährleistet  
- [ ] Abhängigkeiten und Build-Umgebung eingerichtet  
- [ ] Dokumentation und Architekturdiagramme überprüft  
- [ ] Liste der sensiblen Funktionen und kritischen Komponenten erstellt  

### 2.2 **Scope und Zielsetzung**  
- [ ] Umfang des Audits definiert (z. B. gesamte Codebase oder bestimmte Module)  
- [ ] Sicherheitsziele festgelegt (z. B. Schutz vor SQLi, XSS, etc.)  
- [ ] Zu prüfende Sicherheitsrichtlinien und Standards festgelegt (z. B. OWASP, SANS Top 25)  

---

## ⚙ **3. Sicherheits-Checkliste**  

### 3.1 **Authentifizierung und Autorisierung**  
- [ ] Sichere Passwort-Hashing-Algorithmen verwendet (z. B. bcrypt, Argon2)  
- [ ] Multi-Faktor-Authentifizierung implementiert (falls erforderlich)  
- [ ] Schutz vor Brute-Force-Angriffen (Rate Limiting, Captcha)  
- [ ] Zugriffskontrollen korrekt implementiert (RBAC/ABAC)  
- [ ] Session-Management sicher konfiguriert (z. B. HttpOnly, Secure Cookies)  

### 3.2 **Eingabevalidierung und Sanitization**  
- [ ] Alle Benutzereingaben validiert und bereinigt  
- [ ] Schutz vor SQL Injection (Prepared Statements, ORM)  
- [ ] Schutz vor Cross-Site Scripting (XSS) (Escaping, Content Security Policy)  
- [ ] Schutz vor Cross-Site Request Forgery (CSRF) (Tokens, SameSite Cookies)  
- [ ] Reguläre Ausdrücke gegen ReDoS geprüft  

### 3.3 **Fehlerbehandlung und Logging**  
- [ ] Keine sensiblen Informationen in Fehlermeldungen offengelegt  
- [ ] Einheitliche Fehlerbehandlung implementiert  
- [ ] Sichere Protokollierung (Log Injection verhindern)  
- [ ] Zugriffskontrolle auf Logdateien gewährleistet  

### 3.4 **Kryptographie und Datenschutz**  
- [ ] Starke Verschlüsselungsalgorithmen verwendet (AES-256, RSA-2048)  
- [ ] Sichere Speicherung sensibler Daten (z. B. Kreditkartendaten, PII)  
- [ ] Sichere Schlüsselverwaltung (z. B. Vault, AWS KMS)  
- [ ] Schutz vor Insecure Direct Object References (IDOR)  

### 3.5 **Abhängigkeiten und Bibliotheken**  
- [ ] Veraltete oder unsichere Bibliotheken identifiziert und aktualisiert  
- [ ] Verwendung von Software Composition Analysis (SCA) Tools (z. B. Snyk, OWASP Dependency-Check)  
- [ ] Keine bekannten Schwachstellen (CVE) in Drittanbieter-Bibliotheken vorhanden  

### 3.6 **Sichere Programmierpraktiken**  
- [ ] Keine Hardcoded-Credentials im Code  
- [ ] Ressourcen-Freigabe geprüft (Memory Leaks, File Handles)  
- [ ] Schutz vor Command Injection und Path Traversal  
- [ ] Verwendung sicherer APIs und Bibliotheken  

---

## ⚠️ **4. Überprüfung auf spezifische Schwachstellen**  

| **Schwachstelle**                   | **Vorhanden?** | **Kommentar**                            |  
|-------------------------------------|---------------|------------------------------------------|  
| SQL Injection (SQLi)                | [ ] Ja [ ] Nein | ____________________________________ |  
| Cross-Site Scripting (XSS)          | [ ] Ja [ ] Nein | ____________________________________ |  
| Cross-Site Request Forgery (CSRF)   | [ ] Ja [ ] Nein | ____________________________________ |  
| Remote Code Execution (RCE)         | [ ] Ja [ ] Nein | ____________________________________ |  
| Command Injection                   | [ ] Ja [ ] Nein | ____________________________________ |  
| Insecure Deserialization            | [ ] Ja [ ] Nein | ____________________________________ |  
| Sensitive Data Exposure             | [ ] Ja [ ] Nein | ____________________________________ |  
| Broken Authentication               | [ ] Ja [ ] Nein | ____________________________________ |  
| Insecure Direct Object References   | [ ] Ja [ ] Nein | ____________________________________ |  
| Security Misconfiguration           | [ ] Ja [ ] Nein | ____________________________________ |  

---

## 🛠 **5. Verwendete Tools und Techniken**  

- **Statical Analysis Tools (SAST):**  
  - [ ] SonarQube  
  - [ ] Checkmarx  
  - [ ] Fortify  
  - [ ] Andere: ________________________  

- **Dynamische Codeanalyse:**  
  - [ ] Burp Suite  
  - [ ] OWASP ZAP  
  - [ ] Andere: ________________________  

- **Manuelle Codeüberprüfung:**  
  - [ ] Fokus auf kritische Komponenten (z. B. Authentifizierung, Datenzugriff)  
  - [ ] Überprüfung komplexer Logiken und Algorithmen  

---

## 📊 **6. Zusammenfassung der Ergebnisse**  

- **Gesamtzahl gefundener Schwachstellen:** ___  
- **Kritische Schwachstellen:** ___  
- **Hohe Schwachstellen:** ___  
- **Mittlere Schwachstellen:** ___  
- **Niedrige Schwachstellen:** ___  

---

## 📅 **7. Handlungsempfehlungen**  

| **Schwachstelle**                   | **Schweregrad** | **Empfohlene Maßnahme**               | **Verantwortlich**   | **Frist**     |  
|-------------------------------------|----------------|---------------------------------------|----------------------|--------------|  
| SQL Injection im Login-Formular     | Kritisch       | Prepared Statements verwenden         | Max Mustermann       | 10.04.2024   |  
| Hartecodierte Passwörter im Code    | Hoch           | Nutzung sicherer Secrets Management   | Sarah Müller         | 12.04.2024   |  
| Fehlende XSS-Validierung            | Mittel         | Input-Sanitization implementieren     | Jonas Becker         | 15.04.2024   |  
| Unsichere Bibliothek (CVE-2023-1234)| Hoch           | Bibliothek auf neueste Version aktualisieren | Laura Schmidt | 20.04.2024   |  

---

## 🚨 **8. Lessons Learned**  

- [ ] Welche häufigen Fehler traten im Code auf?  
- [ ] Welche Best Practices wurden nicht eingehalten?  
- [ ] Welche Maßnahmen könnten zukünftige Schwachstellen verhindern?  
- [ ] Welche Schulungen sind für das Entwicklerteam sinnvoll?  

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