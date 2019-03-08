# Käyttöohje

# Asennus

Tee jar tiedosto komennolla gradle installDist

Aja jar tiedosto komennolla java -jar Puzzle-Solver.jar

Suositeltavaa on antaa java virtual machinelle oletusarvoa enemmän heapmuistia esimerkiksi -Xmx2G

# Käyttö

Ohjelman käyttöliittymä neuvoo eteenpäin, mutta perus idea on, että kaikki syöte tapahtuu kokonaisluvuilla.

# Virhetilanteet

Mikäli syötteenä annetaan jotain muuta kuin kokonaisluku ohjelma kaatuu, sillä tarkistuksia ei ole toteutettu

Mikäli ohjelma ei saa varattua tarpeeksi muistia, kaatuu se muistin ylityttyessä.
