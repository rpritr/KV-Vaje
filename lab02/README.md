# Varnost posameznikov v kibernetskem prostoru

Kibernetski prostor uporabljamo vsakodnevno. Primer uporabe kibernetskega prostora je komunikacija, nakupovanje, bančništvo, pa tudi delo in zabava. Posamezniki smo uporabniki kibernetskega prostora, hkrati pa tudi tarče in se pogosto ne zavedamo vseh nevarnosti in posledic svojih dejanj.

Cilj vaj pri predmetu Varnost posameznikov v kibernetskem prostoru je študentom približati ključne pojme kibernetske varnosti z vidika posameznika, razviti občutek za tveganja in ranljivosti ter jih opremiti z osnovnimi znanji za varnejšo uporabo sodobnih tehnologij.

# 🧪 Spoznajmo kibernetski prostor

Prva vaja je namenjena uvodu v kibernetsko varnost ter spoznavanju osnovnih pojmov in izzivov:

- Kdo ali kaj je posameznik v kibernetskem prostoru?
- Kaj pomeni pojem kibernetski prostor in kako ga zaznavamo?
- Kaj razumemo pod pojmom kibernetska varnost?

## 1️⃣ Uvod: Analiza osebne izpostavljenosti v kibernetskem prostoru

Cilji vaje:  
✅ Spoznati osnovne pojme: posameznik, kibernetski prostor, kibernetska varnost, zasebnost.  
✅ Prepoznati osebne podatke in kako so dostopni v spletnem okolju.  
✅ Razumeti, kako sodobne tehnologije vplivajo na varnost in zasebnost posameznika.  

### Varnost in zasebnost

Posameznik v kibernetskem prostoru je vsak uporabnik tehnologij in naprav, ki so povezane v omrežje ter uporabljajo storitve interneta.

Varnost:
Varnost (kibernetska varnost) obsega varovanje IKT sistemov, omrežij in podatkov pred nepooblaščenim dostopom, napadi, okvarami ali zlorabo. Namen je zagotavljanje zaupnosti, celovitosti in dostopnosti podatkov ter storitev.
Primer: preprečiti vdor v uporabnikov e-poštni račun.

Zasebnost:
Zasebnost se dotika pravice osebe, da ima nadzor nad svojimi osebnimi podatki ter načinom, kako se ti zbirajo, uporabljajo, razkrivajo ali shranjujejo. Gre za to, koliko podatkov o sebi želi oseba odpreti in komu.
Primer: pravica, da spletna platforma brez soglasja ne deli uporabnikovih podatkov z oglaševalci.

## 2️⃣ Aktivnost: Analiza osebne izpostavljenosti

V brskalniku odprite način incognito/private in poiščite informacije o sebi (npr. preko iskalnikov in storitev za preverjanje izpostavljenosti):
- Poiščite svoje ime in priimek v Googlu.
- Preverite morebitne javne profile (Facebook, LinkedIn, Instagram, forumi).
- Uporabite orodja za preverjanje izpostavljenosti (HaveIBeenPwned, OSINTLeak)
- Orodja: PimEyes, haveibeenpwned, OSINTLeak

### Google dorking/hacking

Google Dorking (znan tudi kot Google Hacking) je metoda, ki izkorišča napredne iskalne operaterje v Googlu (ali drugih iskalnikih), da pridobimo podatke, ki niso mišljeni za javnost, a so še vedno dosegljivi na spletu.

Gre za izkoriščanje napačno nastavljene spletne strani, strežnikov ali aplikacij, kjer so datoteke, dokumenti ali celo gesla dostopni javnosti, a skriti pred navadnimi uporabniki.

Google Dorking sicer ni nezakonit, dokler ne posegamo v zaščitene sisteme. Vendar pa najdenih informacij ne smemo zlorabiti, shranjevati brez dovoljenja ali javno razkrivati.


### 📘 Primeri Google Dork iskalnih poizvedb

| Iskalna poizvedba                       | Kaj najde?                                        |
|----------------------------------------|---------------------------------------------------|
| `filetype:pdf site:gov.si`             | PDF dokumenti na slovenskih vladnih straneh       |
| `intitle:"index of" passwords`         | Mape z imenom "index of" in datotekami z gesli    |
| `inurl:admin login`                    | Strani z možnostjo prijave v administracijo       |
| `site:pastebin.com password`           | Objave z gesli na Pastebin                        |
| `"confidential" filetype:pdf`          | Dokumenti z oznako "confidential" v PDF obliki    |
| `ext:sql intext:"password"`            | Javne SQL datoteke, ki vsebujejo gesla            |
| `intitle:"webcamXP 5"`                 | Nezaščiteni vmesniki IP kamer                     |
| `inurl:/phpinfo.php`                   | Javne PHP konfiguracijske datoteke                |
| `filetype:env intext:DB_PASSWORD`      | Javne `.env` datoteke z gesli do baz              |
| `site:*.* inurl:/config.json`          | Javne konfiguracijske datoteke aplikacij          |


## 3️⃣ Refleksija in analiza

- Razmislite in zapišite katere podatke ste našli.
- Kakšno potencialno tveganje predstavljajo?
- Zapišite primer črnega scenarija kako bi nekomu ti podatki lahko prišli prav na primeru osebne izpostavljenosti.
- Kako bi ocenili svojo osebno varnost/zasebnost?

## Reference

1. PimEyes., *Face recognition search engine*, https://pimeyes.com/  
2. Have I Been Pwned, *Data breach search and notification service*, https://haveibeenpwned.com/  
3. OSINT Framework, *OSINT tools and resources collection*,https://osintframework.com/  
4. OpenAI, (2025), *ChatGPT* (Aug 2025) [Large language model], https://chat.openai.com/
