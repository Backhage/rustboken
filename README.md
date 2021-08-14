# Programmera i Rust

Det här repot innehåller källkoden till boken "Programmera i Rust".

## Förutsättningar

Instruktionerna nedan, och även det kapitel i boken som beskriver uppsättning av
utvecklingsmiljön, förutsätter att du använder Linux som operativsystem.
Självklart är boken användbar även om du inte använder Linux, du behöver dock
hitta en annan källa som beskriver hur du installerar Rust på din miljö.

## Bygg källkoden

För att bygga källkoden och generera boken behöver du ha Rust installerat och 
använda verktyget ```mdBook```. I Linux kan du använda ```cargo``` för att
installera ```mdBook``` med kommandot:

```shell
$ cargo install mdbook
```

Därefter kan du generera boken genom att i reporoten exekvera kommandot:

```shell
$ mdbook build
```

Boken kan du sedan läsa i din webbläsare genom att öppna filen ```<repo root>/book/index.html```