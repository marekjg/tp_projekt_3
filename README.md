# Techniki Programowania - projekt 3
Projekt polega na zbudowaniu biblioteki w c++ do przetwarzania sygnałów. Biblioteka ma być udostępniona jako moduł pythonowy przy użyciu biblioteki pybind11.

## Zależności
W celu realizacji projektu należy przygotować środowisko pracy. Niezbędne będą:
1. CMake
2. Kompilator (MSVC2019 na Windowsie, g++ na linuksie)
3. git (git bash/ git for desktop na windowsie, git na linuksie)
4. Python (najlepiej miniconda)

<details><summary><b>Windows</b></summary>
<p>

[CMake](https://cmake.org/download/)

[MSVC](https://visualstudio.microsoft.com/pl/vs/community/)

[git](https://git-scm.com/download/win)

[miniconda](https://docs.anaconda.com/free/miniconda/index.html)

</p>
</details>

<details><summary><b>Ubuntu</b></summary>
<p>

```bash
sudo apt install build-essential cmake git
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
chmod +x Miniconda3-latest-Linux-x86_64.sh
./Miniconda3-latest-Linux-x86_64.sh
```

</p>
</details>

## Szablon projektu
Jako punkt wyjściowy najwygodniej jest pobrać przykład udostępniony przez autorów pybind11:

```bash
git clone https://github.com/pybind/scikit_build_example
```

## Zadanie projektowe
Funkcjonalność do zaimplementolwania:
1. Wizualizacja sygnału z wykorzystaniem biblioteki [matplotplusplus](https://github.com/alandefreitas/matplotplusplus)
2. [DFT](https://en.wikipedia.org/wiki/Discrete_Fourier_transform) i transformata odwrotna
3. [Filtracja 1D i 2D](https://docs.scipy.org/doc/scipy/tutorial/signal.html#filtering)
4. [Pochodna sygnału](https://en.wikipedia.org/wiki/Finite_difference)
5. Generowanie sygnałów o zadanej częstotliwości (sin, cos, prostokątny, piłokształtny)
6. Wykrywanie krawędzi (korzystajac z 3.)
7. Rozmycie gaussa (korzystajac z 3.)
8. Wykrywanie piku w sygnale dowolną metodą
9. Progowanie sygnału (1 dla > progu, 0 dla mniejszego)
10. Usuwanie niskich/wysokich częstotliwości z sygnału
