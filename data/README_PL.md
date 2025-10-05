# 📂 Katalog danych — Sherlock OSINT Database (Wersja polska)

> 🌍 English version: [README.md](README.md)

Ten katalog zawiera rozszerzony i zaktualizowany zestaw danych (`data.json`) przeznaczony do współpracy z narzędziem [Sherlock](https://github.com/sherlock-project/sherlock).

Celem tego zbioru danych jest zwiększenie liczby obsługiwanych serwisów internetowych i poprawa dokładności wykrywania nazw użytkowników — zarówno w serwisach polskich, jak i międzynarodowych.

---

## 📁 Zawartość katalogu

| Plik | Opis |
|------|------|
| `data.json` | Główny plik datasetu — lista serwisów kompatybilnych z Sherlockiem |
| `README_PL.md` | Ten plik — dokumentacja katalogu w języku polskim |

---

## ⚙️ Użycie z Sherlockiem

Uruchom Sherlocka z własnym zestawem danych:
```bash
python3 sherlock --json data/data.json nazwa_użytkownika
```
lub zastąp oryginalny plik w katalogu Sherlocka:
```bash
cp data/data.json sherlock_project/resources/data.json
```
***
## ⚠️ Uwaga
Zanim dodasz nowy wpis, upewnij się, że:
- serwis faktycznie pozwala publicznie weryfikować istnienie kont,
- wpis działa poprawnie (sprawdź testowy login i komunikat błędu),
- nie narusza to zasad serwisu ani przepisów o ochronie danych.
***
## 🪪 Licencja
Udostępnione na zasadach MIT License — zobacz [LICENSE](LICENSE).
© 2025 Piotr Wichrań