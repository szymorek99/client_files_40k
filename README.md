# Metin2 Client Source – File Overview

Dokument zawiera opis plików źródłowych klienta Metin2.
Styl i forma opisu są zgodne z dokumentacją server source.

---

## CLIENT (Core)

- **main.cpp**  
  Główny punkt wejścia klienta.  
  Inicjalizacja DirectX, okna gry oraz uruchomienie pętli aplikacji.

- **PythonApplication.cpp / .h**  
  Główna pętla klienta.  
  Łączy silnik C++ z warstwą Python (UI, logika klienta).

- **PythonNetworkStream.cpp / .h**  
  Odpowiada za komunikację z serwerem.  
  Wysyłanie i odbieranie pakietów sieciowych.

- **Game.cpp / .h**  
  Logika klienta gry.  
  Stany gry, przejścia między ekranami (login, wybór postaci, gra).

- **Packet.h**  
  Definicje pakietów sieciowych po stronie klienta.  
  Musi być zgodne z `packet.h` po stronie servera.

---

## UserInterface

- **PythonUI.cpp / .h**  
  Obsługa systemu UI po stronie C++.

- **ui.py**  
  Główny plik interfejsu użytkownika.

- **uicommon.py**  
  Wspólne komponenty UI (okna, przyciski, inputy).

- **uiscript/**  
  Skrypty layoutów UI.  
  Okna ekwipunku, sklepów, NPC, questów itd.

---

## GameLib

- **ActorInstance.cpp / .h**  
  Reprezentacja postaci i mobów po stronie klienta.

- **GameEventManager.cpp / .h**  
  Obsługa eventów klienta.

- **ItemManager.cpp / .h**  
  Zarządzanie przedmiotami po stronie klienta.

---

## EterLib

- **GrpDevice.cpp / .h**  
  Inicjalizacja DirectX 8.

- **GrpImage.cpp / .h**  
  Renderowanie tekstur.

- **Camera.cpp / .h**  
  Kamera gry.

- **Light.cpp / .h**  
  Oświetlenie sceny.

---

## EffectLib

- **EffectManager.cpp / .h**  
  Zarządzanie efektami wizualnymi (skille, buffy).

- **EffectInstance.cpp / .h**  
  Instancje efektów w grze.

---

## MilesLib

- **MilesSound.cpp / .h**  
  System dźwięku (Miles Sound System).

---

## ScriptLib

- **PythonScriptLoader.cpp / .h**  
  Ładowanie skryptów Python.

- **PythonUtils.cpp / .h**  
  Funkcje pomocnicze do obsługi Pythona.

---

## PackLib

- **PackManager.cpp / .h**  
  Obsługa plików `.epk` / `.eix`.

- **FileLoader.cpp / .h**  
  Odczyt plików z paczek clienta.

---

## Network

- **NetStream.cpp / .h**  
  Niskopoziomowa obsługa socketów.

- **NetworkAddress.cpp / .h**  
  Adresy IP i porty połączeń.

---

## Locale & Data

- **locale/**  
  Tłumaczenia klienta, teksty NPC, UI.

- **pack/**  
  Modele, tekstury, UI, efekty, mapy.

---

## Informacje końcowe

- Client napisany w **C++ + Python**
- Render: **DirectX 8**
- UI: **Python**
- Pakiety: **muszą być zgodne z server source**
- Client **nie posiada logiki gry** (walka, drop, questy)  
  – wszystko jest walidowane po stronie servera

---
