[English](Home) · **Dansk** · [Bahasa Melayu](Home-ms)

# Mail Merge

Et lille script, der skriver ét personligt brev pr. gæst ud fra en skabelon og en liste med navne.

## Hvad er det?

Dag 24 af Udemy-kurset *100 Days of Code: The Complete Python Pro Bootcamp*. `main.py` læser gæsternes navne fra `Input/Names/invited_names.txt`, erstatter pladsholderen `[name]` i `Input/Letters/starting_letter.txt` med hvert navn og skriver ét brev pr. gæst i `Output/ReadyToSend/`. Det har ingen tests og ingen afhængigheder.

## Hvad øvelsen lærer dig

- At læse en fil linje for linje med `readlines()` og en hel fil med `read()`
- At fjerne det afsluttende linjeskift fra hvert navn med `strip()`
- At erstatte en pladsholder i en skabelon med `replace()`
- At skrive én outputfil pr. navn med `open(..., "w")`

## Hvad det gør

- Læser gæsternes navne, ét pr. linje, fra `Input/Names/invited_names.txt`
- Erstatter `[name]` i brevskabelonen `Input/Letters/starting_letter.txt` med hvert navn
- Skriver ét brev pr. gæst til `Output/ReadyToSend/letter_for_<name>.txt`

## Videre

- [Kom godt i gang](Getting-Started-da)
- [Projektdokumenter](Project-Documents-da)
