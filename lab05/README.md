# Uvod v Kali Linux

Na tej vaji boste spoznali okolje **Kali Linux**, ki je standardno orodje za testiranje varnosti in etični hacking. Seznanili se boste z namenom uporabe Kali Linuxa, njegovimi glavnimi orodji in osnovnimi koncepti, ki jih mora poznati vsak varnostni strokovnjak.

# 🧪 Uvod v Kali Linux

Kali Linux je specializirana distribucija Linuxa, ki jo uporabljajo varnostni strokovnjaki za izvajanje preizkusov vdorov, analiz omrežij, forenzične analize in drugih varnostnih nalog. Vsebuje več kot 600 prednameščenih orodij.  
Poznavanje okolja Kali Linux je pomembno, saj omogoča izvajanje simulacij napadov in odkrivanje ranljivosti, še preden jih izkoristijo napadalci.

---

## 1️⃣ Uvod

Cilj je, da se kot uporabniki naučimo kako:  
✅ razumeti namen in vlogo Kali Linuxa v kibernetski varnosti  
✅ se znajti v osnovnem grafičnem in ukaznem okolju Kali Linuxa  
✅ najti in zagnati nekaj ključnih orodij  
✅ izvesti osnovne ukaze in analizirati rezultate

---

## 2️⃣ Aktivnost

### 🖥️ Navodila

Študenti boste izvedli naslednje korake in dokumentirali rezultate:

---

#### 1️⃣ Kaj je Kali Linux?
- Preberite osnovne informacije o Kali Linuxu na: [https://www.kali.org](https://www.kali.org)
- Zapišite, kdo razvija Kali Linux in za kakšne namene je namenjen.
- Naštejte 3 področja uporabe Kali Linuxa (npr. penetration testing, digital forensics …).

---

#### 2️⃣ Zagon okolja Kali Linux
- Zaženite virtualni stroj z **Kali Linuxom** ali uporabite pripravljeno učilniško namestitev.
- Raziskujte grafično okolje (meniji, sistemske informacije).
- Poiščite meni z varnostnimi orodji in naštejte 5 orodij, ki jih najdete.

---

#### 3️⃣ Preverjanje sistema in osnovni ukazi
Odprite **terminal** in izvedite naslednje ukaze ter zapišite rezultate.

| Ukaz                     | Pomen |
|--------------------------|-------|
| `whoami`                 | Prikaže prijavljenega uporabnika |
| `hostnamectl`            | Pokaže ime gostitelja in OS |
| `uname -a`               | Pokaže podatke o jedru |
| `df -h`                  | Prikaže zasedenost diska |
| `ip a`                   | Pokaže mrežne nastavitve |

Primer:
```bash
whoami
hostnamectl
uname -a
df -h
ip a
```

4️⃣ Preverjanje orodij v terminalu

```bash
which nmap
which john
which hydra
which sqlmap
which nikto
```

### 📝 Analiza in poročilo

Oddajte poročilo z naslednjimi vsebinami:
- Kratek opis Kali Linuxa in njegovih področij uporabe
- Izpisi zgoraj navedenih ukazov
- Seznam 5 orodij iz menija in 5 orodij iz terminala
- Komentar: kaj vas je presenetilo pri okolju Kali Linux?

⸻

## 3️⃣ Refleksija in analiza
	•	Zakaj je pomembno izvajati preizkuse varnosti v varnem okolju?
	•	Katere funkcionalnosti Kali Linuxa so vas najbolj pritegnile?
	•	Kako bi v prihodnje uporabili to znanje v praksi?