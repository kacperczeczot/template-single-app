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

## 4. Czystość Katalogu Root
Katalog główny (`root`) służy wyłącznie jako tablica rozdzielcza dla narzędzi i konfiguracji. Zakazuje się tworzenia nowych folderów w root oraz umieszczania w nim luźnych plików z kodem źródłowym, danymi czy swobodnymi notatkami.
