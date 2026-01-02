# Dashboard Sprzedaży i Rentowności – Coffee Roast Co.

![Dashboard Coffee Roast Co - Analiza Liberica](dashboard.png)

## 1. Cel projektu
Celem projektu było przygotowanie interaktywnego raportu operacyjnego dla dystrybutora kawy **"Coffee Roast Co."**. Dashboard służy do monitorowania kluczowych wskaźników efektywności (KPI) oraz wspierania decyzji handlowych na rynkach USA, Wielkiej Brytanii i Irlandii w oparciu o dane historyczne z lat 2019–2022.

## 2. Źródło i struktura danych
Źródło danych: W projekcie wykorzystano otwarty zbiór danych udostępniony przez Mo Chena w celach edukacyjnych.
Analiza bazuje na trzech arkuszach w pliku Excel:
* **Orders:** Rejestr transakcji (ID zamówienia, daty, ilości).
* **Customers:** Dane o klientach, lokalizacji oraz statusie lojalnościowym.
* **Products:** Cennik, koszty jednostkowe oraz specyfikacja gatunków kawy.

## 3. Pytania biznesowe
Raport został zaprojektowany tak, aby odpowiadać na następujące pytania:
* **Trendy sprzedaży:** Jak zmieniały się przychody w czasie i które kraje dominują w sprzedaży?
* **Analiza asortymentu:** Które gatunki kawy (Arabica, Robusta, Liberica, Excelsa) są najbardziej zyskowne?
* **Efektywność lojalności:** Jaki udział w wynikach mają klienci korzystający z karty lojalnościowej?
* **Koncentracja klientów:** Jak duży wpływ na całkowity przychód ma 5 największych odbiorców?

## 4. Wykorzystane narzędzia i techniki
* **Excel – Przygotowanie danych (ETL):** Połączenie danych z trzech arkuszy za pomocą funkcji **XLOOKUP** oraz **INDEX/MATCH**. Oczyszczanie danych oraz stworzenie autorskich kolumn obliczeniowych w celu wyliczenia zysku netto dla każdego zamówienia.
* **Excel – Analiza:** Wykorzystanie Tabel Przestawnych do agregacji danych oraz pól obliczeniowych do wyliczenia marży procentowej.
* **Zaawansowana interaktywność:** Zastosowanie **statycznych punktów odniesienia (Baseline)** – wskaźniki Total Revenue i Total Profit zostały celowo odłączone od fragmentatorów, aby umożliwić stałe porównanie wyników wybranego segmentu do skali całej firmy.
* **Dashboard:** Wykorzystanie osi czasu (**Timeline**) oraz fragmentatorów (**Slicers**) do dynamicznego filtrowania danych według: czasu, gatunku kawy, stopnia wypalenia, wielkości opakowania oraz statusu karty lojalnościowej.

## 5. Kluczowe wskaźniki (KPI)
Na dashboardzie zastosowano system dynamicznych kart KPI, które pokazują wartości bezwzględne oraz ich procentowy udział w skali całej firmy:
* **Total Revenue & Total Profit:** Statyczne punkty odniesienia pokazujące całkowitą skalę operacji firmy.
* **Segment Revenue (% of Total Revenue):** Udział wybranego segmentu w całkowitym przychodzie.
* **Segment Profit (% of Total Profit):** Kluczowy wskaźnik rentowności danego segmentu na tle całej firmy.
* **Segment Orders (% of Total Orders):** Udział segmentu w całkowitej liczbie zamówień.

---

## 6. Kluczowe wnioski

### 📈 Trendy sprzedaży i analiza geograficzna
Przychody firmy charakteryzowały się stabilnym wzrostem z poziomu 12,2 tys. USD (lata 2019-2020) do 13,8 tys. USD w 2021 roku (wzrost o ok. **13%**). Dane z 2022 roku wskazują na wyhamowanie dynamiki.
* **Dominacja USA:** Udział rynku USA systematycznie rośnie – z 78% w 2019 roku do rekordowych **82%** w 2022 roku.
* **Wniosek:** Firma staje się silnie uzależniona finansowo od jednego kraju.
* **Rekomendacja:** Należy podjąć działania marketingowe na rynkach europejskich, aby zdywersyfikować źródła przychodu i zmniejszyć ryzyko geograficzne.

### ☕ Analiza asortymentu i rentowności (Segment Share)
Zastosowanie statycznego punktu odniesienia pozwoliło na precyzyjne odkrycie istotnych dysproporcji:
* **Wysoka rentowność Liberiki:** Odpowiada za 25% liczby zamówień, ale generuje aż **35% całkowitego zysku** firmy (1,57 tys. USD). Jest to najbardziej marżowy produkt.
* **Niska efektywność Robusty:** Mimo dużej popularności (24% zamówień), jej realny wpływ na całkowity zysk to tylko **12%** (0,54 tys. USD).
* **Wniosek:** Optymalizacja oferty powinna skupiać się na promocji Liberiki, zamiast na walce o wolumen niskomarżowej Robusty.

### 💳 Efektywność programu lojalnościowego
* **Fundament sprzedaży:** Klienci z kartą lojalnościową odpowiadają za blisko połowę wyników firmy (**48% zamówień oraz 46% zysku**).
* **Zmiana w 2021 roku:** W rekordowym dla firmy roku odnotowano nagły wzrost udziału zamówień od osób spoza programu lojalnościowego.
* **Dalsze kroki:** Należałoby przeanalizować unikalne ID klientów, aby sprawdzić, czy wzrost ten wynika z pozyskania nowych osób, czy z rezygnacji obecnych klientów z korzystania z karty.

### 👥 Koncentracja klientów (Customer Concentration)
* **Bezpieczeństwo:** Top 5 największych klientów generuje łącznie jedynie **5,85% całkowitego przychodu** firmy (największy z nich odpowiada za 1,31%).
* **Wniosek:** Tak niskie skupienie przychodu oznacza, że sprzedaż jest doskonale rozproszona. Firma nie jest uzależniona od pojedynczych odbiorców, co zapewnia jej wysoką stabilność finansow
