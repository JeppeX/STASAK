# STASAK0
STASAK0-järjestelmää käytetään tilanteissa, kun sakkoja ei haluta normittaa kilpailijoiden ominaisuuksien mukaan. Tällöin absoluuttinen viinantuhoamiskyky on kilpailun keskiössä. 

$$
S_{kaikki} = C \times \frac{0.047}{v} \times 100\ \text{mL},
$$

missä *C* on vakiokerroin (oletusarvoisesti 1), *v* on kilpailijan juoman alkoholipitoisuus tilavuusyksikköä kohden (oluelle: 4.7% / 4.7% = 1, eli termi katoaa).

Tapauksessa, jossa kilpailijalla on erivahvuisia juomia, tulee hänen valita sellainen alkoholipitoisuus *v*, jonka juotujen juomien keskiarvo ylittää tai on vähintäänkin samalla tasolla kaikilla kilpailun hetkillä. Esimerkiksi kilpailija voi valita tasoksi *v* juomien keskiarvon ja aloittaa juomisen vahvimmasta päästä. Tällöin juotujen juomien alkoholitason keskiarvo ei koskaan alita määritettyä tasoa.

Muutokset vakiokertoimeen ilmoitetaan väliviivalla standardilyhenteessä. Esimerkiksi *C* = 1.5 ilmoitettaisiin `STASAK0-1.5`.

### Esimerkki
Kilpailu käyttää `STASAK0`-standardia.
Matti on 21 vuotias mies. Hän on 190cm pitkä ja painaa 90kg. Matti käyttää kilpajuomanaan Sandels (4.7%).

$$
S_{matti} = 1 \times \frac{0.047}{0.047} \times 100\ \text{mL} = 100\ \text{mL}.
$$
