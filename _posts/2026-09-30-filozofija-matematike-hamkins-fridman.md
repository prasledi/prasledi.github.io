---
layout: post
title: "Filozofija matematike: neskončnost, paradoksi in meje resnice — pogovor z Joelom Davidom Hamkinsom"
date: 2026-09-30
categories: [Matematika, Filozofija]
tags: [teorija-množic, neskončnost, godel, zfc, filozofija-matematike, kontinuumska-hipoteza, transfinitni]
image: https://images.unsplash.com/photo-1462331940025-496dfbfc7564?q=80&w=2000&auto=format&fit=crop
---

{% include embed/youtube.html id='14OPT6CcsH4' %}

## Kazalo

- [Cantorjeva revolucija in različno velike neskončnosti](#cantorjeva-revolucija)
- [Hilbertov hotel in narava preštevne neskončnosti](#hilbertov-hotel)
- [Cantorjev diagonalni argument in nepreštevne neskončnosti](#diagonalni-argument)
- [ZFC, Gödelovi izreki in meje dokazljivosti](#zfc-in-godel)
- [Neskončni šah in transfinitni ordinali](#nesconcni-sah)
- [Umetna inteligenca in prihodnost matematike](#umetna-inteligenca)

V najnovejši epizodi podcasta Lexa Fridmana je gostoval Joel David Hamkins — matematik in filozof, specialist za teorijo množic in filozofijo matematike ter avtor knjig *Proof and the Art of Mathematics* in *Lectures on the Philosophy of Mathematics*. Hamkins je prvi uvrščeni uporabnik vseh časov na MathOverflowu, ki je matematični ekvivalent StackOverflowa za raziskovalne matematike. V pogovoru, ki traja več ur, sta z Fridmanom razpravljala o temeljih moderne matematike, o vprašanjih resnice in dokazljivosti, o paradoksih, ki so pretresli matematično skupnost na prelomu 20. stoletja, in o tem, ali bo umetna inteligenca kdaj postala resničen partner matematiku. Pogovor razkriva, da so temelji matematike hkrati trdni in globoko skrivnostni — in da nekatera vprašanja, ki so zaposlovala največje matematične ume preteklega stoletja, ostajajo odprta še danes.

## Cantorjeva revolucija in različno velike neskončnosti {#cantorjeva-revolucija}

![Profesor piše matematične enačbe na tablo](https://images.unsplash.com/photo-1758685734643-db77920292bc?q=80&w=1200&auto=format&fit=crop)

Zgodba neskončnosti se ne začne pri Georgu Cantorju, a prav on jo je prvi pripeljal do logičnega konca. Hamkins pogovor začne daleč nazaj — pri Aristotelu, ki je ostro ločeval med potencialno neskončnostjo (procesom, ki se nikoli ne zaključi) in dejansko neskončnostjo (dovršenim neskončnim predmetom). Za tisoče let so matematiki skoraj brez izjeme sprejemali Aristotelovo stališče: dejanska neskončnost je nesmiselna.

Galileo Galilei je bil med redkimi, ki so se temu upirali. V *Dialogu o dveh novih vedah* je opazil skrb vzbujajoče dejstvo: vsako naravno število ima natanko en kvadrat, vsak kvadrat pa natanko en koren — med naravnimi in kvadratnimi števili torej obstaja bijektivna preslikava ena na ena. Toda kvadratna števila so le del naravnih, vmesnih pa je brez meja. Ali sta dve množici enako veliki, če sta si vzajemno prirejeni? Ali pa je tista, ki vsebuje drugo, večja? Galileo ni mogel razrešiti tega napetja in je vprašanje preprosto opustil.

Cantor tega ni mogel. Razvil je natančno definicijo enake moči množic: dve množici sta enakoštevni, kadar obstaja bijektivna preslikava med njunimi elementi. Ta Cantor-Humov princip je neposredno nasprotoval Evklidovemu principu — »celota je vedno večja od dela« — in Cantor ga je zavestno odločno zavrnil. Posledica je bila osupljiva: neskončnosti niso vse enake. Nekatere so strogo večje od drugih, in to ne le za kakšen element ali dva, temveč v globoko temeljnem smislu.

Ta ugotovitev je povzročila tisto, kar Hamkins imenuje »krizo in preobrazbo matematike«. Ker je bila neskončnost od nekdaj tesno prepletena s teologijo in pojmom božanskega, je Cantorjevo odkritje sprožilo teološke debate. Vodilni nemški matematik Leopold Kronecker je Cantorja javno imenoval »kvaritelja mladine« in si prizadeval uničiti njegovo kariero. Iz logičnih neskladnosti, ki so sledile, so se porodili paradoksi — med njimi Russellov —, ki so ogrozili konsistentnost celotne matematike. Cantor sam je v poznih letih trpel za hudo depresijo in zadnja leta preživel v psihiatričnih zavodih, obseden z dokazovanjem kontinuumske hipoteze.

## Hilbertov hotel in narava preštevne neskončnosti {#hilbertov-hotel}

![Neskončni hodnik hotelskih sob](https://images.unsplash.com/photo-1647751513478-b1501f21f76f?q=80&w=1200&auto=format&fit=crop)

Za razumevanje preštevne neskončnosti — tiste, ki jo dosežemo s štetjem naravnih števil — je Hamkins predstavil sloviti miselni eksperiment Davida Hilberta: Hilbertov hotel.

Zamislimo si hotel z neskončno sobami, oštevilčenimi od 0 dalje. Hotel je poln; v vsaki sobi je gost. Vseeno prispe nov gost in prosi za sobo. Upravnik pošlje sporočilo vsem obstoječim gostom: preselite se v sobo z eno višjo številko. Gost iz sobe 5 gre v sobo 6, gost iz sobe 99 gre v sobo 100 in tako dalje. Soba 0 se sprosti — novi gost je nastanjen. Ta enostavni postopek razodeva temeljno lastnost neskončnih množic: dodajanje enega elementa jo lahko pusti enako »veliko« v smislu enakoštevnosti.

Ko prispe neskončni avtobus z neskončno potniki, upravnik vse obstoječe goste preseli v sobe z dvojnimi številkami (gost iz sobe n gre v sobo 2n). Sprostijo se vse lihe sobe, ki sprejmejo potnike iz avtobusa. Ko pa prispe neskončni vlak z neskončno vagoni, od katerih ima vsak neskončno sedežev, je rešitev elegantna in hkrati presenetljiva: potniku v vagonu c na sedežu s dodelimo sobo s številko 3^c × 5^s. Ker je razčlenitev na prafaktorje enolična, vsak potnik dobi edinstveno sobo in nobeni dve se ne prekrivata.

Miselni eksperiment ponazori dva osrednja izreka: unija dveh preštevno neskončnih množic ostane preštevno neskončna, enako pa velja za neskončno unijo preštevno neskončnih množic. Celo množica racionalnih števil — zlomkov, ki so med katerima koli dvema realnima točkama gosto razporejeni — je preštevna, saj je vsak ulomek p/q mogoče predpisati sobi s številko 3^p × 5^q. Hamkins to opiše kot presenetljivo lastnost preštevne neskončnosti: ne glede na to, koliko preštevno neskončnih množic združimo, rezultat ostane preštevno neskončen.

## Cantorjev diagonalni argument in nepreštevne neskončnosti {#diagonalni-argument}

![Profesor in studentka razpravljata ob matematičnih enačbah](https://images.unsplash.com/photo-1758685848238-001e0cc182ae?q=80&w=1200&auto=format&fit=crop)

Cantorjev največji dosežek je bil dokaz, da je množica realnih števil strogo večja od množice naravnih. Tu nastopi ena najpomembnejših dokaznih metod v zgodovini matematike: diagonalni argument.

Predpostavimo nasprotno — da je mogoče vsa realna števila razvrstiti v neskončen seznam: r₀, r₁, r₂, r₃ in tako naprej, pri čemer vsako realno število nastopi natanko enkrat. Cantorjeva metoda: za vsako naravno število n pogledamo n-to decimalno mesto n-tega realnega števila v seznamu, nato pa izberemo drugačno cifro (pri tem se izognemo 0 in 9, da ne nastopijo dvoznačne decimalne reprezentacije, kot sta 1,000... in 0,999...). S tem konstruiramo novo realno število z, katerega n-to decimalno mesto je vselej drugačno od n-tega decimalnega mesta n-tega elementa v seznamu. Število z se razlikuje od r₀ na prvem decimalnem mestu, od r₁ na drugem, od r₂ na tretjem in tako naprej. Torej z ni v seznamu — protislovje z začetno predpostavko.

Dokaz ni le tehničen; razkriva globoko strukturo: realna števila so nepreštevna, neskončnost realnih je strogo večja od neskončnosti naravnih. Enaki diagonalni principi se pojavljajo v Russellovem paradoksu in v dokazih teorije izračunljivosti. Hamkins posebej poudari, da gre za isti logični mehanizem: vsem tem dokazom je skupno, da ustvarijo objekt, ki se od vsakega elementa predpostavljenega seznama razlikuje v natanko enem, a bistveno predpisanem vidiku.

Russellova različica tega principa pokaže, da ne more obstajati množica vseh množic: če bi ta obstajala, bi lahko tvorili množico vseh množic, ki same sebe ne vsebujejo — toda ta množica bi sama sebe vsebovala natanko tedaj, ko se ne bi. Hamkins to raje imenuje Russellov izrek kot Russellov paradoks — saj gre za globok matematični rezultat, ne za protislovje v dobro zasnovanem sistemu. Ko je Bertrand Russell sporočil to odkritje Gottlobu Fregeju, je ta ravno zaključeval monumentalno delo, ki naj bi utemeljilo celotno matematiko na logiki. Fregejeva odgovor v dodatku je ostal eden najbolj pretresljivih stavkov v zgodovini matematike: »Komaj kaj bolj neprijetnega se lahko primeri piscu o znanosti, kot da mu po zaključenem delu pretresejo enega od temeljev.«

## ZFC, Gödelovi izreki in meje dokazljivosti {#zfc-in-godel}

![Galaksija — simbol globine matematičnih temeljev](https://images.unsplash.com/photo-1620882581777-9b35bf408f09?q=80&w=1200&auto=format&fit=crop)

Cantorjeve neskončnosti in Russellov paradoks so matematično skupnost prisilili v iskanje trdnih temeljev. Zermelo je leta 1908 formaliziral aksiome teorije množic, ki so do danes — z Fraenkelovimi dopolnitvami in aksiomu izbire — znani pod kratico ZFC (Zermelo-Fraenkel z aksiomu izbire). Ti aksiomi opisujejo, kaj je množica in kakšne operacije so z množicami dopustne: obstoj prazne množice, možnost tvorjenja unije, potenčne množice in neskončnih množic, pa tudi aksiom izbire — preprost na videz, a filozofsko globok.

Aksiom izbire pravi, da za vsako zbirko nepraznih množic obstaja funkcija, ki iz vsake izbere natanko en element. Hamkins ga ilustrira z Russellovim primerom: za neskončno zbirko parov čevljev je izbira enostavna (vedno vzamemo levega), za neskončno zbirko parov nogavic, ki si znotraj para sploh niso ločljive, pa ne obstaja nobeno naravno pravilo izbire. Aksiom zagotavlja, da takšna funkcija kljub temu obstaja — a njene vsebine ne moremo predpisati. Natanko ta razlika med »eksistenca« in »konstruktivnost« je bila vir žolčnih matematičnih sporov na prelomu 20. stoletja.

Na temelju ZFC je David Hilbert zasnoval program, ki je bil ambiciozen do skrajnosti: s finitistično analizo simbolnih dokazov dokazati konsistentnost celotne matematike. Iz tega bi sledilo, da za vsako matematično vprašanje obstaja odgovor in da ga je načeloma mogoče najti s sistematičnim pregledovanjem dokazov.

Kurt Gödel je leta 1931 ta program dokončno razbil. Z izreki o nepopolnosti je dokazal: (1) vsak dovolj bogat konsistenten formalni sistem vsebuje resnične stavke, ki jih v njem ni mogoče dokazati; (2) takšen sistem ne more dokazati lastne konsistentnosti. David Hilbert je na pokojniškem govoru izjavil: »Moramo vedeti, bomo vedeli.« Gödel mu je v bistvu odgovoril: »Ne. Nikoli ne boste mogli vedeti vsega.«

Hamkins nato prikaže, da je problem ustavitve v računalništvu — Turingov dokaz iz leta 1936, da ne obstaja splošni algoritem, ki bi za vsak program odločil, ali se bo ta ustavil — le drug obraz iste diagonalne logike. Če bi obstajal algoritem za reševanje problema ustavitve, bi ga bilo mogoče uporabiti za gradnjo popolne teorije elementarne matematike. Ker pa problem ustavitve ni izračunljivo odločljiv, popolna teorija ne more obstajati — in s tem je Gödelov izrek o nepopolnosti dobil neposreden, eleganten dokaz.

Hamkins poudari, da ga to ne žalosti. Nepopolnost ni tragedija, temveč razodetje: matematična resnica je resnična kategorija, ki presega dokazljivost v kateremkoli danem sistemu. Razlika med »resnično« in »dokazljivo« je ena najpomembnejših distinkcij sodobne matematike in logike.

Pogovor se dotakne tudi Cantorjeve kontinuumske hipoteze — vprašanja, ki je Cantorja preganjalo do konca življenja: ali obstaja neskončnost med kardinalnostjo naravnih in realnih števil? Gödel je leta 1938 dokazal, da je hipoteza konsistentna z ZFC (ne moremo je ovreči), Paul Cohen pa je leta 1963 z metodo prisiljevanja (*forcing*) dokazal, da je konsistentna tudi njena negacija (ne moremo je dokazati). Hipoteza je torej neodvisna od ZFC — ne drži ne lažna. Hamkins vidi v tisoče primerih takšne neodvisnosti potrditev svojega pluralističnega pogleda na matematično resničnost: ne obstaja en sam matematični svet, temveč multiverz teorij množic, ki ima vsaka svojo resnico glede kontinuumske hipoteze. Aksiomi so za Hamkinsa bolj podobni izbiram sveta, v katerem delamo, kot pa odrazom edine dejanske resnice.

## Neskončni šah in transfinitni ordinali {#nesconcni-sah}

![Šahovske figure na šahovnici](https://images.unsplash.com/photo-1585038021831-8afd9f9ab27f?q=80&w=1200&auto=format&fit=crop)

Med bolj nenavadnimi poglavji v Hamkinsovem delu je neskončni šah — igra na neskončni šahovnici (mreži s celimi števili v vse smeri), pri kateri figure sledijo enakim pravilom gibanja kot pri klasičnem šahu, le da so premiki v vse smeri neomejeni. Hamkins se je te teme lotil po vprašanju na MathOverflowu in ugotovil, da neskončni šah omogoča pojave, ki so v klasičnem šahu nemogoči.

V klasičnem šahu je vsaka pozicija ali neodločena, remizirana ali pa mat v n potezah za nekatero določeno naravno število n. V neskončnem šahu pa obstajajo pozicije, pri katerih ima beli zmagovalno strategijo, a ne obstaja nobeno naravno število n, za katerega bi bila zmaga zagotovljena v največ n potezah. Beli bo zmago zagotovo dosegel, a črni nadzira, koliko potez bo to trajalo: za vsako naravno število n bo črni sposoben igrati tako, da bo beli potreboval več kot n potez. To je točno to, kar matematiki imenujejo vrednost pozicije omega — prvi transfinitni ordinal.

Hamkins in njegov soavtor Corey Evans, ki je tako ameriški mojster šaha kot filozofski profesor prava, sta zgradila pozicije z vrednostmi omega, omega-kvadrat, omega-kubik in omega na četrto potenco. Kasnejša dela so razširila ta rezultat na vse preštevne ordinalte: vsak preštevni ordinal se pojavlja kot vrednost neke pozicije v neskončnem šahu.

Transfinitni ordinali — Cantorjev sistem štetja onkraj neskončnosti — so za Hamkinsa osebno najpomembnejši matematični pojem. Začnemo z naravnimi števili 0, 1, 2, 3 in naprej; po vseh naravnih pride omega (ω), nato ω + 1, ω + 2 ... nato ω · 2, ω · 3 ... nato ω², ω³ ... Proces nikoli ne konča. Hamkins: »Preprosta ideja štetja onkraj neskončnosti je tako elegantna in je rodila toliko globoke matematike, da jo štejem za najlepšo matematično idejo nasploh.«

## Umetna inteligenca in prihodnost matematike {#umetna-inteligenca}

![Nevronske mreže in umetna inteligenca](https://images.unsplash.com/photo-1736430043488-0c369959a5c6?q=80&w=1200&auto=format&fit=crop)

Pogovor se zaključi z vprašanjem, ki je v matematičnih krogih vse bolj prisotno: ali bo umetna inteligenca postala resničen matematični sodelavec? Hamkins je pri tem odločno skeptičen — a ne iz površnega odpora do tehnologije.

Po izkušnjah z različnimi sistemi Hamkins ugotavlja, da so odgovori na matematična vprašanja pogosto napačni in da sistemi trdijo, da so pravilni, čeprav jim eksplicitno opozoriš na napako. »Če bi se tako vedel sodelavec, bi prenehal z njim delati,« pravi. Bolj kot napake same ga skrbi sistemska napaka velikih jezikovnih modelov: ti so oblikovani tako, da proizvajajo besedilo, ki *zveni kot* matematični dokaz — ne pa besedilo, ki *je* matematični dokaz. Razlika je ključna. Hamkins se spomni lastne izkušnje iz študentskih let, ko je oddajal naloge, ki so bile tipografsko brezmadežno oblikovane v LaTeXu — a polne napak. Lep videz je zmanjševal kritičnost. Isti učinek, trdi, imajo sodobni jezikovni modeli na matematično razmišljanje.

To ne pomeni, da Hamkins zavrača vsak možni vpliv. Prizna, da nekateri matematiki, ki jim globoko zaupa, trdijo, da jim ti sistemi koristijo — in da morda sam ne zna z njimi dovolj dobro delati. Meni pa, da za pristno matematično odkritje ne zadošča sposobnost generiranja argumentov, ki *so podobni* matematičnim dokazom — potrebno je resnično razumevanje matematičnih objektov.

Hamkins zaključi z optimizmom glede prihodnosti matematike kot discipline: v nasprotju s filozofijo, ki se vrti v večnih krogih okrog istih vprašanj, matematika napreduje. Razumemo neskončnost globlje kot pred sto leti, ta pa globlje kot pred tisoč leti. Matematik čez tisoč let bo verjetno deloval v konceptualnem svetu, ki bi nam danes ostal povsem tuj — tako kot bi bil Arhimed presenečen, a morda ne povsem zgubljen, ko bi mu razložili sodobno matematiko. Ta dolgoročni napredek, in ne morebitna umetna inteligenca, je za Hamkinsa pravi razlog za optimizem.

---

*Joel David Hamkins vodi blog in Substack [Infinitely More](https://infinitelymore.xyz), kjer redno objavlja eseje o teoriji množic, filozofiji matematike in surealnih številih. Podrobnejši pregled njegovih del, vključno s serijo esejev o surealnih številih Johna Conwaya, je dostopen na tej spletni strani.*
