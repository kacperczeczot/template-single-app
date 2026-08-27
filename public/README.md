[Strona główna](../README.md) > [public](README.md)

---

# `public/` (Statyczne Zasoby Webowe)

* **Status:** ⚪ `[OPCJONALNY]`

Katalog przeznaczony na pliki serwowane bezpośrednio pod ścieżką główną domeny przez frameworki webowe (Astro, Vite, Next.js):
- `robots.txt`, `favicon.ico` / `favicon.svg`, `sitemap.xml`.
- Manifesty aplikacji internetowych (`manifest.json`, ikony PWA).
- Pliki weryfikacyjne domen i panele CMS (np. Pages CMS `/admin/`).

> [!NOTE]
> **`public/` vs `assets/`:** Pliki w `public/` są serwowane *verbatim* (wprost do przeglądarki bez hashowania i bundlowania). Źródłowe grafiki, modele 3D, audio oraz pliki do druku PnP gier umieszczaj w `assets/`.
