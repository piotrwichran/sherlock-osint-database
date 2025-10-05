> 🌍 English version: [README.md](README.md)
# sherlock-osint-database
Extended dataset for the Sherlock OSINT tool — includes additional websites, improved detection patterns, and localized (Polish &amp; global) sources for user reconnaissance and open-source intelligence research.
```
# 🕵️ Sherlock OSINT Database — Polska wersja

**Sherlock OSINT Database** to rozszerzony zbiór danych przeznaczony do współpracy z narzędziem [Sherlock](https://github.com/sherlock-project/sherlock), służącym do wyszukiwania nazw użytkowników w serwisach społecznościowych i platformach internetowych.

Repozytorium zawiera zaktualizowany i rozbudowany plik `data.json`, obejmujący nowe serwisy, ulepszone reguły rozpoznawania oraz wpisy lokalne (polskie i międzynarodowe) przydatne w pracy OSINT, cyberbezpieczeństwie i informatyce śledczej.

---

## ⚙️ Funkcjonalności

- ✅ Zgodność z oryginalnym narzędziem **Sherlock**  
- 🌍 Obsługa polskich i zagranicznych platform  
- 🔎 Ulepszone wykrywanie błędów i dopasowań nazw użytkowników  
- 🧩 Łatwa rozbudowa i aktualizacja — projekt społecznościowy  

---

## 📁 Struktura repozytorium

| Folder / Plik | Opis |
|----------------|------|
| `/data/data.json` | Główny zbiór serwisów obsługiwanych przez Sherlocka |
| `/data/README_PL.md` | Opis katalogu danych w języku polskim |
| `LICENSE` | Licencja MIT — swobodne użycie i modyfikacja |
| `.gitignore` | Lista plików ignorowanych przez Git |
| `README_PL.md` | Dokumentacja projektu w języku polskim |

---

## 🚀 Jak używać

### 🔹 Opcja 1 — zastąp oryginalny plik w Sherlocku
Skopiuj zmodyfikowany plik:
```bash
cp data/data.json sherlock_project/resources/data.json
```
### 🔹 Opcja 2 — uruchom Sherlocka z własnym plikiem
Run Sherlock and point it to this file:
```bash
python3 sherlock --json data/data.json nazwa_użytkownika
```
Where username is the handle you want to search across supported platforms.
### 🧩 Przykład wpisu
```json
"Sympatia": {
    "url": "https://sympatia.onet.pl/profil/{}",
    "errorMsg": "Nie znaleziono użytkownika",
    "urlMain": "https://sympatia.onet.pl/",
    "username_claimed": "anna"
}
```
***
### ⚠️ Zastrzeżenie
Projekt nie jest powiązany z oficjalnym Sherlock Project.
To niezależne rozszerzenie społecznościowe, przeznaczone wyłącznie do celów edukacyjnych i badawczych w obszarze OSINT i cyberbezpieczeństwa.

Wszystkie dane pochodzą z publicznie dostępnych źródeł.
Używaj z zachowaniem obowiązujących przepisów prawa.
***
### 🪪 Licencja
Udostępnione na zasadach MIT License — zobacz [LICENSE](LICENSE).
© 2025 Piotr Wichrań
