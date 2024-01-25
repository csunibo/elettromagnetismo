---
date: 2024-01-14
ripasso: 20
Rating: 🌕🌕🌕🌕🌕
tags:
  - ⚡elettromagnetism
---

### Particelle in campi magnetici
#### Moto in campo magnetico uniforme 🟩
Se abbiamo una particella carica con velocità uniforme in campo magnetico uniforme, come abbiamo detto in precedenza, una forza centripeta, questo farà **curvare la carica**, una cosa interessante sarebbe provare a capire **raggio di curvatura** della nostra carica. Sotto in immagine abbiamo l'esempio di curvatura.
![Magnetismo-1700054485909](images/Magnetismo-1700054485909.jpeg)

$$
F = qvB= ma = \frac{mv^{2}}{r}
\implies r = \frac{mv^{2}}{qvB} = \frac{mv}{qB} = \frac{p}{qB}
$$
Dove $p$ è la quantità di moto, quantità che credo sia relazionata al lavoro ed inerzia, parte di fisica 1 che non ho studiato da più di due anni.
Questa stessa relazione, conoscendo il raggio *può essere usata per calcolare il campo magnetico!*.

Possiamo anche avere una **velocità angolare!**
$$
\omega = \frac{v}{r} = \frac{vqB}{mv} = \frac{qB}{m}
$$
Questo risultato si poteva anche avere osservando che $F = m \vec{\omega} \times \vec{v}$
E si noterà che il verso è **opposto al campo magnetico**.
Quindi:
$$
\vec{\omega} = -\frac{q\vec{B}}{m}
$$
Ma questo vale solo classicamente, perché poi entrano in gioco **irradiazioni** che fanno perdere energia e anche cose relativistiche se accelero troppo.


Supponiamo ora che ci sia un certo angolo fra i due allora ho che solamente la parte normale ha forza, avrò un moto elicoidale.

#### Angolo generico 🟩
![Magnetismo-1700055358930](images/Magnetismo-1700055358930.jpeg)

$$
F = qv \times B = q(\vec{v}_{n} + \vec{v}_{p}) \times \vec{B} = q\vec{v}_{n}\times \vec{B}
$$
**Passo dell'elica**
Vogliamo capire quale sia la distanza fra un top di elica e una altra, avremo che questo è 
$$
p = v_{p} T 
= v_{p} \frac{2\pi}{\omega}
= \frac{2\pi mv_{p}\cos \theta}{qB}
$$
Dove $v_{p}$ è la velocità parallela al campo magnetico, e $T$ è il periodo che è calcolato dalla velocità angolare.
Il coseno serve per prendere la componente corretta credo....


#### Effetto Hall 🟩
Da studiare bene pagina 230 Mazzoldi.
![Spettrometri di massa-1700844643754](images/Spettrometri di massa-1700844643754.jpeg)
Sia dato un conduttore parallelepipedo, una piccola sottile lastra, che scorre una corrente, allora avremo una forza
$$
\vec{F} = q\vec{v}_{d} \times \vec{B}
$$
La forza è non-elettrostatica, chiamata forza elettromotore, simile a quello per i circuiti, lo scrivo così:
$$
F = qE_{m} = q\vec{v}_{d}\times \vec{B} \implies 
E_{m} = v_{d}B
$$
Questo fa accumulare carica positiva sopra, che crea un altro campo elettrico statico che prova a bilanciare. Il primo passaggio è motivato perché è come se esistesse un campo elettrico fittizio, per spostarlo su. (È un campo elettrico generato!).

Questo campo elettrico che bilancia si chiama **campo elettrico di Hall**.
È utile per *capire se i portatori di carica è negativo o positivo*, forse ha una cosa storica questa cosa.
Avremo che
$$
\Delta V_{M} = E_{m} b 
= v_{d}Bb
= b\vec{J}\times \frac{\vec{B}}{nq}
= i \frac{\hat{u}}{a}\times \frac{\vec{B}}{nq}
\implies \Delta V = \frac{iB}{nqa}
$$
Dove $b$ è l'altezza, e $a$ è la width del nostro filo.

Questo permette di **misurare il campo magnetico** ed è chiamato *sonda di Hall*, basta misurare la differenza potenziale presente.
Per esempio questo diventa molto utile quando per [[Magnetismo nella materia]] andiamo poi a misurare il campo magnetico in buchi, basta mettere questa sonda di Hall.

### Spettrometri di massa
#### Spettrometro di massa di Thomson 🟩
![Spettrometri di massa-1700473509303](images/Spettrometri di massa-1700473509303.jpeg)
Ho un coso che emette particelle in tutte le direzioni, faccio passare una zona per aumentare energia e poi campo magnetico

Abbiamo che 
$$
\frac{1}{2}mv^{2} = q\Delta V \implies
v = \sqrt{ \frac{2qV}{m} }
$$
Usiamo poi questo valore che ci permette di descrivere la velocità della particella prima che entrino nel campo magnetico, e otteniamo poi che, considerando l'accelerazione centripeta.
$$
F = qvB = \frac{mv^{2}}{r}
\implies r =  \frac{mv}{qB} =

\sqrt{ 2 \frac{m\Delta V}{qB^{2}} }
$$
Questo è uno strumento buono per separare **isotopi**, perché hanno una massa diversa, ma stessa carica.
Posso anche definire il rapporto fra i raggi degli isotopi che è
$$
\frac{r_{1}}{r_{2}} = \sqrt{ \frac{m_{1}}{m_{2}} }
$$
#### Selettore di velocità 🟩
![Spettrometri di massa-1700473442834](images/Spettrometri di massa-1700473442834.jpeg)

Metto in modo che ci sia un condensatore che abbia un certo campo elettrico, e anche che ci sia un campo magnetico, vorrei avere che abbiamo stesso valore, ossia
$$
qE = q\vec{v} \times \vec{B} \implies
E = vB
$$
Nel nostro setting, questo è utile per sapere la velocità da mettere poi in uno spettrometro di massa e fargli fare un certo giro!
Allora abbiamo di nuovo
$$
qvB_{0} = \frac{mv^{2}}{R} \implies
R = \frac{mv}{qB_{0}} = \frac{mE}{qBB_{0}}
$$
Anche questo posso usarlo per separare isotopi diversi, ma la cosa bella è che **questo è lineare** mentre prima avevamo una radice quadrata.

### Spire 

#### Setting classico: spira rettangolare 🟩
Prendiamo un campo magnetico costante, e un rettangolo di filo **indeformabile** (perché ci sono forze che potrebbero deformarla), in cui c'è corrente, questo fa girare.
![Magnetismo-1700058718118](images/Magnetismo-1700058718118.jpeg)

Il campo magnetico ha un angolo con la nostra spira.
Ossia ->
$$
F_{4} = F_{3} = 0, F_{1} = F_{2} = 0
$$
Ossia la spira non trasla, perché non c'è accelerazione, non trasla il centro di massa. E questo per qualche motivo ci permette anche di usare qualunque sistema di riferimento, tanto diventerà uguale...

I due invece fanno ruotare la spira:
$$
M = \vec{M}_{1} + \vec{M}_{2} = \vec{r}_{1}\times \vec{F}_{1} + \vec{r}_{2}\vec{F}_{2} 
= \frac{b}{2}\sin \theta F_{1} + \frac{b}{2} \sin \theta F_{2} = bsen\theta F = b \sin \theta iaB = i \vec{S} \times \vec{B}
$$

Per i lati su e giù abbiamo stessa forza che si annulla, per altri invece abbiamo un momento ora.

#### Momento magnetico di spira 🟩
dal risultato precedente sembra sensato definire una nuova variabile:
$$
\vec{m} = i\vec{S}
$$
Il che ci permette di scrivere la relazione di sopra come
$$
\vec{M} = \vec{m} \times \vec{B}
$$
Che sta clean.
Questo è molto simile al valore trovato per il momento nel [[Dipolo elettrico]], in cui abbiamo il momento di dipolo.

#### Piccole oscillazioni 🟥
usiamo quanto scritto sopra, e valutiamo cosa succede per cose piccole:
$$
\lvert   \vec{M} \rvert = -mB\sin \theta = mB\theta = I\dot{\omega}= I\ddot{\theta}
$$
E abbiamo che
$$
\ddot{\theta} +  \omega^{2}\theta=0
$$
Questo permette di calcolare il campo magnetico, col periodo.
La cosa interessante è che questo si comporta come un **ago magnetico**, stesso comportamento.



## Note di ripasso

| Data | Commenti |
| ---- | -------- |
|12/26/2023      | Definire meglio il concetto di ago magnetico e piccole oscillazioni che mi manca.          |

