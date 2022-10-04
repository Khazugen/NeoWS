#Specifikace požadavků
#pro
#WikiAsteroid






##verze: 1.0
##datum vytvoření: 28.9. 2022
##autor: Nguyen Michal
##Obsah
##1.Úvod	2
###1.1 Účel	2
1.2 Konvence dokumentu	3
1.3 Pro koho je dokument určený	3
1.4 Kontakty	3
2. Celkový popis	3
2.1 Produkt jako celek	3
2.2 Funkce	3
2.3 Uživatelské skupiny	3
2.4 Provozní prostředí	3
2.5 Uživatelské prostředí	3
3. Požadavky na rozhraní	3
3.1 Uživatelská rozhraní	3
3.2 Hardwarová rozhraní	3
4. Vlastnosti systému	4
4.1 Vlastnost A – Zobrazit	4
4.1.1 Popis a důležitost	4
4.1.2 Vstupy – Akce – Výsledek	4
4.1.3 Funkční požadavky	4
4.2 Vlastnost B – Filtrování a vyhledávání	4
4.2.1 Popis a důležitost	4
4.2.2 Vstupy – Akce – Výsledek	4
4.2.3 Funkční požadavky	4




1.Úvod
1.1 Účel 
Účelem tohoto dokumentu je specifikovat požadavky pro encyklopedii asteroidů, které mohu ohrozit Zemi (dále jenom “WikiAsteroid“).
1.2 Konvence dokumentu 
Příklady jsou v tomto dokumentu uzavřeny v kulatých závorkách (takto), změny od poslední verze jsou zvýrazněny červeně. Celý dokument je rozdělen do jednotlivých témat a podtémat a jsou napsány modře.
1.3 Pro koho je dokument určený 
Tento dokument je určený pro vývojáře WikiAsteroid.  
1.4 Kontakty 
Nguyen Michal
email: nguyen.mi.2019@ssps.cz
tel.: 774 825 827

2. Celkový popis
2.1 Produkt jako celek
Produktem byl měla být okenní aplikace C# .NET určený pro informování o asteroidech blížící se k Zemi.
2.2 Funkce
- Zobrazování informace o asteroidech blížící se k Zemi, získané z API od NASA 
- Vyhledávání jednotlivých objektů
2.3 Uživatelské skupiny 
Uživatelská skupina bude pouze jenom jedna
2.4 Provozní prostředí 
Provozním prostředí bude počítač s operačním systémem s Windows 
2.5 Uživatelské prostředí
Uživatelské prostředí bude okenní aplikace
3. Požadavky na rozhraní
3.1 Uživatelská rozhraní 
Po zapnutí aplikace se uživateli seznam jednotlivých asteroidů, která jsou získaná díky NeoWS API. Na horní liště bude tlačítko pro vyhledávání a filtrování jednotlivých asteroidů.

3.2 Hardwarová rozhraní 
PC, klávesnice a myš
4. Vlastnosti systému
4.1 Vlastnost A – Hlavní stránka
4.1.1 Popis a důležitost 
Jedna z nejdůležitějších vlastností této aplikace. Tato stránka se zobrazí hned po zapnutí aplikace a zobrazí jednotlivé asteroidy seřazené defaultně podle vzdálenosti od Země a základní informace o nich.
4.1.2 Vstupy – Akce – Výsledek 

4.2 Vlastnost B – Filtrování a seřazování
4.2.1 Popis a důležitost 
Uživatel bude moct, nastavit seřazování podle jednotlivých vlastností asteroidu a také filtrovat je. Příklady vlastností na základě kterých můžeme seřazovat a filtrovat: jméno, velikost asteroidu, vzdálenost od Země, potencionální nebezpečí pro Zemi.
4.2.2 Vstupy – Akce – Výsledek 

4.3 Vlastnost C – Zobrazení detailů
4.2.1 Popis a důležitost 
Zobrazí detailnější informace o asteroidu, než na hlavní stránce
4.2.2 Vstupy – Akce – Výsledek 





