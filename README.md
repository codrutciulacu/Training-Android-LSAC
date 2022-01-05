# Training Android

## Prerequisites
Pentru a incepe sa dezvoltati aplicatii de Android aveti nevoie de [Android Studio](https://developer.android.com/studio) si un device pe care sa rulati aplicatia(fizic sau un [emulator](https://developer.android.com/studio/run/managing-avds))

## Ce este Android?
Android este un sistem de operare destinat device-urilor mobile. Acesta platforma are mai mult de 2 miliarde de utilizatori activi lunar.

## De ce Android?
- O piata foarte mare
- Ecosistemul Android ofera o experienta placuta atat pentru dezvoltatori, cat si pentru utilizatori
- Comunitate foarte prietenoasa
- Android ofera un sistem liber si accesibil pentru toata lumea

## Prima aplicatie Android
1. Deschide Android Studio
2. Odata ce a aparut panoul **Welcome to Android Studio** selecteaza optiunea **Start a new Android Studio project.**
3. Apoi selecteaza **Empty Activity**
4. Denumeste-ti proiectul 
5. Asigura-te ca limbajul selectat este **Java** 
6. Apasa pe butonul de **Finish**

## Structura unui proiect Android
![Strictura unui proiect](/docs/grafic-structura.png "Structura proiectului")

## Intro to Java

- Clase
    - clasele sunt constructii care definesc caracteriosticiile si comporatmentele obiectelor.
    - sunt elementul de baza al limbajului Java
- Constructori
    - constructorul este prima metoda care se executa intr-o clasa. Aceasta este apelata imediat dupa creerea obietului
    - in general este folosita pentru a initializa field-urile clasei
- Modificatori de acces
    - in Java, sunt 4 tipuri de modificatori de access:
        - **private** -> cel mai restrictiv, ofera vizibilitate doar in cadrul clasei
        - **protective** -> ofera vizibilitate in cadrul clasei si a mostenitorilor ei
        - **default** -> ofera vizibilitate claselor din acelasi pachet
        - **public** -> cel mai permisiv, vizibil pentru toate clasele
- Mostenire
    - permite claselor sa preia proprietati ale altor clase
    - clasa copil devine un sub-tip al clasei parinte
    - pentru a mosteni o clasa folosim cuvantul cheie `extends`


## Intro to XML
- pentru a putea dezvolta partea de user interface a unei aplicatie vom folosi limbajul XML 
- acesta ne permite o structura ierarhica a componentelor noastre vizuale
- el are mai multe **tag-uri** si **atribute**

## Views
- un view este elementul de baza folosit de framework-ul Android pentru a defini componenete vizuale
- toate view-urile trebuie sa extinda clasa **View**
- exista 2 tiprui de view-uri: 
    - simple views
    - complex views

### Simple Views
- definesc elemente punctuale precum casute de text, butoane, checkbox-uri
- principalele view-uri din aceste categorie sunt: **TextView**, **EditText**, **Button**, **CheckBox**, **RadioButton**,  **ProgressBar**, **RatingBar**, **ImageView**

### Complex Views 
- sunt view-uri care au in componenta lor alte view-uri
- ele sunt radacina pentru layout-ul ecranului nostru
- principalele complex view-uri sunt: **LinearLayout**, **ConstraintLayout**,
**ScrollView**, **FrameLayout**, **RecyclerView**

## RecyclerView
- un view care permite afisarea unei liste de view-uri care pot ocupa mai mult decat permite ecranul
- Componente:
    - data source
    - layout-ul pentru un element al listei
    - layout manager
    - view holder
    - adapter
![RecyclerView](/docs/grafic-recyclerview.png "RecyclerView")

## Activities
- o activitate este un ecran al aplicatiei 
- fiecare activitate are un lifecycle(o serie de metode apelate in functie de starea in care se afla aplicatia)
![Activity Lifecycle](/docs/grafic-activity-lifecycle.png "Activity Lifecycle")

## Intents
- este un obiect folosit pentru a cere o actiune catre alta componenta a aplicatiei
- exista 2 tipuri de intent-uri:
    - explicit intents = pornesc o activitate definita de developer
    - implicit intents = interogheza sistemul si cauta o activitate care sa poate gestiona request-ul(call, share, open a website, etc)

## Bundles
- pentru a putea trimite date prin intermediul clasei Intent va trebuie sa ne folosim de clasa **Bundle**
- aceasta clasa ne permite sa trimitem date primitive sau serializabile


