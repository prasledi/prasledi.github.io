---
layout: post
title: "Claude in Riemannova hipoteza: napredek, zmote in prihodnost matematike z UI"
date: 2026-09-29
categories: [Matematika, Umetna inteligenca]
tags: [riemannova-hipoteza, claude, anthropic, teorija-stevil, ui-v-matematiki]
image: https://images.unsplash.com/photo-1462331940025-496dfbfc7564?q=80&w=2000&auto=format&fit=crop
---

{% include embed/youtube.html id='kvLOiTxYSzA' %}

## Kazalo {#kazalo}

<div style="background:#f8f9fa;border:1px solid #dee2e6;border-radius:8px;padding:24px 28px;margin-bottom:32px;font-family:Arial,sans-serif;">
  <p style="font-size:1.15em;font-weight:700;margin:0 0 16px 0;color:#212529;border-bottom:2px solid #6c757d;padding-bottom:8px;">📋 Kazalo vsebine</p>
  <ol style="margin:0;padding-left:20px;line-height:2;">
    <li><a href="#prastevila-in-stevna-funkcija" style="color:#0d6efd;text-decoration:none;">Praštevila in števna funkcija</a> — <em>Zakaj so praštevila gradbeni bloki celih števil in kako jih štejemo.</em></li>
    <li><a href="#baslovski-problem-in-riemannova-dzeta" style="color:#0d6efd;text-decoration:none;">Baslov problem in Riemannova dzeta funkcija</a> — <em>Od vsote recipročnih kvadratov do kompleksne razširitve.</em></li>
    <li><a href="#eulerjeva-produktna-formula" style="color:#0d6efd;text-decoration:none;">Eulerjeva produktna formula</a> — <em>Presenetljiva zveza med dzeta funkcijo in praštevili.</em></li>
    <li><a href="#riemannova-hipoteza" style="color:#0d6efd;text-decoration:none;">Riemannova hipoteza</a> — <em>Kaj je kritični trak, kritična premica in zakaj je hipoteza vredna milijon dolarjev.</em></li>
    <li><a href="#zgodovinski-napredek" style="color:#0d6efd;text-decoration:none;">Zgodovinski napredek do Claudea</a> — <em>Od Hardyja leta 1914 do Claudeovega preboja leta 2026.</em></li>
    <li><a href="#kaj-je-claude-dejansko-naredil" style="color:#0d6efd;text-decoration:none;">Kaj je Claude dejansko naredil</a> — <em>Podrobni opis poteka dela z agenti in kako je prišlo do rezultata.</em></li>
    <li><a href="#zmote-in-dezinformacije" style="color:#0d6efd;text-decoration:none;">Zmote in dezinformacije</a> — <em>Zakaj 67 % ni dokaz Riemannove hipoteze in zakaj nikoli ne bo.</em></li>
    <li><a href="#misli-o-prihodnosti-matematike" style="color:#0d6efd;text-decoration:none;">Misli o prihodnosti matematike</a> — <em>Napredek, varovalke, preglednost in vprašanje: kaj sploh pomeni biti matematik?</em></li>
  </ol>
</div>

---

## Praštevila in števna funkcija {#prastevila-in-stevna-funkcija}

Praštevila so vsa cela števila, večja od ena, ki so deljiva le z ena in sama s seboj: 2, 3, 5, 7, 11, 13 in tako naprej. Eden od razlogov, zakaj so matematiki tako navdušeni nad njimi, je ta, da lahko vsako celo število enolično razstavimo na produkt praštevil. Na primer: 60 = 2 × 2 × 3 × 5. Praštevila so torej nekakšni gradbeni bloki celih števil.

Definiramo lahko funkcijo štetja praštevil π(x), ki pove, koliko praštevil je manjših ali enakih x. Na primer, π(10) = 4, ker so praštevila pod 10 ravno 2, 3, 5 in 7. Graf te funkcije ima obliko stopnic — med dvema praštevilo ni porasta, ob vsakem novem praštevilu pa se stopnica dvigne za ena.

Konec 18. stoletja sta Gauss in Legendre ugotovila, da je število praštevil do vrednosti x priblžno x / log(x). Ta ugotovitev se je uveljavila kot izrek o praštevili in bila dokazana leta 1896 (Hadamard in de la Vallée Poussin). Povprečno obnašanje praštevil torej razumemo — a ravno odstopanja od tega povprečja skrivajo globlje matematične resnice.

[⬆️ Nazaj na kazalo](#kazalo){: .back-to-top}

---

## Baslov problem in Riemannova dzeta funkcija {#baslovski-problem-in-riemannova-dzeta}

Stoletje pred Riemannom so matematike zaposloval drug problem. Gre za vsoto recipročnih kvadratov:

$$1/1^2 + 1/2^2 + 1/3^2 + \cdots$$

To je t. i. Baslov problem. Euler je v tridesetih letih 18. stoletja dokazal, da ta vsota konvergira k π²/6 — ena najlepših vsot v vsej matematiki.

Matematiki radi posplošujejo. Namesto kvadriranja vrednosti dvignemo na potenco s in dobimo:

$$\zeta(s) = \sum_{n=1}^{\infty} \frac{1}{n^s}$$

To je Riemannova dzeta funkcija. Da vsota konvergira, mora biti realni del s večji od 1. Baslov problem dobimo nazaj preprosto z vrednostjo s = 2.

Riemann je nato naredil ključni korak: razširil je definicijo dzeta funkcije na kompleksna števila s = σ + ti, pri čemer je σ realni, t pa imaginarni del. Ta razširitev — ki jo imenujemo analitično nadaljevanje — ni poljubna; kompleksna analiza pokaže, da obstaja natanko en način, da jo izvedemo.

[⬆️ Nazaj na kazalo](#kazalo){: .back-to-top}

---

## Eulerjeva produktna formula {#eulerjeva-produktna-formula}

Zakaj sploh govorimo o dzeta funkciji v zvezi s praštevili? Odgovor tiči v Eulerjevi produktni formuli.

Iz teorije geometrijskih vrst vemo, da za |r| < 1 velja:

$$1 + r + r^2 + \cdots = \frac{1}{1-r}$$

Euler je vstavil r = 1/p^s za vsako praštevilo p in nato pomnoži neskončno mnogo takih izrazov med seboj — za vsako praštevilo posebej. Ko razvijemo produkt, dobimo natanko vse recipročne vrednosti celih števil (ker ima vsako celo število enolično praštevično faktorizacijo). Tako dobimo presenetljivo enačbo:

$$\zeta(s) = \prod_{p \text{ praštevilo}} \frac{1}{1 - p^{-s}}$$

Z drugimi besedami: dzeta funkcija kodira informacijo o vseh praštevili. Prek ničel te funkcije lahko razumemo porazdelitev praštevil — in to je bistvo Riemannove hipoteze.

[⬆️ Nazaj na kazalo](#kazalo){: .back-to-top}

---

## Riemannova hipoteza {#riemannova-hipoteza}

Riemann je v svojem slavnem članku iz leta 1859 — le peščica strani, a eden najvplivnejših matematičnih tekstov vseh časov — vprašal: kje ima Riemannova dzeta funkcija ničle, torej pri katerih vrednostih s velja ζ(s) = 0?

Obstajata dve vrsti ničel. Prve so trivialne ničle: pri s = −2, −4, −6, −8, … (negativna soda cela števila). Te matematike manj zanimajo, ker izhajajo iz oblike funkcije in so v nekem smislu predvidljive.

Zanimivejše so netrivialne ničle. Riemann je dokazal, da ležijo vse v t. i. kritičnem traku — področju kompleksne ravnine, kjer je realni del s med 0 in 1. Kaj pa ni dokazal, je bila njegova domneva, da vse netrivialne ničle ležijo na kritični premici, kjer je realni del s natanko 1/2.

**Riemannova hipoteza** trdi ravno to: vsaka netrivialna ničla Riemannove dzeta funkcije leži na kritični premici.

To je eden od sedmih Millenniumskih problemov Clayevega matematičnega inštituta, za katerega je nagrada milijon dolarjev. Zakaj je tako težko? Ker ena sama izjema — ena ničla zunaj kritične premice — bi hipotezo ovrgla, skupaj z vsemi teoremi, ki jo predpostavljajo.

[⬆️ Nazaj na kazalo](#kazalo){: .back-to-top}

---

## Zgodovinski napredek do Claudea {#zgodovinski-napredek}

Ker hipoteze ni mogoče preveriti z enim protiprimerom, so matematiki skušali vsaj določiti, koliko ničel leži na kritični premici.

- **1914 — Hardy** je dokazal, da obstaja neskončno mnogo netrivialnih ničel na kritični premici. Vendar to ne pomeni, da jih ni neskončno mnogo tudi zunaj nje.
- **1942 — Selberg** je dokazal, da pozitivni delež vseh netrivialnih ničel leži na kritični premici — torej ne le neskončno mnogo, ampak merljiv odstotek.
- **1974 — Levinson** je ta delež povzpel na 34,7 %.
- **1989 — Conrey** ga je povzpel na 40,9 %.
- **2022** — nadaljnji napredek do 41,7 %.
- **2026 — Claude (Anthropic)** je ta mejo potisnil na **67,25 %**.

Ob tej objavi je internet nekoliko podivjal — in z njim množica dezinformacij.

[⬆️ Nazaj na kazalo](#kazalo){: .back-to-top}

---

## Kaj je Claude dejansko naredil {#kaj-je-claude-dejansko-naredil}

Anthropic je na Twitterju objavil, da so zaposleni pozvali (takrat še neobjavljeno) različico Claudea, naj se resno loti Riemannove hipoteze. In takoj dodali: hipoteze ni rešil, so pa dosegli napredek pri sorodnem problemu.

Proces je bil naslednji. Zaposleni Jared Sumner — matematik po izobrazbi ni — je Claudea pozval, naj pristopi k hipotezi. V prvi iteraciji je Claude preizkusil 650 idej — nobena ni delovala. V drugi iteraciji pa je Claude preživel dan in pol tako, da je koordiniral okoli 60 pod-agentov: specializiranih podzasebnosti, ki so reševale različne dele problema.

Od teh 60 agentov:
- 2 sta razvila ključne matematične ideje,
- 13 ju je pri tem podpiralo z idejami,
- 30 ni uspelo razviti novih idej,
- 13 je preverjalo pravilnost argumentov,
- 2 sta pomagala pri pisanju članka.

Agenti so skupaj izvedli okoli 2.400 ukazov lupine, napisali stotine Pythonovih skript in porabili 31 milijonov izhodnih žetonov.

Ključni preobrat se je zgodil prek agenta R4, ki je odkril, da ima določena matematična struktura, ki jo je Claude preučeval, negativne smeri (je indefinitna). Claude je to sprva obravnaval kot oviro. Dvanajst ur pozneje pa je spoznal, da bi ravno ta ovira lahko koristila — in poslal agenta E2, naj preveri, ali je mogoče negativne smeri izkoristiti za štetje ničel zunaj kritične premice.

E2 tega ni uspel, je pa odkril obratno: pozitivni del matematičnega objekta je mogoče uporabiti za potrditev ničel *na* kritični premici. Rezultat je bil trditev, da vsaj 50 % ničel leži na kritični premici.

Claude je bil do tega rezultata skeptičen. Poslal je več neodvisnih agentov — »sovražnih recenzentov« — ki so iskali napake. Našli so vrzel v enem od matričnih argumentov, a hkrati tudi popravek. Meja se je potrdila pri 50 %.

Nato je Claude poiskal pot do 2/3. Optimizacija matematičnega okna je prinesla le skok na 50,66 %. Drugi pristop z višjimi momenti je naletel na matematično steno. Rešitev je znova prinesel E2 — prek novega agenta E2-pari, ki je dokazal, da vsaj 2/3 ničel leži na kritični premici. (Zanimiv stranski detajl: agent je dokaz zapisal na disk, nato pa se je sesul zaradi infrastrukturne napake. Koordinator je našel nedokončan dokaz, ga pregledal vrstico po vrstico in agenta obnovil.)

Zadnja izboljšava je mejo potisnila na **67,25 %**. Ko je Claude menil, da ima rezultat, je druge agente poslal po protiprimer, jih prosil za neodvisno reprodiciranje argumentov in naložil 54 člankov z arhiva, da bi preveril, ali je bil rezultat že znan.

Claude je nato predlagal, da se rezultat napiše kot članek, in izrecno priporočil, da ga pregleda človeški teoretik števil. Dva matematika iz Anthropica sta rezultat preverila in potrdila, prav tako pa sta ga na kratko pregledala Brian Conrey in Dan Goldston. Hkrati je Claude skupaj z Ericem Easleyjem pripravil formalizacijo dokaza v programskem jeziku Lean — orodju, ki vsak logični korak preveri računalniško.

**Pomembno:** članek do danes ni bil recenziran v standardnem matematičnem postopku.

[⬆️ Nazaj na kazalo](#kazalo){: .back-to-top}

---

## Zmote in dezinformacije {#zmote-in-dezinformacije}

Na spletu se je hitro razširila vrsta napačnih trditev. Najpogostejše:

1. **»Claude je dokazal Riemannovo hipotezo.«** — Ni je. Anthropic je to takoj pojasnil. Claude sam je med delom večkrat poudaril, da rezultat o pozitivnem deležu ničel na kritični premici ne pove ničesar — niti za, niti proti — o Riemannovi hipotezi.

2. **»Samo povečajmo računsko moč in bomo prišli do 100 % — in s tem dokazali hipotezo.«** — Napačno iz dveh razlogov. Prvič, Anthropic je sam povedal, da obstajajo omejitve, kako daleč je ta mejo mogoče potisniti. Drugič, in to je bistveno: **tudi 100 % ne bi dokazalo Riemannove hipoteze.**

Zakaj? Ponazoritev: med celimi števili je asimptotično 100 % takih, ki niso popolni kvadrati (ker je popolnih kvadratov do n le okoli √n, torej njihov delež → 0). A to seveda ne pomeni, da ni neskončno popolnih kvadratov. Prav tako bi lahko imela Riemannova dzeta funkcija redke ničle zunaj kritične premice — morda celo neskončno mnogo — ki bi jih kljub temu v primerjavi z vsemi ničlami bilo zanemarljivo malo.

Pozitiven delež ničel na kritični premici in dokaz, da so *vse* ničle tam, sta torej temeljno različni izjavi.

[⬆️ Nazaj na kazalo](#kazalo){: .back-to-top}

---

## Misli o prihodnosti matematike {#misli-o-prihodnosti-matematike}

**Napredek je neizpodbiten.** Pred petimi leti smo od umetne inteligence pričakovali odgovore na specifična vprašanja. Danes imamo dobro organizirane ekipe pod-agentov, ki avtonomno izvajajo matematične raziskave. To je neposredniku podobno kot akademska raziskovalna skupina.

**Varovalke so nujne.** Če si zamislimo, da bi zlonamerni akter imel dostop do takšnega sistema, je mogoče ugotoviti, kakšno škodo bi lahko povzročil. Anthropic je nedavno objavil poročilo o zlorabah umetne inteligence — in to bi morale početi vse AI-podjetja. Pritisk javnosti na te korporacije, da omejijo zlorabljanje, je nujen.

**Matematika ni le dokazovanje.** Nekateri matematiki opozarjajo, da umetna inteligenca postaja merilo za dosežke v matematiki, kar odvrača pozornost od tega, čemur je matematika zares namenjena. Ko sistemi UI producirajo stotine strani dokazov, matematična skupnost ne utegne vsega prebrati in preveriti — preden že prispe naslednji rezultat. Terence Tao opominja, da matematika ni le o čim hitrejšem produciranju pravilnih dokazov, temveč tudi o razvijanju novih idej, razumevanju rezultatov, razlaganju, povezovanju področij in prenašanju znanja na naslednje generacije.

**Preglednost je ključna.** Anthropic je bil pri tej objavi izjemno pregleden: takoj so razložili, kaj so poskušali, česa niso dosegli, in objavili celotne zapise dela. To je v ostrem nasprotju z nekaterimi drugimi primeri v industriji, kjer so bila ključna matematična izhodišča omenjena šele po pritisku javnosti. Kadar gre za tako disruptivno tehnologijo, mora skupnost vedeti, kaj točno je bilo narejeno in kako.

**Kaj sploh pomeni biti matematik?** To je morda najpomembnejše vprašanje. Matematik ni le tisti, ki prvi pride do odgovora — je tisti, ki razume, kaj odgovor pomeni, kako se umešča v obstoječe znanje in kako to znanje predati naprej. Če UI olajša produciranje dokazov, postanejo ti drugi vidiki le še bolj dragoceni.

Gre za vznemirljiv, malce tesnobno razburljiv čas. Prihodnost matematike je odprta — in verjetno je pametno, da jo oblikujemo skupaj: matematiki, inženinji in vsi, ki jim ni vseeno.

[⬆️ Nazaj na kazalo](#kazalo){: .back-to-top}

---
