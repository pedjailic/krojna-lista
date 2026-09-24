# Krojna lista stolarije

Besplatan kalkulator za PVC i ALU stolariju. Unesete zidarski otvor, a dobijete:

- spoljnu meru štoka i krila
- krojnu listu profila (štok, krilo, srednjak, lajsne) sa uglovima sečenja
- dimenzije stakla i ukupnu površinu u m²
- raspored sečenja po šipkama (optimizacija, otpad i upotrebljivi ostaci)
- kopiranje krojne liste u Excel jednim klikom
- **porudžbinu stakla**: dodajete stakla iz više pozicija u jednu listu, iste dimenzije se spajaju, a gotov tekst porudžbine kopirate u mejl, Viber ili Excel
- **pregled svih pozicija**: svaka dodata pozicija se pamti sa crtežom i krojnom listom; na kraju unosa dobijate zbirnu krojnu listu, zbirno sečenje šipki i sve pozicije jednu ispod druge, spremno za štampu

Radi u pregledaču, bez instalacije i bez servera. Samo otvorite `index.html`.

## Porudžbina stakla

1. Upišite oznaku pozicije (npr. P1) i tip stakla (npr. 4-16-4 Low-E, Ar).
2. Izračunajte poziciju i kliknite **Dodaj u porudžbinu**. Oznaka se sama poveća na P2.
3. Ponovite za sve pozicije. Unesite proizvođača (podrazumevano: Zoran), dobavljača, rok i napomenu.
4. Kliknite **Kopiraj porudžbinu** i nalepite tekst u mejl ili Viber, ili **Kopiraj za Excel**.

Porudžbina se čuva u pregledaču na tom uređaju dok je ne obrišete.

## Tipovi pozicija

Fiksni · Jednokrilni · Dvokrilni sa srednjakom · Dvokrilni sa lažnim srednjakom · Krilo + fiks · Krilo – fiks – krilo · Krilo + nadsvetlo

## Formule

```
Štok               = otvor − montažni zazor
Svetli otvor štoka = štok − 2 × vidna širina štoka
Krilo              = svetlo polja + 2 × preklop krila
Staklo             = svetlo profila + 2 × (dubina falca − zazor stakla)
Rez štoka/krila    = mera + 2 × dodatak za varenje
Srednjak           = svetli otvor + 2 × dodatak po kraju

Lažni srednjak:
Krilo (svako)      = (svetla širina štoka + 2 × preklop − razmak krila) / 2
Visina krila       = svetla visina štoka + 2 × preklop
Lažni srednjak     = svetla visina štoka − odbitak (rez 90°)
```

## Podrazumevani odbici (okvirni, PVC 70 mm, 5 komora)

| Parametar | mm |
|---|---|
| Montažni zazor po strani | 10 |
| Štok, vidna širina | 64 |
| Krilo, vidna širina | 77 |
| Preklop krila | 8 |
| Srednjak (T) | 84 |
| Lažni srednjak: razmak krila | 6 |
| Lažni srednjak: kraći od svetlog otvora | 4 |
| Dodatak za varenje po kraju | 3 |
| Dubina falca | 20 |
| Zazor stakla | 5 |
| Dužina šipke | 6500 |
| Rez testere | 4 |

**Važno:** ovo su okvirne vrednosti. Pre proizvodnje upišite odbitke iz kataloga vašeg sistema profila (u delu „Odbici sistema“). Za ALU dodatak za varenje stavite na 0. Prve pozicije uvek proverite ručno.

## Objavljivanje na GitHub Pages

Settings → Pages → Branch: `main`, folder `/ (root)` → Save. Stranica će biti na `https://<korisnik>.github.io/<repo>/`.

## Licenca

MIT
