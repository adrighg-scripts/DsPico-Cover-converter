# 🎨 DsPico Cover Converter

Ein effizientes Web-Tool zur Konvertierung von Spiel-Covern in das für **DsPico** erforderliche 8-Bit-BMP-Format. Unterstützt automatisches Suchen, Zuordnen und organisierte Speicherung auf SD-Karten.

## 🚀 Funktionen
- **Zwei Modi:** Einfacher Download oder automatisches Speichern auf SD-Karten.
- **Header-Analyse:** Automatische Erkennung der GameID für `.nds` und `.gba` ROMs.
- **Smart Sorting:** Automatisches Sortieren in Unterordner (`gba/`, `nds/`, `user/`).
- **Optimierte Konvertierung:** Korrektes 8-Bit-BMP-Mapping (128x96) mit sauberer Farbdarstellung.
- **Browser-basiert:** Keine Installation erforderlich, läuft direkt im Browser.

## 🛠 Verwendung

### Option 1: Simple Download
Ideal, wenn du nur schnell ein einzelnes oder wenige Cover konvertieren möchtest.
1. Bilder hochladen.
2. "Simple Download" wählen.
3. Cover als ZIP oder einzeln herunterladen.

### Option 2: Pro SD-Card Save
Ideal für die Verwaltung deiner gesamten Spiele-Bibliothek auf der SD-Karte.
1. Bilder hochladen.
2. "Pro SD-Card Save" wählen.
3. Root-Verzeichnis deiner SD-Karte auswählen.
4. Das Tool scannt nach ROMs und lässt dich die Cover direkt zuordnen.
5. "Save & Finish" – das Tool erstellt automatisch die `_pico/covers/`-Struktur.

## 📂 Ordnerstruktur
Das Tool erstellt automatisch folgende Struktur auf deiner SD-Karte:
```text
_pico/
└── covers/
    ├── gba/       # Hier landen GBA-Spiele (benannt nach 4-stelligem GameCode)
    ├── nds/       # Hier landen NDS-Spiele (benannt nach 4-stelligem GameCode)
    └── user/      # Hier landen alle anderen Formate (mit vollem Original-Namen)
