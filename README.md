# TurboRower - System Zarządzania Flotą Mikromobilności

System dedykowany do kompleksowej obsługi rozproszonej floty elektrycznych hulajnóg i rowerów miejskich. Projekt obejmuje monitorowanie pojazdów w czasie rzeczywistym, automatyzację serwisu oraz egzekwowanie stref wirtualnych (Geofencing).

## O projekcie
„TurboRower” to platforma łącząca operatora floty, ekipy terenowe oraz użytkowników końcowych. System rozwiązuje kluczowe problemy logistyczne związane z utrzymaniem wysokiej dostępności pojazdów w przestrzeni miejskiej.



## Kluczowe Funkcjonalności

### 1. Zarządzanie Flotą i Telemetria
* **Real-time Tracking:** Monitorowanie lokalizacji, stanu technicznego i poziomu baterii każdego pojazdu.
* **Smart Alerts:** Automatyczne generowanie zleceń dla Ekip Terenowych przy niskim stanie energii (< próg krytyczny) lub zgłoszeniu usterki.

### 2. Geofencing (Wirtualne Strefy)
* Definiowanie obszarów z ograniczeniami bezpośrednio w systemie.
* Automatyczne egzekwowanie limitów prędkości (np. na deptakach) oraz blokada parkowania w strefach wyłączonych (np. parki).

### 3. Obsługa Użytkownika i Płatności
* **Elastyczne Taryfy:** Obsługa płatności za minutę, subskrypcje oraz rezerwację pojazdów.
* **Integracja Finansowa:** Automatyczne raportowanie i rozliczanie przychodów z zewnętrznym Operatorem Płatności.

### 4. Logistyka Terenowa
* System zleceń dla pracowników (wymiana baterii, transport do serwisu).
* Priorytetyzacja zadań na podstawie lokalizacji i pilności usterki.

## Architektura Systemu
* **Core:** System centralny przetwarzający dane telemetryczne.
* **Firmware Integration:** Moduł komunikacji z oprogramowaniem pojazdów.
* **API:** Interfejsy dla aplikacji mobilnej użytkownika oraz terminala Ekipy Terenowej.

## Przykładowy przepływ procesu (Workflow)
1. **Zdarzenie:** Bateria w hulajnodze X spada do 10%.
2. **Akcja:** System generuje zlecenie "Wymiana baterii".
3. **Realizacja:** Pracownik Ekipy Terenowej otrzymuje powiadomienie z GPS pojazdu.
4. **Finał:** Po wymianie stan pojazdu w systemie zmienia się na "Gotowy do jazdy".