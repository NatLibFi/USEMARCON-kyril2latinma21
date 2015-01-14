# Kyrillisten tietueiden primääriluettelointi

KUVAUS

USEMARCON-ohjelmalla käytettävä konversiosääntö itse luetteloiduille kyrillisille bibliografisille tietueille. Konversio tuottaa tietueisiin ISBD-kuvailusääntöjen mukaiset kentät. Huomaa että Melinda-kirjastojen ei tule käyttää tätä konversiota, vaan suoraan palvelimella toimivaa konversio-ohjelmaa. Tarkemmat ohjeet tiedostossa "konvertointiohje.pdf" ja Linnea2-intrassa: http://www.kansalliskirjasto.fi/kirjastoala/linnea2intra/ohjeita/luettelointi/kyrilliikka.html.

Lisätietoja USEMARCON-ohjelmasta: http://www.nationallibrary.fi/libraries/format/usemarcon.html.

KÄYTTÖ

Kopioi konversiopaketti päätteellesi "Download ZIP" -painikkeesta. Pura paketti haluamaasi sijaintiin esimerkiksi C:\Usemarcon\ -hakemiston alle. USEMARCONilla käytettävä varsinainen konversiotiedosto on kyril2latinma21.ini. 

Luetteloi tietue:
- Kirjoitusjärjestelmä merkitään kenttään 066 ## $c (N)Q
- Kyrilliset tiedot tallennetaan 880-kenttiin:
	* 880 on toistettava kenttä
	* 880 kentän indikaattorit ovat samat kuin ”tavallisissa” kentässä
	* 880 kentän osakentässä ‡6 viitataan ”tavalliseen” kenttään (020-700)
	* ”tavallisen” kentän jälkeen merkitään 880-kentän järjestysnumero (-01 jne.)
	* muut tiedot (= ei kyrilliset) tallennetaan latinitsalla ”tavallisiin” kenttiin (006-998)
	* Esim. 650 _7 ‡a muistelmat ‡x runoilijat ‡z Venäjä ‡2 ysa

	HUOM, Voyager-järjestelmä ei toimiakseen vaadi 066-kenttää eikä 880-kenttien
	/(N ”häkkyröitä”, mutta ne on tallennettava, jotta tietokannoista saa poimittua ulos oikeaa MARC-8 -merkistöä.
- Tarkista, että luettelointiklientin merkistömääritykseksi on valittu UFT-8.

- Lisätietoja Linnea2-intrassa: http://www.kansalliskirjasto.fi/kirjastoala/linnea2intra/ohjeita/luettelointi/kyrilliikka.html.

PALAUTE

marc-posti (at) helsinki.fi

=================

DESCRIPTION

A USEMARCON rule for Finnish libraries for transliteration of cyrillic MARC 21 records.
