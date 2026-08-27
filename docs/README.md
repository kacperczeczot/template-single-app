[Strona główna](../README.md) > [Dokumentacja](README.md)

---

# Dokumentacja Projektu

Katalog przeznaczony na dokumentację merytoryczną, architektoniczną i specyfikacje **tego konkretnego projektu**.

---

## 1. Struktura i Podkatalogi Dokumentacji

| Sekcja | Ścieżka | Status | Kiedy stosować? |
| :--- | :--- | :--- | :--- |
| [Rejestr Decyzji (ADR)](adr/README.md) | [docs/adr/](adr/README.md) | 🔴 `[WYMAGANY]` | W każdym projekcie do rejestrowania kluczowych wyborów technologicznych |
| [Architektura Projektu](architecture/README.md) | [docs/architecture/](architecture/README.md) | 🟡 `[ZALECANY]` | W projektach posiadających diagramy, modele bazy danych lub wiele modułów |
| [Specyfikacja API](api/README.md) | [docs/api/](api/README.md) | ⚪ `[OPCJONALNY]` | Gdy projekt wystawia lub konsumuje API zewnętrzne / IPC / kontrakty |

---

## 2. Standardy Inżynieryjne (Globalne)

Projekt dziedziczy wszystkie fundamentalne standardy architektoniczne, zasady czystości kodu oraz reguły AI z centralnego repozytorium:
👉 [Standardy Architektury i DevEx (devex-standards)](../../devex-standards/docs/README.md)
