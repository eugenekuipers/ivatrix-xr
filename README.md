# ivatrix-xr

WebXR-demo's voor Ivatrix-workshops op PICO 4 Enterprise-brillen. Gehost op `xr.ivatrix.nl` via deploybase.

- Statische site, geen buildstap. Elke map is een losse demo met een eigen `index.html`.
- Three.js wordt geladen via CDN (importmap).
- Alle pagina's staan op `noindex`; `robots.txt` blokkeert crawlers.

## Structuur

| Pad | Inhoud |
|---|---|
| `/` | Startpagina met links naar de demo's (kioskpagina voor de brillen) |
| `/test/` | Capability test: WebXR-sessies, toegekende features, input, FPS |

## Testen

Open `https://xr.ivatrix.nl/test/` in de PICO-browser. Start de VR-test en de passthrough-test, en kopieer daarna de resultaten.
