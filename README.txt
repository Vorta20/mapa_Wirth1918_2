# Putování (1914–1918)

Interaktivní webová mapa zobrazující cesty čtyř českých historiků umění a architektů — **Pavla Janáka, Vincence Kramáře, Antonína Matějčka a Zdeňka Wirtha** — v letech 1914–1918, tedy v období první světové války.

Mapa vizualizuje navštívená místa a trasy pohybu mezi nimi (se směrovými šipkami označujícími pořadí cesty), spolu s dobovým politickým členěním Evropy (hranice a názvy tehdejších státních útvarů, např. Rakousko-Uhersko, Německé císařství, Ruské impérium apod.). Obsah lze filtrovat podle roku (posuvník 1914–1918) a podle jména sledované osoby. U jednotlivých navštívených míst i úseků trasy jsou k dispozici popisky s podrobnostmi (místo, rok, pořadí v trase, osoba).

Mapa byla vytvořena v prostředí QGIS a exportována do podoby samostatné webové aplikace (HTML/JavaScript, knihovna Leaflet) pomocí pluginu qgis2web; řada funkcí (dynamické popisky států, směrové šipky, filtrování, legenda) byla oproti standardnímu exportu dále upravena přímo v kódu.

## Struktura projektu

```
index.html          hlavní soubor mapy (otevře se v prohlížeči)
data/                geodata (hranice, trasy, navštívená místa) ve formátu GeoJSON/JS
css/, js/, legend/, webfonts/   podpůrné soubory knihovny Leaflet a pluginů
```

Mapu lze spustit buď nahráním na webový server (např. GitHub Pages), nebo (s výjimkou vrstvy OSM Standard, viz níže) otevřením souboru `index.html` přímo v prohlížeči.

**Poznámka k podkladovým mapám:** mapa nabízí tři alternativní podkladové vrstvy (Podkladová mapa 1 — reliéf, Podkladová mapa 2 — politická mapa, OSM Standard). Vrstva OSM Standard načítá dlaždice přímo ze serveru `tile.openstreetmap.org`, který z bezpečnostních důvodů nemusí dlaždice poskytnout stránce otevřené jako lokální soubor (`file://`) — pro její zobrazení mapu prosím prohlížejte nahranou na skutečném webovém serveru (např. přes GitHub Pages).

## Citace a zdroje

### Použité nástroje

QGIS DEVELOPMENT TEAM (2025): QGIS Geographic Information System. Open Source Geospatial Foundation Project, https://qgis.org (cit. 24. 9. 2026).

QGIS2WEB DEVELOPMENT TEAM (2025): qgis2web — QGIS plugin for exporting projects to Leaflet/OpenLayers web maps, https://github.com/qgis2web/qgis2web (cit. 24. 9. 2026).

LEAFLET (2025): Leaflet — a JavaScript library for interactive maps, https://leafletjs.com (cit. 24. 9. 2026).

### Podkladové mapy

**OpenStreetMap** (vrstva „OSM Standard“). V souladu s požadavky OpenStreetMap Foundation je nutné uvádět následující označení autorství, a to viditelně u mapy nebo v jejím okolí:

> © OpenStreetMap contributors

Text „OpenStreetMap" by měl odkazovat na https://www.openstreetmap.org/copyright. Mapová data OpenStreetMap jsou poskytována pod licencí **Open Database License (ODbL) 1.0** — https://opendatacommons.org/licenses/odbl/1-0/. V bibliografickém seznamu lze uvést:

OPENSTREETMAP CONTRIBUTORS (2025): OpenStreetMap [databáze]. OpenStreetMap Foundation. Dostupné pod licencí Open Database License z: https://www.openstreetmap.org (cit. 24. 9. 2026).

**Esri World Shaded Relief** (vrstva „Podkladová mapa 1"):

ESRI (2014): World Shaded Relief [mapová služba]. https://server.arcgisonline.com/ArcGIS/rest/services/World_Shaded_Relief/MapServer (cit. 24. 9. 2026).

### Geodata

*[Doplňte prosím zdroj dat pro vrstvu dobových politických hranic (Hranice_3) — např. konkrétní historický atlas, digitalizovaný podklad nebo vlastní zpracování.]*

*[Doplňte prosím zdroj/e primárních pramenů pro trasy a navštívená místa jednotlivých osob (Pohybosob_4, Navštívená místa) — např. archivní materiály, korespondence, deníky, sekundární literatura.]*

---

*Vytvořeno v rámci výzkumného projektu [doplňte název/instituci].*
