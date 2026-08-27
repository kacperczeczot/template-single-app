[Strona główna](../README.md) > [tests](README.md)

---

# `tests/` (Testy Globalne)

* **Status:** 🟡 `[ZALECANY]`

Katalog przeznaczony na testy wyższego rzędu, których nie da się skolokować bezpośrednio przy pojedynczych plikach wewnątrz `src/`.

---

## Podział Testów (Poziom 2)

| Podkatalog | Ścieżka | Status | Przeznaczenie |
| :--- | :--- | :--- | :--- |
| [Testy E2E](e2e/README.md) | [tests/e2e/](e2e/README.md) | 🟡 `[ZALECANY]` | Testy End-to-End, scenariusze użytkownika, symulacje |
| [Testy Integracyjne](integration/README.md) | [tests/integration/](integration/README.md) | 🟡 `[ZALECANY]` | Integracja z bazą danych, testy adapterów i serwisów |

> [!NOTE]
> **Zasada Kolokacji:** Testy jednostkowe (Unit Tests) komponentów i funkcji powinny znajdować się bezpośrednio obok kodu wewnątrz `src/` (np. `src/auth/login.test.ts`).
