# Portal: Revolution — polskie tłumaczenie

Nieoficjalne polskie tłumaczenie gry **Portal: Revolution**

---

## Szybki start

1. Pobierz ZIP: zielony przycisk **`<> Code`** → **Download ZIP**.
2. Wypakuj folder `revolution/` do katalogu gry: `…\steamapps\common\Portal Revolution\` (zezwól na nadpisanie plików).
3. W Steamie: prawy klik na grę → **Właściwości** → w polu **Opcje uruchamiania** wpisz: `-language polish`.
4. Uruchom grę. Gotowe.

> Opcjonalnie: w grze wejdź w **Ustawienia → Dźwięk → Język napisów → Polski**, jeśli chcesz wymusić polskie napisy niezależnie od ustawień Steama.

---

## Pełna instrukcja

### 1. Wymagania

- **Portal: Revolution** na Steamie.
- Program do otwierania archiwów ZIP (Windows ma to wbudowane; ewentualnie [7-Zip](https://www.7-zip.org/) lub [WinRAR](https://www.win-rar.com/)).

### 2. Pobranie tłumaczenia

1. Na górze tej strony GitHub kliknij zielony przycisk **`<> Code`**.
2. W menu wybierz **Download ZIP**.
3. Zapisz plik `Portal-Revolution-Polish-main.zip` w dowolnym miejscu (np. na pulpicie).

### 3. Znalezienie folderu gry

1. W bibliotece Steam kliknij prawym przyciskiem **Portal: Revolution**.
2. Wybierz **Zarządzaj → Przeglądaj pliki lokalne**.
3. Otworzy się folder gry, np.: `D:\SteamLibrary\steamapps\common\Portal Revolution\`. Zostaw go otwarty.

### 4. Instalacja plików

1. Otwórz pobrany ZIP. W środku znajdziesz folder `translation/`, a w nim folder `revolution/`.
2. **Skopiuj cały folder `revolution/`** (z folderu `translation/`) do katalogu gry z punktu 3.
3. System zapyta o **scalenie / nadpisanie** istniejących plików — **zgódź się**. To celowe; nadpisywane pliki (`clientscheme.res`, `settings-audio.xml`) zawierają poprawki niezbędne do prawidłowego wyświetlania polskich znaków.

Po skopiowaniu drzewo plików w katalogu gry powinno zawierać m.in.:

```
…\steamapps\common\Portal Revolution\revolution\
├── resource\
│   ├── clientscheme.res            ← zaktualizowany (poszerzony zakres czcionek)
│   ├── revolution_polish.txt
│   ├── subtitles_polish.txt
│   ├── valve_polish.txt
│   └── … (reszta plików _polish.txt + .dat)
└── panorama\
    └── layout\pages\main-menu\
        └── settings-audio.xml      ← zaktualizowany (dodany "Polski" do listy języków)
```

### 5. Ustawienie polskiego języka w Steamie

1. W bibliotece Steam → prawy klik na **Portal: Revolution** → **Właściwości**.
2. Zakładka **Ogólne** → pole **Opcje uruchamiania**.
3. Wpisz dokładnie: `-language polish`
4. Zamknij okno (zostanie zapisane automatycznie).

### 6. Pierwsze uruchomienie

1. Uruchom Portal: Revolution.
2. Menu główne, dialogi i napisy powinny być po polsku, ze wszystkimi znakami diakrytycznymi.
3. (Opcjonalnie) **Ustawienia → Dźwięk → Język napisów → Polski**.

---

## 👥 Twórcy

- **Menu / interfejs** — Odlotowy_ser
- **Korekta** — DeBondor, enderek, kyoshuske
- **Napisy, rozdziały 1–4** — kyoshuske
- **Napisy, rozdziały 5–8** — Odlotowy_ser
- **Napisy, epilog** — DeBondor

---

## 📝 Uwaga dla deweloperów modu

Modyfikacja jakichkolwiek plików `subtitles_*.txt` lub `closecaption_*.txt` wymaga rekompilacji odpowiedniego pliku `.dat`. Najprostszy sposób — gotowy [skrypt batch](https://gist.github.com/kyoshuske/4b7c3e92f2293bf2eb731ee399482057) (autor: kyoshuske).
