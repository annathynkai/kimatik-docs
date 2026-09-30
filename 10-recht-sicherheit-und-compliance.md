## 10. Recht, Sicherheit & Compliance

### 10.1 Anbieter

**dryven GmbH**
- Geschäftsführung: Anna Kofler, Jörg Summer.
- UID: ATU78748278. FN: 590486 m (Landesgericht St. Pölten).
- Sitz & Büro Niederösterreich: Europaplatz 7, 3100 St. Pölten.
- Büro Oberösterreich: Römerstraße 4, 4020 Linz.

### 10.2 Rechtliche Dokumente (Website, Stand 04.09.2026)

| Dokument | Pfad |
| --- | --- |
| AGB | `kimatik.com/agb` |
| Auftragsverarbeitungsvertrag (AVV, Art. 28 DSGVO) | `kimatik.com/avv` |
| Datenschutzerklärung (Website) | `kimatik.com/datenschutz` |
| Impressum | `kimatik.com/impressum` |
| Sicherheit & Datenschutz (Überblick) | `kimatik.com/sicherheit-datenschutz` |

In der App führen `/agb` und `/impressum` zur Website, `/datenschutz` zum AVV. Bei der Registrierung werden AGB und AVV akzeptiert.

### 10.3 Wesentliche AGB-Punkte

- **Zielgruppe:** Unternehmer im Sinne des § 1 UGB (B2B).
- **Leistung:** Digitale Mitarbeitende auf Basis von KI-Modellen (LLMs), teils mit Automatisierungsplattformen. Zugriff auf Drittsysteme über API.
- **Kein dezidiertes SLA.** Angestrebt ist eine Verfügbarkeit von **99 % im Jahresmittel**. Ausgenommen sind angekündigte Wartungsfenster und Störungen bei Drittanbietern.
- **KI-Hinweis:** Ergebnisse können fehlerhaft sein („Halluzinationen“). Für die inhaltliche Richtigkeit wird keine Garantie übernommen.
- **Human-in-the-Loop als Pflicht der Kund:innen:** Alle Ergebnisse müssen vor jeder Verwendung geprüft werden. Die Qualität des Briefings (Einschulung) liegt bei den Kund:innen.
- **Rechte:** Arbeitsergebnisse gehen mit ihrer Entstehung auf die Kund:innen über. Die Rechte an Software und Plattform bleiben beim Anbieter.
- **Preise:** Anpassungen werden vorab angekündigt und berechtigen zur Sonderkündigung. Bei Zahlungsverzug oder Missbrauch darf der Dienst ausgesetzt werden.
- **Mängel:** innerhalb von 7 Werktagen schriftlich melden (E-Mail genügt).
- **Recht und Gerichtsstand:** Es gilt österreichisches Recht (ohne UN-Kaufrecht). Gerichtsstand ist der Sitz des Anbieters.

### 10.4 Datenschutz & DSGVO

- Verarbeitung auf Basis des **AVV nach Art. 28 DSGVO**. Für Daten, die digitale Mitarbeitende im Auftrag verarbeiten, ist kimatik Auftragsverarbeiter; die Kund:innen bleiben Verantwortliche.
- **Kein Training:** Weder kimatik noch die eingesetzten KI-Anbieter nutzen Eingaben oder Ergebnisse zum Modelltraining; das ist vertraglich ausgeschlossen.
- **Keine unnötige Speicherung:** Anfragen werden zur Bearbeitung an die KI-Modelle weitergeleitet, dort aber nicht dauerhaft gespeichert.
- **Datensparsamkeit:** Es wird nur verarbeitet, was die jeweilige Aufgabe erfordert.
- **Nach Vertragsende:** Personenbezogene Daten werden gelöscht, soweit keine gesetzliche Aufbewahrungspflicht besteht.
- **Betroffenenrechte:** über `office@kimatik.com` (wie in der Datenschutzerklärung). Beschwerden sind bei der Österreichischen Datenschutzbehörde möglich.

### 10.5 Serverstandorte & Dienstleister (öffentliche Liste laut AVV, Anlage II)

| Zweck | Dienstleister | Standort / Grundlage |
| --- | --- | --- |
| Hosting (Frontend, API, Website) | Hetzner Online GmbH | EU-Rechenzentren (Deutschland) |
| Datenbank, Login, Dateispeicher | Supabase | EU-Region |
| KI-Modelle Gemini | Google Cloud (Vertex AI) | EU-Regionen, keine globalen Modellvarianten |
| KI-Modelle Claude | OpenRouter (EU-Routing) → AWS Bedrock / Google Vertex AI | EU-Endpunkte; ohne EU-Endpunkt schlägt die Anfrage fehl |
| Modell-Weiterleitung | LiteLLM (von kimatik selbst betrieben) | Hetzner EU, keine Speicherung personenbezogener Daten |
| Zahlungen | Stripe Payments Europe | Stripe-DPA, EU-Standardvertragsklauseln |
| Fehlerüberwachung | Sentry (EU-Hosting) | nur technische, pseudonymisierte Metadaten, keine Inhalte |
| E-Mail-Versand | Loops (USA) | EU-Standardvertragsklauseln (Art. 46 DSGVO) |

Über Änderungen an den Dienstleistern werden Kund:innen informiert. Widerspruch ist innerhalb von 14 Tagen möglich. Die rechtlich verbindliche Liste ist Anlage II des AVV (`kimatik.com/avv`). Weicht eine Kurzfassung davon ab, gilt der AVV.

**Wo Daten liegen (Trust Center):** Hosting in den EU-Rechenzentren von Hetzner (Deutschland). Benutzer-, Lizenz- und Konfigurationsdaten in der EU (Supabase). KI-Anfragen innerhalb der EU („EU Residency“ / „EU in-region Routing“).

**Anfrageweg (Trust Center):**
1. Anfrage an ein digitales Teammitglied (Frage oder Dokument).
2. Aufbereitung auf der Plattform, gehostet in der EU, inklusive Konto- und Lizenzdaten.
3. Weiterleitung an das passende KI-Modell. Eingesetzt werden Modelle der großen Anbieter (derzeit Gemini und Claude) auf EU-Servern.
4. Die Antwort entsteht auf dem EU-Server. Der Anbieter speichert die Anfrage nicht dauerhaft und nutzt sie nicht fürs Training.
5. Das Ergebnis wird angezeigt.

### 10.6 Technische Sicherheit

Entspricht dem Trust Center auf `kimatik.com/sicherheit-datenschutz`.

**Verschlüsselung**
- Verschlüsselte Übertragung (TLS/SSL) zwischen Nutzer:innen, der Plattform und allen angebundenen Diensten.
- Verschlüsselte Speicherung („at rest“).

**Zugriff nach dem Prinzip der minimalen Rechte**
- Interner Zugriff nur für Personen, die ihn zur Aufgabenerfüllung brauchen (Need-to-know).
- Absicherung der wichtigsten Systeme mit Multi-Faktor-Authentifizierung.
- Trennung der Daten, sodass Inhalte voneinander abgegrenzt bleiben.
- Zugangsdaten und API-Schlüssel werden sicher verwahrt und sind nie im Frontend sichtbar.

**Sicherer Betrieb**
- Regelmäßige Backups und Wiederherstellungskonzepte.
- Monitoring und laufende Aktualisierung der Systeme.
- Protokollierung administrativer Zugriffe. Fehlerprotokolle enthalten keine personenbezogenen Inhalte.

### 10.7 Human-in-the-Loop in der App

- **Ivana:** Belege stehen zunächst auf **Entwurf** und werden erst über **Speichern & freigeben** übernommen.
- **Redaktionsplan:** Veröffentlichung nur über den Statuswechsel durch die Nutzer:innen.
- **Emil (auf Anfrage):** Kalenderänderungen und ClickUp-Aufgaben nur nach Bestätigung.
- **Stefan:** GHS-Symbole und Lagerklasse werden regelbasiert berechnet, nicht von der KI geschätzt.

### 10.8 EU AI Act: KI-Kennzeichnung

Generierte oder bearbeitete Bilder lassen sich pro Bild über den Schalter **KI-Kennzeichnung** sichtbar als KI-erzeugt markieren (Kapitel 7.4). Ob eine Kennzeichnung für die jeweilige Verwendung nötig ist, entscheiden die Kund:innen.

### 10.9 Konto- & Datenlöschung

Einstellungen → **Gefahrenzone** → **Account löschen** (Bestätigung durch Eintippen von `DELETE`). Ein laufendes Abo vorher unter **Abrechnung → Abo kündigen** beenden.

---
