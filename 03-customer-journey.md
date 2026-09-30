## 3. Customer Journey

Die Reise vom ersten Websitebesuch bis zur produktiven Nutzung in sechs Schritten.

### 3.1 Schritt 1: Entdecken (Website)

Auf `kimatik.com` lernen Besucher:innen das Personalverleih-Konzept kennen. Wichtige Seiten:

- `/digitale-mitarbeitende` — Marktplatz aller 25 Teammitglieder mit Filter nach Bereich (Admin & Buchhaltung, Marketing & Sales, Produktmanagement, Ingenieurbüros) und Status („Sofort verfügbar“ / „Auf Anfrage“).
- `/digitale-mitarbeitende/sven` und `/digitale-mitarbeitende/ivana` — eigene Landingpages; andere Teammitglieder werden im Marktplatz-Profil gezeigt.
- `/preise` (Abo, Credit-Rechner nach Tätigkeiten, „Was ist ein Credit?“), `/funktionen`, `/zusammenarbeit`, `/vergleich`, `/glossar`, `/faq`, `/sicherheit-datenschutz`, `/loesungen/…`.
- Demo-Termin mit Anna Kofler über Microsoft Bookings (Link auf der Website).

### 3.2 Schritt 2: Team zusammenstellen & registrieren

- Auf der Website führt **„Einschulen“** bei einem Teammitglied zu `app.kimatik.com/registrieren?dma=<ID>`; der Team-Builder `kimatik.com/einschulen` („Stelle dein Team in wenigen Minuten zusammen“) zeigt alle Teammitglieder auf einen Blick.
- Kauf-Buttons auf `/preise` führen zu `/registrieren?dma=<Alina-ID>&price=<Paket>`.
- `/registrieren` funktioniert nur mit `?dma=` oder `?checkout=`; ohne Parameter leitet die App zu `/digitales-team` weiter. `/login?mode=signup` und „Jetzt registrieren“ auf der Login-Seite führen zu `kimatik.com/einschulen`.
- Registrierungsformular: Vorname, Nachname, „Dein Unternehmen“, E-Mail, Passwort (min. 6 Zeichen), Zustimmung zu AGB und AVV.
- „Auf Anfrage“-Teammitglieder können nicht registriert werden; stattdessen Anfrage über Kontaktformular bzw. Button **Anfragen** in der App.

### 3.3 Schritt 3: E-Mail bestätigen

Nach dem Absenden kommt ein **6-stelliger Bestätigungscode** per E-Mail (gültig 60 Minuten, erneut anforderbar nach 60 Sekunden). Nach Eingabe erscheint „E-Mail erfolgreich bestätigt!“ mit **Onboarding starten** bzw. **Weiter zum Checkout**. Das Teammitglied aus dem Link wird angelegt; **Alina** kommt automatisch dazu.

### 3.4 Schritt 4: Abo abschließen

Für Chat und Apps ist ein **aktives Abo** nötig — es gibt **keine Probe-Credits**. Ohne Abo führt die App zu `/checkout` („Ein Abo. Alle Teammitglieder.“). Pakete werden live aus Stripe geladen; Bezahlung über Stripe Checkout. Nach Erfolg: weiter in die Einschulung bzw. `/checkout-erfolg`.

### 3.5 Schritt 5: Einschulung

Im **Einschulungs-Chat** (`/onboarding/<Enrollment-ID>`) lernt das Teammitglied Unternehmen, Marke, Tonalität und Anwendungsfälle kennen (z. B. Website-URL für Sven, Autorisierte Absender für Ivana/Stefan/Bernhard). Die Einschulung kann unterbrochen und fortgesetzt und später pro Profil neu gestartet werden (**Einschulung neu starten**). Weitere Teammitglieder holst du jederzeit kostenfrei dazu — in der App über `/digitales-team` → **Jetzt einschulen** oder über eine noch nicht freigeschaltete App (**Einschulen** im Dialog „So bekommst du diese App“).

### 3.6 Schritt 6: Produktiv arbeiten

- **Startseite `/`** — neuen Chat starten: Teammitglied und Profil wählen oder einfach losschreiben.
- **Chats `/chats`** — alle Konversationen.
- **Apps `/apps`** — Buchhaltung, Redaktionsplan, Galerie, News, Bescheide, Sicherheitsdatenblätter, Videopräsentationen.
- **E-Mail-Weiterleitung** an `ivana@kimatik.com` bzw. `bernhard@kimatik.com`.
- Credits und Abo unter **Abrechnung** (`/abrechnung`); nachkaufen unter `/credits-aufladen`.

---
