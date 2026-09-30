## 4. Authentifizierung & Konto

### 4.1 Anmeldung

- Seite `/login` („Willkommen zurück“), Felder **E-Mail** und **Passwort**, Button **Anmelden**, Link **Passwort vergessen?**.
- Anmeldung ausschließlich mit **E-Mail und Passwort**. Login über Google, Apple, Microsoft o. ä. gibt es nicht.
- Kein Einmalcode bei normalem Login oder neuem Gerät.

### 4.2 Registrierung

- Über `/registrieren?dma=<ID>` (siehe Kapitel 3.2). Button **Konto erstellen**.
- Felder: Vorname, Nachname, „Dein Unternehmen“, E-Mail, „Neues Passwort“ (mindestens **6 Zeichen**), Zustimmung zu AGB und AVV.
- Probe-Credits bei Registrierung gibt es **nicht**.

### 4.3 E-Mail-Bestätigung (Code)

- Nach der Registrierung wird ein **6-stelliger Code** per E-Mail verschickt, gültig **60 Minuten**.
- Eingabe auf `/email-sent` bzw. direkt im Registrierungsschritt („Bestätigungscode eingeben“).
- **Code erneut senden** ist nach **60 Sekunden** möglich.
- Wird die E-Mail in einem anderen Tab/Gerät bestätigt, erkennt die Seite das automatisch.

### 4.4 Passwort vergessen / zurücksetzen

1. `/passwort-vergessen` → E-Mail eingeben.
2. 6-stelligen Code aus der E-Mail eingeben (gültig 60 Minuten, erneut senden nach 60 Sekunden).
3. `/passwort-zuruecksetzen` → neues Passwort (mindestens 6 Zeichen) → danach Anmeldung unter `/login`.

### 4.5 Sitzungen & Abmeldung

- Sitzungen bleiben nach dem Schließen des Browsers aktiv und werden automatisch verlängert.
- **Abmelden**: Desktop über das Avatar-Menü unten in der Seitenleiste; mobil über das Konto-Menü rechts oben auf der Startseite. Das Menü enthält außerdem **Abrechnung** und **Einstellungen**.

### 4.6 Einstellungen (`/einstellungen`)

| Tab | Inhalt |
| --- | --- |
| **Profil** | Firmenname, Vorname, Nachname, Telefon; E-Mail nur lesbar |
| **Verbindungen** | Outlook und ClickUp verbinden/trennen (Kapitel 8.2) |
| **Sicherheit** | Passwort ändern (mindestens **8 Zeichen**) |
| **Gefahrenzone** | **Account löschen** |

Benachrichtigungs-Einstellungen gibt es nicht. Die Seite `/benachrichtigungen` ist ein Platzhalter („Benachrichtigungssystem – In Kürze verfügbar“).

### 4.7 Konto löschen

**Einstellungen → Gefahrenzone → Account löschen**. Zur Bestätigung muss `DELETE` eingetippt werden. Danach wird das Konto gelöscht und du wirst abgemeldet. Ein laufendes Abo sollte vorher unter **Abrechnung → Abo kündigen** beendet werden.

---
