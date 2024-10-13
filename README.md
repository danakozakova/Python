[PYTHON 1](https://github.com/danakozakova/dana-python/blob/main/PYTH1-Random_Filtering_Dictionary.ipynb) - Generovanie náhodných čísel, filtrovanie zoznamu, dictionaries – triedenie a výpis 
1.	Generovanie náhodných čísel a opakovateľnosť výsledkov pomocou random.seed()
2.	Filtrovanie zoznamu: 
•	for cyklus 
•	"list comprehensions"
•	funkcia filter() s lambda výrazom -	objekt typu filter, "lazy", pri konvertovaní do zoznamu sa spotrebuje
3.	vypisovanie a triedenie dictionary

PYTHON 2 - Práca s textovými súbormi
1. Otvorenie a zatvorenie súboru
2. Prečítanie a spracovanie obsahu textového súboru:
• spracovanie riadkov vo for cykle
• line.split() vráti zoznam slov
• počet slov ako veľkosť listu
3. Frekvencia slov v textovom súbore:
• cez klasický dictionary s podmieneným pripočítavaním v cykle
• s použitím defaultdict, ktorý automaticky inializuje nové kľúče
- s použitím slovníka Counter, textový reťazec ako parameter pri inicializácii, so šikovnou funkciou most_common()

Zoptimalizovanie výsledkov pre veľké / malé písmená.
Zobrazenie frekvencie v histograme cez plotly.express

PYTHON 3 - Práca s JSON súborom
1. Načítanie JSON súboru
•  pri načítaní sa automaticky vytvorí premenná typu dict alebo list - podľa toho, koľko objektov obsahuje JSON súbor
2. Príkaz pprint
• na prehľadné zobrazenie obsahu slovníka
• formátuje, odsadzuje, zalamuje riadky
3. Konverzia do pandas.DataFrame
•  ak je jeden objekt (dictionary), zabaliť do listu
• normalizovanie s nastavením separatora na "_", nenechať defaultnú bodku

PYTHON 4 - Rest API
1. Získanie dát z REST API
•  knižnica requests: Funkcia requests.get() odošle HTTP GET požiadavku na zadanú URL adresu a vráti nám odpoveď zo servera.
•  Odpoveď obsahuje:
    Stavový kód (status_code): kód 200 je OK, 404 error...
    Hlavičky (headers): Obsahujú metadáta o odpovedi, ako napríklad typ obsahu alebo kódovanie.
    Obsah (content): samotné dáta, ktoré server vrátil. Často sú vo formáte JSON.
Ak je všetko v poriadku (status_code == 200), môžeme obsah odpovede (JSON súbor) previesť na slovník alebo zoznam pomocou metódy response.json(). Typ premennej - slovník alebo zoznam - sa nastaví automaticky, v závislosti od dát.
2. Príkazy pprint a pd.json_normalize() 🛠️
•  pprint: Ak chceme obsah JSON dát zobraziť prehľadne a čitateľne, môžeme použiť príkaz pprint z modulu pprint.
•  pd.json_normalize(): pd.json_normalize() nám pomôže rozbaliť vnorené štruktúry v JSON dátach a vytvoriť z nich DataFrame, nastaviť separátor
3. Výber údajov z listu / dataframu🎯
•  For cyklus pre list
•  Boolean indexing: Efektívnejší pre dataframe
•  Metóda query(): výhodnejšie pre zložitejšie podmienky výberu

PYTHON 5 - CSV súbory / PYTHON 6 - Excelovské súbory
1. Načítanie CSV súboru
2. Analýza Dataframu
3. Uloženie do CSV - s alebo bez indexov

PYTHON 7 - Dáta z HTML
1. Stiahnutie dát cez HTTP request
2. Knižnica BeautifulSoup
•  spracovanie requestu
•  spracovanie contentu - dictionary z dát
•  ipywidgets Dropwdown
3. Dočasné súbory
•  knižnica tempfile - vytvorenie / zápis do / výpis z dočasného súboru

