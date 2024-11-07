# Oppimispäiväkirja: Paikallinen git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet?__

## Oppimispäiväkirja osa 1 #

### Johdanto ###
Johdannon aiheet Github-tilin tekemisestä, VS Coden asentamisesta ja gitin asentamisesta omalle koneelle olivat tuttuja jo ajalta ennen kurssia. Nämä olivat siis itsellä jo hyvin hallussa, joskin kävin vielä tarkistamassa global configit. Varmistin, että global username ja email olivat edelleen oikein. Toisen kurssin takia minulla oli jo tili myös yhdistetty Github-repooni ja Github Pages käytössä.

Halusin kuitenkin käydä tämän kurssin, koska gitin käyttöni oli ollut aiemmilla kursseilla vähäistä ja niillä kursseilla joissa sitä tarvittiin, oli käyttöni haparoivaa. Halusin saada gitin käyttöön varmuutta ja harjoitusta, joten päätin ottaa tämän kurssin mukaan opsiini.

### Paikallinen git ###

Paikallisen gitin harjoittelu meni mukavasti. Edelleen hieman epäröin monia peruskomentoja tehdessäni ja tulee aloittelijan virheitä, kuten add-komentojen kanssa. Vaikka olen saanut haarautumistehtävät jo tehtyä, edelleen täytyy paljon katsoa oppimateriaaleista mallia. Onneksi ne ovat olemassa. Uskon kuitenkin, että kurssin lopussa olen jo paljon varmempi gitin käyttäjä.

Erityisesti gitin konseptin ymmärtäminen tuottaa itselleni hahmottamisvaikeuksia. Sen selittäminen itselleni käyttäen hyväksi analogisia esimerkkejä ja oikean elämän vastaavia konsepteja voi olla toimiva tapa ymmärtää sitä paremmin.

> Jos ohjelmakoodi on talonrakennustyömään konkreettiset työohjeet ja pohjapiirustukset, git on työnjohtajan excel.

Mielestäni ko. analogia kuvaa gitin toimintaa suhteellisen hyvin.

## Osiossa käyttämäni Git-komennot

| Komento | Kuvaus |
| --------| ------ |
| git add | Lisää yksittäiseen tiedostoon tehdyt muutokset commit-joukkoon. Toisin sanoen alustaa muutokset niin, että git tietää lisätä ne seuraavaan commit-komentoon. |
| git commit | Tallentaa add-komennolla alustetut tiedostomuutokset repositorioon ja luo niistä oman lokimerkintänsä. Näitä commit-komennoilla luotuja lokimerkintöjä voi navigoida esim. alla olevalla git log–komennolla | 
| git log | Log-komento listaa repositorioon tehdyt commitit. Siihen voi liittää muita komentoja kuten --graph-komennon, joka lisää commit-komentoihin pientä visualisointia. |
| git reset | Poistaa git add–komennolla alustetut tiedostot seuraavasta tallennuksesta. Jos kommennossa ei tarkenna tiedostoa, komento poistaa kaikki alustetut tiedostot. |
| git revert | Käytännössä anti-commit–komento. Komennolla tehdään muutos, joka peruuttaa sille parametrina annetun tallennuksen (commitin) kokonaan. |
| git status | Antaa tilannekuvan tilanteesta komennon antohetkellä. Tilannekuva pitää sisällään tiedon siitä, missä repositorion haarassa parhaillaan ollaan onko haara ajan tasalla suhteessa mahdolliseen etärepositorioon ja onko repositoriossa muutoksia, joita ei ole vielä alustettu commit–komennolle. |