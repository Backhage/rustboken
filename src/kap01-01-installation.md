# Installation

De instruktioner som följer nedan har testats på Linux, närmare bestämt på
Linux Mint 20.2. Om du använder något annat operativsystem så finns
instruktioner tillgängliga på Rusts
[officiella hemsida](https://www.rust-lang.org/tools/install "Installationsinstruktioner på rust-lang.org").

För att installera Rust använder du ```rustup```, som är ett verktyg som du kör
i terminalen. Så starta en terminal och klistra in följande kommando:
```shell
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
Detta kommer att installera de verktyg du behöver i din hemkatalog och uppdatera
din miljövariabel ```path``` så att du kan exekvera verktygen oavsett vilken
katalog du kör kommandot från.

Eftersom verktygen installeras i din egen hemkatalog behöver du inte några
administratörsrättigheter för att installera Rust.

Du kan använda ```rustup``` för att senare uppdatera Rust[^1] eller helt
avinstallera[^2] det om du vill.

Om allt gick som det skulle så är du nu redo att skriva ditt första program.

[^1]: Använd kommandot ```rustup update``` för att hålla Rust uppdaterat.

[^2]: Använd kommandot ```rustup self uninstall``` för att avinstallera Rust.