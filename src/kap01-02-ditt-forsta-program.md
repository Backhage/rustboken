# Ditt första program

Enligt traditionen bör varje programmeringsbok inledas med ett exempel på ett
program som skriver ut texten ```Hello, world!``` i terminalen.
I Rust skrivs ett sådant program så här:

```rust
fn main() {
    println!("Hello, world!");
}
```

Skapa nu ditt första program i Rust genom att:
1. Skapa en ny fil och döp den till ```main.rs```
2. Skriv in koden ovan och spara
3. Kompilera filen med kommandot ```rustc ./main.rs```
4. Kör programmet med kommandot ```./main```

Gick allt bra ska du inte få några felmeddelanden och ```Hello, world!``` skrivs
ut i terminalen.

## Programmets uppbyggnad 

En snabb analys av programkoden ger att den består av en funktion, ```main```,
där ```println!``` anropas. Funktionen ```main``` är speciell genom att den 
anropas per automatik när det kompilerade programmet körs. Prova gärna att byta
namn på funktionen till något annat och försök att kompilera programmet igen.
Kompilatorn kommer då att ge ett felmeddelande som säger att ingen funktion med
namnet ```main``` kunde hittas och att du behöver lägga till en sådan.

Den uppmärksamma läsaren noterade utropstecknet i ```println!``` vilket
förtjänar en förklaring. Detta beror på att ```println!``` inte är en vanlig
funktion, utan ett makro. I Rust skiljer sig anrop till funktioner och makron
genom att makron har ett avslutande utropstecken i namnet.

## Makrot println!

Makron är vanligt förekommande i flera programspråk. Ofta omvandlas makrokoden
till vanlig kod i ett försteg innan själva kompileringen. Du som utvecklare
behöver oftast inte tänka så mycket på att det är ett makro som används istället
för ett funktionsanrop men det är intressant att förstå vilka egenskaper hos
```println!``` som gör att det inte passar som en vanlig funktion.

Att definiera ```println!``` som ett makro tillåter:
1. Varierande antal argument
2. Kontroll att antalet platshållare och argument överensstämmer
3. Att argumenten automatisk behandlas som referenser

Dessa egenskaper stöds inte av vanliga funktioner. Det gör inget om du inte
förstår de här detaljerna än, de förklaras mer ingående i senare kapitel. Just
nu räcker det att du accepterar att makron har viktiga egenskaper som funktioner
saknar.
