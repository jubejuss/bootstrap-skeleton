# bootstrap-skeleton
Lihtne bootstrapi skelett, lihtsalt demonstreerimaks bootstrapi ülesehitust.

## Bootstrapi põhiklassid
Bootstrapi põhiklassid on – container, row ja col  

Nende paigutamisel on oluline järgida kindlat järjekorda ja struktuuri, et tagada reageeriva disaini ja korrektse paigutuse loomine.

### Container
Alusta container klassiga. See on kõige välimine kiht ja seda kasutatakse sisu tsentreerimiseks ja paigutamiseks lehel. Bootstrapis on kaks konteineri tüüpi:
`.container`: Fikseeritud laiusega konteiner, mis muutub erinevatel ekraanisuurustel.  
`.container-fluid`: Konteiner, mis venib kogu ekraani laiusele igal seadmel.
Miks? Konteiner on oluline, kuna see loob lehele kindla "lava", millel kõik muu sisu asetseb. See tagab, et kõik elemendid on korralikult tsentreeritud ja paigutatud.
### Row
Järgmine samm on lisada `.row`. See peaks alati asuma konteineri sees. Rida kasutatakse veergude (columns) grupeerimiseks ja see tagab, et kõik veerud asuvad ühel ja samal horisontaaltasandil.  
Row klass aitab hallata veergude vahelisi vahekaugusi (gutters) ja ridade ühtlust. Ilma reata võivad veerud paigutuda ebaühtlaselt.
### Col (Columns)
Viimane samm on lisada veerud col klassi abil ridade sisse. Veerge saab jagada erinevateks suurusteks, kasutades spetsiifilisi klassinimede prefikseid, mis vastavad ekraanisuurustele (nt `.col-*`, `col-sm-*`, `col-md-*`, jne).  
Veerud on Bootstrapi võrkude süsteemi põhielemendid. Nad võimaldavad sisu jagada mitmeks veeruks, mis kohanduvad automaatselt vastavalt ekraani suurusele. See tagab, et sisu on korralikult organiseeritud ja reageeriv.  

## Layout'i näidis

```html
<div class="container">
  <div class="row">
    <div class="col-md-4">Veeru 1 sisu</div>
    <div class="col-md-4">Veeru 2 sisu</div>
    <div class="col-md-4">Veeru 3 sisu</div>
  </div>
</div>
```

### Ülesanne 1:
*Kasutades Bootstrapi klasse:*
1. Lisa oma Node bootstrapi projekti siinse `index.html` faili veebilehitsejas kuvatav sisu.
2. Nimeta töös kasutusel olevad klassid ja selgita, milline on neist igaühe funktsioon. Kirjuta selgitused artikkel elemendi sisse. Kasuta inimlikku vormistust – sobiva taseme pealkiri jms.
3. Muuda päise taustavärv tumedaks ja tõmba see servast servani.
4. Lisa iga kaardi ülemisse osasse erinevas suuruses pilt nii, et see järgiks kaardi raadiuseid.
5. Lisa piltidele 2rem-i paddingut ja muuda piltide nurkade raadiusteks 2rem-i.
6. Muuda pildid css-i kasutades sama suurteks ja sama külje suhtega piltideks. VIHJE: aspect ratio, object-fit