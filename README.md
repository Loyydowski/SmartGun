# SmartGun
A DIY embedded system project combining hardware and software to create a smart “Iron Man” style water blaster.

> **Status:** 🚧 Early Designing (WIP)  
> **Tech Stack:** C++, ESP32, OLED, IMU, Embedded Systems

 ### 📊 Status prac
![Progress Bar](https://geps.dev/progress/0)


## 🎯 O Projekcie
**HydroHUD** to projekt inżynierski mający na celu stworzenie zaawansowanego systemu "Iron Man" dla pistoletu na wodę. Projekt łączy elektronikę, optykę i programowanie systemów wbudowanych, aby przekształcić zwykłą zabawkę w taktyczny gadżet z systemem rozszerzonej rzeczywistości (AR/HUD).

Głównym celem jest stworzenie nakładki na okulary (Heads-Up Display), która komunikuje się bezprzewodowo lub przewodowo z pistoletem, wyświetlając kluczowe parametry w czasie rzeczywistym.

## ✨ Główne Funkcjonalności

* **Monitorowanie Amunicji:** Pomiar poziomu wody w zbiorniku w czasie rzeczywistym i wyświetlanie go jako procent "Ammo".
* **Wearable HUD (Heads-Up Display):** Okulary z wyświetlaczem OLED i optyką (beam splitter), prezentujące dane bezpośrednio przed okiem użytkownika.
* **Dynamiczny Celownik:** Krzyżyk celowniczy reagujący na ruch głowy i pistoletu (stabilizacja/pozycjonowanie).
* **System Radarowy (Eksperymentalny):** Wykrywanie ruchu w promieniu 360 stopni (ostrzeganie przed zbliżającym się celem).

## 🛠️ Architektura Sprzętowa (Hardware)

System oparty jest na mikrokontrolerach z rodziny ESP32/Arduino. Poniżej znajduje się zestawienie planowanych komponentów:

| Moduł | Komponent | Opis / Zastosowanie |
| :--- | :--- | :--- |
| **MCU** | **ESP32** | Główny mózg operacji (obsługa wielu czujników + potencjalne Wi-Fi/BLE). |
| **Pistolet** | **HC-SR04** lub Czujnik Ciśnienia | **Opcja A (Poziom):** Ultradźwiękowy pomiar lustra wody.<br>**Opcja B (Ciśnienie):** Pomiar słupa cieczy. |
| **Pistolet** | **Flow Sensor** | **Opcja C (Przepływ):** Zliczanie impulsów przy każdym strzale (alternatywa). |
| **HUD** | **OLED 0.96" / Micro OLED** | Wyświetlanie interfejsu graficznego. |
| **HUD** | **Szybka + Beam Splitter** | Układ optyczny do rzutowania obrazu na okulary. |
| **IMU** | **MPU6050** | Akcelerometr i żyroskop do śledzenia ruchów i obsługi celownika. |
| **Radar** | **PIR / Mikrofale / LiDAR** | Wykrywanie ruchu wokół użytkownika (zależnie od budżetu). |

## 🗺️ Roadmapa (Etapy Rozwoju)

Projekt realizowany jest w modelu przyrostowym:

### Faza 1: MVP (Minimum Viable Product) 🏁
- [ ] Implementacja pomiaru poziomu wody (czujnik w zbiorniku).
- [ ] Podłączenie wyświetlacza OLED.
- [ ] Wyświetlanie statycznego celownika (krzyżyk) i % amunicji.
- [ ] Montaż elektroniki na prototypowej ramie okularów.

### Faza 2: Dynamika i Precyzja 🎯
- [ ] Integracja modułu IMU (MPU6050).
- [ ] Algorytm przeliczania kąta wychylenia na pozycję celownika na ekranie.
- [ ] Kalibracja układu optycznego.

### Faza 3: Advanced Situational Awareness 📡
- [ ] Dodanie czujników ruchu (PIR lub moduły mikrofalowe).
- [ ] Wizualizacja "radaru" lub ostrzeżeń na HUD.
- [ ] Optymalizacja zużycia energii i miniaturyzacja obudowy (druk 3D).



---
*Projekt inspirowany snem, realizowany przez inżynierię.* 🔧
