# STASAK1
STASAK1-järjestelmää käytetään tilanteissa, kun sakkojen normitukseen halutaan mahdollisimman yksinkertainen järjestelmä.

Koska etanoli on vesiliukoinen, tulee normituksen pohjautua kehon veden määrään, joka määritetään STASAK1:ssä kehon painon avulla:

$$
S_{miehet} = C \times \frac{0.047}{v} \times \frac{m}{\text{kg}}\ \text{mL},
$$

$$
S_{naiset} = C \times 0.8 \times \frac{0.047}{v} \times \frac{m}{\text{kg}}\ \text{mL},
$$

missä *C* on vakiokerroin (oletusarvoisesti 1), *v* on kilpailijan juoman alkoholipitoisuus tilavuusyksikköä kohden (oluelle: 4.7% / 4.7% = 1, eli termi katoaa) ja *m* kilpailijan massa. Naisten kehon pienemmän vesikonsentraation vuoksi heidän kaavaan sisällytetään korjauskerroin.

Tapauksessa, jossa kilpailijalla on erivahvuisia juomia, tulee hänen valita sellainen alkoholipitoisuus *v*, jonka juotujen juomien keskiarvo ylittää tai on vähintäänkin samalla tasolla kaikilla kilpailun hetkillä. Esimerkiksi kilpailija voi valita tasoksi *v* juomien keskiarvon ja aloittaa juomisen vahvimmasta päästä. Tällöin juotujen juomien alkoholitason keskiarvo ei koskaan alita määritettyä tasoa.

Muutokset vakiokertoimeen ilmoitetaan väliviivalla standardilyhenteessä. Esimerkiksi *C* = 1.5 ilmoitettaisiin `STASAK1-1.5`.

### Esimerkki
Kilpailu käyttää `STASAK1`-standardia.
Matti on 21 vuotias mies. Hän on 190cm pitkä ja painaa 90kg. Matti käyttää kilpajuomanaan Sandels (4.7%).

$$
S_{matti} = 1 \times \frac{0.047}{0.047} \times \frac{90\text{kg}}{\text{kg}}\ \text{mL}
$$

$$
S_{matti} = 90\ \text{mL}
$$
