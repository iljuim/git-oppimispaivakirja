# Oppimispäiväkirja: Hajautettu git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet, jotka vaikuttivat tehtävän suorittamiseen?__

Koska gitin ja Githubin käyttö oli minulle uutta, käytännössä kaikki kurssilla oli aluksi vaikeaa. Gitin konseptin hahmottaminen oli sinällään helppoa, mutta sen ymmärtäminen käytännön tasolla kesti varsin kauan. Suhteellisen helppoa oli ymmärtää virheilmoituksia, joita git antoi yrittäessäni pushata paikallista repositoriota Githubiin.

Olin käyttänyt Githubia kerran aiemmalla kurssilla, jonka palautus oli tätä kurssia aloittaessani kesken. Minulla oli koko kurssin ajan ollut ongelmia Github Pagesin kanssa. Koitin ratkaista asian tekemällä kurssin hakemistosta muualle sijoitetun varmuuskopion ja liittämällä sen jälkikäteen Github Pages–repositoriooni `iljuim.github.io`.

Tämä kuitenkin aiheutti konflikteja, sillä mukana olleet näkymättömät `.git`-tiedostot pitivät repositorion mukana varmuuskopiossa. Liittäminen uuteen olemassaolevaan hakemistoon ja repositorioon siis sai aikaan konfliktin. Tätä minun oli selviteltävä ja loppujen lopuksi päädyin luomaan täysin uuden `iljuim.github.io`–repositorion. Tähän repositorioon liitin varmuuskopioidut tiedostot ilman `.git`-tiedostoja ja käytin `-f`–komentoa pushatessani repositorion. Tämä ratkaisi ongelman.

Tätä kirjoitettaessa (6.11.2024) minulla on edelleen ongelma paikallisen repositorioni kanssa, jossa on kaksi päähaaraa (`master`ja `main`), joita ei pystynyt aiemmin yhdistämään. Nyt halutessani testata tätä vielä, terminaali antaa minulle seuraavanlaisen ilmoituksen:

```

omakansio@Ilmari-MacBook-Air-2 iljuim.github.io % git branch
    main
    * master
    uusimain
omakansio@Ilmari-MacBook-Air-2 iljuim.github.io % git merge main
Already up to date.

```

En tiedä mitä on tapahtunut, koska aiemmin yhdistäminen on antanut jonkin virheraportin. Tätä lienee syytä selvitellä lisää.

7.11.2024. Nyt vasta ymmärsin, että siitä huolimatta, että nämä haarat on kerran yhdistetty, ne jatkavat olemassaoloaan erillisinä haaroina, ellei niitä nimenomaan poisteta.

Päädyin myös luomaan uuden repositorion Harjoitus 5:ä varten, jotta saisin testattua repositorion luontia puhtaalle alustalle, sen sijaan että jatkaisin ``github.io``-repositorion käyttöä. Näin ollen harjoitus 5 ja 6 tehtiin repositorioon ``Git-1noppa``.

## Osiossa käyttämäni Git-komennot

| Komento | Kuvaus |
| --------| ------ |
| git clone | Kloonaa parametrina annetun repositorion juuri luotuun hakemistoon (directory) ja luo kauko-jäljitettyjä (remote-tracking) haaroja joka haaralle kloonatussa repositoriossa. |
| git push | Lähettää commitoidut muutokset etärepositorioon. Eli toisin sanoen synkkaa paikallisen repositorion etärepositorioon. |
| git fetch | Hakee etärepositorion tiedot paikalliseen repositorioon. Ei itsessään tee mitään sen enempää, joten komentona vaaraton. |
| git merge | Yhdistää senhetkisen repositorion repositorioon jonka komennolle antaa parametrina |
| git pull | Tämä komento on yhdistetty fetch + merge, eli se hakee etärepositorion tiedot ja yhdistää sen repositorioon, joka komennon antamisen hetkellä on aktiivinen. |
| git branch | Jos komennon antaa ilman parametria, se listaa kaikki repositorion haarat. Jos komennolle antaa parametrin, se luo uuden repositorion parametrin nimellä. |
| git switch | Komento ei itsessään tee mitään vaan se tarvitsee parametrin toimiakseen. Parametrin on oltava jokin repositorion haaran nimi ja validin parametrin saadessaan komento vaihtaa parametrina annettuun repositorioon. |
| git log | Log-komento listaa repositorioon tehdyt commitit. Siihen voi liittää muita komentoja kuten --graph-komennon, joka lisää commit-komentoihin pientä visualisointia. Opintojakson kakkosmoduulissa erityisesti komentojen --stat --graph --oneline avulla tämä komento auttoi navigoimaan versiohistoriaa. |