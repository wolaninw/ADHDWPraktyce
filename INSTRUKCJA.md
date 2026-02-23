# Instrukcja wdrożenia na GitHub Pages

## Krok 1: Utwórz konto na GitHub (jeśli nie masz)

1. Wejdź na https://github.com
2. Kliknij "Sign up"
3. Wypełnij formularz rejestracyjny

## Krok 2: Utwórz nowe repozytorium

1. Zaloguj się na GitHub
2. Kliknij "+" w prawym górnym rogu → "New repository"
3. Wypełnij:
   - Repository name: `adhd-w-praktyce` (lub inna nazwa)
   - Description: "Blog edukacyjny o życiu z ADHD"
   - Public/Private: **Public** (wymagane dla darmowego GitHub Pages)
   - ✅ Zaznacz "Add a README file"
4. Kliknij "Create repository"

## Krok 3: Wgraj pliki

### Opcja A: Przez przeglądarkę (prostsze)

1. W swoim repozytorium kliknij "Add file" → "Upload files"
2. Przeciągnij wszystkie pliki z folderu `github-package`:
   - index.html
   - o-mnie.html
   - podejrzenia.html
   - diagnoza.html
   - oswiecenie.html
   - cechy-dysfunkcyjne.html
   - logo.png
   - README.md
   - .gitignore
3. Dodaj commit message: "Initial commit - strona ADHD w Praktyce"
4. Kliknij "Commit changes"

### Opcja B: Przez Git (dla zaawansowanych)

```bash
# W folderze github-package
git init
git add .
git commit -m "Initial commit - strona ADHD w Praktyce"
git branch -M main
git remote add origin https://github.com/[twoj-username]/adhd-w-praktyce.git
git push -u origin main
```

## Krok 4: Włącz GitHub Pages

1. W repozytorium przejdź do **Settings** (ustawienia)
2. W menu po lewej kliknij **Pages**
3. W sekcji "Source" wybierz:
   - Branch: **main**
   - Folder: **/ (root)**
4. Kliknij "Save"
5. Poczekaj 1-2 minuty

## Krok 5: Sprawdź stronę

Twoja strona będzie dostępna pod adresem:
```
https://[twoj-username].github.io/adhd-w-praktyce/
```

Na przykład:
- Username: `jankowalski`
- Adres strony: `https://jankowalski.github.io/adhd-w-praktyce/`

## Aktualizacja strony

Gdy wprowadzisz zmiany w plikach:

1. Wejdź do repozytorium na GitHub
2. Kliknij na plik, który chcesz edytować
3. Kliknij ikonę ołówka (Edit)
4. Wprowadź zmiany
5. Kliknij "Commit changes"
6. Poczekaj ~1 minutę, aż strona się zaktualizuje

## Własna domena (opcjonalne)

Jeśli chcesz użyć własnej domeny (np. `adhd-w-praktyce.pl`):

1. Kup domenę (np. na home.pl, OVH, Cloudflare)
2. W ustawieniach domeny dodaj rekord CNAME:
   ```
   www -> [twoj-username].github.io
   ```
3. W GitHub Pages (Settings → Pages) wpisz swoją domenę w "Custom domain"
4. Zaznacz "Enforce HTTPS"

## Rozwiązywanie problemów

### Strona nie działa (404)
- Sprawdź czy GitHub Pages jest włączony (Settings → Pages)
- Sprawdź czy branch jest ustawiony na `main`
- Poczekaj 5 minut i odśwież

### Zmiany nie widać
- GitHub Pages aktualizuje się z ~1 minutowym opóźnieniem
- Wymuś odświeżenie: Ctrl+F5 (Windows) lub Cmd+Shift+R (Mac)

### Logo się nie wyświetla
- Upewnij się, że plik `logo.png` jest wgrany
- Sprawdź wielkość liter w nazwie pliku (musi być dokładnie `logo.png`)

## Wsparcie

Jeśli masz problemy:
1. Sprawdź dokumentację GitHub Pages: https://pages.github.com
2. Otwórz Issue w repozytorium
3. Napisz na forum GitHub Community

---

**Powodzenia!** 🚀
