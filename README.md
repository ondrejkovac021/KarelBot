# Karel Robot 

## Přehled
Tato aplikace představuje jednoduchou implementaci "Karla bota", která běží kompletně v prohlížeči pomocí HTML, CSS a JavaScriptu. Uživatel může ovládat Karla, robota, který se pohybuje po 2D mřížce, pomocí textových příkazů zadaných v textovém poli.

## Funkce
1. **Pohyb Karla**:
   - Příkaz: `KROK x`
   - Karel se posune o x políček ve směru, kterým je otočen.
   - Pokud není uvedeno číslo, Karel se posune o 1 políčko.
2. **Otočení vlevo**:
   - Příkaz: `VLEVOBOK x`
   - Karel se otočí vlevo X-krát (o 90° na každé otočení).
   - Pokud není uvedeno číslo, Karel se otočí jednou.
3. **Položení symbolu**:
   - Příkaz: `POLOZ a`
   - Na aktuální pozici Karla se položí zadaný znak nebo symbol (např. `a`).
4. **Reset hry**:
   - Příkaz: `RESET`
   - Vymaže mřížku a resetuje Karla do levého horního rohu, otočeného doprava.
5. **Nezáleží na velikosti písmen**:
   - Příkazy lze zadávat velkými i malými písmeny.

## Návod k použití
1. Otevřete soubor `karel.html` v libovolném webovém prohlížeči.
2. Do textového pole napište příkazy pro Karla, každý příkaz na nový řádek.
3. Klikněte na tlačítko "Spustit" pro vykonání příkazů.
4. Klikněte na tlačítko "Reset" pro vymazání mřížky a resetování pozice Karla.

## Ukázkové příkazy
```
KROK 3
VLEVOBOK 2
POLOZ A
KROK
RESET
```

## Technické detaily
- Aplikace používá mřížku o velikosti 10x10, která je dynamicky vytvořena pomocí JavaScriptu.
- CSS zajišťuje čisté a přehledné rozhraní s vizuální zpětnou vazbou pro pozici Karla a položené symboly.
- Nepoužívají se žádné externí knihovny, aplikace je lehká a snadno použitelná.

## Jak to funguje
1. **Inicializace mřížky**:
   - Vytvoří se mřížka 10x10, kde každé políčko je reprezentováno pomocí `div` elementu.
2. **Zpracování příkazů**:
   - Příkazy jsou zpracovány po jednotlivých řádcích.
   - Příkazy nejsou citlivé na velikost písmen.
3. **Pohyb Karla**:
   - Pozice a směr Karla se aktualizují podle příkazů.
   - Mřížka se vizuálně aktualizuje tak, aby zobrazovala aktuální pozici Karla.
