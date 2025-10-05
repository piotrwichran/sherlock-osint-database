# 📂 Data Directory — Sherlock OSINT Database (English version)

> 🇵🇱 Polish version: [README_PL.md](README_PL.md)

This directory contains the extended and updated dataset (`data.json`) intended for use with the [Sherlock](https://github.com/sherlock-project/sherlock) tool.

The purpose of this dataset is to expand the number of supported websites and improve the accuracy of username detection — across both Polish and international platforms.

---

## 📁 Directory Contents

| File | Description |
|------|--------------|
| `data.json` | Main dataset — list of websites compatible with Sherlock |
| `README.md` | This file — documentation of the data directory in English |

---

## ⚙️ Usage with Sherlock

Run Sherlock with this custom dataset:
```bash
python3 sherlock --json data/data.json username
```
or replace the default file in the Sherlock directory:
```bash
cp data/data.json sherlock_project/resources/data.json
```
## 🧩 Structure of data.json
Each entry in the file defines one website and specifies how Sherlock should check whether a given username exists.
An example structure looks like this:
```json
"Sympatia": {
    "url": "https://sympatia.onet.pl/profil/{}",
    "errorMsg": "Nie znaleziono użytkownika",
    "urlMain": "https://sympatia.onet.pl/",
    "username_claimed": "anna"
}
```
***
## ⚠️ Note
Before adding a new entry, make sure that:
- the website actually allows public verification of user existence,
- the entry works correctly (verify a test username and error message),
- it does not violate the website’s terms of service or data protection regulations.
***
## 🪪 License
Distributed under the MIT License — see [LICENSE](LICENSE) for details.
© 2025 Piotr Wichrań