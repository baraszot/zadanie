# Podstawowa składnia Markdowna<!-- omit in toc -->

Markdown to uproszczony język znaczników do tworzenia sformatowanego tekstu w prostych edytorach.

- [Podział tekstu](#podział-tekstu)
  - [Akapity, podziały wierszy](#akapity-podziały-wierszy)
  - [Nagłówki](#nagłówki)
  - [Listy](#listy)
    - [Listy numerowane](#listy-numerowane)
    - [Listy nienumerowane](#listy-nienumerowane)
  - [Tworzenie spisu treści](#tworzenie-spisu-treści)
  - [Tworzenie tabel](#tworzenie-tabel)
  - [Dodawanie poziomej linii](#dodawanie-poziomej-linii)
- [Wyróżnianie tekstu](#wyróżnianie-tekstu)
  - [Kursywa, pogrubienie](#kursywa-pogrubienie)
  - [Cytaty blokowe](#cytaty-blokowe)
  - [Cytowanie kodu, znaczników itp.](#cytowanie-kodu-znaczników-itp)
- [Dodawanie elementów](#dodawanie-elementów)
  - [Odsyłacze](#odsyłacze)
  - [Obrazki](#obrazki)


## Podział tekstu

### Akapity, podziały wierszy

Przejście do nowego akapitu wymaga dwukrotnego przyciśnięcia klawisza Enter.

Między akapitami musi znajdować się pusta linia.

Aby rozpocząć tekst od nowego wiersza bez tworzenia nowego akapitu, należy poprzedzić nową linię co najmniej dwiema spacjami.   
(Sam Enter nie dałby takiego efektu.)

### Nagłówki

Nagłówki tworzy się poprzedzając tekst nagłówka znakiem lub kilkoma znakami hash. Hierarchię nagłówków wyznacza liczba hashów - im mniejsza, tym ważniejszy jest nagłówek (# - nagłówek główny, ## - stopień niżej itd.).

### Listy

#### Listy numerowane

Tworzenie listy numerowanej:

1. Należy wpisać cyfrę, po niej kropkę i spację, a następnie tekst.
1. Listę powinna rozpoczynać cyfra, od której rozpoczyna się numerowanie punktów (zazwyczaj 1), następne zaś w dokumencie wyjściowym będą wyświetlane jako kolejne liczby bez względu na to, jaką liczbę się wpisze (czyli np. wpisując same cyfry 1. i tak uzyskujemy punkty 1., 2. itd.).
2. Do przejścia do kolejnego punktu wystarcza jeden Enter.

#### Listy nienumerowane

Tworzenie listy nienumerowanej:

- Listy nienumerowane tworzy się zaczynając punkt od dywizu (-) i spacji.
- Zamiast dywizu można użyć znaku asteryksa (*) lub plusa (+).
- Do przejścia do kolejnego punktu wystarcza jeden Enter.

### Tworzenie spisu treści

Z nagłówków wygenerować można spis treści. Aby to zrobić, należy wpisać tekst nagłówka w nawias kwadratowy poprzedzony dywizem i spacją, a następnie w nawiasie okrągłym wpisać # i tekst nagłówka małymi literami oraz pozbawiony spacji (należy zastąpić je dywizem).

Format to:

>`- [Podział tekstu](#podział-tekstu)`  
`  - [Akapity, podziały wierszy](#akapity-podziały-wierszy)`  
itd.

(Jest to de facto połączenie tworzenia listy i zamieszczania odnośników, patrz [Listy nienumerowane](#listy-nienumerowane) i [Odsyłacze](#odsyłacze))

Dla ułatwienia sobie życia warto skorzystać przy tym z dodatków, które wygenerują spis treści z nagłówków dostępnych w tekście np. Markdown All in One. W przypadku nagłówków, które mają zostać pominięte w spisie treści, za tekstem nagłówka dodaje się `<!-- omit in toc -->`.

### Tworzenie tabel

Kolumny tabeli tworzy się za pomocą znaku |. Kolejny wiersz tabeli dodaje się wprowadzając kolumnę w kolejnym wierszu. Nagłówek oddziela się za pomocą wprowadzenia linii przed kolejnym wierszem.

Format to:

`|Tekst nagłówka 1|Tekst nagłówka 2|Tekst nagłówka 3|`  
`|---|---|---|`  
`|Tekst w tabeli 1|Tekst w tabeli 2|Tekst w tabeli 3|`  
`|Tekst w tabeli 4|Tekst w tabeli 5|Tekst w tabeli 6|`

Co daje w dokumencie wyjściowym następujący efekt:


|Tekst nagłówka 1|Tekst nagłówka 2|Tekst nagłówka 3|
|---|---|---|
|Tekst w tabeli 1|Tekst w tabeli 2|Tekst w tabeli 3|
|Tekst w tabeli 4|Tekst w tabeli 5|Tekst w tabeli 6|

Do wyjustowania tabeli używa się dwukropka dodanego do dywizów tworzących linię tabeli - z lewej dla wyjustowania do lewej, z prawej - do prawej i z obu stron dla wyśrodkowania tekstu.

`|Nagłówek do lewej|Nagłówek do prawej|Nagłówek wyśrodkowany|`  
`|:---|---:|:---:|`  
`|Tekst do lewej 2|Tekst do prawej 1|Tekst wyśrodkowany 1|`  
`|Tekst do lewej 4|Tekst do prawej 2|Tekst wyśrodkowany 2|`

|Nagłówek do lewej|Nagłówek do prawej|Nagłówek wyśrodkowany|
|:---|---:|:---:|
|Tekst do lewej 1|Tekst do prawej 1|Tekst wyśrodkowany 1|
|Tekst do lewej 2|Tekst do prawej 2|Tekst wyśrodkowany 2|

### Dodawanie poziomej linii

Poziomą linię rysuje się za pomocą użycia co najmniej trzech znaków asteryksa (*), dywizu (-) lub podkreślnika (_). Dodatkowo można używać między nimi spacji.

Linia narysowana za pomocą `---`,

---

za pomocą `* * *` 
* * *

i za pomocą `___`
___ 

wyglądają tak samo.

## Wyróżnianie tekstu

### Kursywa, pogrubienie

Efekt *kursywy* i **pogrubienia** osiąga się za pomocą znaku asteryksa lub podkreślnika umieszczonego na początku i na końcu tekstu, który chcemy wyróżnić - po jednym znaku z każdej strony dla kursywy i dwóch dla pogrubienia.

**Pogrubienie** tworzy się dwoma znakami z obu stron wyróżnianego tekstu: `**pogrubienie**` lub `__pogrubienie__`.  
Do _kursywy_ wystarcza jeden znak z każdej strony: `*kursywa*` lub `_kursywa_`.

### Cytaty blokowe

Cytaty blokowe wprowadza się za pomocą znaku > umieszczanego na początku linii, w której ma znaleźć się cytat. Znak ten może znajdować się na początku każdego wiersza cytatu lub tylko na początku każdego z osobnych akapitów.

Cytaty blokowe można zagnieżdżać za pomocą dodatkowego znaku >.

>Cytaty blokowe wprowadza się za pomocą znaku < umieszczanego na początku linii, w której ma znaleźć się cytat. Znak ten może znajdować się na początku każdego wiersza cytatu lub tylko na początku każdego akapitu.
>>Cytaty blokowe można zagnieżdżać za pomocą dodatkowego znaku <.

### Cytowanie kodu, znaczników itp.

Za pomocą użycia znaku ` z obu stron możemy zaznaczyć elementy, które powinny wyświetlać się na stronie w formie tekstowej. Użycie trzech znaków z obu stron generuje osobny blok tekstu np. na przytaczany kod.

` ```
started_in = os.getcwd()
    download_content(terminology_url, terminology_languages)
    os.chdir(started_in)
``` `

```
started_in = os.getcwd()
    download_content(terminology_url, terminology_languages)
    os.chdir(started_in)
```

## Dodawanie elementów

### Odsyłacze

Odnośniki do stron internetowych (ale też wyróżnionych nagłówkami części markdownowego dokumentu) dodaje się za pomocą dwóch rodzajów nawiasów. W nawiasy kwadratowe wpisuje się tekst, jaki wyświetli się w dokumencie wyjściowym, po czym w nawiasach okrągłych zamieszcza się sam odnośnik.

Format to:

`[Nazwa odnośnika](Odsyłacz, np. adres internetowy)`  

`np. [Link do strony Johna Grubera, jednego z twórców Markdowna, gdzie znajdziemy opis składni](https://daringfireball.net/projects/markdown/syntax)`

Co daje w dokumencie wyjściowym następujący efekt:

[Link do strony Johna Grubera, jednego z twórców Markdowna, gdzie znajdziemy opis składni](https://daringfireball.net/projects/markdown/syntax)

### Obrazki

Dodawanie obrazków jest formą dodawania odsyłacza, w której odsyłamy do ścieżki pliku graficznego, który chcemy umieścić w dokumencie, ale by obraz wyświetlił się na stronie, musimy poprzedzić całą formułę znakiem wykrzyknika.  
Tytuł grafiki dodawany w nawiasach kwadratowych pojawia się jako tekst alternatywny, nie pojawia się natomiast przy wyświetlaniu obrazu.

Format to:

`![Tytuł obrazka](ścieżka pliku)`  
`np. [Zdjęcie twórców Markdowna](chlopaki.png)`

Co daje w dokumencie wyjściowym następujący efekt:

![Zdjęcie twórców Markdowna](chlopaki.png)

(Folder, w którym znajduje się plik .md, jest domyślną ścieżką, więc dla znajdujących się w nim plików graficznych wystarcza samo podanie ich nazwy.)








