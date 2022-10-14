# Funkční specifikace
# pro
# WikiAsteroid
## verze: 1.0
## datum vytvoření: 06.10. 2022
## autor: Nguyen Michal
## Obsah
* 1 [Úvod](#1úvod)
  * 1.1 [Účel](11-účel)
  * 1.2 [Konvence dokumentu](#12-konvence-dokumentu)
  * 1.3 [Pro koho je dokument určený](#13-pro-koho-je-dokument-určený)
  * 1.4 [Kontakty](#14-kontakty)
  * 1.5 [Odkazy na ostatní dokumenty](#15-odkazy-na-ostatní-dokumenty)
* 2 [Scénáře](#2-scénáře)
  * 2.1 [Všechny reálné způsoby použití](#21-všechny-reálné-způsoby-použití)
  * 2.2 [Funkce](#22-funkce)
  * 2.3 [Uživatelské skupiny](23-uživatelské-skupiny)
  * 2.4 [Vymezení rozsahu](#24-vymezení-rozsahu)
* 3 [Celková hrubá architektura](#3-celková-hrubá-architektura)
  * 3.1 [Pracovní tok](#31-pracovní-tok)
  * 3.2 [Hlavní moduly](32-hlavní-moduly)
  * 3.3 [Všechny detaily: obrazovky, okna, tisky, chybové zprávy, logování](#33-všechny-detaily-obrazovky-okna-tisky-chybové-zprávy-logování)
  * 3.4 [Všechny možné toky programu a jejich projevy](#34-all-possible-program-flows-and-their-manifestations)
  * 3.5 [All agreed principles](#34-všechny-možné-toky-programu-a-jejich-projevy)
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
- aktualizace dat
### 2.3 Uživatelské skupiny
- čtenář (uživatel)
### 2.4 Vymezení rozsahu
Aplikace slouží pouze k četbe a nebude uživateli povolen změnit informace.
### 2.5 Na co se nebude klást důraz (výkonnost)
Na rychlost aktualizace dat (záleží na množství dat, které nám API poskytne) 
## 3. Celková hrubá architektura
### 3.1 Pracovní tok
Po zaponutí aplikace se uživateli zobrazí aktualizovaný list asteroidů seřazené podle vzdálenosti od země, pokud bude uživatel připojen k internetu. Poté bude uživatel moct na každý asteroid zmáčknout, aby si zobrazil detailnější informace. Také bude v rohu tlačítko pro změnu seřazení podle vypsaných vlastností. Uživatel bude moct ručně atualizovat data nebo se vše atualizuje samo po nějaký čas.
### 3.2 Hlavní moduly
Aplikace bude mít 2 moduly. 
- 1. hlavní modul pro zobrezení všsch objektů
- 2. modul pro zobrezení detailů
### 3.3 Všechny detaily: obrazovky, okna, tisky, chybové zprávy, logování
Pokud uživatel nebude připojen k internetu a nebude moct aktualizovat stránku, tak se zobrazí chybová hláška.
Pokud uživatel aktualizuje data ručně, tak se zobrazí jestli se to provedlo úspěšně nebo ne.
Barvy budou laděny do tmava jako motiv vesmíru.
![Untitled (1)](https://user-images.githubusercontent.com/91062219/195085272-bcf5a54e-6633-48a0-b8ea-b12c76c27882.png)
### 3.4 Všechny možné toky programu a jejich projevy
První tok bude, když pošleme request na nasu. Druhý pak bude jejich odpověd, kterou následně zpracujem a uložíme do lokalní databáze.![Home - default](https://user-images.githubusercontent.com/91062219/195913635-3ce180ae-a747-4758-bf14-132194c22de6.png)



