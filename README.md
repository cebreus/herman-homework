# Úkol: Interaktivní galerie obrázků se zobrazením polohy na mapě

## Požadavky

- Validní a přístupný kód (W3C a WCAG).
- Optimalizace pro rychlost načítání a efektivní práce s daty.
- Použití plně statických souborů.
- HTML5, čisté CSS, možnost použití frameworku nebo preprocesoru.
- Preferováno použití Leaflet pro mapové podklady.
- Pro práci s metadaty doporučujeme knihovnu `exifr`.

## Vizuál a Chování

- Responzivní design od mobilních telefonů po desktopy.
- Levá část (2/3) galerie fotografií, pravá část mapa.
- Na telefonu zobrazení v jednom sloupci. Galerie v horní části zabírá maximálně 70% viewportu, pod ní mapa vyplňující zbývající prostor.
- Mapa dynamicky zobrazuje polohy všech obrázků ve viewportu.
- Volitelně: Pokud data obsahují informace o směru (azimutu), zobrazte je.
- Volitelně: Zobrazte cestu nebo trasu mezi jednotlivými body jako simulaci fyzického přemísťování mezi lokacemi.

### Příklad sloučených metadat dat

```json
{
  "CountryCode": "ISR",
  "CreatorContactInfo": {
    "parseType": "Resource",
    "CiEmailWork": "photos@cebre.us",
    "CiUrlWork": "https://cebre.us"
  },
  "Location": "Baha’istické zahrady",
  "creator": "Cebreus",
  "DateTimeDigitized": "2022-10-20T08:50:41+02:00",
  "DateTimeOriginal": "2022-10-20T08:50:41+02:00",
  "GPSAltitude": 267.2,
  "GPSAltitudeRef": <Uint8Array 00>,
  "GPSImgDirection": 103.78,
  "GPSImgDirectionRef": "T",
  "GPSLatitude": [32, 36, 44.42039972432805],
  "GPSLongitude": [34, 55, 5.7288],
  "GPSSpeed": 0,
  "GPSSpeedRef": "K",
  "GPSTimeStamp": "6:50:41",
  "City": "Haifa",
  "Country": "Izrael",
  "DateCreated": "2022-10-20T08:50:41+02:00",
  "CreateDate": "2022-10-20T07:49:49",
  "ModifyDate": "2022-10-20T08:50:41+02:00",
  "WebStatement": "http://creativecommons.org/licenses/by-nc/4.0/",
  "GPSVersionID": "2.2.0.0",
  "GPSLatitudeRef": "N",
  "GPSLongitudeRef": "E",
  "GPSMapDatum": "WGS-84",
  "GPSDestBearingRef": "True North",
  "GPSDestBearing": 281.28466796875,
  "GPSDateStamp": "2022:10:20",
  "GPSHPositioningError": 3.5355339046563916,
  "latitude": 32.61233899992342,
  "longitude": 34.918257999999994
}
```
