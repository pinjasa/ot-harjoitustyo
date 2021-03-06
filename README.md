# Tetris

**sovelluksen tarkoitus**
- toimii kuten perus tetris; 
  - ylhäältä putoaa yksitellen paloja, joita käyttäjä pystyy liikuttamaan vasemmalle ja oikealle sekä kääntelemään tavoitteenaan asettaa ne mahdollisimman tiiviisti. Kun saa rivin täyteen, se häviää ruudukosta.

**perusversion toiminnallisuus**
- pystyy pelaamaan:
  - palikat tippuvat ja niitä voi liikuttaa 
  - palikoita pystyy kääntämään
  - näkyy seuraavaksi jonossa oleva palikka
- pelaaja näkee pisteensä sekä aikaisemman parhaan pistetuloksen

**jatkokehitysideoita**
- pelaaja voi luoda käyttäjätunnuksen ja kirjautua sisään/ulos
- voi nähdä aikaisemmat pisteensä suuruusjärjestyksessä
- käyttäjä pystyy lisäämään muita käyttäjiä kaverikseen ja nähdä myös heidän huippupisteensä. 
- näkee kaverilistan kaikkien käyttäjien pisteet suuruusjärjestyksessä

## Dokumentaatio

- [vaatimuusmaarittely.md](/laskarit/viikko1/vaatimusmaarittely.md)
- [arkkitehtuuri.md](./dokumentaatio/arkkitehtuuri.md)
- [testaus.md](./dokumentaatio/testaus.md)
- [kayttoohje.md](./dokumentaatio/kayttoohje.md)
- [tuntikirjanpito.md](./dokumentaatio/tuntikirjanpito.md)

## Releaset
- [viikko 5](https://github.com/pinjasa/ot-harjoitustyo/releases/tag/viikko5)
- [viikko 6](https://github.com/pinjasa/ot-harjoitustyo/releases/tag/viikko6)
- [Lopullinen versio](https://github.com/pinjasa/ot-harjoitustyo/releases/tag/viikko7)

## Asennus

1. Asenna riippuvuudet komennolla:

```bash
poetry install
```
2. Käynnistä sovellus komennolla:

```bash
poetry run invoke start
```

## Komentorivitoiminnot

### Ohjelman suorittaminen

Ohjelman pystyy suorittamaan komennolla:

```bash
poetry run invoke start
```

### Testaus

Testit suoritetaan komennolla:

```bash
poetry run invoke test
```

### Testikattavuus

Testikattavuusraportin voi generoida komennolla:

```bash
poetry run invoke coverage-report
```

Raportti generoituu _htmlcov_-hakemistoon.

### Pylint

Tiedoston [.pylintrc](./.pylintrc) määrittelemät tarkistukset voi suorittaa komennolla:

```bash
poetry run invoke lint
```
