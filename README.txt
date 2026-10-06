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

QGIS Development Team, QGIS Geographic Information System, Open Source Geospatial Foundation Project 2025, https://qgis.org, vyhledáno 24. 9. 2026.

qgis2web Development Team, qgis2web: QGIS plugin for exporting projects to Leaflet/OpenLayers web maps, 2025, https://github.com/qgis2web/qgis2web, vyhledáno 24. 9. 2026.

Leaflet: A JavaScript library for interactive maps, 2025, https://leafletjs.com, vyhledáno 24. 9. 2026.

### Podkladové mapy

OpenStreetMap, OpenStreetMap Foundation, https://www.openstreetmap.org, vyhledáno 17. 7. 2026.

Esri, World Shaded Relief (mapová služba), 2014, https://server.arcgisonline.com/ArcGIS/rest/services/World_Shaded_Relief/MapServer, vyhledáno 24. 9. 2026.

### Geodata

Department of History, United States Military Academy, Atlases, Digital History Center, https://dhc.westpoint.edu/atlases/, vyhledáno 2. 10. 2026.
---

*Vytvořeno v rámci výzkumného projektu NAKI II.
