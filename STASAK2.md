# STASAK2
STASAK2-järjestelmää käytetään kilpailullisissa tilanteissa, kun sakkojen normitukseen halutaan tarkka, mutta järkevä järjestelmä.

Koska etanoli on vesiliukoinen, tulee normituksen pohjautua kehon veden määrään, joka määritetään STASAK2:ssa [Watsonin kaavojen](https://doi.org/10.1093%2Fajcn%2F33.1.27) avulla. Sakot määritetään kaavoilla:

$$
S_{miehet} = C\times\frac{0.047}{v}\times (2.447 − 0.09516 \frac{a}{\text{yr}} + 0.1074 \frac{h}{\text{cm}} + 0.3362 \frac{m}{\text{kg}})\ \text{mL},
$$

$$
S_{naiset} = C\times\frac{0.047}{v}\times (−2.097 + 0.1069 \frac{h}{\text{cm}} + 0.2466 \frac{m}{\text{kg}})\ \text{mL},
$$

missä *C* on vakiokerroin (oletusarvoisesti 2), *v* on kilpailijan juoman alkoholipitoisuus tilavuusyksikköä kohden (oluelle: 4.7% / 4.7% = 1, eli termi katoaa), *a* on kilpailijan ikä, *h* on pituus ja *m* massa.

Tapauksessa, jossa kilpailijalla on erivahvuisia juomia, tulee hänen valita sellainen alkoholipitoisuus *v*, jonka juotujen juomien keskiarvo ylittää tai on vähintäänkin samalla tasolla kaikilla kilpailun hetkillä. Esimerkiksi kilpailija voi valita tasoksi *v* juomien keskiarvon ja aloittaa juomisen vahvimmasta päästä. Tällöin juotujen juomien alkoholitason keskiarvo ei koskaan alita määritettyä tasoa.

Muutokset vakiokertoimeen ilmoitetaan väliviivalla standardilyhenteessä. Esimerkiksi *C* = 1.5 ilmoitettaisiin `STASAK2-1.5`.

### Esimerkki
Kilpailu käyttää `STASAK2`-standardia.
Matti on 21 vuotias mies. Hän on 190cm pitkä ja painaa 90kg. Matti käyttää kilpajuomanaan Sandels (4.7%).

$$
S_{matti} = 2\times\frac{0.047}{0.047}\times (2.447 − 0.09516 \frac{21\text{yr}}{\text{yr}} + 0.1074 \frac{190\text{cm}}{\text{cm}} + 0.3362 \frac{90\text{kg}}{\text{kg}})\ \text{mL}
$$

$$
S_{matti} = 102.22528\ \text{mL}
$$
