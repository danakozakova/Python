**Python - Dátová analýza**

[PYTHON 01](https://github.com/danakozakova/dana-python/blob/main/PYTH01-Random_Filtering_Dictionary.ipynb) - Generovanie náhodných čísel, filtrovanie zoznamu, dictionaries – triedenie a výpis 
1.	Generovanie náhodných čísel a opakovateľnosť výsledkov pomocou random.seed()
2.	Filtrovanie zoznamu: 
•	for cyklus 
•	"list comprehensions"
•	funkcia filter() s lambda výrazom -	objekt typu filter, "lazy", pri konvertovaní do zoznamu sa spotrebuje
3.	vypisovanie a triedenie dictionary

[PYTHON 02](https://github.com/danakozakova/Python/blob/main/PYTH02-Text-files.ipynb) - Práca s textovými súbormi
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

[PYTHON 03](https://github.com/danakozakova/Python/blob/main/PYTH03-JSON_file.ipynb) - Práca s JSON súborom
1. Načítanie JSON súboru
•  pri načítaní sa automaticky vytvorí premenná typu dict alebo list - podľa toho, koľko objektov obsahuje JSON súbor
2. Príkaz pprint
• na prehľadné zobrazenie obsahu slovníka
• formátuje, odsadzuje, zalamuje riadky
3. Konverzia do pandas.DataFrame
•  ak je jeden objekt (dictionary), zabaliť do listu
• normalizovanie s nastavením separatora na "_", nenechať defaultnú bodku

[PYTHON 04](https://github.com/danakozakova/Python/blob/main/PYTH04-Rest_API.ipynb) - Rest API
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

[PYTHON 05](https://github.com/danakozakova/Python/blob/main/PYTH05-CSV_file.ipynb) - CSV súbory / [PYTHON 06](https://github.com/danakozakova/Python/blob/main/PYTH06-XLXS.ipynb) - Excelovské súbory
1. Načítanie CSV súboru
2. Analýza Dataframu
3. Uloženie do CSV - s alebo bez indexov

[PYTHON 07](https://github.com/danakozakova/Python/blob/main/PYTH07-HTML.ipynb) - Dáta z HTML
1. Stiahnutie dát cez HTTP request
2. Knižnica BeautifulSoup
•  spracovanie requestu
•  spracovanie contentu - dictionary z dát
•  ipywidgets Dropwdown
3. Dočasné súbory
•  knižnica tempfile - vytvorenie / zápis do / výpis z dočasného súboru

[PYTHON 08](https://github.com/danakozakova/Python/blob/main/PYTH08-RDBMS.ipynb) - RDBMS
1. MYSQL DB
- Pripojenie k mysql databáze
- SQL dopyty cez rozšírenie load_ext sql
- overenie DB, dostupné tabuľky
- %%sql na vykonanie viacerých SQL príkazov
- create schema / create table
2. JDBC/ODBC pripojenie
-  getpass na bezpečné zadanie hesla bez zobrazenia na obrazovke
3. ORM s Pandas/SQLAlchemy:
- sqlalchemy a pandas na prácu s databázou objektovo-relačným spôsobom
- create_engine - objekt engine na pripojenie k DB

[PYTHON 09](https://github.com/danakozakova/Python/blob/main/PYTH09-Numpy.ipynb) - Numpy
1. numpy polia
- automatické konverzie
- defaultné polia
2. Výkonnosť
- magická funkcia %timeit
- porovnanie np.array a listu
- použitie funkcie na np.array
3. Numba
  - @jit funkcie
  - výkonnnost numba
 4. Ďalšie operácie s numpy
