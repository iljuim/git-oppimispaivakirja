# Oppimispäiväkirja: Git projektissa

__Mitä hyötyä voisi olla versionhallinnasta, jos kehität projektia yksin?__

Versionhallinnassa on ilmeisiä hyötyjä yksintyöskentelylle. Se auttaa pitämään kirjaa muutoksista, joita on tehnyt, kehittämään uusia ominaisuuksia omassa haarassaan ja päivittämään main-haaran tuotetta bugien yms. kannalta ilman, että nämä haarat missään vaiheessa aiheuttavat konflikteja jo käytössä olevalle tuotteelle tai kehityksessä oleville lisäosille. Tiimityössä olennainen muutosten jäljitettävyys on hyödyllinen myös yksintyöskentelyssä.

__Mitä hyötyä voisi olla versionhallinnasta, jos projektissa on useita kehittäjiä?__

Versionhallinta auttaa jäljittämään kehittäjän tekemiä muutoksia. Se selkeyttää tuotteen projektin työvaiheiden haarauttamista, helpottaa työn organisointia ja mahdollistaa projektin kehityksen eri suuntiin. Viimeisimmällä tarkoitan sitä, että projektin tuotetta voidaan kehittää viimeisimmästä julkaistusta versiosta eri tavoin ja vertaillen ilman, että ne vaikuttavat toisiinsa.

__Miten järjestäisit projektitiimin versionhallinnan 3-4 hengen ohjelmistoprojektikurssilla? Laadi tiimiläisille lyhyt ohje, miten projektissa toimitaan.__

Alla lyhyt ohje siitä, miten projektin pää- ja työrepositorioiden käyttö on järjestetty. Tämä voisi olla aloitustilanne, kun kurssi lähtee käyntiin ja sovimme työtavoista.

| Toiminto | Kuvaus |
| --------| ------- |
| Katselmointi | Yhteinen koodintarkastussessio. Ainoa tilaisuus, jossa koodia voi laittaa main–haaraan! |
| main | Projektin päärepositorio. Tänne lisätään uutta tavaraa vain katselmoinnissa! |
| dev | Projektin työrepositorio. Lisää tähän koodia, jonka haluat tuoda katselmointiin! |
| File / commit | Parhaimman jäljitettävyyden vuoksi commitoi kerrallaan vain yksi tiedosto. Näin voidaan ongelmatilanteissa jäljittää juuri se muutos joka rikkoi koodin. |



__Kommenttini opintojaksosta, esim. sisällöstä, materiaalista, työmäärästä, hyödyllisyydestä, työmäärästä. Mitä toivoisit olevan enemmän, mitä vähemmän?__

Sisältö on mielestäni sopivan laaja kurssille, josta saa 1 op. Gitin oppimiskäyrä oli ainakin itselleni varsin jyrkkä, joten en usko, että 1 opintopisteen laskettu 27 tuntia omalla kohdallani riitti. 
Mielestäni tämä on kuitenkin kurssina sellainen, että jos IT-tradenomiopiskelija aikoo suuntautua yhtään mihinkään, missä on koodattava edes hiukan, tämä on aivan keskeinen kurssi sellaiselle opiskelijalle. 

Itse sain tästä kurssista valtavasti itseluottamusta gitin käyttöön. Ottaen huomioon kuinka keskeinen teknologia ja infrastruktuuri se on koodaamisen maailmassa tämä oli hyödyllisyydeltään yksi Haaga-Helian opintojeni tärkeimmistä opintopisteistä.

En ole vieläkään suvereeni gitin käyttäjä ja joudun todennäköisesti monta kertaa palaamaan kurssin materiaaleihin vielä syksyn aikana, mutta tämä kurssi on antanut hyvät eväät aloittaa gitin käyttö.

Mielestäni oppimateriaalien visualisointi on tärkeää ja kuvia olikin käytetty hyvin havainnollistamaan esimerkiksi ``Git projektissa``-osuuden rinnakkaiskoodausesimerkeissä. Repositorion versiohistorian kuvauksissa kuitenkin olisi hyvä tähdentää, miksi nuolet eri kuplien välillä kulkevat eri suuntaan kuin versiohistoria menee. Lieneekö tässä jonkinlainen joki-vertaus (upstream), että aiemmat versiot ovat ikäänkuin projektin "yläjuoksu".

Tuleville toteutuksille esimerkiksi opetusvideot voisivat olla uusi median muoto mitä hyödyntää.