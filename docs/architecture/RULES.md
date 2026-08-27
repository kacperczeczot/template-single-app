[Strona główna](../../README.md) > [Dokumentacja](../README.md) > [Architektura](RULES.md)

---

# Architektura i Konwencje Kodu

## 1. Strażnik Granic (Boundary Guardian) - Zod
Wszelkie dane przekraczające granice systemów (IPC, API, pliki konfiguracyjne) muszą być rygorystycznie walidowane przy użyciu biblioteki `zod`. Typy TypeScript są generowane ze schematów (`z.infer`).

## 2. Obsługa Błędów - Result Object
W logice domenowej stosujemy jawny wzorzec `Result Object` zamiast niekontrolowanego rzucania wyjątków:
`type Result<T, E> = { ok: true; data: T } | { ok: false; error: E; code?: string };`

## 3. Architektura Kolokacji
Układamy kod domenowo, trzymając komponenty, ich style (CSS Modules), logikę i testy jednostkowe w jednym dedykowanym katalogu wewnątrz `src/`.

## 4. Czystość Katalogu Root i Konwencje Folderów
Katalog główny (`root`) służy wyłącznie jako tablica rozdzielcza dla narzędzi i konfiguracji. Obowiązują następujące reguły:

- **Automatyzacja (`scripts/` vs `tools/`):** Domyślnym folderem automatyzacji jest `scripts/`. W projektach natywnych (C++, Rust) dopuszczalne jest używanie katalogu `tools/` (np. na kompilatory, telemetrię, generatory kodu) zamiast lub obok `scripts/`.
- **ZAKAZ umieszczania kodu w root:** Cały kod źródłowy musi znajdować się wewnątrz `src/`.
- **ZAKAZ umieszczania danych w root:** Wszelkie zrzuty i bazy lokalne muszą trafiać do `data/`.
- **ZAKAZ luźnej dokumentacji:** W root dopuszczalna jest wyłącznie "Złota Trójca" (`README.md`, `LICENSE`, `CHANGELOG.md`/`STATUS.md`). Wszelkie inne dokumenty lądują w `docs/`.
