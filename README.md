# Earth Information Jukebox: Hear the Arctic Ice Disappear

Built for the **NASA International Space Apps Challenge 2026** ("The Earth Information Jukebox" challenge).

**Live demo:** https://joselynrajeev55-ops.github.io/earth-information-jukebox/

## What it does
Earth Information Jukebox turns Arctic sea ice data into sound. Each year is one note:
a **low note** means a lot of ice, and a **high note** means less ice.
As the pitch climbs, you can hear the ice shrinking.

The page also shows a chart with a moving marker and a live caption with the year
and ice extent (million km²) for each note.

## How to use it
1. Open the live demo.
2. Press **Play**.
3. Listen to the pitch rise from 1979 to 2026 while the marker moves along the chart.

## Data
- **NSIDC Sea Ice Index** (NOAA at NSIDC), monthly sea ice extent by year, Northern Hemisphere.
- Derived from satellite passive microwave observations.
- Source: https://nsidc.org/arcticseaicenews/sea-ice-tools/
- This project uses the **September** value for each year, when Arctic ice is at its yearly minimum.

## How it works
- Data was cleaned in Python (Pandas) in Google Colab.
- `index.html` is the interactive page, built with HTML, CSS, JavaScript and the Web Audio API.
- Mapping: sea ice extent is mapped to pitch (most ice = 220 Hz, least ice = 880 Hz).

## Run it locally
Download `index.html` and open it in a browser (Chrome recommended). No installation needed.

## Future work
- More tracks (Antarctic ice, sea surface temperature, air quality)
- NASA satellite imagery that changes along with the sound
- User-selectable instruments, regions and speed

## Credits
Data: NSIDC / NOAA at NSIDC, based on NASA satellite observations.
Built by Joselyn Rajeev for NASA Space Apps Challenge 2026.
