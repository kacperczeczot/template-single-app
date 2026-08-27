---
name: Uniwersalne Reguły AI
description: Twarde reguły określające zachowanie agentów i asystentów AI wewnątrz projektu.
---

# Reguły Współpracy z AI

## 1. Zero Samowolki
AI ma absolutny zakaz wprowadzania jakichkolwiek modyfikacji do istniejących plików, tworzenia nowych katalogów czy uruchamiania skryptów bez wyraźnej, bezpośredniej prośby ze strony użytkownika. Każda większa zmiana architektoniczna wymaga zatwierdzenia.

## 2. Przenośność i Brak Hardcodowania
AI ma bezwzględny zakaz "hardcodowania" (zaszywania na sztywno) konkretnych nazw repozytoriów biznesowych oraz bezwzględnych ścieżek z lokalnego komputera w generowanym przez siebie kodzie źródłowym. Kod ma być zawsze przenośny i oparty na ścieżkach relatywnych lub zmiennych środowiskowych.

## 3. Standardy Technologiczne dla AI
- **Walidacja Danych:** Zawsze używaj biblioteki `zod` do walidacji danych zewnętrznych na wszystkich stykach aplikacji (IPC, API).
- **Stylowanie:** Zawsze używaj `CSS Modules` w projektach frontendowych. Unikaj stylów globalnych.
- **Błędy:** Stosuj wzorzec "Result Object" zapobiegający niezłapanym wyjątkom na poziomie domenowym.
