# ivatrix-xr

WebXR-demo's voor Ivatrix-workshops op PICO 4 Enterprise (en Meta Quest 3 / Pro). Gehost op `xr.ivatrix.nl` via deploybase.

- Statische site, geen buildstap. Elke map is een losse demo met een eigen `index.html`.
- Three.js via CDN (importmap).
- Alle pagina's op `noindex`; `robots.txt` blokkeert crawlers.

## Structuur

| Pad | Inhoud |
|---|---|
| `/` | Startpagina (kiosk-launcher) met tegels naar de demo's |
| `/test/` | Capability test; resultaten gaan naar deploybase-formulier `xr-testresultaten` |
| `/objecten/` | 3D-objecten oppakken, draaien en verplaatsen met de controllers |

## Nieuwe demo toevoegen

1. Maak een map, bijvoorbeeld `/veiligheid/`, met een eigen `index.html`.
2. Zet bovenaan de pagina een link `<a href="../">← Alle demo's</a>` (in kioskmodus is er geen adresbalk).
3. Voeg de demo toe aan de array `DEMOS` in `/index.html`.

## Kioskmodus

In PICO Business Suite: WebXR-link `https://xr.ivatrix.nl/` toevoegen en in kioskmodus zetten.

## Deploy

Push naar `main`. Zolang deploy-on-push in deploybase nog niet aan staat: handmatig "Deploy main" in het dashboard.

## Licenties 3D-modellen (`/objecten/models/`)

| Bestand | Bron | Licentie |
|---|---|---|
| `robot.glb` | RobotExpressive, Tomás Laulhé (Quaternius), aangepast door Don McCurdy | CC0 1.0 |
| `toycar.glb` | Khronos glTF Sample Assets, ToyCar | CC0 1.0 |
| `sheenchair.glb` | Khronos glTF Sample Assets, SheenChair | CC0 1.0 |
| `lantern.glb` | Khronos glTF Sample Assets, Lantern | CC0 1.0 |
| `avocado.glb` | Khronos glTF Sample Assets, Avocado | CC0 1.0 |
