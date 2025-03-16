# GRK - Kocie Muzeum – Aplikacja do nauki grafiki komputerowej i symulacji ruchu
### Twórcy
- Michał Łuczak - oświetlenie, cienie, kolizje
- Bartosz Hornung - algorytm aabb, interakcje z boidami
- Katarzyna Róg & Maciej Kot - wizualny wygląd, umiejscowienie oraz tekstury obiektów

### Opis projektu

Kocie Muzeum to interaktywna aplikacja stworzona w celu nauki grafiki komputerowej, renderowania w OpenGL oraz symulacji ruchu obiektów w przestrzeni 3D. Projekt łączy elementy sztucznej inteligencji, fizyki symulacyjnej oraz wizualizacji trójwymiarowej, umożliwiając użytkownikowi eksplorację muzeum, w którym poruszają się boidy – wirtualne obiekty inspirowane zachowaniem zwierząt stadnych.

Aplikacja pozwala użytkownikowi na swobodną eksplorację świata, interakcję z obiektami i dynamiczną obserwację ruchu boidów w przestrzeni muzeum. Dzięki zastosowaniu programów shaderowych oraz zaawansowanych algorytmów kolizji, środowisko wirtualne jest realistyczne i immersyjne.

## Główne funkcjonalności
- Interaktywna eksploracja muzeum – użytkownik może swobodnie poruszać się po otoczeniu.
- Symulacja zachowań grupowych (boidów) – separacja, wyrównanie, spójność.
- Realistyczne kolizje – zarówno między boidami, jak i z elementami otoczenia (ściany, podłoga, sufit).
- Algorytm AABB (Axis-Aligned Bounding Box) – optymalizacja detekcji kolizji.
- Dynamiczne oświetlenie i cieniowanie – lepsza percepcja przestrzeni.
- Interakcje z obiektami muzealnymi – możliwość oglądania eksponatów i wchodzenia w interakcję z otoczeniem.
- Swobodny ruch kamery – użytkownik może zmieniać perspektywę i obserwować zachowanie boidów z różnych kątów.

## Stos technologiczny
- Silnik symulacji: Algorytm boidów w języku C++ .
- Silnik graficzny: OpenGL do renderowania obiektów.
- Shader Program: Obsługa cieniowania poprzez GLSL.
## Biblioteki wspierające:
- GLM – operacje na wektorach i macierzach.
- GLEW – obsługa funkcji OpenGL.
- GLFW – zarządzanie oknem i kontekstem OpenGL.

## Jak działa system
Eksploracja muzeum – użytkownik może swobodnie poruszać się po przestrzeni muzealnej, korzystając z mechaniki sterowania kamerą.
Symulacja boidów – wirtualne stworzenia poruszają się według zasad separacji, wyrównania i spójności.
Detekcja kolizji (AABB) – system sprawdza, czy boidy zderzają się ze sobą lub z obiektami otoczenia.
Dynamiczne oświetlenie i cienie – zapewniają realistyczną oprawę wizualną.
Interakcje z eksponatami – użytkownik może podchodzić do obiektów i oglądać je z różnych perspektyw / wpływać na zachowanie boidów

### Podsumowanie
Kocie Muzeum to eksperymentalna aplikacja edukacyjna, która pozwala na zrozumienie podstaw grafiki komputerowej, symulacji ruchu i interakcji w środowisku 3D. Dzięki wykorzystaniu OpenGL, programów shaderowych i algorytmu boidów, projekt oferuje realistyczne odwzorowanie zachowań grupowych oraz immersyjne środowisko muzealne. Jest to idealna platforma do nauki, eksploracji oraz testowania różnych koncepcji związanych z grafiką komputerową i symulacją fizyczną.

Co można poprawić?
1. Czystość kodu i organizacja
- ✅ Segmentacja kodu – część funkcji mogłaby zostać lepiej podzielona na mniejsze moduły, co poprawiłoby czytelność.
- ✅ Dokumentacja kodu – większa liczba komentarzy w kodzie ułatwiłaby przyszłą rozbudowę projektu.
- ✅ Unifikacja stylu kodowania – jednolity styl kodowania (np. konwencje nazewnicze) może zwiększyć przejrzystość kodu.

2. Optymalizacja algorytmów
- ✅ Lepsza obsługa kolizji – obecnie AABB działa poprawnie, ale można zoptymalizować przeszukiwanie boidów poprzez np. drzewa BVH (Bounding Volume Hierarchy) lub grid przestrzenny.
- ✅ Ulepszenie zachowania boidów – bardziej realistyczne unikanie kolizji i płynniejsze ruchy mogą poprawić wrażenia wizualne.

3. Interfejs i interakcje
- ✅ Bardziej intuicyjne sterowanie kamerą – aktualnie ruch kamery może wymagać dopracowania w zakresie ergonomii.
- ✅ Większa interaktywność muzeum – możliwość bardziej zaawansowanych interakcji z obiektami, np. otwieranie opisów eksponatów, aktywacja specjalnych animacji.

4. Warstwa wizualna i efekty
- ✅ Dopracowanie oświetlenia – dynamiczne światła i lepsze cieniowanie mogą nadać bardziej realistyczny wygląd.
- ✅ Lepsze tekstury i materiały – wykorzystanie bardziej zaawansowanych shaderów do poprawy wyglądu obiektów.
