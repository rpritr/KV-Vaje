# OSINT – zbiranje informacij o posameznikih na spletu

📅 **Trajanje: 2 uri**

Odprti viri (OSINT) so viri informacij, ki so javno dostopni: spletne strani, družbena omrežja, forumi, iskalniki … Ta vaja študentom pokaže, kako se lahko tudi povprečen uporabnik interneta dokoplje do osebnih informacij druge osebe, če te niso ustrezno zaščitene.


# 🧪 Osnovno o OSINT

OSINT (ang. Open Source Intelligence, slovensko: obveščevalni podatki iz odprtih virov) označuje tehnike zbiranja in analize informacij, ki so dostopne javno, prek odprtih, zakonitih virov.

OSINT temelji na načelu, da je na spletu in drugih javnih medijih mogoče najti ogromno podatkov, ki jih lahko uporabimo za različne namene – od kibernetske varnosti, etičnega hekanja, do novinarstva, raziskav in varnostnih preiskav.

## 1️⃣ Uvod: Zbiranje informacij o posameznikih na spletu

Cilji vaje so: 
✅ Spoznati tehnike OSINT za zbiranje javno dostopnih informacij o posameznikih.   
✅ Zavedanje, koliko osebnih podatkov je mogoče najti na spletu.   
✅ Razprava o tem, kako se zaščititi pred preveliko izpostavljenostjo.   

### Varnost zgoščenih vrednosti

Zgoščevanje (hashing) je enosmerni matematični postopek, ki iz poljubno dolgega niza podatkov izračuna fiksno dolgo »prstno odtisno« vrednost (hash). V informacijskih sistemih se uporablja predvsem za shranjevanje preverjanj gesel, saj strežnik ne shranjuje dejanskih gesel, temveč njihove zgoščene vrednosti. Ko uporabnik vnese geslo, sistem izračuna njegov hash in ga primerja s shranjenim.

Čeprav je zgoščevanje pomemben varnostni mehanizem, pa samo po sebi ne preprečuje napadov. Napadalci lahko s slovarskimi ali brutalnimi napadi ugibajo gesla in izračunavajo njihove hash-e, dokler ne najdejo ujemanja. Zato so ključni dodatni ukrepi, kot so uporaba dolgih in kompleksnih gesel, uporaba »soli« (salt), ki prepreči uporabo vnaprej pripravljenih tabel (rainbow tables), ter počasnejši algoritmi (npr. bcrypt, scrypt ali Argon2), ki otežijo množično računanje hash-ov.

Pomembno je torej razumeti, da varnost gesla ne zagotavlja le zgoščevanje, ampak kombinacija varnostnih praks: močna gesla, dodajanje soli in uporaba primernih algoritmov.


## 2️⃣ Aktivnost: OSINT - Zbiranje informacij o posamezniku

Izberite javno osebo (npr. znanega novinarja, politika, športnika) ali fiktivno osebo z vnaprej pripravljenimi podatki za vadbo (priporoča se uporaba anonimiziranih podatkov za spoštovanje zasebnosti).

### 🖥️ Sherlock

🔷 1️⃣ Priprava okolja

Sherlock je orodje, ki teče na Linux/MacOS/Windows z nameščenim Pythonom.

✅ Če delate v Linux okolju (npr. Kali), Sherlock je že pogosto nameščen ali ga namestite:

```bash
git clone https://github.com/sherlock-project/sherlock.git
cd sherlock
pip3 install -r requirements.txt
```

Zaženete Sherlock:

```bash
python3 sherlock <username>
```

### 🖥️ Maigret

🔷 2️⃣ Alternativa oz. dopolnitev Sherlocku

Maigret je podobno OSINT orodje za iskanje uporabniških imen, vendar preveri še širši nabor spletnih mest in pogosto ponuja preglednejše poročilo.

✅ Namestitev Maigret (če še ni nameščen):
```bash
pip install maigret
```
ali iz izvorne kode:

```bash
git clone https://github.com/soxoj/maigret.git
cd maigret
pip install -r requirements.txt
```

Zagon Maigret: 

```bash
maigret <username>

```

🔷 Primerjalna opažanja
Uporabite oba programa za isto uporabniško ime.

Primerjajte rezultate: katero orodje je našlo več profilov? Katero je dalo bolj pregledne podatke?

Razmislite: ali sta se našla profila na družbenih omrežjih, kjer tega niste pričakovali?

### 📝 Analiza in poročilo

- Primerjajte rezultate Sherlocka in Maigreta. Katere razlike ste opazili? Katerega bi priporočili za podobne naloge in zakaj?
- Ali ste našli kakšno občutljivo informacijo (npr. e‑poštni naslov, zasebne slike, telefonsko številko)? Kako bi jo lahko oseba zaščitila pred tem, da je javno dostopna?

## 3️⃣ Refleksija in analiza

- Katere informacije so bile najlažje najdene? Katere je bilo najtežje najti?
- Kako bi vi sami prilagodili svoje vedenje na spletu, potem ko ste izvedli to vajo?
- Ali menite, da je uporaba OSINT orodij etično sporna? V katerih primerih je upravičena?