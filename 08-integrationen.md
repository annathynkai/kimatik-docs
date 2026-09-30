---
title: Integrationen
description: E-Mail-Eingang, Verbindungen, KI-Modelle, Stripe und was nicht angebunden ist.
---

## 8. Integrationen

### 8.1 E-Mail-Eingang

| Teammitglied | Adresse |
| --- | --- |
| Ivana Invoice | `ivana@kimatik.com` |
| Bernhard Bescheide | `bernhard@kimatik.com` |
| Stefan Sicherheitsdatenblatt | `stefan@kimatik.com` |

- Nur Absender auf der Liste **Autorisierte Absender** werden verarbeitet („Nur E-Mails von diesen Adressen werden verarbeitet. Andere Absender erhalten eine automatische Ablehnungs-E-Mail.“).
- Die E-Mail-Adresse des eigenen Kontos ist automatisch freigegeben.
- Die Liste wird in der Einschulung angelegt und auf der Detailseite des Teammitglieds (Standard-Profil) gepflegt.
- Die Dokumente kommen als **Anhang**; sie erscheinen danach in der jeweiligen App.
- Die früheren Adressen `…@thynkai.at` werden weiterhin angenommen.

### 8.2 Verbindungen

Unter **Einstellungen → Verbindungen** lassen sich die folgenden Dienste verbinden:

- **Outlook:** „Mails lesen, Entwürfe senden und den Kalender für Emil.“
- **ClickUp:** „Aufgaben suchen und nach deiner Bestätigung anlegen.“

Der Status wird als **Verbunden**, **Erneut verbinden nötig** oder **Nicht verbunden** angezeigt; mit **Trennen** hebst du eine Verbindung auf. Angemeldet wird im Anmeldefenster des jeweiligen Dienstes; kimatik sieht dein Passwort nicht. 

### 8.5 KI-Modelle & automatische Auswahl

- kimatik wählt die KI-Modelle passend zur Aufgabe. Eine Modellauswahl gibt es für Kund:innen nicht; einzige Stellschraube ist der Modus **Expertin** bei Alina.
- Eingesetzt werden laut Website Modelle der großen Anbieter, derzeit Google Gemini und Anthropic Claude, jeweils auf EU-Servern:
  - Gemini über Google Vertex AI in der EU.
  - Claude über OpenRouter mit Routing innerhalb der EU (AWS Bedrock bzw. Google Vertex AI).
- Wird ein Modell abgekündigt, stellt kimatik automatisch um.

### 8.6 Zahlungen (Stripe)

Abos, Top-Ups, Rechnungen und Zahlungsmethoden laufen über Stripe (Checkout und Kundenportal).

### 8.7 E-Mail-Kommunikation (Loops)

Systemmails und Produkt-/Marketing-Mails (z. B. Produkt-Updates) werden über Loops verschickt. Eine Abmeldung ist über den Link in jeder E-Mail möglich. In der App gibt es dafür keine Einstellungen.

### 8.8 Nicht vorhanden

- **Microsoft Teams:** keine Anbindung. Kopierte Antworten sind aber so formatiert, dass sie sich in Teams und Outlook sauber einfügen lassen.
- **Export-Profile für Buchhaltungsprogramme** (z. B. BMD, DATEV): keine. Verfügbar sind CSV, Excel, JSON und die Originaldateien.
- **Login über Drittanbieter** (Google, Microsoft …): nicht vorhanden.
