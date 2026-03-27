# Instrukcja dodawania nowych rekordów do katalogu

Aby nowa kontrola pojawiła się w systemie, należy wykonać dwa kroki: dodać wpis w pliku CSV oraz wgrać zdjęcia do odpowiedniego folderu.

---

## 1. Dodawanie danych (Plik dane.csv)

Otwórz plik `dane.csv` i dopisz nowy wiersz na samym dole. Pamiętaj o zachowaniu kolejności pól i oddzielaniu ich **średnikami (;)**.

**Schemat wpisu:**
`Kod;SKU;RSL TAG;Data kontroli;Kondycja;Opis;Asortyment`

**Przykład:**
`234122678;48116;WAR-7234;27.03.2026;HDLS;pod nową kondycję;Greenhouse`

### Ważne zasady:
* **Kod:** To unikalny numer (np. 234122678). Musi być taki sam jak nazwa pliku zdjęcia.
* **Kondycja:** Używaj wielkich liter (HDL, DAM, HDLS). System automatycznie pokoloruje status.
* **Data:** Wpisuj w formacie `DD.MM.RRRR`.

---

## 2. Dodawanie zdjęć (Folder /foto)

Zdjęcia muszą trafić do folderu o nazwie `foto`. System automatycznie szuka do trzech zdjęć dla każdego kodu.

### Nazewnictwo plików:
Nazwa zdjęcia musi zaczynać się od **Kodu** wpisanego w pliku CSV:

1. **Główne zdjęcie:** `KOD.jpg` (np. `234122678.jpg`)
2. **Drugie zdjęcie:** `KOD_2.jpg` (np. `234122678_2.jpg`)
3. **Trzecie zdjęcie:** `KOD_3.jpg` (np. `234122678_3.jpg`)

### Specyfikacja techniczna:
* **Format:** Wyłącznie `.jpg` (małe litery rozszerzenia).
* **Rozmiar:** Staraj się, aby zdjęcia nie były zbyt ciężkie (optymalnie poniżej 500 KB), aby katalog ładował się szybko.

---

## 3. Jak zapisać zmiany na GitHub?

1. Wejdź w plik `dane.csv` na GitHubie i kliknij ikonę ołówka (**Edit**).
2. Dopisz dane, zjedź na dół i kliknij **Commit changes**.
3. Wejdź do folderu `foto`, kliknij **Add file** -> **Upload files** i przeciągnij zdjęcia z komputera.
4. Kliknij **Commit changes**.

Po chwili zmiany będą widoczne w Twoim katalogu online!
