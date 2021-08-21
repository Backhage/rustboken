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