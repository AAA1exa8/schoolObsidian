## Zvuková zařízení PC
- dříve malý reproduktor zvaný speaker
- zvukové schopnosti velmi omezené
- kvalitní zvuk přineslo až rozšíření o zvukovou kartu

### Funkce zvukové karty
- digitální zpracování zvuku
- nahrávání (mikrofon)
- reprodukce (sluchátka reproduktory)
- tvorba (editace zvuku) - soubory MID
- digitalizace zvuku - vstup Line In - D/A převodník

### Typy zvukových karet
- běžné/profesionální
- integrované na MB (čip -audiocodec)
- rozšiřující karta do sběrnice (PCI, PCIexpress 1x)
- externí karta přes rozhrání (FireWire, USB)

### Integrované vs. externí
- ##### integrované
- nahovno
- nižší výkon
- levnější

- ##### externí
- dobrý
- dražší
- sloty na základní desce


### Kvalitativní parametry zvukového signálu

#### odstup signál//šum
- decibely (db)
- rozdíl mezi užitečným signálem a hladinou šumu
#### přeslechy
- decibely (db)
- slyšitelné zvuky, které jsou nežádoucí ("prolezou" do výstupu)
#### dynamický rozsah
- decibely(db)
- maximální rozdíl mezi nejišší a nejhlasitější padáží bez skreslení výstupního signálu
- běžný rozsah je 92 db a šířka záznamu 16 bitů
- hodnota je ovlivněna šířkou záznamu a přesností vstupního signálu
#### latence
- milisekundy (ms)
- zpoždění mezi vstupem signálu, zpracováním signálů, a jeho výstupem na další konektor
- ovlivněna velikostí bufferu
  - vyrovnávací paměť mezi D/A převodníkem a procesorem počítače
- max. 10 ms
#### zpracovávání zvuku
- zvuková karta sama o sobě nedokáže zaznamenat **analogový** signál
- analogový zvuk musí být převeden do jedniček a nul, které popisují průběh **digitálního** zvukového signálu
#### Shannonova vzorkovací věta
- libovolný periodický signál lze digitalizovat bez ztráty informace, jestliže **je frekvence vzorkování** alespoň dvojnásobná, než nejvyšší frekvence obsažená v signálu.
- čím vyšší tato frekvence je, tím je převod zvuku věrnější
- normální zvuk - 44.1 kHz (VD kvalita)
  profesionální - 96 kHz a 192 kHz
#### Šířka záznamu (kvantizace)
- kvalita výsledného zvuku ovlivňuje přesnost snímání analogového signálu
- určuje se v počtech bytů
- běžné digitální audio přesnost na 16 bitů
- kvalitnější záznam - 24 bitů
#### zpracovávání zvuku
- telefoní kvalita - 11 kHz, 8 bit, mono, 11 kB/s
- rádiová kvalita - 22 kHz, 8-bit, mono, 22 kB/S
- CD kvalita - 44,1 kHz, 16-bit, stereo, 172 kB/s


### Formát WAV
- bezkompresní a bezztrátový
- výhoda: velice dobrá výstupní kvalita
- nevýhoda: velikost (1 hodina = cca. 600 MB)
- záleží na použítém vzorkování a šíře záznamu
- standart pro všechny audio zařízení (CD audio)  44,1 kHz a 16-bit

### Formát MP3
- MP3 (MPEG Audio Layer 3)
- výhoda: zmenšení velikosti výstupního souboru
- MP3 kodér odstraňuje z původního signálu frekvence které jsou vyhodnoceny jako nepotřebné - ty které běžné ucho nepozná
- na obou stereo kanálech je často stejný signál, Joint Stereo informaci odstraní a vytvoří monofoní signál
- něktré kodéry podporují takzvaný variabilní bitrate (VBR) tišší a klidnější pasáže jsou zaznamenávány s nižším bitrate a dynamické s vyšším

### Formát AAC
- AAC (MPEG-4 Advance Audio Coding)
- Podobné metody jako u MP3
- Použitých v zařízení společnosti apple

### Formát OGG
- OGG vorbis
- kvalitnější zvuk oproti MP3
- vyvýjen jako opensource

### Formát WMA
- windows media audio
- vyvýjený a prosaovaný firmou microshit

### Formát MIDI
-  Musical Instrument Digital Interface
- standart pro komunikaci mezi hudebními nástroji a počítači
- soubot MID - stručný digitální popis frekvence jednotlivých tónů, jejich intenzity, délky a nejrůznějších efektů
- soubory MID tedy neobsahují žádný signál ale stručné pokyny pro jejich vytvoření
  - existují dva základní postupy, jak dostat z MIDI souboru požadovaný výstup
  - méně kvalitní **FM syntéza**, což je vlastně jakýsi soubor matematických rovnic na základě kterých se vypočítává přibližný zvukový průběh konkrétních nástrojů.
  - Výstup je tedy velmi snadno rozpoznatelný od skutečných živých nahrávek.
  - **Wavetable syntéza** - funguje na principu jakési audiobanky, tedy pro každý nástroj je ve zvukové kartě (na disku, CD...) uložen kokrétní krátký zvukový záznam, tzv. sample skutečného hudebního nástroje. Z těchto samplů se pak na základě MIDI předpisu sestavý výseldná skladba