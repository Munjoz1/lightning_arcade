# Lightning Arcade – Mini Game Platform

## Opis problema

U savremenom digitalnom okruženju korisnici često traže jednostavne, brze i zabavne igre koje mogu igrati bez instalacije kompleksnih sistema ili velikih aplikacija. Većina postojećih platformi je ili previše opterećena reklamama, zahteva registraciju, ili nije prilagođena svim uređajima.

Problem koji se rešava ovim projektom jeste nedostatak jednostavne, sigurne i efikasne arcade platforme koja omogućava igranje više mini-igara na jednom mestu, uz visok nivo performansi i stabilnosti.

Takođe, postoji potreba za demonstracijom savremenih softverskih arhitektura i korišćenjem programskog jezika Rust u realnom projektu.

---

## Predlog rešenja

Predloženo rešenje je razvoj **Lightning Arcade** aplikacije — mini arcade platforme koja sadrži sledeće igre:

- Wordle  
- Sudoku  
- Blackjack  
- Tic-Tac-Toe
- I slično

Aplikacija omogućava korisniku da iz glavnog menija izabere željenu igru i odmah započne igranje. Svaka igra funkcioniše kao nezavisni modul, dok zajednički sistem upravlja korisničkim interfejsom, navigacijom i evidencijom rezultata.

Rešenje koristi Rust kao osnovni programski jezik zbog njegove:

- visoke bezbednosti memorije,
- odličnih performansi,
- pogodnosti za modularni dizajn,
- stabilnosti za dugoročne projekte.

---

## Arhitektura sistema

Sistem je zasnovan na **modularnoj slojevitoj arhitekturi**.

### Slojevi sistema:

1. **Presentation Layer (UI sloj)**
   - Prikaz menija i igara
   - Komunikacija sa korisnikom
   - Implementiran pomoću terminal UI ili grafičkog prozora

2. **Game Logic Layer**
   - Logika svake igre
   - Pravila, bodovanje, validacija poteza

3. **Core Layer**
   - Upravljanje stanjima igre
   - Navigacija između igara
   - Zajedničke strukture podataka

4. **Utility Layer**
   - Generisanje slučajnih vrednosti
   - Rad sa fajlovima
   - Čuvanje rezultata

---

## Opis igara

### Wordle
Igra pogađanja reči u ograničenom broju pokušaja uz vizuelne indikatore tačnosti slova.

### Sudoku
Logička igra popunjavanja brojeva u mreži 9x9 prema zadatim pravilima.

### Blackjack
Kartaška igra protiv računara sa standardnim pravilima bodovanja.

### Tic-Tac-Toe
Klasična igra iks-oks za dva igrača ili protiv računara.

---

## Tehnologije

- Rust
- Cargo
- Terminal UI biblioteke (npr. ratatui / crossterm) ili grafički engine (Bevy)
- Git za verzionisanje

---

## Prednosti rešenja

- Modularan dizajn
- Lako dodavanje novih igara
- Visoke performanse
- Sigurno upravljanje memorijom
- Pogodno za učenje i proširenje

---

## Zaključak

Lightning Arcade predstavlja stabilnu, sigurnu i proširivu mini-game platformu koja rešava problem fragmentacije igara i pruža korisniku jednostavno i zabavno iskustvo. Projekat istovremeno služi kao primer kvalitetne softverske arhitekture i praktične primene Rust programskog jezika.

---

## Autor

Stefan Stanivuković
SR49/2023


