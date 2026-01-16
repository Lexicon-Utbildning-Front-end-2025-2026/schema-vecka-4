# 📅 Schema vecka 4

**TypeScript, vecka 3 av 3 (Fördjupning & Interaktivitet)**

Denna vecka tar vi steget från statisk data till fullt interaktiva applikationer. Vi kommer att fokusera på hur användaren kan mata in information via formulär, hur vi strukturerar vår växande kodbas med moduler, och hur vi hämtar data utifrån.

---

## 📅 Måndag

### Mål för dagen
* Förstå hur man hanterar formulär i TypeScript.
* Kunna hämta värden från `input`-fält och skapa objekt av dem.
* Kunna använda **Destructuring** för att skriva renare kod.

### Läsning
* [(MDN) Working with forms](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form)
* [(MDN) Destructuring assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)
* [(TypeScript Handbook) Type Assertion (as HTMLInputElement)](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#type-assertions)

### Övningar
* **Implementera Formulär:** Skapa ett formulär i ditt projekt (t.ex. "Lägg till ny låt", "Lägg till produkt" eller "Ny Todo").
* **Logga data:** Se till att du kan fånga upp det användaren skriver och logga det i konsolen som ett snyggt objekt.
* **Destructuring:** Gå igenom din kod och se var du kan använda destructuring (t.ex. `const { title, artist } = song` istället för `song.title`).

---

## 📅 Tisdag

### Mål för dagen
* Förstå **Events** på djupet (Bubbling vs Capturing).
* Förstå **JSON** vad det är.
* Kunna använda `event.preventDefault()` för att stoppa formulär från att ladda om sidan.
* Kunna använda **Event Delegation** för att hantera klick i listor effektivt.
* Kunna använda **Local Storage** för att spara data lokalt.

### Läsning
* [(MDN) Event bubbling and capture](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events#event_bubbling_and_capture)
* [(MDN) Event.preventDefault()](https://developer.mozilla.org/en-US/docs/Web/API/Event/preventDefault)
* [(JavaScript.info) Event Delegation](https://javascript.info/event-delegation)

### Övningar
* **Spara data:** Koppla ihop ditt formulär med din lista. När användaren klickar "Spara" ska det nya objektet läggas till i din array och synas på skärmen.
* **Optimera klick:** Om du har en `addEventListener` på varje kort i din lista – skriv om det så att du bara har *en* lyssnare på hela behållaren (Event Delegation).

---

## 📅 Onsdag

### Mål för dagen
* Förstå varför och hur vi använder **Moduler** (Import/Export).
* Kunna strukturera ett större projekt genom att dela upp koden i logiska filer (t.ex. `types.ts`, `functions.ts`, `main.ts`).

### Läsning
* [(MDN) JavaScript modules](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules)
* [(TypeScript Handbook) Modules](https://www.typescriptlang.org/docs/handbook/2/modules.html)

### Övningar
* **Städa koden:** Dela upp din `main.ts`.
    * Flytta alla `interface` till en egen fil (t.ex. `interfaces.ts`).
    * Flytta hjälpfunktioner till en egen fil (t.ex. `utils.ts`).
* **Importera/Exportera:** Se till att allt fungerar som förut genom att använda `import` och `export`.

---

## 📅 Torsdag

### Mål för dagen
* Repetition av veckans moment.
* **Code-Along:** Vi knyter ihop säcken genom att reflektera över hur strukturen förbättrats.
* **Överkurs (Bonus):** Introduktion till asynkron kod (`async`/`await`) och `fetch` för att hämta data från en extern JSON-fil istället för en hårdkodad array.

### Läsning
* [(MDN) How to use Promises (Async/Await)](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Promises)
* [(MDN) Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)

### Övningar
* **Refactoring:** Fortsätt putsa på ditt projekt. Är dina variabelnamn tydliga? Är koden uppdelad i bra funktioner?
* **Bonus:** Försök flytta din hårdkodade data till en `data.json`-fil och hämta in den med `fetch()` när sidan laddas.

---

## 📅 Fredag

### Mål för dagen
Fördjupa förståelsen genom att granska och diskutera kod. Vi fokuserar på hur applikationen hanterar dataflödet från användare till skärm.

**Frågor för Code Review:**

* **I grupp:**
    * Visa hur ni hanterar formuläret: Var skapas objektet? Var valideras det?
    * Visa hur ni strukturerat era filer: Varför valde ni att dela upp det som ni gjorde?
* **Gemensamt:**
    * Vad är fördelen med att använda `Event Delegation` istället för att ha lyssnare på varje element?
    * Hur kändes det att bryta upp koden i moduler – blev det lättare eller svårare att hitta?

### Övningar
* **Code Review:** Gå igenom era projekt i basgrupperna.
* **Final Polish:** Använd feedbacken för att göra de sista justeringarna på ert projekt innan helgen.
