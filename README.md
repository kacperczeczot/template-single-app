# Single-App Project Template

Oficjalny szablon startowy dla pojedynczych aplikacji, bibliotek, gier i narzędzi jednozadaniowych w naszym ekosystemie.

---

## 1. Struktura Katalogów i Statusy

Projekt ściśle przestrzega zamkniętego kanonu katalogu `root` w modelu **Single-App**. Szablon udostępnia ustandaryzowaną strukturę (z nadwyżką), w której każdy folder posiada określony status:

| Katalog | Status | Kiedy stosować? |
| :--- | :--- | :--- |
| [src/](src/README.md) | 🔴 `[WYMAGANY]` | Zawsze — główny kod źródłowy aplikacji |
| [docs/](docs/README.md) | 🔴 `[WYMAGANY]` | Zawsze — dokumentacja projektu, GDD, [rejestr ADR](docs/adr/README.md) |
| [tests/](tests/README.md) | 🟡 `[ZALECANY]` | Gdy projekt posiada testy [E2E](tests/e2e/README.md) lub [integracyjne](tests/integration/README.md) |
| [public/](public/README.md) | ⚪ `[OPCJONALNY]` | Gdy aplikacja webowa wymaga plików serwowanych wprost (robots.txt, favicon, CMS) |
| [assets/](assets/README.md) | ⚪ `[OPCJONALNY]` | Gdy aplikacja posiada grafiki, audio, modele 3D, pliki do druku/PnP |
| [data/](data/README.md) | ⚪ `[OPCJONALNY]` | Gdy aplikacja korzysta z lokalnej bazy SQLite, zrzutów JSON lub cache |
| [scripts/](scripts/README.md) | ⚪ `[OPCJONALNY]` | Gdy projekt wymaga skryptów pomocniczych (w C++ alternatywnie `tools/`) |
| [.agents/](.agents/rules/project.md) | 🔴 `[WYMAGANY]` | Zawsze — reguły i wytyczne domenowe dla systemów AI |

> [!CAUTION]
> **Zakaz Samowolki Folderowej i Plikowej**
> Tworzenie jakichkolwiek innych folderów w `root` jest zabronione. W korzeniu nie mogą również znajdować się żadne luźne pliki z kodem źródłowym ani danymi.

---

## 2. Dokumentacja i Standardy

| Dokument / Sekcja | Opis |
| :--- | :--- |
| [Standardy Projektu (`docs/STANDARDS.md`)](docs/STANDARDS.md) | Deklaracja zgodności ze standardami, progi testów |
| [Dokumentacja Projektu (`docs/README.md`)](docs/README.md) | Centralny hub dokumentacji projektu |
| [Rejestr Decyzji ADR (`docs/adr/`)](docs/adr/README.md) | Rejestr Decyzji Architektonicznych |
| [Globalne Standardy DevEx (`devex-standards`)](https://github.com/kacperczeczot/devex-standards) | Nadrzędne reguły inżynieryjne (Zod, Result, Root) |
| [Reguły AI Projektu (`.agents/rules/project.md`)](.agents/rules/project.md) | Wytyczne domenowe dla asystentów AI |

