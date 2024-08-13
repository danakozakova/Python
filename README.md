PYTHON 1 - Generovanie náhodných čísel, filtrovanie zoznamu, dictionaries – triedenie a výpis 
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
