# Test 1 - Pravděpodobnost a statistika
## Příklad 1
 V dílně pracuje nezávisle na sobě 8 strojů. Pravděpodobnost, že první, druhý …, osmý stroj nebude potřebovat během směny opravit jsou 
| 0,8 | 0,89 | 0,84 | 0,90 | 0,85 | 0,92 | 0,86 | 0,95 |
|-----|------|------|------|------|------|------|------|

# Jaká je pravděpodobnost, že během směny:
- ## a)	Ani jeden stroj nebude potřebovat opravit.
  - ***Postup:*** vynásobení pravděpodobností, že stroje nebudou potřebovat opravit mezi sebou, nebo jinými slovy, že bude potřeba opravit přesně 0 strojů.
  - ***Výpočet:*** 0.8 ∙ 0.89 ∙ 0.84 ∙ 0.9 ∙ 0.85∙ 0.92 ∙ 0.86 ∙ 0.95 = 0.3438988 = 34.38%
- ## b)	Alespoň jeden stroj bude potřebovat opravu.
  - ***Postup:*** 100% pravděpodobnost odečteme od výsledku z a)
  - ***Výpočet:*** 1,00 - 0.3438988 = 0.6561012 = 65.61%
-  ## c) 1,3 a 5 stroj bude potřebovat opravu, ale ostatní ne.
    - ***Postup:*** U strojů 1,3 a 5 budeme počítat s obrácenou hodnotou
   - ***Výpočet:*** 0.2 ∙ 0.89 ∙ 0.16 ∙ 0.9 ∙ 0.15 ∙ 0.92 ∙ 0.86 ∙ 0.95 = 0.002889905 = 0.2889%

## Příklad 2
Střelec střílí nezávisle 10krát na terč. Pravděpodobnost zásahu terče při 1 výstřelu je 0,8. Předpokládejte, že výstřely jsou navzájem nezávislé.
# Jaká je pravděpodobnost, že: 
- a) Střelec mine terč nejvýše 1krát
   - ***Postup:*** Nejvýše 1, znamená pravděpodobnost, že se 9x trefí a 1 netrefí a ZÁROVEŇ, že se trefí vždy.
   - ***Výpočet:*** 0.8^10 + 0.8^9 ∙ 0.2= 0.1342177= 13.42%

   - ***Slovní odpověď:*** Pravděpodobnost, že střelec mine terč nejvýše 1krát je 13.42%
- b) Střelec mine terč alespoň 2krát, tedy mine 2,3,4,5,6,7,8,9,10 krát.
   - ***Postup:*** 100% pravděpodobnost odečteme z odpověďi z příkladu a)
   - ***Výpočet:*** 1,00 – 0.1342177 = 0.8657823 = 86.57%
   - ***Slovní odpověď:*** Pravděpodobnost, že střelec mine terč alespoň 2krát je 86.57%
- c)	Střelec nemine ani jednou
   - ***Postup*** Nemine ani jednou = trefí vždy = vynásobit pravděpodobnost, že se trefí počtem výstřelů.
   - ***Výpočet:*** 0.8^10 = 0.1073742 = 10.73%
   - ***Slovní odpověď:*** Pravděpodobnost, že střelec ani jednou nemine je 10.73%.
- d)	Určete střední hodnotu, modus, rozptyl, směrodatnou odchylku, koeficient šikmosti a špičatosti počtu výstřelů mimo terč.
   - ***Postup:*** dosazení do vzorečků viz. povolené materiály ke zkoušce.pdf
   - ***Výpočet:***
   - Diskrétní rozdělení binomické = B(10,0.8)
   - Střední hodnota E(X) = 10 ∙ 0.8 = 8
   - Rozptyl D(X) =  10 ∙ 0.8 ∙ (1-0.8) = 1.6
   - Koeficient šikmosti a3(X) = (1-2*0.8)/sqrt(10*0.8*(1-0.8)) = -0.4743416
   - Koeficient špičatosti a4(X) = (1-6*0.8*(1-0.8))/10*0.8*(1-0.8) = 0.00064

## Příklad 3
V jisté nemocnici bylo náhodně vybráno 50 novorozenců u nichž byla,  mimo jiné, sledována porodní hmotnost (v gramech) a věk matky (v letech) narozeného dítěte. Na základě tohoto náhodného výběru byla spočtena průměrná hmotnost novorozence 3496,08g a směrodatná odchylka hmotnosti 502,688g. Podobně průměrný věk matky 25,38 let a směrodatná odchylka věku 4,522 let.
Určete:
- a) 95% interval spolehlivosti pro hmotnost novorozenců
   - ***Postup:*** výpočet dat za pomocí Stat1 záložka 1V – normální > výpočty z charakteristik

![Postup příklad 3/1]()



Modrá barva = náš výsledek
Hnědá barva = co zadáváme
Slovní odpověď: S 95% pravděpodobností se váha dítěte nachází v rozmezí od 3489,708 g do 3502,45g.

b)	S 95% spolehlivostí dolní hranici pro střední hodnotu věku matky. 
O: Výpočet dat za pomocí Stat1 záložka 1V – normální > výpočty z charakteristik

![Postup příklad 3/2]()

Modrá barva = náš výsledek
Hnědá barva = co zadáváme
Slovní odpověď: S 95% pravděpodobností je dolní hranice střední hodnoty věku matky dítěte 24,876 let.

Příklad 4
V tabulce jsou uvedeny hmotnosti samců a samic vlka (v kg).
Samice	28	38	41	32	35	31	33			
Samec	32	42	46	38	40	53	39	42	39	48

a)	Zjistěte. Zda lze obecně očekávat vyšší tělesnou hmotnost u samců nez u samic. Test proveďte na hladině významnosti a=0,05. Předpokládejme, že se jedná o náhodné výběry z normálního rozdělení.
O:Výpočet dat za pomocí Stat1, vložit do data > záložka 2V – normální
Modrá barva = náš výsledek hnědá barva = co zadáváme 
Slovní odpověď: S pravděpodobností 95% můžeme říci, že váha samců vlka je statisticky významněji větší, než váha samice vlka.
