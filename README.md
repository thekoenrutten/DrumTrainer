# DrumTrainer 🥁
 
Een simpele webapp voor drummers om nummers in te studeren op verminderd tempo — zonder reclames, zonder gedoe.
 
**[→ Open DrumTrainer](https://thekoenrutten.github.io/DrumTrainer/)**
 
---
 
## Wat doet het?
 
DrumTrainer laadt een lokaal audiobestand en speelt het af met **pitch-corrected time stretching**: het tempo gaat omlaag, de toonhoogte blijft gelijk. Zo kun je een nummer stap voor stap opbouwen van 40% naar 100%.
 
- **Tempoladder** — stap voor stap van 40% naar 100% via vaste stappen
- **Loop instellen** — één knop, CDJ-stijl (zie hieronder)
- **Voortgang bijhouden** — lang indrukken op play markeert een tempo als geoefend ✓
- **Werkt volledig offline** — geen server, geen account, geen reclames
 
---
 
## Gebruik
 
1. Open de pagina in Safari op iPad of in een moderne browser
2. Tik op het uploadgebied en kies een mp3 (of ander audiobestand)
3. Het nummer speelt direct af op 100%
4. Gebruik de tempoladder of slider om het tempo aan te passen
5. Tik op de waveform om naar een positie te springen
 
### Loop instellen
 
De loop-knop (↺) werkt als een Pioneer CDJ:
 
| Druk | Actie |
|------|-------|
| 1e druk | Stelt het **beginpunt** in op de huidige positie — knop pulseert |
| 2e druk | Stelt het **eindpunt** in, loop springt meteen aan |
| 3e druk | Loop **gepauzeerd** — reloop beschikbaar |
| 4e druk | **Reloop** — springt terug naar begin en speelt opnieuw |
 
De tijdstempels en loopstatus worden onder de knoppen getoond.
 
### Voortgang markeren
 
Lang indrukken op de play-knop (±0,8 sec) markeert het huidige tempo als geoefend. De stap kleurt groen en de voortgangsbalk vult verder.
 
---
 
## Technisch
 
- Puur HTML/CSS/JS — één enkel bestand, geen dependencies buiten [SoundTouchJS](https://github.com/cutterbl/SoundTouchJS)
- SoundTouchJS is **ingebundeld** in het HTML-bestand — werkt offline
- Audio time stretching via het WSOLA-algoritme (SoundTouch)
- Getest op Safari iOS 16+ en Chrome desktop
