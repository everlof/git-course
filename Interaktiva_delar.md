
##### Interaktiv del 1

- Skapa fil `att-handla.txt`
- Vi skapar vårt repo med: `git init`
- Visa `git status` att den är untracked
- Lätt till i staging area 'git add att-handla.txt'
- Commit `git commit -m "Lade till 'att-handla.txt'"`
- `git log` för att kolla på commiten vi precis skapat

##### Interaktiv del 2

- Modifiera `att-handla.txt`
- Skapa `att-göra.txt`
- Visa status `git status`
- Visa på `git diff`
- Lägg till filerna
 - `git add att-handla.txt`
 - `git add att-göra.txt`
- Committa ändringarna `git commit -m "Skapa att-göra.txt + fler inköp"`
- Visa `git status`
- Visa `git log`


##### Interaktiv del 3

- Gör en ändring i `att-handla.txt`
- Visa: `git status`
- Nu vill inte ha kvar ändringen
- `git restore att-handla` återställer `att-handla` till hur den såg ut i staging-area (tidigare: `git checkout -- att-handla.txt`)
- Visa innehållet `cat att-handla.txt`

##### Interaktiv del 4

- Gör en ändring
- Lägg till med `git add att-handla.txt`
- Visa `git diff --staged`
- `git restore --staged att-handla.txt` (`git reset HEAD att-handla.txt`)
- `git status`

##### Interaktiv del 5

- `git slog`
- Vi ser master/main och så ser vi den symboliska branche HEAD
- Nu skapar vi brancher, som skapas där HEAD finns.
- Vi skapar `git branch todo` och `git branch handla`
- Visa att `git branch` visar alla brancher
- Asterix var vårt HEAD är
- Visa `git slog`
- Nu skall vi jobba på våra brancher 
- Checkout `todo`
- Lägg till saker att göra: 'Gå till gymmet'
- `git add att-gora.txt`
- Commit `git commit -m "More work to do "`
- Eftersom HEAD pekar på `gora` är det bara `gora` som kommer flyttas med.
- `cat att-göra.txt`
- `git checkout handla`
- `git slog`
- `cat att-handla`
- Lägg till `Banan` + `Mjöl`
- `git status`
- `git commit -a -m "Lade till mer att handla`"
- `git slog`

##### Interaktiv del 6

- `git status`
- `git checkout master`
- `git diff master..todo`
- `git merge todo`
- `git slog`
- Nu kan vi ta bort `todo`
- `git branch --merge`
- git branch -d todo
- git branch -d handla

##### Interaktiv del 7

- `git status`
- `git merge handla`
- `git slog`
- `git branch --merged`
- `git branch -d handla`