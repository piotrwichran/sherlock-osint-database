# sherlock-osint-database
Extended dataset for the Sherlock OSINT tool — includes additional websites, improved detection patterns, and localized (Polish &amp; global) sources for user reconnaissance and open-source intelligence research.

# 🕵️ Sherlock OSINT Database

**Sherlock OSINT Database** is an extended dataset designed for use with the [Sherlock Project](https://github.com/sherlock-project/sherlock) — an open-source tool for discovering usernames across social networks and online platforms.

This repository provides an updated and expanded `data.json` containing additional websites, improved detection rules, and localized (Polish & global) entries useful for OSINT, cybersecurity, and digital forensics research.

---

## ⚙️ Features

- ✅ Fully compatible with the official **Sherlock** tool  
- 🌍 Includes both **Polish and international** platforms  
- 🔎 Enhanced error detection and username matching patterns  
- 🧩 Modular and easy to update — community-driven dataset  

---

## 📁 Repository Structure

| Folder / File | Description |
|----------------|-------------|
| `/data/data.json` | Main dataset of websites compatible with Sherlock |
| `/data/README.md` | Documentation specific to the data folder |
| `LICENSE` | MIT License — free use, modification, and redistribution |
| `.gitignore` | Excludes system, cache, and temporary files |
| `README.md` | Main documentation for this repository |

---

## 🚀 How to Use

### 🔹 Option 1 — Replace Sherlock’s default dataset
Copy this custom dataset into your local Sherlock installation:
```bash
cp data/data.json sherlock_project/resources/data.json
```
### 🔹 Option 2 — Run Sherlock directly with this dataset
Run Sherlock and point it to this file:
```bash
python3 sherlock --json data/data.json username
```
Where username is the handle you want to search across supported platforms.
