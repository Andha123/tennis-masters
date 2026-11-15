# Tennis Duell 🎾

**Spill her: https://andha123.github.io/tennis-masters/**

Et realistisk 3D-tennisspill i nettleseren, sett fra siden som på TV. Spill mot datamaskinen, mot en kompis på samme tastatur, eller **online på hver deres PC eller Mac** med en firetegns kode. Ingen konto og ingen installasjon.

## Spill

- **Mot datamaskin** – tre vanskelighetsgrader
- **2 spillere – samme tastatur**
- **Online** – én trykker «Lag kamp» og sender koden, den andre skriver inn koden og trykker «Bli med»
- **Lag din spiller** – antrekk (shorts, skjørt, kjole), farger og mønster, hudfarge, kroppsbygning, frisyre, skjegg, hodeplagg, briller, svettebånd, racket og sko
- **Grafikk** – Rask, Høy eller Ultra 4K (rendrer i 3840×2160)
- **Lyd** – Alt (publikum, slag og dommer som roper ut stillingen), Uten dommer eller Av

## Kontroller

| Tast | Handling |
|---|---|
| A / D eller ← / → | Løp frem og tilbake |
| W eller ↑ | Hopp |
| **X** | Slå (og serve: X kaster opp ballen, X igjen slår) |
| **C** | Smash: kraftig slag ovenfra når ballen er over hodet (hopp med W for å nå høyere). Lynrask, bratt og spretter høyt |
| Hold mot nettet når du slår | Hard topspin, langt |
| Hold bakover når du slår | Lobb, høy og dyp. Gir motspilleren sjansen til smash |
| Esc | Pause / meny |

To på samme tastatur: venstre spiller bruker A/D/W, X og C, mens høyre spiller bruker piltastene, L (slå) og K (smash).

## Regler og fysikk

- Vanlig tennistelling (15–30–40, deuce, fordel). Den som først vinner det valgte antallet games, vinner kampen.
- Serven må lande i serveruten. To feil gir dobbeltfeil.
- Ballen har luftmotstand og spinn (Magnus-effekt). Topspin dykker og spretter høyt. En smash går over 40 m/s, treffer bratt og spretter høyt opp.
- Banen har ekte mål: 23,77 m lang, med nett på 0,914 m.

## Spillerne

- Hode, ansikt og hår er formet og malt i programmet: øyne med øyelokk, nese, lepper, ører, bryn, hårstrå, skjegg og skjeggstubb.
- Armer og bein er sammenhengende og bøyer seg mykt i albue og kne, med muskelformer (lår, legger, biceps). Fingrene griper rundt racketen.
- Bevegelsene følger fjærer: serven har oppkast med racketen ned og bak før trofé-stillingen, og armene går rolig tilbake til klarstilling etter slaget.

## Legg spillet ut på GitHub Pages

1. Lag et nytt **public** repository på github.com, for eksempel `tennis-masters`.
2. Trykk **Add file → Upload files** og last opp `index.html` og `README.md` fra denne mappen. Trykk **Commit changes**.
3. Gå til **Settings → Pages**. Under *Build and deployment* velger du **Deploy from a branch**, deretter `main` og `/ (root)`, og trykker **Save**.
4. Etter et minutt eller to ligger spillet på `https://andha123.github.io/tennis-masters/`. Send lenken til kompisen din.

## Teknisk

- Én fil (`index.html`). 3D-grafikken bruker [three.js](https://threejs.org) fra jsDelivr.
- Online-spill går via en relétjeneste over sikre websockets (MQTT), så det virker gjennom de fleste brannmurer og nett. Spillet kobler til flere offentlige servere samtidig for å være robust.
- Hvis koblingen svikter: last siden på nytt hos begge, og lag en ny kode.
