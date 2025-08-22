# 🐧 Uvod v Linux: osnove dela v ukazni lupini

## 🎯 Cilj
Naučiti se osnovnega dela z ukazno vrstico v Linux okolju. Po tej vaji bomo spoznali kako:  
- krmariti po imenikih,
- pregledovati vsebine,
- ustvarjati in brisati datoteke,
- preveriti velikost in pravice.

✅ se povežemo na Linux strežnik preko ssh  
✅ pregledamo imenike, ustvarimo imenike in datoteke  
✅ izvajamo osnovne ukaze v Linuxu  

---

## ⚙️ Priprava okolja

Za to vajo bomo uporabili [GitHub Codespaces](https://github.com/features/codespaces)

Zaželjeno je, da si za potrebe vaj do naslednjič pripravite svoje okolje bodisi:
- znotraj virtualega okolja (VMWare, VirtualBox ipd.)
- Windows Subsystem for Linux (WSL)
- Microsoft Azure ali druga oblačna storitev
- obstoječe okolje v kolikor uporabljate Linux OS/Max OS X/BSD ipd. 

Priporočeno je, da si namestite distribucijo Kali Linux, ki že vključuje vsa orodja, ki jih bomo uporabljali.

---

## 🧪 Ustvarjanje Github Codespace okolja:

1. Na povezavi [GitHub Codespaces](https://github.com/features/codespaces) izberemo opcijo "Get  started for free"
2. Na levi strani ali preko hitrega dostopa izberemo opcijo "Blank"
3. Github Codespaces bo za nas ustvaril spletno okolje preko katerega lahko dostopamo do ukazne vrstice. 

Privzeto Github Codespaces ne omogoča dostopa preko SSH, zato bomo uporabili trik in si uredili dostop preko SSH. Za produkcijsko reštitev tovorsten pristop odsvetujem, uporabite raje gh cli. Nadlednji del služi zgolj kot demonstracija. 

Najprej ustvarimo uporabnika s katerim bomo delali, da ne uporabljamo prizetega uporabnika.

```bash
whoami # preverimo trenutnega uporabnika
sudo adduser user # user je vaše željeno uporabniško ime, čarovnik nas bo vprašal po geslu in podatkih uporabnika, kar potrdimo. Pozor: geslo se ne vidi, ko se vpisuje.
sudo usermod -aG sudo user
sudo visudo
```

Dodamo naslednji zapis pod # User privilege specification
```bash
user ALL=(ALL:ALL) ALL
```

Sedaj zaženemo SSH storitev
```bash
sudo service ssh start # zagon storitve ssh
sudo apt update # posodobimo seznam paketov
sudo apt install tmate # namestimo paket tmate
tmate # zaženemo tmate
```

Izpiše se nam podatek za povezavo na ssh preko posebne seje. S Ctrl + C prekinemo izpis in dobimo dostop do uporabe ukazne vrstice.

## 🧪 Povezava na strežnik

Na strežnik se lahko prijavimo iz obsoječe lupine. 
```bash
su - user # preklopimo na uporabnika, ki smo ga ustvarili in vpišemo geslo
```

## 🧪 Vaja: Osnovni ukazi

### 1️⃣ Krmarjenje po sistemu
```bash
pwd           # prikaže trenutno pot
ls            # prikaže vsebino imenika
ls -l         # prikaže vsebino s podrobnostmi
cd /pot/do/imenika  # spremeni imenik
cd ..         # premik na nadrejeni imenik
```

✅ **Naloga:**  
- Premaknite se v domači imenik.
- Ustvarite imenik `linux-vaja`.
- Vstopite vanj.

---

### 2️⃣ Delo z datotekami in imeniki
```bash
mkdir novaMapa         # ustvari nov imenik
touch datoteka.txt     # ustvari prazno datoteko
nano datoteka.txt      # urejanje vsebine (ali `vim` / `code`)
cat datoteka.txt       # izpiše vsebino
rm datoteka.txt        # izbriše datoteko
rm -r novaMapa         # izbriše imenik z vsebino
```

✅ **Naloga:**
- Ustvarite datoteko `opis.txt` in vanjo zapiši svoje ime.
- Ustvarite imenik `testni`.
- Premaknite `opis.txt` v `testni`.

---

### 3️⃣ Premikanje in kopiranje
```bash
mv dat.txt druga.txt      # preimenuje datoteko
cp file1.txt file2.txt    # kopira datoteko
mv file.txt /pot/do/drugamape/  # premik
```

✅ **Naloga:**
- Preimenujte `opis.txt` v `moj_profil.txt`.
- Kopirajte `moj_profil.txt` v domačo mapo.

---

### 4️⃣ Pravice in velikosti
```bash
ls -lh          # velikost in pravice
du -sh ./*      # velikost datotek/imenikov
chmod 644 file  # spremeni pravice
```

✅ **Naloga:**
- Preverite velikost vseh datotek v mapi.
- Spremenite pravice datoteki `moj_profil.txt` tako, da je samo za branje za vse.

---

### 5️⃣ Prikaz sistemskih informacij
```bash
whoami           # tvoje uporabniško ime
uname -a         # podatki o sistemu
df -h            # poraba diska
top              # aktivni procesi
```

✅ **Naloga:**
- Ugotovite ime svojega uporabnika in velikost domačega imenika.
- Preverite, koliko prostora je na voljo v sistemu.

---

## 💡 Dodatna naloga
Poiščite največjo datoteko v svojem domačem imeniku:

```bash
du -ah ~ | sort -rh | head -n 5
```


## Reference

1. Reddit, SSH into Codespace without GitHub CLI, https://www.reddit.com/r/github/comments/15pvnj3/comment/kd23ess/

2. OpenAI, (2025), *ChatGPT* (Aug 2025) [Large language model], https://chat.openai.com/
