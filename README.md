# 2020L-WarsztatyBadawcze-Imputacja

## Plan zajęć
* 2020-02-25 - O co chodzi z artykułami naukowymi?
    - [Learning Multiple Defaults for Machine Learning Algorithms](https://arxiv.org/pdf/1811.09409.pdf) 
    - [FHDI: An R Package for Fractional Hot Deck Imputation](https://journal.r-project.org/archive/2018/RJ-2018-020/RJ-2018-020.pdf)
    
    Warto zobaczyć:
    - [Limitations of Interpretable Machine Learning Methods](https://compstat-lmu.github.io/iml_methods_limitations/)

* 2020-03-03 - typy braków danych, metody ad-hoc
   
* 2020-03-10 - algorytmy machine learningu, metody oceny jakości klasyfikatorów

 - [Wstęp do mlr3](https://mlr3.mlr-org.com/reference/index.html)
 - [Tutorial mlr3](https://mlr3book.mlr-org.com/introduction.html)

* 2020-03-17 - praca domowa 1

* 2020-03-24 - praca domowa 1

* 2020-03-31 - prezentacje o technikach imputacji 

* 2020-04-07 - prezentacje o technikach imputacji

* 2020-04-21 - praca domowa 2

* 2020-04-28 - projekt

* 2020-05-05 - projekt

* 2020-05-19 - projekt

* 2020-05-26 - projekt

* 2020-06-02 - projekt

* 2020-06-09 - ?

* 2020-06-16 - ?

## Prezentacje (15 pkt.)


Należy przygotować prezentację o wybranej pakiecie do imputacji danych. Prezentacje należy wykonać w grupach, najlepiej grupach projektowych. Oprócz krótkiej prezentacji z wprowadzeniem do technik użytych w danym pakiecie należy przygotować krótki skrypt z przykładem użycia pakietu. Propozycje pakietów:
- [Amelia](https://cran.r-project.org/web/packages/Amelia/index.html)
- [softImpute](https://cran.r-project.org/web/packages/softImpute/index.html)
- [missMDA](https://cran.r-project.org/web/packages/missMDA/index.html)
- [mice](https://cran.r-project.org/web/packages/mice/index.html)
- [missForest](https://cran.r-project.org/web/packages/missForest/index.html)
- [FHDI](https://cran.r-project.org/web/packages/FHDI/index.html)

Inne pakiety R dotyczace technik imputacji można znaleźć [tutaj](https://cran.r-project.org/web/views/MissingData.html)


## Prace domowe (15 pkt.)

### Praca domowa 1 
Praca domowa wykonywana jest pojednczo. 
Należy wybrać jeden zbiór danych z [OpenML100](https://www.openml.org/search?q=tags.tag%3AOpenML100&type=data&table=1&size=100), w którym występują braki danych i dla wybranego zbioru danych:

- wykonać analizę eksploracyjną,
- zastosować proste techniki obróbki brakujących danych (usunięcie kolumn, wierszy, uzupełnienie średnią lub medianą),
- wytrenować jeden algorytm uczenia maszynowego dla każdego sposobu uzupełnienia braków danych

Na podstawie otrzymanych wyników trzeba przygotować krótki raport, który będzie zawierał opis metodologii i podsumowanie wyników. Na zajęciach każdy powinien zaprezentować 5 min podsumowanie.

**Baza zbiorów danych**

W folderze [datasets](/datasets/) stworzymy bazę zbiorów danych dotyczących klasyfikacji binarnej. 
Dla każdego zbioru danych należy stworzyć podfolder o nazwie *openml_dataset_id*. W podfolderze powinien znajdować się:
- `code.R` - skrypt, w których wykonywane jest czyszczenie danych [wzór](/skrypty/code_preprocessing.R). W tym skrypcie nie należy wykonywać imputacji brakujących danych (zmiana typów danych, usunięcie kolumn, zakodowanie pewnych znaków jako `NA`).

    Ważne, aby w skrypcie ostateczny zbiór danych zapisany był w zmiennej `dataset` a nazwa kolumn ze zmienną objaśnianą `target_column`.

- `dataset.json` - plik json z najważniejszymi charakterystykami **wyczyszczonego zbioru danych**. Kod do jego wygenerowania znajduje się [tutaj](/skrypty/create_summary_json.R)

### Praca domowa 2


## Projekt (55 pkt.)
Celem projektu jest wykonanie analizy porówanwczej dla różnych zbiorów danych z brakującymi danymi jakości działania różnych technik imputacji braków danych i różnych algorytmów uczenia maszynowego.

Rezultatem prac powinien być krótki artykuł naukowy (40 pkt.), minimum 3 strony umieszczony jako rozdział książki online, która powstanie w ramach przedmiotu. Podział punktów w ramach artykułu
* Abstrakt: 5 pkt.
* Wstęp + Motywacja: 10 pkt
* Opis metodologii i wyników: 15 pkt.
* Wnioski: 10 pkt.

Projekt nalezy zaprezentować w postaci Lightning Talka na jednym z ostatnich wykładów (15 pkt.).


## Blog (15 pkt.)
Informacje w [repzytorium Wykładu](https://github.com/mini-pw/2020L-WarsztatyBadawcze)
