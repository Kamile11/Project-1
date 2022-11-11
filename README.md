# Studentų galutinio balo skaičiuoklė v0.1 #
Programa skirta apskaičiuoti kiekvieno studento galutinį balą panaudojant vidukį/medianą.

- - - 
## Veikimo principas ##
1. Vartotojas įvedą studento vardą ir pavardę. Studentų kiekis nėra ribojamas. Suvedus reikiamus duomenis apie studentą, vartotojas gauna užkalausą: "Ar norite ivesti dar vieno studento duomenis: [y/n]";
2. Vartotojas turi pasirinkimą namų darbų pažymius ir egzamino rezultatą suvesti rankiniu būdų arba sugeneruoti atsitiktinai. Užklausa:  "Ar norite atsitiktinai generuoti pazymius? [y/n]";
  2.2 Jei pazymius vartotojas veda pats. Vartotojas įvedą egzamino pažymį ir taip pat iki 10 namų darbų pažymių;
3. Galutinis pažymys yra apsakičiaujamas tiek su pažymių vidurkiu, tiek ir su mediana;

Programa išvedą studentų vardus ir pavardes bei studentų galutinius pažymius suskaičiuotus su pažymiu vidurkiu ir mediana.

# Antroji užduotis v0.2 #
Šioje versijoje yra apskaičiuojamas studento ar studentų galutinis įvertinimas.

- - - 
## Veikimo principas ##
1. v0.1 buvo papildyta, tuo kad dabar galima duomenis ne tik įvesti bet ir nuskaityti iš failo. Vartotojui suteikiamas pasirinkimas.
2. Studentai yra surūšiuojami pagal vardus.
3. Funkcijos, nauji duomenų tipai buvo perkelti į antraštinius (header) failus, bei sukurti trys nauji .cpp failai.
4. Minimaliai panaudotas išimčių valdymas.

# Trečioji užduotis v0.3 #
Šioje versijoje yra apskaičiuojamas studento ar studentų galutinis įvertinimas;

- - - 
## Veikimo principas ##
1. Atsirado nauja funkcija Failų generacija. Vartotojas pasirenka kiek studentų ir kiek studentų pažymių bus.
2. Studentai yra surušiuojami į dvi grupes; vargšiukai ( x>5 ) ir gudročiai ( x<5 ).
3. Studentai atspausdinami į du skirtingus failus.

# Ketvirtoji užduotis v0.4 #

- - - 
## Veikimo principas ##
Šioje versijoje yra apskaičiuojamas studento ar studentų galutinis įvertinimas;
1. Buvo sukurtos dvi atskiros programos su dviejais skirtingais konteineriais: vector, list.
2. Buvo atlikti laiko matavymai šių dvieju konteinerių spartumo.
3. Laiko matavimai:

|        |              | 1000         | 10000        | 100000      | 1000000    |
|--------|--------------|--------------|--------------|-------------|------------|
| Vector | Nuskaitymas  | 0.00071426 s | 0.0046599 s  | 0.0524893 s | 0.833517 s |
|        | Isskirstymas | 0.00017619 s | 0.00187795   | 0.01768 s   | 0.442079 s |
| List   | Nuskaitymas  | 0.00068584 s | 0.00538527 s | 0.0978146 s | 1.08923 s  |
|        | Isskirstymas | 0.00017354 s | 0.00249038 s | 0.018878 s  | 0.331265 s |

Analizė: 
Greičiausias suskirstymas studentu į skirtingus konteinerius - vector;
Greičiausias failo nuskaitymas ir suskaičiavimas - List;

# Penktoji užduotis v1.0 #

- - - 
## Veikimo principas ##
Šioje versijoje yra apskaičiuojamas studento ar studentų galutinis įvertinimas;
1. Buvo ištestuotos 2 strategijos - vector, list konteineriams

| Konteineris | Kiekis  | 1 strategija  | 2 strategija |
|-------------|---------|---------------|--------------|
| Vector      | 1000    | 0.000167511 s | 0.00385861 s |
|             | 10000   | 0.00183247 s  | 0.745063 s   |
|             | 100000  | 0.0228837 s   | 82.761 s     |
|             | 1000000 | 0.511233 s    |       -      |
|             |         |               |              |
| List        | 1000    | 0.00014788 s  | 0.0001256 s  |
|             | 10000   | 0.00150157 s  | 0.00136816 s |
|             | 100000  | 0.0188806 s   | 0.011321 s   |
|             | 1000000 | 0.485813 s    | 0.141843 s   |

Analizė:
1 strategija greitesnė - List konteineriu;
2 strategija greitesnė - List konteineriu;
2. Pritaikyti algoritmai studentų dalijimo procedūrai paspartinti (vector - konteinerio) - pritaikytas remove_if algoritmas

| Strategija    | Kiekis  | Studentu iskirstymas i viena varksiuku vektoriu |
|---------------|---------|-------------------------------------------------|
|               |         |                                                 |
| II strategija | 1000    | 0.00385861 s                                    |
| erase         | 10000   | 0.745063 s                                      |
|               | 100000  | 82.761 s                                        |
|               | 1000000 | -                                               |
|               |         |                                                 |
| Algoritmas    | 1000    | 0.00019944 s                                    |
| remove_if     | 10000   | 0.00139885 s                                    |
|               | 100000  | 0.0148008 s                                     |
|               | 1000000 | 0.322558 s                                      |

II strategija pagreitėjo ir optimizavosi panaudojus remove_if algoritmą.

### Versijos ###
*[v0.1](https://github.com/Kamile11/Project-1.git) - pirminė programos versija.
*[v0.2] 
*[v0.3]
*[v0.4]
*[v1.0]

