# Aš sergu

Paprasta, šviesi programėlė tėvams: ji apskaičiuoja vaikui skirtą vaisto dozę pagal svorį, primena, kada vaistas buvo duotas paskutinį kartą, ir leidžia sekti temperatūrą.

Veikia „iPhone“ ir „Android“ telefonuose kaip įprasta programėlė. Nereikia paskyros, diegimo iš „App Store“ ar „Google Play“. Visi duomenys saugomi tik jūsų telefone.

> **Svarbu.** Programėlė yra skaičiuoklė ir žurnalas, o ne medicininė priemonė. Ji nepakeičia gydytojo, vaistininko ar vaisto lapelio nurodymų. Prieš duodami vaistą patikrinkite dozę, stiprumą ir intervalus pagal lapelį ar gydytojo rekomendacijas.

## Galimybės

- Keli vaikai su vardu ir svoriu, tarp jų galima greitai persijungti.
- Kiekvienam vaistui apskaičiuojama dozė (ml ir mg) pagal svorį.
- Mygtukas „Išgerta“ išsaugo laiką, o kortelėje matyti, kiek laiko praėjo nuo paskutinės dozės.
- Likęs laikas iki kitos galimos dozės.
- Kiek dozių duota per paskutines 24 val. (slenkančios 24 val.).
- Įspėjimas, jei vaistas duodamas per anksti arba viršijama paros riba.
- Įrašų pridėjimas kitu laiku, laiko keitimas ir įrašų trynimas.
- Temperatūros grafikas (24 val., 3 d., 7 d.) su pažymėtais vaistų išgėrimo momentais.
- Duomenų atsarginė kopija ir atkūrimas.

## Kaip naudotis

### 1. Pridėkite vaiką
Pirmą kartą atidarę paspauskite **Pridėti vaiką**, įveskite vardą ir svorį kilogramais. Daugiau vaikų pridedama viršuje mygtuku **+ Vaikas**. Svorį ar vardą pakeisite paspaudę **keisti** šalia vaiko vardo.

### 2. Peržiūrėkite vaistų nustatymus (⚙︎)
Viršuje dešinėje paspauskite krumpliaračio ženklą. Kiekvienam vaistui galima nustatyti:

| Laukas | Reikšmė |
| --- | --- |
| Pavadinimas | Kaip vaistas bus rodomas programėlėje |
| Stiprumas, mg … per ml | Pvz., 200 mg per 5 ml |
| Dozė, mg/kg | Pradinės reikšmės: paracetamolis 15, ibuprofenas 10 |
| Min. intervalas, val. | Per kiek laiko galima duoti kitą dozę |
| Maks. dozių per 24 val. | Didžiausias dozių skaičius per parą |

Minimalus intervalas ir paros riba pradžioje **tušti**. Įveskite juos pagal vaisto lapelį ar gydytojo nurodymus. Kol jie neįvesti, įspėjimų ir laiko iki kitos dozės programėlė nerodo.

Stiprumą visada patikrinkite pagal savo vaisto buteliuką, nes skirtingų gamintojų sirupų koncentracija skiriasi.

Čia galima pridėti ir daugiau vaistų arba pašalinti nereikalingus.

### 3. Dozės skaičiavimas
Dozė apskaičiuojama taip:

```
mg  = svoris (kg) × mg/kg
ml  = mg ÷ stiprumas (mg) × tūris (ml)
```

Pavyzdys: 17 kg vaikui, paracetamolis 15 mg/kg, stiprumas 200 mg per 5 ml → 255 mg = 6,375 ml.

### 4. Vaisto išgėrimas
- **Išgerta** įrašo dabartinį laiką.
- **Kitu laiku** leidžia įrašyti praeityje duotą dozę (pvz., prieš 40 min.).
- Jei dozė duodama per anksti ar viršijama paros riba, programėlė paprašys patvirtinimo.
- Kortelėje matote paskutinės dozės laiką, likusį laiką iki kitos galimos dozės ir dozių skaičių per 24 val.

### 5. Temperatūra
Įveskite temperatūrą ir paspauskite **Įrašyti**. Jei matavote anksčiau, pasirinkite **Įrašyti kitu laiku**. Grafike spalvoti taškai apačioje rodo, kada buvo duoti vaistai. Punktyrinė linija žymi 38 °C.

### 6. Istorija ir taisymas
Apačioje matomi visi įrašai. Paspaudę įrašą galite pakeisti jo laiką (ar temperatūrą) arba jį ištrinti.

### 7. Atsarginė kopija
Nustatymuose (⚙︎) yra mygtukai **Atsisiųsti kopiją** ir **Įkelti kopiją**. Naudokite juos prieš keisdami telefoną, valydami naršyklės duomenis ar norėdami perduoti duomenis kitam telefonui (pvz., žmonai ar vyrui). Kopijos failą galima išsiųsti žinute ar el. paštu. Įkėlus kopiją, dabartiniai duomenys pakeičiami.

## Įdiegimas telefone

Pirmiausia atsidarykite programėlės nuorodą (gausite ją įkėlę failus, žr. žemiau).

**„iPhone“ (būtinai „Safari“ naršyklėje)**
1. Paspauskite **Bendrinti** (kvadratas su rodykle).
2. Slinkite sąrašu žemyn ir pasirinkite **Pridėti prie pradžios ekrano**.
3. Paspauskite **Pridėti**.

**„Android“ („Chrome“)**
1. Paspauskite trijų taškų meniu (⋮).
2. Pasirinkite **Įdiegti programėlę** (arba **Pridėti prie pagrindinio ekrano**).
3. Patvirtinkite.

Kiekvieno telefono duomenys yra atskiri. Programėlė veikia ir be interneto, kai ji jau buvo atidaryta bent kartą.

## Kaip patalpinti „GitHub Pages“ (nemokamai)

Šiam sprendimui nereikia serverio. Tereikia statinių failų talpinimo, kurį nemokamai suteikia „GitHub Pages“.

### Failai
Saugykloje turi būti šie failai, visi pačiame šakniniame aplanke (ne poaplankyje):

- `index.html` – pati programėlė
- `manifest.webmanifest` – programėlės pavadinimas ir nustatymai
- `sw.js` – leidžia veikti be interneto
- `icon-180.png`, `icon-192.png`, `icon-512.png` – piktogramos
- `README.md` – šis aprašymas

### Žingsniai
1. Prisijunkite prie [github.com](https://github.com) arba susikurkite nemokamą paskyrą.
2. Viršuje dešinėje paspauskite **+** → **New repository**.
3. **Repository name:** `as-sergu` (pavadinime negalima tarpų ir lietuviškų raidžių). Pasirinkite **Public** ir paspauskite **Create repository**.
4. Paspauskite nuorodą **uploading an existing file**.
5. Nuvilkite visus failus (ne zip archyvą ir ne aplanką) ir apačioje paspauskite **Commit changes**.
6. Atidarykite **Settings** → **Pages**.
7. Skiltyje **Build and deployment** pasirinkite **Source: Deploy from a branch**, **Branch: main**, aplankas **/ (root)** ir paspauskite **Save**.
8. Po 1–3 minučių puslapio viršuje atsiras nuoroda:
   `https://JUSU-VARDAS.github.io/as-sergu/`
9. Šią nuorodą atsidarykite telefone ir įdiekite (žr. aukščiau). Tą pačią nuorodą galite siųsti draugams ir šeimai.

Jei matote klaidą 404, palaukite kelias minutes ir perkraukite puslapį.

### Atnaujinimas
Saugykloje paspauskite **Add file** → **Upload files**, įkelkite naujus failus tais pačiais pavadinimais ir paspauskite **Commit changes**. Telefone programėlė atsinaujins po kito atidarymo (kartais prireikia ją uždaryti ir atidaryti iš naujo).

## Privatumas

- Programėlė neturi serverio, paskyrų ir sekimo. Duomenys siunčiami niekur.
- Vaikų vardai, svoriai ir įrašai saugomi tik jūsų telefone, naršyklės vietinėje saugykloje.
- Saugykloje (GitHub) matomas tik programėlės kodas, ne jūsų duomenys. Į saugyklą jokių asmeninių duomenų neįkelkite.
- Išvalius naršyklės duomenis arba pašalinus programėlę, įrašai dingsta, todėl reguliariai darykite atsarginę kopiją.

## Atsakomybės apribojimas

Programėlė pateikiama „tokia, kokia yra“, be jokių garantijų. Dozių skaičiavimas pagrįstas jūsų įvestais duomenimis (svoriu, stiprumu ir mg/kg reikšmėmis). Už įvestų reikšmių teisingumą ir vaisto davimą atsakote jūs. Abejodami kreipkitės į gydytoją ar vaistininką. Skubiu atveju skambinkite 112.
