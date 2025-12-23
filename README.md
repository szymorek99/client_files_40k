# Metin2 Client Source – File Overview

Dokument zawiera opis katalogów klienta Metin2.
Opisy mają charakter techniczny i zachowują prostą, rzeczową formę.

---

## CWebBrowser

- Integracja wbudowanej przeglądarki w kliencie gry.
- Używane m.in. do wyświetlania stron eventowych, regulaminów lub paneli webowych.

---

## Discord

- Integracja klienta gry z Discordem.
- Odpowiada za Discord Rich Presence (status gry, lokalizacja, postać).

---

## EffectLib

- Biblioteka efektów wizualnych.
- Obsługuje efekty umiejętności, buffów, hitów, animacji specjalnych.

---

## EterBase

- Podstawowe klasy i definicje używane w całym kliencie.
- Typy danych, makra, narzędzia pomocnicze.

---

## EterGrnLib

- Obsługa modeli w formacie `.grn`.
- Animacje, szkielety, przypisania do postaci i mobów.

---

## EterImageLib

- Obsługa tekstur i obrazów.
- Ładowanie, zarządzanie i render grafik w kliencie.

---

## EterLib

- Główna biblioteka renderująca.
- Odpowiada za DirectX 8, kamerę, światło, scenę oraz rendering świata gry.

---

## EterLocale

- Obsługa lokalizacji językowych klienta.
- Ładowanie tekstów, tłumaczeń oraz ustawień regionalnych.

---

## EterPack

- System paczek klienta (`.eix` / `.epk`).
- Odczyt plików danych, tekstur, map i UI z paczek.

---

## EterPythonLib

- Warstwa łącząca C++ z Pythonem.
- Udostępnia funkcje silnika do skryptów Python.

---

## GameLib

- Logika klienta gry.
- Obsługa postaci, mobów, przedmiotów i interakcji po stronie klienta.

---

## MilesLib

- System dźwięku klienta.
- Odpowiada za muzykę, dźwięki efektów i otoczenia.

---

## PRTerrainLib

- Obsługa terenu gry.
- Wczytywanie map, wysoko powiedni, kolizji oraz podłoża.

---

## ScriptLib

- Obsługa skryptów Python.
- Ładowanie, interpretacja i wykonywanie skryptów klienta.

---

## SpeedTreeLib

- Obsługa drzew i roślinności (SpeedTree).
- Renderowanie obiektów naturalnych na mapach.

---

## SphereLib

- Obsługa kolizji i obszarów sferycznych.
- Wykorzystywana w obliczeniach zasięgów i interakcji.

---

## UserInterface

- Interfejs użytkownika klienta.
- Okna gry, ekwipunek, NPC, questy, UI napisane w Pythonie.

---

## README.md

- Dokumentacja projektu.
- Opis struktury client source.

---

## Informacje końcowe

- Client napisany w **C++ + Python**
- Render oparty o **DirectX 8**
- UI w całości obsługiwane przez **Python**
- Client odpowiada za render, input i prezentację danych  
- Logika gry i walidacja danych znajdują się po stronie **server source**

---
