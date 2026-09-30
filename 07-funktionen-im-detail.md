## 7. Funktionen im Detail

### 7.1 Navigation & Aufbau der App

**Desktop (ab 1024 px Breite) — Seitenleiste:**
- Logo (→ Startseite)
- **Neu** → neuer Chat (`/`)
- **Chats** (mit Zähler ungelesener Chats) → `/chats`
- **Team** → `/digitales-team`
- **Apps** → `/apps`
- **Suchen** (Tastenkürzel ⌘K / Strg+K)
- Avatar-Menü: **Abrechnung**, **Einstellungen**, **Abmelden**

**Mobil / Tablet (unter 1024 px):**
- Untere Leiste mit **Chats**, **Team**, **Apps**, **Suchen** (nur Icons) plus runder Button **Neuer Chat**.
- Konto-Menü rechts oben auf der Startseite.
- In einem geöffneten Chat ist die untere Leiste ausgeblendet; oben gibt es Zurück und **Neuer Chat**.
- Die Suche öffnet sich als Blatt von unten.
- Die Auswahl von Teammitglied und Profil läuft in zwei Schritten.

**Suche („Suche oder navigiere...“):** durchsucht Chats, Teammitglieder und Apps (je max. 5 Treffer, insgesamt max. 8). Ohne Suchbegriff zeigt sie **Zuletzt aufgerufen**. Eine eigene Suche nur in der Chat-Liste gibt es nicht.

**Tab-Titel:** Bei ungelesenen Antworten steht die Anzahl vor dem Seitentitel, z. B. „(1) …“.

### 7.2 Chat

#### Neuer Chat (Startseite `/`)
- Überschrift „Lege mit deinem digitalen Team los“, darunter „Willkommen zurück, {Vorname}. Wähle Teammitglied und Profil — oder schreib einfach los.“
- Eingabefeld mit Auswahl **Teammitglied wählen** / **Profil wählen** sowie **Teammitglied hinzufügen** und **Profil hinzufügen**.
- Dateien lassen sich per Drag & Drop anhängen.
- Bei Alina gibt es zusätzlich den Schalter **Expertin**.
- Ohne Team: „Noch kein digitales Team“ → **Digitales Team**.
- Jeder Chat gehört zu **einem Teammitglied und einem Profil**.

#### Chats (`/chats`)
- Liste links, Chat rechts (mobil gestapelt).
- Leerzustand: „Wähle einen Chat aus der Liste oder starte einen neuen.“
- Titel werden automatisch vergeben (anfangs „Neuer Chat“).
- Aktionen: **Umbenennen** und **Löschen** (Rückfrage „Chat löschen?“).
- Ungelesen-Punkte an den Avataren; ein drehender Ring zeigt, dass gerade gearbeitet wird.

#### Im Chat
- **Begrüßung:** individuelle Willkommensnachricht pro Teammitglied.
- **Datei-Upload:**
  - Max. **10 Dateien pro Nachricht**, je max. **20 MB**.
  - Alle Dateitypen erlaubt; der Server prüft, was verarbeitet werden kann.
  - Bilder werden vor dem Upload auf max. 1920 × 1920 px verkleinert.
- **Nachrichtenlänge:** max. 32.000 Zeichen.
- **Arbeitsstatus:** Statuszeilen in Ich-Form, z. B. „Ich schau kurz online nach…“.
- **Nachvollziehbarkeit:** Unter **So bin ich vorgegangen** stehen die einzelnen Schritte mit Quellen. Gescheiterte Schritte erscheinen als „Ich passe den Ansatz an…“.
- **Stoppen:** Eine laufende Antwort lässt sich abbrechen.
- **Eingabe-Sperre:** Während Hintergrundaufgaben laufen, ist das Eingabefeld gesperrt.
- **Status-Pill im Kopf:** **{n} Credits übrig**, sobald die inkludierten Credits fast aufgebraucht sind.
- **Kopieren:** Antworten werden formatiert kopiert, passend zum Einfügen in Outlook oder Teams („In Zwischenablage kopiert“).
- **Bilder:** Bildansicht mit Vor/Zurück, Download und Schalter **KI-Kennzeichnung** (Kapitel 7.4).
- **Weitergabe an Kolleg:innen:** Karte „Anfrage an {Name} weitergeben“ (Kapitel 2.3).
- **Verbindungs-Hinweis:** „{Dienst} ist noch nicht verbunden.“ bzw. „Der Zugriff auf {Dienst} ist abgelaufen.“ mit **Verbinden** / **Erneut verbinden**.
- **Nicht vorhanden:** Daumen-Bewertung pro Nachricht, Credit-Anzeige pro Nachricht, Gruppenchat mit mehreren Teammitgliedern.

#### Modus „Expertin“ (nur Alina)
Schalter im Eingabefeld. Banner: „Expertin: Höchste logische Präzision und tiefere Analysen für komplexe Aufgaben (~3x Credits)“. Im Hintergrund arbeitet ein leistungsstärkeres, vorkonfiguriertes Modell. Ein Modell kann man nicht selbst auswählen.

### 7.3 Apps

Apps sind spezialisierte Oberflächen für strukturierte Daten.
- **Übersicht:** `/apps`.
- **App eines Teammitglieds:** `/apps/<Enrollment-ID>`.
- Alle Apps setzen ein aktives Abo voraus.

**App noch nicht freigeschaltet:**
- Mittels Klick auf eine App erscheint der Dialog **„So bekommst du diese App“** mit den passenden Teammitgliedern und dem Button **Einschulen** (sofort verfügbar) oder **Anfragen** / **Angefragt** (auf Anfrage).

| App | Teammitglied(er) | Kurzbeschreibung |
| --- | --- | --- |
| **Buchhaltung** | Ivana | Rechnungen & Belege verwalten und prüfen |
| **Redaktionsplan** | Sven, Theo | Plane & erstelle Social-Media-Posts |
| **Galerie** | Penelope (Viola liefert zu) | Medien zentral speichern und wiederverwenden |
| **News** | Nina | Relevante Branchennews im Blick behalten |
| **Bescheide** | Bernhard | Bescheide erfassen und verwalten |
| **Sicherheitsdatenblätter** | Stefan | Sicherheitsdatenblätter erfassen und verwalten |
| **Videopräsentationen** | Viola | Präsentationen in Videos umwandeln |

#### 7.3.1 Gemeinsame Tabellenfunktionen (Buchhaltung → Rechnungen, Bescheide, Sicherheitsdatenblätter)

- **Upload:**
  - Über **Hochladen**, per Drag & Drop oder **Per E-Mail senden**.
  - Formate: PDF, JPEG, PNG, WebP.
  - Max. 20 MB pro Datei, bei Bescheiden 40 MB.
  - Hinweis im Leerzustand: „Oder per E-Mail weiterleiten an …“ mit der Adresse des Teammitglieds.
- **Suche, Filter, Sortierung:** Freitextsuche, Filter pro Spalte, Datums- und Betragsbereiche, Sortierung.
  - Filter, Suche und Sortierung bleiben erhalten, solange du in der App bleibst, und werden beim Verlassen zurückgesetzt.
  - **Alle Filter entfernen** setzt alles auf einmal zurück.
  - Ergibt die Filterung keine Treffer, erscheint ein zentrierter Hinweis mit Link zum Entfernen aller Filter.
- **Spalten ein-/ausblenden:** Über **Spalten**. Das Menü bleibt offen, bis du daneben klickst.
  - Die Auswahl wird pro Teammitglied im Browser gespeichert und beim nächsten Aufruf wieder geladen.
- **Hinweise-Spalte:** z. B. **Mögliches Duplikat**, unsichere Werte (z. B. „Betrag unklar“, „Handschrift erkannt“), **USt-Prüfung**, **Konto prüfen**, bei SDB **LGK-Prüfung**, bei Bescheiden z. B. unklares Aktenzeichen oder unvollständige Auflagen; Dokumente, die nicht passen (keine Rechnung / kein SDB / kein Bescheid).
- **Seitengröße:** 20 Einträge pro Seite.
- **Mehrfachauswahl:** mehrere Einträge auswählen und gemeinsam **Löschen**.
- **Export:**
  - **Als CSV exportieren** (Semikolon, Excel-kompatibel).
  - **Als Excel exportieren**.
  - **Als JSON exportieren**.
  - **Original-Datei herunterladen** bzw. **Original-Dateien als ZIP**.
  - Vor dem Export wählst du die Spalten aus (**Spalten für Export auswählen**).
  - Export-Profile für bestimmte Buchhaltungsprogramme gibt es nicht.

#### 7.3.2 Buchhaltung (Ivana)

Tabs: **Rechnungen** | **Buchungen** | **E/A-Rechnung** | **UVA**

**Rechnungen**
- **Spalten:** Status, Fälligkeit, Rechnungsnummer, Lieferant, Datum, Netto, Brutto, Art (Eingangs-/Ausgangsrechnung), Konto, Hinweise.
- **Status:** **Entwurf** → nach Freigabe **Offen** → durch Bankzuordnung **Teilbezahlt** / **Bezahlt**. Überfällige Ausgangsrechnungen werden als **Fällig** angezeigt.
- **Prüfung:** Der Banner „{n} Belege warten auf deine Prüfung“ führt über **Jetzt prüfen** zum Dialog **Beleg prüfen**. Er zeigt das Original neben dem Formular:
  - Lieferant bzw. Empfänger mit Adresse und USt-IdNr.
  - **Rechnungsdetails:** Art, Rechnungs-Nr., Datum, Fällig, Leistungszeitraum.
  - **Beträge:**
    - Währung (alle ISO-Währungen, Standard EUR; bei Fremdwährung mit Wechselkurs).
    - Ansicht Netto/Brutto, Steuerzeilen mit Netto, USt. %, USt. und Brutto.
    - **Zeile hinzufügen**, Kategorie pro Zeile, USt.-Befreiung.
  - **Kategorie** (Konto) und **Notizen**.
  - Buttons **Speichern & freigeben** oder **Als Entwurf speichern**.
  - Mögliche Duplikate lassen sich mit **Trotzdem behalten** bestätigen.
- In der Detailansicht werden erkannte **Positionen** angezeigt.
- **E-Mail-Eingang:** Dialog „Rechnungen per E-Mail einsenden“: Absender freigeben → Rechnung als Anhang an `ivana@kimatik.com` senden → Ivana legt sie ab. Nicht freigegebene Absender erhalten eine automatische Ablehnungs-E-Mail.

**Buchungen (Bank)**
- **Bankkonten:** **Konto anlegen** mit Name, IBAN (optional) und Eröffnungskontostand (optional). Letzterer wird zu importierten Buchungen addiert, wenn die CSV keinen Kontostand enthält. Konten lassen sich bearbeiten und löschen; das Löschen ist gesperrt, solange Buchungen mit Belegen verknüpft sind.
- **CSV importieren:**
  - Spalten zuordnen: **Buchungsdatum\***, **Brutto-Betrag\***, Empfänger/Sender, Verwendungszweck, Zahlungsreferenz, Kontostand (nach Buchung).
  - Dezimaltrennzeichen (Komma/Punkt) und Datumsformat (TT.MM.JJJJ, JJJJ-MM-TT, TT/MM/JJJJ) wählen.
  - Überschneidet sich der Zeitraum mit einem früheren Import, erscheint eine Warnung zu möglichen Duplikaten mit **Trotzdem hochladen**.
- **Importhistorie:** Titel „Importhistorie — {Konto}“. Jeder frühere Import lässt sich als **CSV herunterladen** (die Originaldatei bzw. eine aus den Buchungen neu erzeugte Datei).
  - Gelöschte Importe bleiben mit dem Vermerk „gelöscht“ sichtbar.
  - Löschen ist gesperrt, solange Buchungen verknüpft sind.
- **Tabelle:** Status, Empfänger / Sender, Buchungstag, Brutto, Offen, Belege. Status: **Offen**, **Aut. gebucht**, **Gebucht**, **Teilgebucht**, **Privat**. Mit dem Schalter **Privat** markierst du Privatbuchungen.
- **Automatisch zuordnen:** gleicht Buchungen und Belege automatisch ab.
- **Beleg zuordnen** (manuell): Belegsuche in Eingangs- und Ausgangsrechnungen, Markierung „Betrag passt“. Bei Differenzen wählst du einen **Differenzgrund**:
  - Belege höher: **Skonto**, **Teilzahlung**, **Sonstige**.
  - Transaktion höher: **Teil einer Sammelbuchung**, **Kosten des Zahlungsverkehrs (steuerfrei)**, **Mahngebühren**.

**E/A-Rechnung**
- Zeitraum standardmäßig 1. Jänner bis heute, Start- und Enddatum sind wählbar. Die Berechnungsart steht auf **E/A-Rechnung**.
- **Gewinn** steht oben rechts.
- **Betriebseinnahmen:** Konten unter **Umsatzsteuerpflichtige Betriebseinnahmen** und **Nicht umsatzsteuerbare Betriebseinnahmen**, darunter **Umsatz**, **Vereinnahmte Umsatzsteuer** und **Summe Betriebseinnahmen**.
- **Betriebsausgaben:** die einzelnen Aufwandskonten, darunter **Gezahlte Vorsteuer** und **Summe Betriebsausgaben**. Die Auswertung gruppiert die Ausgaben nicht nach Kostenart.
- Konten ohne Zuordnung erscheinen als Hinweis **Nicht zugeordnet**, wenn Belege daran hängen.
- Per Klick auf eine berechnete Zeile siehst du die zugehörigen Belege.
- Die Zuordnung zu Blöcken wie Direkte Kosten, Indirekte Kosten und Abschreibungen liegt in den Einstellungen des Standard-Profils (**Kontenzuordnung**), nicht als eigene Summenzeilen in der Auswertung.

**UVA**
- **Zeitraum:** Monatlich / Quartalsweise / Jährlich, dazu das **Jahr** (aktuelles Jahr und die 4 Jahre davor).
- **Besteuerung:** **Soll** oder **Ist**.
- Tabs für Monate bzw. Quartale.
- Ergebnis: **Zahllast** mit den Seiten Umsatzsteuer und Vorsteuer, gruppiert nach Steuersatz bzw. „Steuerbefreit“. Details lassen sich ein- und ausblenden.

**Einstellungen pro Profil (Standard-Profil):** Autorisierte Absender, USt.-Befreiungen und Kontenzuordnung für die E/A-Rechnung.

#### 7.3.3 Sicherheitsdatenblätter (Stefan)

- **Spalten:** Name, Firmenname, Verwendungszweck, H-Sätze, GHS-Symbole, Flammpunkt [°C], UN-Nummer, VBF 2023, LGK, Inhaltsstoffe, pH-Wert, Wassergefährdungsklasse, Datum.
- GHS-Symbole und Lagerklasse (TRGS 510) werden regelbasiert berechnet, nicht von der KI geschätzt.
- Prüfen und Bearbeiten im Detaildialog.

#### 7.3.4 Bescheide (Bernhard)

- **Spalten:** Status, Geschäftszeichen, Behörde, Datum, Auflagen (Anzahl).
- **Formular:**
  - **Bescheid-Informationen:** Behörde, Geschäftszeichen, Datum.
  - **Auflagen:** Nr., Kategorie, Text.
- Upload bis 40 MB.

#### 7.3.5 Galerie / Mediengalerie (Penelope, Viola)

- **Inhalt:** Raster mit Bildern und Videos (24 pro Seite). Transparente Bilder werden auf Schachbrett-Hintergrund angezeigt.
- **Suche und Filter:** Suche und Datumsfilter bleiben innerhalb der App erhalten; **Alle Filter entfernen**.
- **Aktionen:** Umbenennen, Löschen („Bild löschen?“ / „Video löschen?“), **Zum Chat springen** (zum Chat, in dem das Bild entstanden ist).
- **Download** mit dem originalen Dateinamen und Format.
- **KI-Kennzeichnung:** siehe 7.4.

#### 7.3.6 Redaktionsplan (Sven, Theo)

- **Spalten:** Status, Titel, Plattform, ggf. Teammitglied, Geplant für, Bilder.
- **Status:** **Entwurf**, **Geplant**, **Veröffentlicht**. Die Freigabe erfolgt über den Statuswechsel.
- **Plattformen:** LinkedIn, Instagram, Facebook, X, Blog, Newsletter, E-Mail, Website-Text, Pressetext, Andere. Angezeigt werden die Plattformen, die für das Teammitglied freigeschaltet sind.
- **Editor** (**Neuer Post** / **Post bearbeiten**): Text, Hashtags, Terminkalender.
- **Bilder:** bis zu **10 Bilder** pro Post (JPEG/PNG/WebP, je max. 10 MB), Anzeige „Bilder (n/10)“.

#### 7.3.7 News (Nina)

- **Ansichten:** **Nach Thema** oder **Nach Aktualität**, Filter **Alle Themen** bzw. einzelne Content-Pillars, Suche.
- **Karte:** Quelle, Datum, Titel mit Link und Kurzfassung.
- **Details:** **Das Wichtigste**, **Zusammenfassung** und Bewertungen (0–5 Sterne) für Aktualität, Informationsgehalt, Attraktivität und Tonalität.
- **Löschen** mit Rückfrage „Artikel löschen?“.

#### 7.3.8 Videopräsentationen (Viola)

Workflow in drei Schritten, **ohne Chat**:
1. **Import:**
   - Präsentation als **PDF oder PPTX** hochladen (max. 50 MB, max. 50 Folien).
   - Alternativ einzelne Bilder (JPG/PNG, je max. 10 MB).
2. **Editor:**
   - Folien per Drag & Drop sortieren und Sprechernotizen bearbeiten.
   - **Alle Notizen optimieren** (KI).
   - Vertonung pro Folie (Status „In Warteschlange“ / „Wird vertont…“), Audio-Vorschau.
   - Die Stimme wird im Profil festgelegt (Feld für die Stimme; leer = Standardstimme).
3. **Ergebnis:** MP4-Video zum Download (`viola-video.mp4`), optional in der Galerie ablegen. Die App zeigt die abgerechneten Credits an.

### 7.4 KI-Kennzeichnung (EU AI Act)

- Schalter **KI-Kennzeichnung** in der Bildansicht der **Galerie** und bei **Bildern im Chat**, direkt neben dem Download. 
- **Standard: aus.** Beim Einschalten erzeugt kimatik eine gekennzeichnete Kopie des Bildes mit sichtbarer KI-Markierung und speichert sie. Anzeige und Download zeigen dann diese Version.
- Das **Original bleibt unverändert**. Beim Ausschalten wird die Kennzeichnung entfernt.
- Die Einstellung gilt pro Bild. Einen globalen Schalter in den Einstellungen gibt es nicht.
- Schlägt die Kennzeichnung fehl, erscheint „Kennzeichnung fehlgeschlagen“.

### 7.5 Digitales Team

**Übersicht (`/digitales-team`):**
- Karten der eigenen Teammitglieder mit Anzahl der Chats und Apps.
- Abschnitt **Verfügbare Teammitglieder** mit **Jetzt einschulen**, **Mehr erfahren**, **Anfragen** / **Angefragt**, **Bald verfügbar** und **Im Abo enthalten**.

**Detailseite (`/digitales-team/<Enrollment-ID>`):**
- **Kopf:** Name, Rolle, Beschreibung und, wenn das Teammitglied einen Chat hat, **Neuer Chat**. Anzahl der Chats und Buttons zu den Apps.
- **Profile** als Tabs, dazu **Profil hinzufügen**.
- Pro Profil:
  - **Profilname**, **Profilfarbe**, **Standard-Profil** / **Als Standard setzen**.
  - **Einschulung** mit **Einschulung neu starten** (nur für dieses Profil).
  - **Vorgaben anpassen** bzw. **Vorgaben aus Einschulung anpassen**: die Einstellungen aus der Einschulung, z. B. Tonalität, Zielgruppe, Bildstil, Stimme.
- Im Standard-Profil von Teammitgliedern mit E-Mail-Eingang: **Autorisierte Absender**. Bei Ivana zusätzlich USt.-Befreiungen und Kontenzuordnung.
- `/teammitglied-anpassen/<ID>` leitet auf diese Seite weiter.

### 7.6 Weitere Seiten

| Pfad | Inhalt |
| --- | --- |
| `/abrechnung` | Abo, Credits, Stripe-Kundenportal (Kapitel 5.7) |
| `/credits-aufladen` | Top-Up (nur mit Abo) |
| `/einstellungen` | Profil, Verbindungen, Sicherheit, Gefahrenzone |
| `/benachrichtigungen` | Platzhalter „In Kürze verfügbar“ |
| `/onboarding/<ID>` | Einschulungs-Chat |
| `/feedback?score=1–5` | Öffentliche Dankeseite für Bewertungen aus E-Mails („Danke für dein Feedback!“) |

Frühere Seiten **Übersicht** (`/uebersicht`) und **Berichte** (`/berichte`) gibt es nicht mehr; beide leiten auf die Startseite weiter.

---
