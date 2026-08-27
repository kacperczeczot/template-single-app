[Strona główna](README.md)

---

# Single-App Project Template

Oficjalny szablon startowy dla pojedynczych aplikacji, bibliotek, gier i narzędzi jednozadaniowych w naszym ekosystemie.

---

## 1. Struktura Katalogów

Projekt ściśle przestrzega zamkniętego kanonu katalogu `root` w modelu **Single-App**:

```text
├── src/           # Główny kod źródłowy aplikacji
├── tests/         # Globalne testy integracyjne / E2E
├── docs/          # Dokumentacja projektowa, GDD, ADR-y
├── assets/        # Zasoby statyczne (grafiki, audio, modele 3D)
├── data/          # Lokalne bazy SQLite, zrzuty JSON, dane dev (ignorowane)
├── scripts/       # Lekka automatyzacja (Node.js, bash)
├── tools/         # Ciężkie narzędzia kompilacji / symulacje (C++, Rust)
└── .agents/       # Reguły i instrukcje dla systemów AI
```

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
