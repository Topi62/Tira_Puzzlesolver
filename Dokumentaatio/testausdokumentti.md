# Testausdokumentti

Itse algorithmeja on testattu vain ajamalla main ohjelmaa erikokoisila puzzleilla eri määrä kertoja. 

A* algoritmi on osoittautunut
lupaavammaksi ja useimmat 4x4 puzzlet se ratkaisee muutamassa minuutissa, mutta satunnaisesti ratkaisu kestää yli 10 minuuttia.
Toteutus on tehty minimikeolla (Heap), joka järjestetään max ( manhattandistance , miss placed numbers). 

Syvyyshaku on hitain. Ilmeisesti harhaantuu väärälle polulle alussa, ja koska käyttää pinoa (Stack) niin palaa alkuun vasta, kun kaikki 
muut mahdollisuudet on käytetty.

Leveyshaku on melkein yhtä nopea kuin A*, tai ehkä 5-6 kertaa hitaampi. Se on kummallista, sillä siinä ei edes tutkita, ettei ole jo käsitelty jotain positionia.

## Puzzle

Keskeinen luokka, jonka metodeille on toteutettu yksikkötestejä eniten.

## Queue

Jonosta testataan lisäys tyhjään jonoon, taulukon koon kasvattaminen, yritys hakea tyhjäst jonosta, jonon tulee palauttaa ensin sinne laitettu puzzle

## Stack

Pinosta testataan samat asiat kuin jonosta. Tällä kertaa pinon pitää palauttaa sinne viimeksi laitettu Puzzle
 
## Heap

Keosta testataan, että palauttaa kahdesta arvosta paremman eli minimin ensin. Ja samoin parhaan siirron yhdestä positionista.

## Position

Listasta, mihin talletetaan jo käsitellyt asetelmat testataan, että talletettu asetelma löytyy, että uuden asetelman talletus palauttaa falsen ja että tekemällä neljän ruudun välillä kolme kierrosta, eli loopin, saavutettava asetelma löytyy, sillä sehän on alkuasetelma.


