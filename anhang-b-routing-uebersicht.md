---
title: Routing-Übersicht
description: App-Pfade, Direktlinks und die IDs der Teammitglieder.
---

## B. Routing-Übersicht

### B.1 Website (`kimatik.com`)

| Pfad | Inhalt |
| --- | --- |
| `/` | Landingpage |
| `/digitale-mitarbeitende` | Marktplatz (alle 25 Teammitglieder, Filter nach Bereich) |
| `/digitale-mitarbeitende/sven`, `/digitale-mitarbeitende/ivana` | Eigene Landingpages |
| `/einschulen` | Team-Builder („Stelle dein Team in wenigen Minuten zusammen“) |
| `/loesungen/<art>/<slug>` | Lösungen: Admin & Buchhaltung, Marketing & Sales, Produktmanagement, Ingenieurbüros |
| `/preise` | Abo, Pakete, Credit-Rechner, „Was ist ein Credit?“ |
| `/funktionen`, `/zusammenarbeit`, `/vergleich` | Produkt |
| `/glossar`, `/faq` | Wissen |
| `/sicherheit-datenschutz` | Sicherheit & Datenschutz |
| `/ueber-uns`, `/vortraege`, `/kontakt` | Unternehmen (Kontakt mit `?dma=<slug>` für Anfragen) |
| `/agb`, `/avv`, `/datenschutz`, `/impressum` | Rechtliches |

Einstieg in die App: `app.kimatik.com/registrieren?dma=<ID>` (optional mit `&price=<Paket>`).

### B.2 App (`app.kimatik.com`) — öffentlich

| Pfad | Inhalt |
| --- | --- |
| `/login` | Anmeldung |
| `/registrieren?dma=<ID>` bzw. `?checkout=…` | Registrierung (ohne Parameter → `/digitales-team`) |
| `/email-sent` | Bestätigungscode eingeben |
| `/passwort-vergessen`, `/passwort-zuruecksetzen` | Passwort zurücksetzen |
| `/feedback` | Dankeseite für Bewertungen |
| `/agb`, `/impressum` | → Website |
| `/datenschutz` | → `kimatik.com/avv` |
| `/preise`, `/ueber-uns`, `/vortraege`, `/kontakt` | → Website |
| `/digitale-mitarbeitende`, `/rekrutieren` | → `/registrieren` |
| `/digitale-mitarbeitende/<slug>` | → Profil auf der Website |
| `/digitale-mitarbeitende/<slug>/testen` | → `/registrieren?dma=<slug>` |

### B.3 App — nach Login

| Pfad | Inhalt | Abo nötig |
| --- | --- | --- |
| `/` | Neuer Chat (Startseite) | ja |
| `/chats`, `/chats/<ID>` | Chats | ja |
| `/apps` | Apps-Übersicht | ja |
| `/apps/<Enrollment-ID>` | App eines Teammitglieds | ja |
| `/apps/gate/<App>` | App-Vorschau & Einschulen | ja |
| `/digitales-team` | Mein Team | nein |
| `/digitales-team/<Enrollment-ID>` | Teammitglied: Profile, Einschulung, Vorgaben | nein |
| `/onboarding/<Enrollment-ID>` | Einschulungs-Chat | nein |
| `/abrechnung` | Abo & Credits | nein |
| `/credits-aufladen` | Top-Up | ja (sonst → `/checkout`) |
| `/einstellungen` | Einstellungen (`?tab=profile/company/verbindungen/security/danger`) | nein |
| `/benachrichtigungen` | Platzhalter | nein |
| `/checkout`, `/checkout-erfolg` | Abo-Abschluss | nein |

### B.4 Direktlinks & IDs

Registrierungslink: `app.kimatik.com/registrieren?dma=<ID>`. Er funktioniert nur für „Sofort verfügbar“. 

| Teammitglied | Status | ID | Herkunft |
| --- | --- | --- | --- |
| Alina Allrounder | Sofort verfügbar | `94eddb80-af59-4121-bc73-9d32c0fa42f0` | Plattform |
| Ivana Invoice | Sofort verfügbar | `605c6703-5acd-460c-8606-555ee3de8969` | Plattform |
| Penelope Photo | Sofort verfügbar | `d1d24a39-11bb-4c22-a7b3-3d538a40c1f5` | Plattform |
| Sven Social Media | Sofort verfügbar | `62f806e3-c4d0-4db5-b613-2fee7756571d` | Plattform |
| Stefan Sicherheitsdatenblatt | Sofort verfügbar | `e6cb7d95-d1db-4313-9df6-19ae5fae0184` | Plattform |
| Bernhard Bescheide | Sofort verfügbar | `60f07462-a8f5-41fa-888f-acad3ae96a88` | Plattform |
| Nina News | Auf Anfrage | `8f6d4262-35d5-4d3a-818f-56bbe504e0d8` | Plattform |
| Theo Texter | Auf Anfrage | `5435ddf2-f009-4d0b-9990-2d1d0a42f078` | Plattform |
| Viola Videopräsi | Auf Anfrage | `dc121e1f-7b3e-45e7-bd39-2ec7f10ea265` | Plattform |
| Paula Podcast | Auf Anfrage | `6108fe8a-73af-4f6b-b6cf-7fe020020b94` | Plattform |
| Emil Email | Auf Anfrage | `4a909dc3-f9a0-4ca7-b5c2-06965c1b6ed5` | Plattform |
| Sandra Sales | Auf Anfrage | `76dcef1c-8d06-4b48-a733-32cbd8ea52f5` | Website |

Ohne öffentliche Registrierungs-ID (Auf Anfrage): Tim Textprüfer, Anja Analyse, Mira Marktforschung, Petra Produktmanagerin, Pria Produktmarketerin, Orla Ops, Berta Baubegehung, Bruno Baubericht, Mara Mängel, Anton Angebot, Arne Ausschreibungsprüfer, Lena Leistungsverzeichnis, Tanja Technik.

---
