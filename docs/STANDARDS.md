[Strona główna](../README.md) > [Dokumentacja](README.md) > [Standardy](STANDARDS.md)

---

# Standardy Inżynieryjne Projektu

Niniejszy projekt został zainicjalizowany na bazie szablonu **[template-single-app](../../template-single-app/README.md)** i bezwzględnie przestrzega globalnych reguł zdefiniowanych w centralnej Konstytucji **[devex-standards](../../devex-standards/README.md)**.

---

## 1. Zgodność ze Standardami Zewnętrznymi

| Standard | Implementacja w Projekcie | Oficjalna Specyfikacja |
| :--- | :--- | :--- |
| **Conventional Commits** | Commitlint + Husky (język angielski w commitach) | [conventionalcommits.org](https://www.conventionalcommits.org/pl/v1.0.0/) |
| **Semantic Versioning** | SemVer (`MAJOR.MINOR.PATCH`) + tagi `vX.Y.Z` | [semver.org](https://semver.org/lang/pl/) |
| **Keep a Changelog** | [`CHANGELOG.md`](../CHANGELOG.md) wg specyfikacji 1.1.0 | [keepachangelog.com](https://keepachangelog.com/pl/1.1.0/) |
| **ADR** | Rejestr w [`docs/adr/`](adr/README.md) na podstawie wzorca `0000-*.md` | [adr.github.io](https://adr.github.io/) |
| **EditorConfig** | [`.editorconfig`](../.editorconfig) w root dla spójności IDE | [editorconfig.org](https://editorconfig.org/) |
| **TSDoc / Doxygen** | Dokumentacja publicznych funkcji i interfejsów w `src/` | [tsdoc.org](https://tsdoc.org/) |

---

## 2. Bramki Jakościowe i Pokrycie Testami (Pragmatic Coverage)

Projekt stosuje zasadę pragmatycznego pokrycia per warstwa (brak gonienia ogólnego %):
- **Logika domenowa (`src/`):** docelowo ≥ 85%
- **Integracje i serwisy:** docelowo ≥ 75%
- **Powłoki UI / widoki:** weryfikacja przez testy E2E ([`tests/e2e/`](../tests/e2e/README.md))

---

## 3. Nadrzędne Źródło Prawdy (SSOT)
Szczegółowe zasady kodu (Zod, Result Object, CSS Modules, Czystość Root, Reguły AI) dziedziczone są z:
👉 **[devex-standards/docs/architecture/RULES.md](../../devex-standards/docs/architecture/RULES.md)**
👉 **[devex-standards/docs/tooling/RULES.md](../../devex-standards/docs/tooling/RULES.md)**
