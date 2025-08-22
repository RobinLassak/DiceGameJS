# Pig Game - Školní domácí cvičení

**Autor:** Robin Lassak  
**Předmět:** JavaScript  
**Typ:** Školní domácí cvičení

## Popis aplikace

Pig Game je klasická kostková hra pro dva hráče implementovaná v čistém JavaScriptu. Hra je součástí školního domácího cvičení zaměřeného na práci s JavaScriptem, DOM manipulací a event handlingem.

## Jak hrát

### Pravidla hry:

1. **Cíl:** Jako první dosáhnout celkového skóre 100 bodů
2. **Průběh hry:**
   - Hráči se střídají v hodech kostkou
   - Při hodu 2-6 se body přičítají k aktuálnímu skóre
   - Při hodu 1 se aktuální skóre vynuluje a hraje další hráč
   - Hráč může kdykoliv "držet" své aktuální skóre a přičíst ho k celkovému

### Ovládání:

- ** Roll dice** - Hod kostkou
- ** Hold** - Držet aktuální skóre a přepnout hráče
- ** New game** - Začít novou hru

## Technologie

- **HTML5** - Struktura aplikace
- **CSS3** - Stylování a animace
- **JavaScript (ES6+)** - Herní logika a DOM manipulace
- **GitHub Actions** - Automatické nasazení

## Struktura projektu

```
Hra_Kostka/
├── index.html          # Hlavní HTML soubor
├── style.css           # CSS styly
├── script.js           # JavaScript herní logika
├── dice-1.png až dice-6.png  # Obrázky kostek
├── pig-game-flowchart.png    # Diagram herního toku
├── .prettierrc         # Prettier konfigurace
├── .github/workflows/  # GitHub Actions
│   └── deploy.yml      # Automatické nasazení
└── README.md           # Tento soubor
```

## Spuštění aplikace

1. **Lokální spuštění:**

   - Stáhněte si všechny soubory
   - Otevřete `index.html` v prohlížeči
   - Zadejte jména hráčů a začněte hrát

2. **Online verze:**
   - Aplikace je automaticky nasazována na Endora hosting
   - Aktualizace se nasazují při push do master větve

## Funkce aplikace

### Herní mechaniky:

- Generování náhodných hodů kostkou (1-6)
- Přepínání mezi hráči
- Sledování aktuálního a celkového skóre
- Vizuální indikace aktivního hráče
- Reset hry

### UI/UX prvky:

- Moderní design s glassmorphism efektem
- Responzivní layout
- Animace a přechody
- Vizuální zpětná vazba pro aktivního hráče
- Skrytí kostky před začátkem hry

### Technické funkce:

- DOM manipulace
- Event listeners
- CSS třídy pro stav hry
- Automatické nasazení přes GitHub Actions

## Konfigurace

### Prettier nastavení:

```json
{
  "singleQuote": true,
  "arrowParens": "avoid"
}
```

### Nasazení:

Aplikace používá GitHub Actions pro automatické nasazení na FTP server (Endora) při push do master větve.

## Herní logika

### Klíčové proměnné:

- `currentScore` - Aktuální skóre hráče
- `totalScore` - Pole celkových skóre obou hráčů
- `activePlayer` - Index aktivního hráče (0 nebo 1)

### Hlavní funkce:

- `inicializace()` - Nastavení počátečního stavu hry
- `switchPlayer()` - Přepnutí aktivního hráče
- Event listeners pro tlačítka

## Design

Aplikace používá moderní design s:

- **Font:** Nunito (Google Fonts)
- **Barvy:** Fialová paleta s růžovými akcenty
- **Efekty:** Glassmorphism, stíny, animace
- **Layout:** Flexbox pro responzivní design

## Poznámky k implementaci

- Kód je psán v češtině pro lepší srozumitelnost
- Používá moderní JavaScript funkce
- Implementuje čistou DOM manipulaci bez frameworků
- Obsahuje komentáře pro lepší pochopení kódu

## Odkazy

- **Autor:** Robin Lassak
- **Hosting:** Endora (automatické nasazení)
- **Repository:** GitHub

---

_Tento projekt je školním domácím cvičením zaměřeným na praktické použití JavaScriptu, DOM manipulace a moderních webových technologií._
