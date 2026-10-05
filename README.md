# Árufuvarozó szakmai irányító – online vizsgagyakorló

Ez egy teljesen statikus, egyfájlos webapp. Nem kell hozzá szerver, adatbázis vagy Python.

## GitHub Pages telepítés
1. Hozz létre egy új GitHub repository-t.
2. Töltsd fel az `index.html` fájlt a repository gyökerébe.
3. GitHub: Settings -> Pages.
4. Source: Deploy from a branch.
5. Branch: `main`, folder: `/ (root)`.
6. Save.

## Funkciók
- témakör-választás
- gyakorló- és vizsgamód
- 20 kérdés / 20 perc vizsgaszimuláció
- véletlen kérdés- és válaszsorrend
- helyi eredménytörténet
- hibás kérdések újragyakorlása
- CSV export
- JSON kérdésbank import

## Kérdésbank JSON formátuma
```json
[
  {
    "id": "sajat_001",
    "subject": "Jogi ismeretek",
    "q": "A kérdés szövege?",
    "options": ["A", "B", "C", "D"],
    "answer": "B",
    "explanation": "Rövid magyarázat."
  }
]
```
Az `answer` értékének pontosan szerepelnie kell az `options` listában.

Fontos: ez nem hivatalos KAV kérdésbank.
