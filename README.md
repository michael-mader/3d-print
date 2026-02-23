# Bambu Lab A1 - Einsteiger Guide & Gemini Gem Wissensbasis

Dieses Repository erfüllt zwei zentrale Aufgaben rund um den Einstieg in den 3D-Druck mit dem Bambu Lab Ökosystem:

1. **Hosting der Webseite:** Bereitstellung eines kompakten "Bambu Lab A1 Einsteiger Guides" via GitHub Pages.
2. **Wissensbasis für KI:** Zentrale und versionierte Speicherung der System-Anweisungen und Fakten für ein benutzerdefiniertes Gemini Gem (ein KI-Assistent für 3D-Druck-Beratung).

## 📂 Repository-Struktur

* `index.html`
Der Quellcode der Hauptwebseite (inkl. CSS und Struktur).
* `.github/workflows/static-pages.yml`
Die GitHub Action, die dafür sorgt, dass jede Änderung an der `index.html` automatisch auf GitHub Pages live geschaltet wird.
* `gem-wissen/anweisungen.md`
Die System-Prompts und Verhaltensregeln (Persona) für das Gemini Gem.
* `gem-wissen/wissensbasis.md`
Die harten Fakten, aktuellen Preise, Hardware-Empfehlungen und Filament-Regeln (Stand 2026), auf die das Gem zugreifen soll.

## 🌐 Webseite bearbeiten & ansehen

Die Webseite wird automatisch über GitHub Pages gehostet.

* URL: `https://<dein-github-name>.github.io/<repo-name>/` *(Hinweis: Trage hier nach dem ersten Deploy deine echte URL ein)*

Um den Guide anzupassen:

1. Bearbeite die Datei `index.html`.
2. Committe und pushe die Änderungen in den `main` Branch.
3. Die GitHub Action übernimmt den Rest – die Webseite ist nach wenigen Sekunden aktualisiert.

## 🤖 Gemini Gem aktualisieren

Die Trennung der Daten hilft dabei, das Wissen der KI immer aktuell zu halten, ohne das Web-Design zu berühren.
Wenn sich Preise ändern, neue Filamente erscheinen oder Bambu Lab neue Drucker auf den Markt bringt:

1. Aktualisiere die entsprechenden Daten in `gem-wissen/wissensbasis.md`.
2. Kopiere den aktualisierten Text.
3. Füge ihn in die Konfiguration deines Gemini Gems (im Bereich "Wissen" bzw. "Knowledge") ein.
4. Die Grundanweisungen in `anweisungen.md` (wie das Gem mit dem Nutzer sprechen soll) bleiben in der Regel unberührt.
