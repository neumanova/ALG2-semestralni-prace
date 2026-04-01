# Movie Watchlist and Rating Tracker

## Motivace
Toto téma jsem si vybrala, protože filmy jsou mi blízké a často si chci ukládat, co chci vidět nebo co jsem již viděla. Zároveň jsem chtěla vytvořit aplikaci, která bude praktická a využitelná v běžném životě. Cílem je mít přehledný seznam filmů a možnost si je organizovat podle vlastních potřeb.

## Popis aplikace
Semestrální práce je zaměřena na vytvoření konzolové aplikace v jazyce Java, která slouží k evidenci filmů. Aplikace umožní uživateli ukládat filmy, které chce zhlédnout, i filmy, které již viděl. Každý film bude obsahovat základní informace, jako je název, žánr, rok vydání, stav (zhlédnutý / nezhlédnutý) a případně uživatelské hodnocení.

Uživatel bude moci do aplikace přidávat nové filmy, zobrazovat jejich seznam a upravovat jejich stav. Program umožní označit film jako zhlédnutý, přidat hodnocení a zobrazit pouze vybrané skupiny filmů, například jen zhlédnuté nebo jen nezhlédnuté. Dále bude možné filmy filtrovat podle žánru nebo jiných parametrů.

Součástí aplikace bude také třídění filmů, například podle názvu, roku vydání nebo hodnocení. Díky tomu bude možné se v seznamu snadno orientovat. Data budou ukládána do souboru, aby bylo možné je při dalším spuštění programu znovu načíst.

Cílem aplikace je vytvořit jednoduchý a přehledný nástroj pro správu seznamu filmů, který bude snadno použitelný a zároveň splní požadavky semestrální práce.

---

## Funkční specifikace
Aplikace bude obsahovat menu, které umožní uživateli vybírat jednotlivé funkce:

1. Přidat nový film  
2. Zobrazit všechny filmy  
3. Označit film jako zhlédnutý  
4. Přidat nebo upravit hodnocení filmu  
5. Zobrazit pouze zhlédnuté / nezhlédnuté filmy  
6. Filtrovat filmy podle žánru  
7. Seřadit filmy (podle názvu, roku, hodnocení)  
8. Uložit data do souboru  
9. Načíst data ze souboru  
10. Ukončit program  

---

## Struktura vstupních a výstupních dat
Data budou ukládána do textového souboru, kde každý řádek bude představovat jeden film.

Příklad struktury:

nazev;zanr;rok;stav;hodnoceni

Například:

Inception;SCI-FI;2010;SEEN;9  
Titanic;ROMANCE;1997;UNSEEN;0  

Kromě textového souboru bude možné data ukládat i v binární podobě.

---

## Návrh tříd
Aplikace bude rozdělena do několika tříd:

- **Film** – reprezentuje jeden film (název, žánr, rok, stav, hodnocení)  
- **FilmManager** – spravuje seznam filmů (přidávání, mazání, vyhledávání)  
- **Main** – hlavní třída obsahující menu a komunikaci s uživatelem  
- **FileService** – zajišťuje načítání a ukládání dat do souborů  

---

## Použité prvky jazyka Java
V aplikaci budou využity následující prvky:

- ArrayList pro ukládání seznamu filmů  
- Enum pro typ žánru a stav filmu  
- Comparator a Comparable pro třídění  
- java.time pro práci s datem  
- regulární výrazy pro kontrolu vstupů  
- výjimky pro ošetření chyb  

---

## Testování
Pro testování budou vytvořeny vstupní soubory s minimálně 20 záznamy.  
Budou otestovány základní funkce programu:

- přidání filmu  
- zobrazení seznamu  
- filtrování  
- třídění  
- ukládání a načítání dat  
- ošetření chybného vstupu  

---

## Závěr
Cílem této práce je vytvořit funkční a přehlednou aplikaci, která umožní správu seznamu filmů. Aplikace bude navržena tak, aby byla jednoduchá na používání a zároveň splňovala všechny požadavky zadání.
