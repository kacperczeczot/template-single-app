[Strona główna](README.md)

---

# Single-App Project Template

Oficjalny szablon startowy dla pojedynczych aplikacji, bibliotek, gier i narzędzi jednozadaniowych w naszym ekosystemie.

---

## 1. Struktura Katalogów

Projekt ściśle przestrzega zamkniętego kanonu katalogu `root` w modelu **Single-App**:

| Katalog | Opis |
| :--- | :--- |
| [src/](src/README.md) | Główny kod źródłowy aplikacji |
| [tests/](tests/README.md) | Globalne testy integracyjne / E2E |
| [docs/](docs/README.md) | Dokumentacja projektowa, GDD, ADR-y |
| [assets/](assets/README.md) | Zasoby statyczne (grafiki, audio, modele 3D) |
| [data/](data/README.md) | Lokalne bazy SQLite, zrzuty JSON, dane dev (ignorowane) |
| [scripts/](scripts/README.md) | Automatyzacja (Node.js, bash, Python) [w C++ alternatywnie tools/] |
| [.agents/](.agents/rules/universal.md) | Reguły i instrukcje dla systemów AI |

> [!CAUTION]
> **Zakaz Samowolki Folderowej i Plikowej**
> Tworzenie jakichkolwiek innych folderów w `root` jest zabronione. W korzeniu nie mogą również znajdować się żadne luźne pliki z kodem źródłowym ani danymi.

---

## 2. Dokumentacja Projektu

| Sekcja | Ścieżka | Opis |
| :--- | :--- | :--- |
| [Baza Dokumentacji](docs/README.md) | [docs/README.md](docs/README.md) | Centralny hub dokumentacji |
| [Architektura](docs/architecture/RULES.md) | [docs/architecture/RULES.md](docs/architecture/RULES.md) | Reguły architektoniczne i czystość kodu |
| [Rejestr Decyzji (ADR)](docs/adr/README.md) | [docs/adr/README.md](docs/adr/README.md) | Rejestr Decyzji Architektonicznych |
| [Reguły AI](.agents/rules/universal.md) | [.agents/rules/universal.md](.agents/rules/universal.md) | Standardy współpracy z AI |
