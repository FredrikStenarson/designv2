Kmom05 - Laddningstid
=======================

I denna uppgift ska tre hemsidor analyseras med avseende på laddningstid. Metoden för undersökningen ska beskrivas. Resultat ska samlas in och presenteras. Utifrån resultaten ska det göras en analys av vardera hemsidan och eventuellt en kort jämförande diskussion.

Urval
-----------------------

Jag har valt att undersöka tre tillsatsmaterial tillverkares hemsidor. Bolagen heter ESAB, Voestalpine Böhler och Lincoln Electric. Bolagen verkar alla i samma bransch. Liten till ingen direkt försäljning sker via hemsidorna utan de är främst till för marknadsföring, produktinformation och vara utbildande. Branschen är mycket konservativ och jag tror att det finns stort utrymme för förbättrande åtgärder även om företagen anser sig ha branschledande hemsidor.

Metod
-----------------------

### Pagespeed
Googles tjänst Pagespeed Insights v. 5.5.0 användes för att mäta sidladdningshastighet och hur webbplatserna kunde åtgärdas för att nå ett högre betyg på områdena, performance, accessibility, best practice, SEO.
Webbläsaren som användes var Google Chrome v. 79.0.3945.88 (64-bit).
Testen gjordes för mobil och desktop för de tre webbplatsernas startsidor.
Övriga inställningar i analysverktyget varierades inte mellan testen och de var följande:

* Audits
    * Performance
    * Progressive Web App
    * Best Practice
    * Accessibility
    * SEO
* Throttling
    Simulated Slow 4G, 4x CPU Slowdown
* Clear storage

### Sidladdningsresultat från DevTools
Firefox Developer v. 72.0b9 (64-bitars).
För varje sida gjordes tre sidladdningar med tom cache med Firefox Developer 72.0b8 (64-bitars). Medelvärdet från respektive sidas Devtools data räknades ut och presenteras i avsnittet resultat.

Resultat
-----------------------
Alla data som presenteras nedan hämtades in 2019-12-19.

Här finner du samtlig inhämtad [data och den finns även representerad med pivottabeller](https://1drv.ms/x/s!AiIELn--fnGk2FKbAmqjGXNEZ-5Q?e=XYY5Jc). Observera att excelfilen innehåller fyra flikar.

Här finner du snapshot för webbplatsernas svenska landningssidor:

* [Böhler](https://1drv.ms/u/s!AiIELn--fnGk2FXSp-wmbOcPpyFx?e=5qabQo)
* [ESAB](https://1drv.ms/u/s!AiIELn--fnGk2EBGkGg3sQXf3-_8?e=SS6Yb5)
* [Lincoln](https://1drv.ms/u/s!AiIELn--fnGk2FQVAUnwyszHyDsi?e=MItITo)

### Pagespeed Insights
Här under presenteras medelvärdet i Googles Pagespeed Insights test för de tre undersökta sidorna per webbplats uppdelat på Mobil och Desktop.

Mobil
| Företag | Performance | Accessibility | BestPractice | SEO |
|--------------|----------------------|------------------------|-----------------------|--------------|
| Böhler       | 0.7                  | 79.7                   | 64.0                  | 96.0         |
| ESAB         | 18.7                 | 95.3                   | 57.0                  | 85.3         |
| Lincoln      | 18.0                 | 83.0                   | 78.7                  | 79.7         |

Desktop
| Företag | Performance | Accessibility | BestPractice | SEO |
|--------------|----------------------|------------------------|-----------------------|--------------|
| Böhler       | 0.3                  | 79.7                   | 64.0                  | 100.0        |
| ESAB         | 19.3                 | 90.3                   | 66.3                  | 86.7         |
| Lincoln      | 20.7                 | 83.0                   | 76.3                  | 88.0         |

### Sidladdningsresult från DevTools
Följande sidor laddades tre gånger vardera.

| Företag | Sida | Länk |
| ------- | ---- | --- |
| Böhler | 1 | [Startsida](https://www.voestalpine.com/welding/se)|
| Böhler | 2 | [Varumärken](https://www.voestalpine.com/welding/se/Varumaerken/Boehler-Welding)|
| Böhler | 3 | [Produkt](https://www.voestalpine.com/welding/se/Varumaerken/Boehler-Welding/Solidtraad)|
| ESAB | 1 | [Startsida](https://www.esab.se/se/se/index.cfm)|
| ESAB | 2 | [Produkt](https://www.esab.se/se/se/products/index.cfm)|
| ESAB | 3 | [Varumärke](https://www.esab.se/se/se/products/brands/exaton/index.cfm)|
| Lincoln | 1 | [Startsida](https://www.lincolnelectric.com/en-gb/Pages/default.aspx?locale=1053)|
| Lincoln | 2 | [Produkter](https://www.lincolnelectric.com/en-gb/consumables/Pages/consumables.aspx)|
| Lincoln | 3 | [Produkt](https://www.lincolnelectric.com/en-gb/consumables/mig-wires/Pages/mig-wires.aspx)|

Medelvärdet från Devtools data från tre omladdningar för respektive sida räknades ut och presenteras nedan.

| Företag | Sida | AntalFörfrågningar | Storlek [MB] | ÖverfördStorlek [MB] | Slutfört [s] | DOMContentLoad [s] | Load [s] |
|---------|------|-----------------------------|-----------------------|-------------------------------|-----------------------|-----------------------------|-------------------|
| Böhler  | 1    | 108                         | 4.73                  | 4.00                          | 9.97                  | 5.80                        | 8.42              |
| Böhler  | 2    | 102                         | 8.36                  | 7.62                          | 8.53                  | 4.39                        | 7.40              |
| Böhler  | 3    | 95                          | 3.55                  | 2.81                          | 8.60                  | 5.06                        | 6.44              |
| ESAB    | 1    | 100                         | 5.37                  | 4.13                          | 7.25                  | 3.44                        | 7.23              |
| ESAB    | 2    | 84                          | 2.40                  | 1.19                          | 3.35                  | 1.84                        | 3.36              |
| ESAB    | 3    | 108                         | 2.95                  | 1.73                          | 6.30                  | 3.22                        | 4.46              |
| Lincoln | 1    | 77                          | 5.01                  | 2.18                          | 9.45                  | 1.24                        | 2.41              |
| Lincoln | 2    | 61                          | 4.45                  | 1.73                          | 9.26                  | 0.90                        | 2.97              |
| Lincoln | 3    | 75                          | 4.08                  | 1.14                          | 9.78                  | 1.43                        | 2.32              |

Medelvärdet för alla sidladdningar per webbplats.

| Företag | Page | AntalFörfrågningar | Storlek [MB] | ÖverfördStorlek [MB] | Slutfört [s] | DOMContentLoad [s] | Load [s] |
|---------------|------|-----------------------------|-----------------------|-------------------------------|-----------------------|-----------------------------|-------------------|
| Böhler Medel  |      | 102                         | 5.55                  | 4.81                          | 9.03                  | 5.08                        | 7.42              |
| ESAB Medel    |      | 98                          | 3.57                  | 2.35                          | 5.63                  | 2.83                        | 5.02              |
| Lincoln Medel |      | 71                          | 4.51                  | 1.68                          | 9.50                  | 1.19                        | 2.57              |

Webbplatsernas individuella ranking för både Pagespeed Insights och DevTools laddningar, där ett är bäst resultat och tre sämst resultat.
|Kategori            | Böhler | ESAB | Lincoln |
|-------------------:|-------:|------:|------:|
|Mobil medel score   |       3|      2|      1|
|Desktop medel score |       3|      2|      1|
|AntalFörfrågningar  |       3|      2|      1|
|Storlek [MB]        |       3|      1|      2|
|Slutfört [s]        |       2|      1|      3|
|DOMContentLoad [s]  |       3|      2|      1|
|Load [s]            |       3|      2|      1|
|Medel rank          |     2.9|    1.7|    1.4|


Analys
-----------------------

### Pagespeed Insights
#### Performance
Böhler hade lågt resultat på performance (mobile 0.7 / desktop 0.3). Analysverktyget rödlistade first contentful paint, speed index, time to interact, first meaningful paint, first CPU idle.
Ovan nämnda parametrar tog ca 20sekunder.

Områden för förbättring är att skriva kritiska javascript, JS och CSS inline. Komprimera text med exempelvis Gzip för att minimera "total network bytes". Ta bort outnyttjad CSS. Använd nyare bildformat som JPEG 200, JPEG XR eller WebP då de komprimeras mer än PNG och JPEG.
Vänta med att ladda bilder som inte syns på skärmen för att minska tid till första interaktion.

ESAB och Lincoln fick båda runt 18 i poäng långt högre än Böhler men det är inte på något sätt bra. De har båda en långa lista med kritiska punkter att åtgärda för att snabba upp sina webbplatser.

För att öka webbplatser performance kräver det troligtvis en större insats att åtgärda.

#### Accessibility
Under accessibility känns de flesta saker som anges ganska lätt åtgärdade och borde åtgärdas för att öka poängen.
Samtliga hemsidor visade på kontrast problem "Background and foreground color do not have sufficient contrast ratio".
Böhler saknade lang attribut, ESAB och Lincoln saknade accessible names.

#### Best practice
Alla webbplatser använder sig av HTTP/1.1 vilket skulle kunna göras om till HTTP/2. Samtliga har även säkerhetsbrister då de använder javascriptbiliotek med kända säkerhetsbrister.

#### SEO
Sökmotoroptimering är det enda avsnitt där Böhler är får högst medelpoäng.
Det som drar ner ESAB och Lincoln är bland annat att länkar saknar beskrivande text, bilder saknar alt attribut, document saknar titel element, dokument saknar meta beskriving.

De åtgärder som föreslås för ESAB och Lincoln ter sig relativt enkla att genomföra.

### DevTools
Resultatet för parametrar undersökta med Devtools ger en klar bild över att Böhler har långsammast sida på samtliga punkter. ESAB och Lincoln är varierande bäst i de olika parametrarna även om Lincoln är bättre på fler punkter.

I uppgiften specificerades att sidans laddningstid (Load), tillsammans med antalet resurser som laddas samt (AntalFörfrågningar) sidans totala storlek (Storlek) skulle undersökas.
Lincoln snittade 71st resurser som laddas medan ESAB snittade 98st. Däremot var storleken på ESAB sida mindre med snitt på 3.57MB och Lincoln 4.51MB. Laddningstiden gick dock fortare för Lincoln i snitt med 2.58s jämfört med ESAB som snittade på 5.02s.

### Avslutningsvis
Företagen har inte direkt jämförbara sidor med avseende på exempelvis startsida, produkt och varumärke så det är inte direkt jämförbara. Jag tror det skulle ge en bättre representation av att räkna ett snitt över alla sidladdningar per webbplats och diskutera kring de resultaten, vilket jag försökt göra till viss del med de sidor som undersökts. Webbplatserna innehåller långt fler sidor och en större datamängd skulle troligtvis ge en mer rättvis bild.

Genom att inbördes ranka för respektive kategori, där ett var bäst och tre sämst, och räkna ut medelvärdet fick de tre företagen följande övergripande ranking:

* Böhler: 2.9
* ESAB: 1.7
* Lincoln: 1.4

Även om Böhler har klart lägre rank finns det många punkter Lincoln och ESAB behöver förbättra för att nå ett högre resultat i Pagespeed Insights.

Det ska också sägas att det inte nödvändigtvis den ena webbplatsen är bättre än den andra. Det finns mycket mer än det som undersökts som är av betydelse för en användares upplevelse men ur ett sidladdningsperspektiv ger ovanstående en indikation hur webbplatserna presterar och mäter sig inbördes.

Jag tror min gräns är väldigt varierande med hur gärna jag vill se innehållet på en sida. Gör jag research arbete är min tröskel väldigt låg, runt sekunden medan om jag vill läsa en längre artikel om något som jag vet intresserar mig kan jag nog accepetera 20sekunder. Är det en webbplats som kräver att man hoppar ständigt mellan sidor då blir det mer smärtsamt tydligt när sidladdningarna tar tid.

Övrigt
-----------------------

frst19
