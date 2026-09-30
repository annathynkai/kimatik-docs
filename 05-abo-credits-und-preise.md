## 5. Abo, Credits & Preise

### 5.1 Das Modell in einem Satz

**Ein Abo. Dein ganzes Team.** Das Abo enthält ein monatliches Credit-Kontingent und den Zugang zu allen einschulbaren digitalen Mitarbeitenden — ohne Zusatzkosten pro Teammitglied. Jede Aufgabe verbraucht je nach Umfang und Komplexität Credits.

**Im Abo enthalten (Website):**
- Zugang zu allen digitalen Mitarbeitenden
- Beliebig viele Profile pro digitalen Mitarbeitenden – z. B. für Projekte, Marken oder Teams
- Eigene Assistenten erstellen mit Alina
- Gemeinsame Arbeit an Ressourcen
- Persönlicher Support aus Österreich
- Monatlich kündbar

### 5.2 Was sind Credits?

Credits sind die Verbrauchseinheit von kimatik. Verbraucht wird bei Chat-Antworten, Dokumentverarbeitung, Bildgenerierung, Recherche, Vertonung usw.

**Richtwerte (Website):**

| Teammitglied | Aufgabe | Credits |
| --- | --- | --- |
| Alina | Allgemeine Anfrage | ca. 1 (je nach Komplexität); Expertin ca. 3× |
| Ivana | Rechnung verbuchen | ca. 2 |
| Penelope | Bild erstellen | ca. 16 |
| Sven | Social-Media-Post | ca. 10 |
| Sven | Wochenplan | ca. 12 |
| Sven | Post optimieren | ca. 4 |
| Stefan | Sicherheitsdatenblatt | ca. 50 |
| Bernhard | Bescheid | ca. 50 |
| Nina *(auf Anfrage)* | Recherche | ca. 2 |
| Theo *(auf Anfrage)* | Blogartikel / Newsletter / Website-Text | ca. 8 / 6 / 5 |
| Viola *(auf Anfrage)* | Videominute | ca. 20 |
| Paula *(auf Anfrage)* | Episoden-Skript | ca. 6 |

Beispiel Website: „90 Credits ≈ 45 Beleg-Verarbeitungen“ bei Ivana.

**Credit-Rechner (`kimatik.com/preise`):** Tätigkeiten-Rechner mit den Positionen „Allgemeine Anfragen“, „Social Media Post“, „Rechnungen verarbeiten“, „Dokumente analysieren“ (SDB, Bescheide), „Recherchen durchführen“ (bis zu 12 Artikel pro Recherche) und „Fotos bearbeiten und generieren“. Er schätzt den monatlichen Credit-Bedarf und die eingesparte Zeit (Annahme: 80 % Automatisierung, 20 % bleibt Human-in-the-Loop, 50 €/Stunde).

**Anzeige in der App:** Verbrauchte Credits mit zwei Nachkommastellen, österreichisches Zahlenformat. Im Chat-Kopf erscheint die Pill **„{n} Credits übrig“**, sobald von den Abo-Credits noch höchstens 10 übrig sind. Pro Nachricht wird kein Verbrauch angezeigt. Viola zeigt nach dem Rendern „Credits abgerechnet: {n}“.

### 5.3 Abo-Pakete

Die Pakete werden **live aus Stripe** geladen (App-Checkout und Website). Standardauswahl auf der Website: 90 Credits. Aktueller Katalog bzw. Website-Fallback:

| Credits / Monat | Preis / Monat (netto) |
| --- | --- |
| 90 | 9 € |
| 250 | 25 € |
| 500 | 50 € |
| 1.000 (beliebt) | 100 € |
| 2.500 | 250 € |
| 6.000 | 600 € |

**Alle Preise netto zzgl. 20 % USt.** Einstieg: **ab 9 €/Monat**.

### 5.4 Checkout (`/checkout`)

- Überschrift „Ein Abo. Alle Teammitglieder.“; Paketauswahl (vorausgewählt: Paket aus dem Link, sonst „beliebt“, sonst das günstigste).
- Buttons **Jetzt einschulen** bzw. **Jetzt Abo abschließen**; Hinweis „Sichere Bezahlung über Stripe“; Link „Mehr Infos zu Credits“ → `kimatik.com/preise`.
- Bezahlung auf der Stripe-Checkout-Seite (dort auch Eingabefeld für Aktionscodes).
- Ohne Login leitet `/checkout` zur Registrierung weiter.
- Erfolg: `/checkout-erfolg` bzw. direkt weiter in die Einschulung des gewählten Teammitglieds.

### 5.5 Credits aufladen (Top-Up)

- `/credits-aufladen` — **nur mit aktivem Abo** (sonst Weiterleitung zu `/checkout`).
- **1 bis 10 Pakete** pro Kauf (Schieberegler), Bezahlung über Stripe. Paketgröße und Preis kommen aus dem Stripe-Top-Up-Produkt.
- „Top-Up-Credits verfallen nicht. Sie werden erst verbraucht, sobald die monatlichen Abo-Credits vollständig eingesetzt wurden.“

### 5.6 Verbrauchsreihenfolge

1. **Abo-Credits** der laufenden Periode
2. **Top-Up-Credits** (verfallen nicht)

Ohne aktives Abo sind Chat und Apps gesperrt (Weiterleitung zu `/checkout`).

### 5.7 Abrechnung (`/abrechnung`)

- **Dein Abo:** Paketname, monatliche Credits, Abrechnungszeitraum; Menü **Abo kündigen**.
- **Abo anpassen:** Paketwechsel über das Stripe-Kundenportal; geplante Wechsel werden als Hinweis angezeigt.
- **Deine Credits:** **Abo-Credits**, **Top-Up-Credits**, **Gesamt verfügbar**, Button **Credits aufladen**.
- **Zahlung, Abo & Rechnungen:** **Zahlung & Rechnungen verwalten** öffnet das Stripe-Kundenportal (Rechnungen, Zahlungsmethode, Rechnungsadresse, UID).
- Ohne Abo: „Abo erforderlich“ / **Jetzt Abo abschließen**.

### 5.8 Kündigung

- Monatlich kündbar, keine Mindestlaufzeit; Kündigung über **Abo kündigen** (Stripe-Portal) zum Ende der laufenden Periode.
- Nach der Kündigung zeigt die App: „Abo gekündigt. Dein digitales Team ist noch bis {Datum} einsatzbereit.“ mit **Abo jetzt erneuern**.
- Nach Periodenende sind Chat und Apps gesperrt.
- **Einzelne Teammitglieder** können Kund:innen in der App nicht selbst abmelden. Das erledigt das kimatik-Team auf Anfrage. Ein abgemeldetes Teammitglied kann später wieder eingeschult werden.
- **Geld-zurück-Garantie:** Laut Website 30 Tage („Wenn dich dein digitales Team nicht überzeugt, bekommst du dein Geld zurück.“). Abwicklung über den Support.

---
