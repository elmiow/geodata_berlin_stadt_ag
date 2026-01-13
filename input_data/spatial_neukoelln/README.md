# Berlin Geodaten - Neukölln

Dieser Ordner enthält GeoJSON-Dateien, die auf den Bezirk **Neukölln** zugeschnitten sind.

## Warum Neukölln?

Die originalen Datensätze für ganz Berlin sind teilweise sehr groß (bis zu 48 MB). Für die Verwendung in **uMap** (https://umap.openstreetmap.fr/) sind Dateien unter 5 MB optimal.

Alle Dateien in diesem Ordner wurden auf die Neukölln Bounding Box zugeschnitten:
- **Longitude**: 13.40° - 13.50° Ost
- **Latitude**: 52.45° - 52.50° Nord

## Verfügbare Datensätze (20 Dateien)

| Datei | Größe | Features | Beschreibung |
|-------|-------|----------|--------------|
| `ua_einwohnerdichte_2024_neukoelln.geojson` | 1.23 MB | 1,245 | Einwohnerdichte 2024 |
| `ua_einwohnerdichte_2024_entw_neukoelln.geojson` | 1.11 MB | 1,245 | Einwohnerdichte Entwicklung |
| `denkmale_neukoelln.geojson` | 1.96 MB | 560 | Denkmalgeschützte Gebäude |
| `gruenanlagen_neukoelln.geojson` | 0.97 MB | 161 | Grün- und Erholungsanlagen |
| `a_gruenvol2020_neukoelln.geojson` | 1.97 MB | 1,680 | Grünvolumen 2020 |
| `b_gruenvol2020_veraend_neukoelln.geojson` | 1.99 MB | 1,680 | Grünvolumen Veränderung |
| `versorggruen_2020_neukoelln.geojson` | 0.49 MB | 623 | Versorgung mit öffentlichem Grün |
| `c_buslinien_neukoelln.geojson` | 1.29 MB | 195 | Buslinien |
| `radverkehrsnetz_neukoelln.geojson` | 0.30 MB | 807 | Radverkehrsnetz |
| `parkplaetze_neukoelln.geojson` | 5.78 MB | 5,676 | Parkplätze (⚠️ etwas groß) |
| `parkplaetze_aussen_neukoelln.geojson` | 0.28 MB | 357 | Parkplätze Außenbereich |
| `a_rwvers_strassen_neukoelln.geojson` | 0.77 MB | 1,844 | Regenwasserversickerung |
| `ua_luftbelastung_verkehr_2020_2025_neukoelln.geojson` | 0.41 MB | 802 | Luftbelastung durch Verkehr |
| `mss2023_indizes_542_neukoelln.geojson` | 0.50 MB | 60 | MSS 2023 Indizes |
| `mss2023_indexind_542_neukoelln.geojson` | 0.52 MB | 60 | MSS 2023 Index-Indikatoren |
| `mss2023_kontextind_542_neukoelln.geojson` | 0.55 MB | 60 | MSS 2023 Kontext-Indikatoren |
| `gewalt_gesamt_neukoelln.geojson` | 0.50 MB | 60 | Gewaltdelinquenz Gesamt |
| `gewalt_jugend_neukoelln.geojson` | 0.50 MB | 60 | Gewaltdelinquenz Jugend |
| `gewalt_partner_neukoelln.geojson` | 0.50 MB | 60 | Gewaltdelinquenz Partnergewalt |
| `ab_wohngebaeude2022_neukoelln.geojson` | 0.02 MB | 26 | Wohngebäude Lärmkartierung 2022 |

## Import in uMap

### Option 1: Direkt von GitHub (empfohlen)

Verwende die Raw-URLs für direkten Import:

```
https://raw.githubusercontent.com/elmiow/geodata_berlin_stadt_ag/main/input_data/spatial_neukoelln/DATEINAME.geojson
```

Beispiel für Einwohnerdichte:
```
https://raw.githubusercontent.com/elmiow/geodata_berlin_stadt_ag/main/input_data/spatial_neukoelln/ua_einwohnerdichte_2024_neukoelln.geojson
```

**Anleitung:**
1. Öffne [uMap](https://umap.openstreetmap.fr/)
2. Erstelle eine neue Karte oder öffne eine existierende
3. Klicke auf "Import data" (Pfeil-Symbol)
4. Wähle "Remote data URL"
5. Füge die URL ein
6. Format: "geojson" auswählen
7. Klicke "Import"

### Option 2: Lokaler Upload

1. Lade die Dateien von GitHub herunter
2. Öffne uMap
3. Klicke "Import data"
4. Wähle "Choose file"
5. Wähle die GeoJSON-Datei

## Koordinatensystem

Alle Dateien verwenden **EPSG:4326 (WGS84)** - das Standard-Koordinatensystem für Web-Mapping.

## Datenquellen

Alle Daten stammen vom Berliner Geodatenportal:
- https://gdi.berlin.de

Heruntergeladen über WFS (Web Feature Service) Schnittstellen.

## Andere Bezirke

Für andere Berliner Bezirke können die gleichen Datensätze mit anderen Bounding Boxes zugeschnitten werden. Siehe das Script `clip_to_neukoelln.py` im Hauptverzeichnis.

## Lizenz

Die Geodaten unterliegen den Nutzungsbedingungen des Berliner Geodatenportals. Bitte beachte die jeweiligen Lizenzen der Originaldatensätze.

---

**Erstellt**: 2026-01-13
**Bounding Box**: [13.40, 52.45, 13.50, 52.50]
**Anzahl Datensätze**: 20 von 50 Gesamt-Berlin Layern
