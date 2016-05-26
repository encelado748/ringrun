# Ring Run
Ring Run è un gioco per piattaforme mobile che utilizza unity3D come engine grafico.
La struttura di base del gioco è quella dell'endless runner.

## Ambientazione
Il gioco si svolge all'interno di una catena di montaggio.
### Intro
Due robot sono affiancati nella catena di montaggio. I due robot si scambiano
uno sguardo. Dopo di che il primo lascia cadere su una scatola un anello diretto
al secondo. Purtroppo l'anello viene chiuso nella scatola che parte nella catena
di montaggio e il secondo robot (il protagonista del gioco) parte alla sua ricerca

### La fabbrica
La fabbrica muove le casse grazie a bracci inseriti lungo rotaie. Questo permette
ai pacchi di muoversi con diverse velocità e in diverse direzioni.

#### Elementi Grafici
Il binario è spesso chiuso, anche se in numerose circostanze si aprono finestre
e passaggi limitati su altri binari diagonali o verticali.

Ruolo fondamentale è dato dalle luci all'interno della fabbrica, che permettono
di ottenere effetti di riflessi interessanti. Uso di una reflection probe e di
un lighting group per migliorare la qualità

## Gameplay
Il gioco si svolge su tre binari. Il giocatore deve cercare di avanzare passando
da un binario all'altro quando questi si muovono con differenti velocità.
Passare da un binario all'altro quando questo è vuoto causa il gameover.

### Telecamera
La telecamera è fissa in profondità (mostra sempre il protagonista alla stessa
altezza), e in larghezza (non si muove con il cambio dei binari).
Il gioco viene giocato in portrait.

### Binari
I binari sono l'elemento in costante movimento rispetto allo spazio di gioco.
I binari sono composti da casse e da braccia. Ogni cassa ha un colore diverso a
seconda del possibile contenuto:
 - Arancione E67000 - casse binario, modificano il funzionamento del binario
 - Viola 840097 - casse controllo, attivano e disattivano apparecchi
 - Giallo Verde Limone C3E000 - Casse vuote, possono essere usate per proteggersi durante il percorso
 - Grigio - Casse inattive

 Colore Supplementare - 00788E

### User Interface
In alto al centro viene mostrata la distanza in metri dall'anello. Questa
quantità può aumentare e diminuire durante la partita.
A destra e a sinistra ci sono delle grandi frecce per lo spostamento da un
binario all'altro
In basso al centro c'è il tasto per entrare dentro la scatola. Uscire dalla
scatola attiva l'effetto.

### Nemici
- Laser - entra nella scatola
- Parete - Cambia corsia
-

### Effetti
La lista degli effetti per scatola

Viola:
- Spegni i Laser
- Disattiva le pareti

Arancione:
- Velocizza la corsia corrente
- Rallenta la corsia corrente
- Rimuovi pacchi - calano dall'alto
- Aggiungi pacchi - cadono in basso

### Livelli e scene di chiusura
Ogni volta che il gioco viene portato a termine si assiste ad una scena dove
l'anello viene nuovamente perso.

# TO DO list
## Struttura base
- Creazione modello scatola (3 colori, emission)
- Creazione delle braccia
- Creazione delle pareti con binari
- creazione degli emettitori Laser
- Creazione dei pannelli

## Struttura avanzata
- Variazione nelle pareti
