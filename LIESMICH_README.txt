# Atreia Codex — AION Datenbank

Eine durchsuchbare Datenbank (Waffen, Rüstung, Fertigkeiten) aus den AION-Clientdaten,
mit DE/EN-Umschalter, Klassen-/Typ-/Qualitäts-/Stufen-Filter und Detailansicht.

Inhalt:
  atreia_codex.html   – die Seite (einfach im Browser öffnen)
  data/               – die generierten JSON-Daten (Waffen, Rüstung, Skills, Meta)
  icons/              – die referenzierten Item-/Skill-Icons (PNG)

## Starten (wichtig!)

Moderne Browser blockieren das Laden lokaler JSON-Dateien per Doppelklick (file://).
Starte deshalb einen winzigen lokalen Server IM ORDNER dieser Datei:

    python3 -m http.server 8000

und öffne dann im Browser:

    http://localhost:8000/atreia_codex.html

Der Ordner `data/` und der Ordner `icons/` müssen immer NEBEN der HTML-Datei liegen.

---

# Atreia Codex — AION Database (English)

A searchable database (weapons, armor, skills) built from the AION client data,
with a DE/EN toggle, class/type/quality/level filters and a detail view.

## Run it

Browsers block loading local JSON via double-click (file://). Start a tiny local
server in this folder instead:

    python3 -m http.server 8000

then open:

    http://localhost:8000/atreia_codex.html

Keep the `data/` and `icons/` folders next to the HTML file.

---

Datenstand / counts:
  Waffen / Weapons: 18.389
  Rüstung / Armor:  39.043
  Fertigkeiten / Skills: 10.963

Hinweise:
  - "Alle Klassen" bei einem Eintrag = laut Itemdaten von allen 11 Klassen nutzbar.
  - Waffen sind nach echter Waffen-Proficiency den Klassen zugeordnet
    (z. B. Kugel/Zauberbuch → Zauberer & Beschwörer; Stab → Kantor & Kleriker).
  - Rüstung ist nach Archetyp zugeordnet (Leder, Kette, Stoff/Robe, Platte).
  - Einträge mit "(intern)" haben keinen lokalisierten Namen (NPC-/Test-Items).
