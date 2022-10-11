# Funkční specifikace
# pro
# WikiAsteroid
## verze: 1.0
## datum vytvoření: 06.10. 2022
## autor: Nguyen Michal
## Obsah
## 1.Úvod
### 1.1 Účel
Účelem tohoto dokumentu je popsat chování softwaru z hlediska uživatele Databázi knih (dále jenom “WikiAsteroid“).
### 1.2 Konvence dokumentu
Příklady jsou v tomto dokumentu uzavřeny v kulatých závorkách (takto), změny od poslední verze jsou zvýrazněny červeně. Celý dokument je rozdělen do jednotlivých témat a podtémat a jsou napsány modře.
### 1.3 Pro koho je dokument určený
Tento dokument je určený pro vývojáře WikiAsteroid.  
### 1.4 Kontakty
Nguyen Michal
email: nguyen.mi.2019@ssps.cz
tel.: 774 825 886
### 1.5 Odkazy na ostatní dokumenty
- SRS(https://github.com/Khazugen/NeoWS/blob/master/SRS.md)
## 2. Scénáře
### 2.1 Všechny reálné způsoby použití
Produkt je určen jako zdroj informací a ke vzdělávání
### 2.2 Funkce
- Zobrazení list všech asteroidů seřazené na základě nějaké valstnosti zadaný uživatelem
- Filtrování výsledků
- Zobrazení detailů o jednotlivých objektech
### 2.3 Uživatelské skupiny
- čtenář (uživatel)
### 2.4 Vymezení rozsahu
Aplikace slouží pouze k četbe a nebude uživateli povolen změnit informace.
### 2.5 Na co se nebude klást důraz (výkonnost)

## 3. Celková hrubá architektura
### 3.1 Pracovní tok
Po zaponutí aplikace se uživateli zobrazí list asteroidů seřazené podle vzdálenosti od země, pokud bude uživatel připojen k internetu. Poté bude uživatel moct na každý asteroid zmáčknout, aby si zobrazil detailnější informace. Také bude v rohu tlačítko pro změnu seřazení podle vypsaných vlastností.
### 3.2 Hlavní moduly
Aplikace bude mít 2 moduly. 
- 1. hlavní modul pro zobrezení všsch objektů
- 2. modul pro zobrezení detailů
### 3.3 Všechny detaily: obrazovky, okna, tisky, chybové zprávy, logování
Pokud uživatel nebude připojen k internetu a nebude moct aktualizovat stránku, tak se zobrazí chybová hláška
### 3.4 Všechny možné toky programu a jejich projevy
