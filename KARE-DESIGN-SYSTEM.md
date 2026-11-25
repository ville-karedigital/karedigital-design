# Kare Digital — Design System

**Versio:** 1.0 · 25.11.2026  
**Soveltamisala:** Kare Digital, karedigital.fi ja kaikki Kare-tuotteet  
**Tila:** Hyväksytty brändisuunta; sovelluskohtaiset komponentit viimeistellään käyttöönotossa.

## 1. Tarkoitus

Tämä tiedosto on yhteinen visuaalinen suunnitteluohje ihmisille ja AI-kehitystyökaluille. Noudata sitä uusia näkymiä rakennettaessa ja olemassa olevia uudistettaessa. Älä tulkitse ohjetta luvaksi muuttaa toiminnallisuuksia, sisältöjä tai sovellusarkkitehtuuria.

Kare on ajaton, tekninen, laadukas ja itsevarma mutta lähestyttävä teknologiabrändi. Visuaalinen identiteetti perustuu mustavalkoisuuteen, geometriseen typografiaan, täsmälliseen sommitteluun ja harkittuun tyhjään tilaan. Inhimillisyys syntyy tunnuksesta, kielestä ja aidoista käyttötilanteista, ei koristeista.

Referenssit: Linear (täsmällisyys ja minimalismi), Vercel (kontrasti ja neutraali identiteetti), ClickUp (typografia ja lähestyttävyys), Superlist (tuotteen havainnollistaminen). Älä kopioi referenssien sivustoja tai käyttöliittymiä.

## 2. Logo ja tunnus

Kare tarkoittaa pientä aaltoa, virettä tai värettä, esimerkiksi hymyn karetta. Uusi yhteinen tunnus yhdistää hymyn, liikkeen ja teknologisen geometrisuuden. Vanha susitunnus poistuu käytöstä.

- Käytä virallisia toimitettuja SVG-logoja ensisijaisesti; PNG tarvittaessa.
- Käytä mustaa logoa vaalealla ja valkoista tummalla taustalla.
- Kaikki tuotteet käyttävät samaa tunnusta ja yhtenäistä sanamerkkiperiaatetta: Kare Digital, Kare Point, Kare Maint, Kare Signal ja muut Kare-tuotteet.
- Käytä kunkin tuotteen hyväksyttyä omaa logotiedostoa. Älä rakenna sanamerkkiä uudelleen tekstillä, piirrä tunnusta uudestaan tai muuta sen mittasuhteita.
- Jos virallinen tuotelogo puuttuu, pyydä se ennen lopullista julkaisua.
- Jätä tunnuksen ympärille riittävä suoja-alue; älä venytä, varjosta, kierrä tai väritä sitä.
- Päivitä favicon, manifesti, touch icon, jakokuvien brändäys ja muut aktiiviset logoviittaukset käyttöönotossa. Käytä hyväksyttyjä favicon-versioita.

## 3. Värijärjestelmä

| Token | Arvo | Käyttö |
|---|---|---|
| Primary | `#0A0A0A` | Pääteksti, ensisijainen toiminto, vahva tumma pinta |
| Graphite | `#171717` | Tumma osio, vaihtoehtoinen tumma pinta |
| Secondary text | `#525252` | Leipäteksti ja toissijainen tieto vaalealla |
| Muted | `#A3A3A3` | Harkittu vähämerkityksinen tieto, ei tärkeä teksti vaalealla |
| Border | `#E5E5E5` | Hienovaraiset reunat ja jakoviivat |
| Secondary surface | `#F5F5F5` | Toissijainen pinta |
| Background | `#FFFFFF` | Ensisijainen vaalea tausta |

Paletti on neutraali: ei lämpimiä beigejä, sinertäviä harmaita, petrolia, turkoosia, minttua tai kultaisia brändikorostuksia. Sävyjä saa hienosäätää kontrastin ja käytettävyyden vuoksi, mutta neutraalius säilytetään.

### Brändivärit vs. toiminnalliset värit

Mustavalkoinen brändi ei tarkoita väritöntä ohjelmistoa. Tilat, prioriteetit, varoitukset, onnistumiset, kaaviot ja käyttäjän määrittelemät kategoriat voivat käyttää tarkoituksenmukaisia värejä. Väri ei saa olla ainoa tiedon välittäjä: käytä myös tekstiä, ikonia tai muuta tunnistetta. Älä muuta olemassa olevien tilojen merkitystä brändiuudistuksessa.

### Toteutus

Keskitä värit semanttisiin tokeneihin (background, surface, foreground, muted-foreground, border, primary, primary-foreground, focus, danger, success, warning jne.). Älä levitä heksakoodeja komponentteihin. Erota vaalean ja tumman teeman semanttiset arvot. Tumman sovellusteeman tarkka paletti määritellään erikseen; markkinointisivun tumma osio ei sellaisenaan ole sovelluksen tumma teema.

## 4. Typografia

- Otsikot: **Plus Jakarta Sans**, ensisijaisesti 700.
- Leipäteksti, navigaatio, painikkeet, lomakkeet ja käyttöliittymän data: **Inter**, ensisijaisesti 400, korostukset 500–600.
- Ei tarpeettomia lisäfontteja tai fonttipainoja. Käytä järjestelmäfontteja fallbackina.
- Vahva hierarkia syntyy koosta, painosta, kontrastista ja välistyksestä, ei värikkäistä korostuksista.
- Suurten markkinointiotsikoiden kirjainväli noin −0.04…−0.045em, rivikorkeus noin 1.1. Pienissä otsikoissa väljempi kirjainväli.
- Leipätekstin rivikorkeus markkinointisivuilla noin 1.5–1.6.
- Hero-otsikon lähtökohta noin 66–74 px desktopilla ja 36–40 px mobiilissa. Sovita todelliseen sisältöön ja näkymään; älä pakota näitä arvoja.
- Tavallinen markkinointiteksti noin 16 px; hero-kuvaus 18–20 px desktopilla, 16–18 px mobiilissa.
- Sovellusten typografia on tiiviimpää: lähtökohtaisesti 13–14 px data ja kontrollit, 14–16 px sisältö, 20–28 px sivuotsikot. Nämä ovat ehdotettuja lähtöarvoja, eivät hyväksyttyjä sovelluskohtaisia mittoja.
- Käytä tabular-nums-ominaisuutta numeerisissa taulukoissa, ajoissa ja summissa tarvittaessa.
- Huomioi suomen ja englannin tekstipituudet, luonnolliset rivinvaihdot ja fonttien lataus.

## 5. Yhteiset komponenttiperiaatteet

- Ensisijainen painike: lähes musta pinta ja valkoinen teksti; tummalla pinnalla tarvittaessa käänteinen.
- Toissijainen painike: neutraali pinta, tumma teksti ja tarvittaessa hienovarainen reuna.
- Tertiäärinen toiminto: teksti tai selkeä ikonipainike.
- Vaaralliset toiminnot voivat käyttää semanttista varoitusväriä.
- Käytä johdonmukaista, maltillista pyöristystä. Ehdotettu lähtökohta 6–8 px kontrollit ja 8–12 px suuremmat pinnat. Pill-muoto vain perustellusti, esimerkiksi tilamerkinnöissä.
- Käytä ohuita reunuksia, varjoja vain hierarkian tai kelluvan pinnan erottamiseen.
- Ikonit yhtenäisestä viivakuvakeperheestä; säilytä nykyinen kirjasto, jos se soveltuu. Epäselvillä ikonitoiminnoilla on tekstiselite tai tooltip.
- Käytä johdonmukaista välistysasteikkoa, esimerkiksi 4 px:n perusyksikköä. Vältä satunnaisia komponenttikohtaisia arvoja.
- Kaikilla interaktiivisilla elementeillä on selkeät hover-, focus-, active-, disabled- ja tarvittaessa loading-tilat.

## 6. Markkinointisivustot

Kare Pointin hyväksytty landing page on karedigital.fi:n tulevan uudistuksen visuaalinen referenssi. Säilytä sen hyväksi todettu typografia, neutraali identiteetti, tuotekeskeisyys ja kontrastirytmi.

### Sommittelu

- Pääosin valkoiset pinnat, harkitut vaaleanharmaat alueet ja muutama vahva tumma osio.
- Selkeä, hallitseva hero-otsikko, tiivis kuvaus, ensisijainen CTA ja aito tuotekuva.
- Yhtenäinen sisältöruudukko, täsmälliset linjaukset ja tarkoituksellinen tyhjä tila.
- Vuorottelevat teksti–tuotekuva-osiot; riittävän suuret ja luettavat kuvat.
- Hienovaraiset jakoviivat, ei jokaisen sisältölohkon kehystämistä kortiksi.
- Tumma tuote-esittely voi muodostaa sivun visuaalisen keskikohdan. Tumma loppu-CTA ja footer ovat luonteva päätös, jos sisältö tukee niitä.
- Älä lisää osioita vain visuaalisen vaihtelun vuoksi.

### Sisällön löydettävyys ja liike

Kare Pointissa hyväksytty periaate: tuotenäkymien ja toimialojen sisältö ei jää pelkkien välilehtien taakse. Käytä tarvittaessa scroll-driven storytelling -ratkaisua, pystysuuntaista accordionia ja sticky-tuote-esittelyä.

- Kaikki otsikot näkyvät; sisältö vaihtuu luonnollisen vierityksen mukana ja on myös manuaalisesti valittavissa.
- Käytä natiivia vieritystä, rajattua sticky-aluetta ja vakaita scroll-step-elementtejä. Ei scroll hijackingia, rullan tai kosketuksen kaappausta eikä vierityksen lukitusta.
- Aktiivinen tila toimii molempiin vierityssuuntiin. Manuaalinen valinta ja vieritystila eivät saa taistella keskenään.
- Hillityt 250–400 ms siirtymät ja crossfade; vakaa kuvakoko, ei välkkymistä tai layout-hyppyjä.
- Mobiilissa kaikki olennainen sisältö esitetään luontevasti peräkkäin ilman pakollista klikkaamista. Sticky vain jos tila ja käytettävyys sen sallivat.
- Kaikki sisältö säilyy saavutettavana ja indeksoitavana. Huomioi prefers-reduced-motion.
- Älä käytä scroll-driven-ratkaisua kaikkialla; käytä sitä vain kun se parantaa sisällön ymmärtämistä.

### Kuvamaailma

- Aidot, terävät ohjelmistokuvat ovat pääosassa. Älä generoi fiktiivisiä käyttöliittymiä tai desaturoi tuotekuvia.
- Käytä realistista, eristettyä demodataa; ei asiakkaiden luottamuksellisia tietoja.
- Valokuvissa käytännön työympäristöt: konepajat, tuotanto, asennus ja asiantuntijatyö. Luonnollinen valo ja neutraali yleisilme; aidot värit sallitaan.
- Vältä lavastettua kahvikuppi–kasvi–puupöytä-estetiikkaa, raskaita varjoja ja liioiteltua perspektiiviä.
- Päivitä lopulliset tuotekuvat sovelluksen visuaalisen uudistuksen jälkeen.

## 7. Ohjelmistojen käyttöliittymät

Yhteinen brändi sovelletaan työkaluihin käytettävyyden ehdoilla. Markkinointisivun suurta typografiaa, väljyyttä ja vieritysanimaatioita ei siirretä sellaisenaan operatiivisiin näkymiin.

### Navigaatio ja rakenne

- Neutraali, selkeä navigaatiokehys; ei petrolin tai turkoosin ympärille rakennettua navigaatiota.
- Aktiivinen sivu erottuu kontrastilla, pinnalla ja tarvittaessa ikonilla.
- Sidebarin ja topbarin tarkka vaalea/tumma toteutus valitaan sovelluskohtaisesti. Älä lukitse niitä ilman käytännön testausta.
- Sivun otsikko, tärkeimmät toiminnot, suodattimet ja sisältö muodostavat selkeän hierarkian.
- Säilytä tehokkaat työnkulut ja navigaation ennustettavuus.

### Data ja työskentely

- Suosi kompakteja, helposti silmäiltäviä taulukoita ja listoja operatiivisessa työssä.
- Älä muuta jokaista tietoriviä kortiksi. Käytä kortteja, kun ne palvelevat ryhmittelyä tai yhteenvetoa.
- Käytä hienovaraisia rivijakoja, johdonmukaista sarakekohdistusta ja selkeää aktiivista valintaa.
- Drawer sopii yksityiskohtien käsittelyyn desktopilla, jos taustan konteksti on hyödyllinen. Mobiilissa suosi täysleveitä sivunäkymiä monimutkaisille lomakkeille.
- Säilytä semanttiset tilavärit, selkeät virhetilat, validointi ja toimintojen palaute.
- Animaatiot ovat lyhyitä ja toiminnallisia, eivät markkinointisivun kaltaisia esityksiä. Ehdotettu lähtökohta 120–200 ms tavallisille käyttöliittymäsiirtymille.
- Älä vähennä informaatiotiheyttä tai lisää klikkauksia pelkän visuaalisen minimalismin vuoksi.

## 8. Saavutettavuus ja responsiivisuus

Tavoite WCAG 2.2 AA. Normaali teksti vähintään 4.5:1, suuri teksti 3:1 ja olennaiset käyttöliittymärajat sekä tilailmaisimet soveltuvin osin 3:1. Muted #A3A3A3 ei riitä tavalliseksi tekstiksi valkoisella.

- Näkyvä näppäimistöfokus, looginen tab-järjestys, semanttiset otsikot ja saavutettavat nimet.
- Accordion-kontrolleissa asianmukaiset aria-expanded/aria-controls-attribuutit.
- Kosketuskohteet riittävän suuria; mobiilissa tavoittele 44 px käytännön toimintakohteille.
- Ei tahatonta vaakavieritystä. Tarkista mobiili, tabletti, desktop ja leveät näytöt.
- Lomakekenttien mobiilikoko huomioi iOS:n automaattisen zoomauksen (yleensä vähintään 16 px).
- Tue reduced motion -asetusta. Älä piilota olennaista tietoa animaation tai hoverin taakse.
- Tarkista suomi ja englanti sekä vaalea ja tumma teema silloin kun ne kuuluvat tuotteeseen.

## 9. Vältettävät ratkaisut

- Geneerinen AI-estetiikka: koristegradientit, ambient glow, neon, satunnaiset kelluvat elementit ja ylimääräiset badge-elementit.
- Liiallinen pyöristys, korttien sisäkkäisyys, raskaat varjot ja tarpeettomat kehykset.
- Lämpimät tai kylmät brändiin kuulumattomat harmaasävyt.
- Koristeelliset otsikkoalleviivaukset, mukaan lukien vanha keltainen animaatio.
- Epäaidot tuotekuvat, tekaistut asiakasreferenssit tai perusteettomat markkinointiväitteet.
- Visuaalinen uudistus, joka muuttaa työnkulkuja, oikeuksia, hinnoittelua tai muuta liiketoimintalogiikkaa ilman erillistä hyväksyntää.

## 10. Käyttöönotto ja ylläpito

1. Kare Pointin landing page toimii ensimmäisenä uuden identiteetin referenssinä.
2. Koko karedigital.fi uudistetaan saman visuaalisen perustan mukaiseksi. Kare Pointin markkinointiosoite säilyy aluksi karedigital.fi/kare-point; sovellus point.karehub.fi.
3. Kare Pointin varsinaisen sovelluksen uudistus toteutetaan SaaS-julkaisusuunnitelman KP-19-kokonaisuuden yhteydessä. Vanha petrolia/turkoosia sisältävä visuaalinen suunta korvataan tällä brändisuunnalla. Julkaisusuunnitelma päivitetään erikseen.
4. Muut Kare-tuotteet uudistetaan asteittain omien kehityskokonaisuuksiensa yhteydessä.
5. Yhteiset tokenit, typografia ja komponenttiperiaatteet dokumentoidaan ja toteutetaan kunkin nykyisen frontend-arkkitehtuurin mukaisesti. Älä luo raskasta yhteistä komponenttikirjastoa ilman todellista tarvetta.
6. Hyväksy sovelluskohtaiset tarkat mitat, navigaatioratkaisut, tilavärit ja tumma teema käytännön näkymien perusteella. Päivitä tämä tiedosto, jos yhteinen sääntö muuttuu.

## 11. AI-kehitystyökalun tarkistuslista

Ennen toteutusta: lue tämä ohje ja nykyinen koodi; tunnista olemassa olevat tokenit, komponentit ja viralliset logot. Rajaa muutos pyydettyyn kokonaisuuteen.

Ennen valmistumista varmista:

- [ ] Viralliset logot ja faviconit ovat käytössä, vanha brändi poistettu aktiivisista näkymistä.
- [ ] Plus Jakarta Sans ja Inter ovat johdonmukaisesti käytössä.
- [ ] Neutraali paletti on toteutettu semanttisilla tokeneilla.
- [ ] Toiminnalliset värit ja niiden merkitykset säilyvät.
- [ ] Sommittelu, hierarkia, välistys ja komponentit ovat johdonmukaisia.
- [ ] Saavutettavuus, responsiivisuus ja kieliversiot on tarkistettu.
- [ ] Olemassa olevat toiminnot, oikeudet ja kaupalliset ehdot eivät ole muuttuneet tahattomasti.
- [ ] Muutos on tarkistettu todellisessa selaimessa tai sovelluksessa, ei vain koodin perusteella.
- [ ] Poikkeamat tästä ohjeesta, avoimet päätökset ja testauksen rajoitteet on raportoitu.

## 12. Päätösten status

**Hyväksytty:** mustavalkoinen brändisuunta, hymyn kare -tunnus, yhteinen tuoteidentiteetti, Plus Jakarta Sans + Inter, neutraali paletti, Kare Pointin landing page referenssinä, toiminnallisten värien salliminen, scroll-driven-sisältöperiaate, asteittainen käyttöönotto ja Kare Pointin sovellusuudistus SaaS-julkaisun yhteydessä.

**Lähtöarvoja / myöhemmin hyväksyttäviä:** tarkat fonttikoot, komponenttien mitat ja pyöristykset, välistysasteikko, sovellusten navigaatiopinnat, tumman teeman tokenit, semanttisten tilavärien tarkat sävyt ja tuotekohtaiset komponenttivariantit. Tämä tiedosto ei väitä, että näitä olisi jo toteutettu tai testattu kaikissa tuotteissa.
