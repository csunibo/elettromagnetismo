### Introduzione ai condensatori

#### Analisi introduttiva condensatori: tubi di flusso 
![Materiali e campo elettrico-1697456372758](images/Materiali e campo elettrico-1697456372758.jpeg)
Consideriamo un **tubo di flusso infinitesimo** come in immagine. abbiamo che  $dQ$ è la carica totale dentro al cubo. Tale che segua le linee di campo.
Il flusso totale sarebbe
$$
\oint_{\Sigma} \vec{E} \cdot d\vec{s} = \frac{Q_{T}}{\varepsilon_{0}}
$$
Sappiamo anche che
$$
\vec{E}_{1}d\vec{s}_{1} + \vec{E}_{2}d\vec{s}_{2} = \frac{dQ_{T}}{\varepsilon_{0}}
$$
Ma scegliamo il cubo di flusso in modo che le superfici siano **perpendicolari al nostro campo**, e così posso considerare il problema da un puro punto di vista **scalare**.
Sapendo che nell'esempio sott il campo non è esistente, allora posso scrivere il campo elettrico che va fuori, semplicemente in punto di vista scalare:
$$
E_{2} = \frac{dQ}{\varepsilon_{0}ds_{2}}
$$
esChe è molto molto simile alla forma $\frac{\sigma}{\varepsilon_{0}}$.
il parametro di nostro interesse in questo esempio (almeno la cosa di nostro interesse) è *il concetto di distanza*, se ci allontaniamo dalla nostra superficie, $dS_{2}$ diventa più larga


#### Introduzione ai condensatori 
Poniamo di avere due armature metalliche qualsiasi, che abbiamo **cariche uguali ed opposte in segno** di una forma qualunque a distanza qualunque, in questo setting teorico.
La cosa interessante è che suppongo di avere [[#Induzione completa]] in questo caso.
È una necessità per l'analisi dei condensatori.

#### Potenziale elettrico e carica +
![[Materiali e campo elettrico-1697457325467.jpeg|500]]
Proviamo a seguire una linea di campo elettrico per studiare il potenziale elettrico, andiamo quindi a definire un **tubo di flusso**.
Per risultato precedente abbiamo che  $E_{i} = \frac{dQ_{i}}{\varepsilon_{0}dS_{i}}$

$$
V_{A} - V_{B} = \int _{A}^{B} \vec{E}_{i} \, dr_{i}  = \int _{A}^{B} {E}_{i} \, dr_{i} = \int _{A}^{B} \frac{dQ_{i}}{\varepsilon_{0}dS_{i}}\, dr_{i}  = dQ_{i} \int _{A}^{B} \frac{1}{\varepsilon_{0}dS_{i}}\, dr_{i} 
$$

Portando dall'altra parte abbiamo
$$
dQ_{i} = \frac{V_{A} - V_{B}}{\int \frac{1}{\varepsilon_{0}dS_{i}}\, dr_{i} }
$$
Poi sommo la carica di tutti i singoli tubettini di flusso, dato che abbiamo induzione completa (che non abbiamo ancora discusso, abbiamo allora che 

$$
Q = \sum_{i=1}^{N}dQ_{i} = (V_{A} - V_{B})\sum_{i=1}^{N}\frac{1}{\int \frac{1}{\varepsilon_{0}dS_{i}}\, dr_{i} }
$$
La cosa importante è che **dipende solo dalla geometria** del nostro sistema, una volta fissata è una costante. chiamiamo quella cosa una costante geometrica si può scrivere che 
$$
V_{A} - V_{B} = \frac{Q}{C} \implies C = \frac{Q}{\Delta V}
$$
ossia la capacità del condensatore è la carica fratto la differenza di potenziale.

#### Analisi dimensionale capacità -

$$
\left[ C \right] = \frac{[Q]}{[V]} =\left[ Q \right] / \left[ ML^{2} T^{-2} Q^{-1} \right] = \left[ Q^{2} \right]  \left[ M^{-1}L^{-2} T^{+2} \right]  = \left[ F \right] 
$$
Massa per velocità alla seconda per l'energia.

Un Farad, ma essendo una quantità molto grande, difficile da usare, si utilizza il $1\mu F$ che sono presenti nei circuiti, ma se ho troppa carica forse è difficile da utilizzare (o hanno usi diversi).

### Condensatori piani
Consideriamo un classico caso in cui abbiamo due condensatori piani, con la stessa carica, e area $=S$ 
**Approssimazione**
1. Consideriamo le linee di campo del tutto parallele (campo come se fosse un piano infinito per chiarirci).
2. Facce sono infinite (ma poi nella realtà cambia solamente ai bordi).
#### Campo elettrico in ogni regione 
![Condensatori-1697527856591](images/Condensatori-1697527856591.jpeg)
Si può notare che

**Calcolo della direzione**
- Sinistra: è 0
- Centro sono $2\vec{E}_{1} = \vec{E}$
- Destra: è 0

**Calcolo del modulo**:
Sappiamo che il campo elettrico per una singola armatura metallica è $\frac{\sigma}{2 \varepsilon_{0}}$, in questo caso sono uguali in modulo, e si sommano quindi:

$$
\vec{E} = \frac{\sigma}{\varepsilon_{0}}
$$
In mezzo ai conduttori.
Questa analisi si può fare con Gauss o semplicemente usando sovrapposizione, dovrebbe venire uguale, nel caso di conduttori infiniti.
#### Disposizione superficiale di carica 
**Disposizione esterna**
Nel setting dei condensatori di sopra, possiamo chiederci dove stanno le cariche, si può dimostrare usando Gauss che sulla superficie esterna è nulla.
Procedimento:
1. Prendi una superficie cilindrica, che parte da dentro e arriva fuori a sinistra della piastra di sinistra.
2. Sai che il campo dentro è nullo per induzione elettrostatica
3. Sai che fuori è nullo perché hai supposto che si eliminano i campi (uguali perché stai assumendo siano infiniti).
Quindi per Gauss la carica inclusa dovrà essere nulla in quei punti.

**Disposizione interna**
Applico gauss con un cilindro molto simile, con un cerchio dentro (quindi campo nullo per induzione in [[Conduttori elettrici]]), ma ora l'altra estremità del cilindrò avrà un qualche valore:

$$
\oint_{\Sigma´} \vec{E} \cdot d\vec{s} = \frac{Q_{T}''}{\varepsilon_{0}} \implies \oint_{\Sigma'} \lvert \vec{E} \rvert  ds = \lvert \vec{E} \rvert A = \frac{Q_{T}''}{\varepsilon_{0}} = \frac{\sigma A}{\varepsilon_{0}} \implies \lvert \vec{E} \rvert  = \frac{\sigma}{\varepsilon_{0}}  = \frac{Q}{\varepsilon_{0}S}
$$
Abbiamo messo $S = A$ come superficie ed area, la stessa cosa in pratica.
Quindi la discontinuità che abbiamo discusso (che non ho ancora scritto) è ancora la stessa, solo ridisposta in modo diverso, descritto in [[Campo elettrico]].

#### Potenziale elettrico e capacità -
Utilizziamo la definizione:
$$
\Delta V = \int _{A}^{B} \vec{E} \, d\vec{r} = \lvert \vec{E} \rvert   \int _{A}^{B} \, d\vec{r} = \lvert \vec{E} \rvert d = \frac{Qd}{\varepsilon_{0}S}
$$

Una volta ottenuto entrambi posso calcolare la capacità:
$$
C = \frac{Q}{\Delta V} = \frac{S\varepsilon_{0}}{d}
$$
E possiamo vedere che sono sempre fattori geometrici.

#### Caso piani non infiniti 
Nell'analisi soprastante, abbiamo assunto di avere piani metallici infiniti
Nel caso reale:
1. L'approssimazione funziona in mezzo al condensatore
2. Ai bordi il campo inizia a curvare, quindi non è come modellizzato di sopra.

### Disposizioni di condensatori

#### Parallelo 
![Condensatori-1697529560798](images/Condensatori-1697529560798.jpeg)
Analizziamo sempre potenziali e capacità, da un punto di vista totale (vedendolo come un singolo condensatore).
Chiamiamo a sinistra 1, a destra 2
**Osservazioni**:
1. Potenziale ai capi dei condensatori è uguale, perché i primi due sopra sono collegati, così come quelli sotto
2. Si sommano le capacità (e carica singole), anche perché è *come se aumentassi la superficie*.

$$
C_{T} = \frac{Q_{T}}{\Delta V} = \frac{Q_{1} + Q_{2}}{\Delta V} = C_{1} + C_{2}
$$
> In un sistema composto da due o più condensatori posti in parallelo, la capacità totale è pari alla **somma delle singole capacità**.

#### In serie 
![Condensatori-1697529794365](images/Condensatori-1697529794365.jpeg)
**Osservazione**
1. Conduttori su E è isolato, quindi si *caricheranno solo per induzione*.
Analizziamo le differenze di potenziali, allora abbiamo che
$$
\Delta V_{1} = V_{A} - V_{E} = \frac{Q}{C_{1}}
$$
In modo simile per il secondo, noi vogliamo trovare $\Delta V = V_{A} - V_{B} = \frac{Q}{C_{T}}$, ma posso usare lo stratagemma matematico e risolvere ciò 

$$
\Delta V = V_{A} - V_{B}  =  (V_{A} - V_{E}) + (V_{E} - V_{B}) = Q\left( \frac{1}{C_{1} } + \frac{1}{C_{2}} \right) = \frac{Q}{C_{T}} \implies \frac{1}{C_{T}} = \frac{1}{C_{2}} + \frac{1}{C_{2}}
$$
Possiamo vedere che la **capacità cala**, questo è spiegato fisicamente perché la carica è distribuita, mentre la superficie rimane sempre lo stesso.

>La serie fra due o più condensatori ha capacità totale $C_{T}$ il cui inverso è pari alla somma degli inversi delle singole capacità

### Energia nei condensatori

#### Intuizione sul concetto di energia
Partiamo sempre dal concetto di lavoro, è equivalente al **lavoro usato per caricarlo**. anche chiamato **autoenergia**.
L'energia di un sistema di cariche che cosa è? è il **lavoro esterno compiuto per costruire il sistema**, in modo più intuitivo è quanto sforzo è stato necessario usare per partire dall'infinito e portare le particelle e portarle in quel punto.
Se è repulsiva (quindi energia positiva) io faccio lavoro positivo, altrimenti negativo, questo l'hai visto ieri. Se l'energia è positiva posso *estrarre* energia da utilizzare, altrimenti no.

#### Energia di Interazione 
![Condensatori-1697532550995](images/Condensatori-1697532550995.jpeg)
L'energia di sistema (o di interazione fra le cariche) è calcolato nel modo seguente:

1. La prima carica non fa lavoro perché il campo è nullo inizialmente
2. La seconda carica fa un po' di fatica
3. Se cambio l'ordine cambia l'ordine, ma l'equazione finale non cambia. (forse solo segno)
$$
U_{12} = \frac{1}{4\pi\varepsilon_{0}} \frac{q_{1}q_{2}}{R_{12}} = q_{1} V_{21}
$$
Calcoliamo l'energia necessaria per portare una terza, avremo che
$$
U_{23} = \frac{1}{4\pi\varepsilon_{0}} \frac{q_{2}q_{3}}{R_{23}}  = q_{2}V_{32} = q_{3}V_{23}
$$
E si fa lo stesso per $U_{13}$ e poi si summa tutto
Quindi in generale:

$$
U_{tot} = \sum_{i < j} ^{N} q_{i}V_{ji} = \frac{1}{2} \sum_{i \neq j} ^{N} q_{i}V_{ij}
$$
Probabilmente il segno si deve fare attento. (Nota come semplificazione, sfruttando la sovrapposizione potremmo scrivere la roba di sopra come)
$$
U_{tot} = \frac{1}{2}\sum_{i = 1}^{N}q_{i}V_{i}
$$
Con $V_{i} = \sum_{j\neq i}^{N}V_{ij}$

Questa forma poi ci deve anche essere di interesse nel momento in cui vogliamo andare oltre al semplice caso discreto, perché allora possiamo scriverlo come 
$$
U_{tot} = \frac{1}{2} \int _{\tau} \rho V \, d\tau 
$$
E la *stessa cosa vale per le superfici* in pratica posso calcolare l'energia totale in ogni configurazione.
#### Lavoro di carica dei condensatori 
##### Primo modo: lavoro punto per punto ++
![[Condensatori-1697534464287.jpeg | 500]]
Consideriamo un condensatore, alla prima carica non c'è lavoro, ma poi si crea un campo elettrico che si prova ad opporre al caricamento (quindi **lavoro positivo**, forza di Coulomb è positivo).

Man mano che si carica la $\Delta V(q)$ cambia. Proviamo a vedere la formula superficiale.
Lavoro fatto dal campo quando sposto una carica di un piccolissimo tratto.
$$
dL' = \vec{E} \cdot d\vec{r} = -dV
$$

Lavoro della $\vec{F}_{C}$ forza di coulomb (quello della forza esterna è uguale e contraria).
$$
dL = dq\vec{E} \cdot d\vec{r} = -dqdV
$$

Calcolando da A a B e sommando tutto abbiamo che (contando che il lavoro esterno deve essere opposto rispetto al nostro campo in considerazione).

$$
\Delta L_{E} = \int _{A}^{B} dqdV  = dq \int _{A}^{B} \, dV  = dq \Delta V_{q}
$$
La differenza di potenziale quando le armature non sono state ancora calcolate, abbiamo che $\Delta V_{q} = \frac{q}{C}$ che si può rimettere sopra, ossia il lavoro fatto nel momento in cui c'è una piccola forza su una armatura.
$$
\Delta L_{E} = dq \frac{q}{C}
$$
$$
L_{E} = \int _{0}^{Q} \Delta L_{E} = \int _{0}^{Q} \frac{q}{C} \, dq = \frac{1}{2} \frac{Q^{2}}{C} = \frac{1}{2} Q \Delta V = \frac{1}{2}C \,\Delta V^{2}
$$
Che è esattamente il **lavoro fatto per caricare il condensatore**

##### Secondo modo: energia di interazione 
Posso subito dire che 
$$
U_{E} = \frac{1}{2} \left[ Q_{A} V_{A} + Q_{B}V_{B} \right] = \frac{1}{2} \left[ C(V_{A} - V_{B})V_{A} + C(V_{B} - V_{A})V_{B}\right] = \frac{1}{2} C\, \Delta V^{2}
$$

#### Densità di energia 
L'energia immagazzinata è stata utilizzata per **costruire il campo**. -> Campo elettrico porta energia! Rinnovabili per questo è nice.
Abbiamo che 
$$
U_{E} = \frac{1}{2} C\, \Delta V^{2} \land C=\frac{\varepsilon_{0}S}{d} \land \Delta V = Ed \implies U_{E} = \frac{1}{2}\varepsilon_{0}E^{2}(Sd) = \frac{1}{2}\varepsilon_{0}E^{2}Volume
$$

Questo ci permette di definire il concetto di **densità di energia** di un condensatore, dato che abbiamo un volume.
$$
u_{e} = \frac{1}{2}\varepsilon_{0}E^{2}
$$
Questo servirà per il vettore di Poynting in seguito quando faremo il minimo di propagazione. (Base di energia solare, anche la parte di propagazione che ho fatto io, e spiega che si **può ottenere energia** dal campo elettrico, costruendo o disfacendone).
## Scarica e carica di condensatori
### Carica del condensatore
#### Setting del problema 
Ci stiamo chiedendo, come varia l'intensità di corrente in un circuito fatto di semplice condensatore e resistenza? In che modo cambia il potenziale? Se ho l'intensità di corrente per un dato momento, allora posso calcolare l'intensità di corrente.
![Condensatori nel vuoto-1699945999446](images/Condensatori nel vuoto-1699945999446.jpeg)
Possiamo usare le leggi presenti in [[Leggi di Ohm]] e osservare che vale, perché alla fine il campo esterno è ancora conservativo (credo), anche se la corrente varia.
$$
\varepsilon = V_{C} + V_{R} = \frac{q(t)}{C} + Ri(t) 

$$
In un certo istante specifico $t$, ma notiamo che per definizione, la corrente accumula sul condensatore un valore $i(t) = \frac{dq(t)}{dt}$ e possiamo sostituire questo dentro e risolvere l'equazione differenziale associata.

$$
\varepsilon = \frac{q(t)}{C} + \frac{Rdq(t)}{dt}
$$
Sono equazioni che si risolvono nella forma $Ae^{Bx}$ o qualcosa di simile, infatti possiamo sostituire questo lì dentro e ricevere qualcosa così:
$$
\varepsilon = \frac{A}{C}e^{Bt} + RABe^{Bt}
$$
Ma questo non riesco a risolverlo tutto a un tratto:
$$
dt\left( \varepsilon - \frac{q(t)}{C} \right) = dq(t) R \implies
\frac{dt}{RC} = \frac{dq(t)}{\varepsilon C - q(t)}
$$
Allora sappiamo che fra l'istante 0 in cui metto giù l'interruttore e il nostro tempo abbiamo:
$$
\int _{0}^{q} \frac{dq(t)}{-\varepsilon C + q(t))} = -\int_{0}^{t} \frac{dt}{RC} 
\implies \ln\left( \frac{-\varepsilon C + q(t)}{-\varepsilon C} \right)=- \frac{t}{RC}
\implies
q(t) = -\varepsilon C e^{-t/RC} + \varepsilon C
$$

#### Equazioni per la carica dei condensatori 
Da quanto fatto sopra otteniamo che 
$$
q(t) = \varepsilon C(1 - e^{-t/RC})
$$
$$
i(t) = \frac{\varepsilon}{R} e^{-t/RC}
$$
E poi con questo posso ottenere a cascata tanti altri valori, come la differenza di potenziale sul condensatore, sulla resistenza e simili.
$$
V_{c}(t) = \frac{q(t)}{C} = \varepsilon(1 - e^{-t/RC})
$$
E posso fare la stessa cosa per la resistenza
$$
V_{b}(t) = i(t)R = \varepsilon e^{-t/RC}
$$
Come grafici questi hanno:
![Condensatori nel vuoto-1699947549475](images/Condensatori nel vuoto-1699947549475.jpeg)
#### Note sul tempo di carica 
Nota: il condensatore non si carica mai al valore teorico di carica che può avere (è un asintoto orizzontale). Possiamo considerarlo carico quando è tipo 1% del valore nominale, non ho capito esattamente perché questo, forse è una convenzione.

Tempi tipici di carica sono **microsecondi** perché di solito Parliamo di micro-Farad e migliaia di Ohm di resistenza.

Si può notare risolvendo le equazioni di sopra otteniamo che:
0.95% -> 3$\tau$
0.99% -> 4.6$\tau$
0.999% -> 7$\tau$
Per caricare il condensatore.
#### Potenza erogata ed assorbita 
Con le equazioni di sopra possiamo anche utilizzare le equazioni di energia spesa, perché sappiamo che il generatore eroga
$$
P_{gen} = \varepsilon i(t) = \frac{\varepsilon^{2}}{R}e^{-t/RC}
$$
Mentre la potenza assorbita dalla resistenza è di valore:
$$
P_{b} = Ri(t)^{2} = \frac{\varepsilon^{2}}{R} e^{-2t/RC}
$$
E possiamo notare che  
$$
P_{c} = \frac{Vdq}{dt} = P_{gen} - P_{b}
$$
Una altra cosa interessante è che il valore del lavoro totale si può ricalcolare con l'energia presente nel condensatore!
$$
W_{gen} = \int_{0}^{\infty} P_{gen} \, dt = C\varepsilon^{2} 
$$
Allo stesso modo si poteva ottenere
$$
W_{gen} = \int_{0}^{q_{0}}Vdq = Vq = V^{2}C 
$$
E si può togliere l'energia immagazzinata dal condensatore come 
$$
W_{c} = \frac{1}{2}CV^{2} = \frac{W_{gen}}{2} \implies W_{r} = W_{c}
$$

### Scarica del condensatore
#### Setting del problema 
Ho un condensatore completamente carico come in figura
![Condensatori nel vuoto-1699948578740](images/Condensatori nel vuoto-1699948578740.jpeg)
Ad un certo punto chiudo l'interruttore e inizierà a scorrere della carica, vogliamo capire in che modo varia $q(t)$ e in che modo varia $i(t)$
#### Equazioni per la scarica dei condensatori 
In modo simile al precedente possiamo mettere su una equazione differenziale:
$$
0 = \frac{q(t)}{C} + \frac{d(q)}{dt}R
\implies -\frac{dt}{RC} = \frac{d(q)}{q(t)}
$$
E con questo abbiamo in modo del tutto analogo al precedente che
$$
\int_{q_{0}}^{q} \, \frac{dq}{q} = -\int_{0}^{t} \frac{dt}{RC} \implies \ln\left( \frac{q}{q_{0}} \right) = -\frac{t}{RC}
\implies q(t) = q_{0}e^{-t/RC}
$$
E poi si possono fare tutte le altre cose.

### Campo magnetico in condensatore 
Guardando [[Ampere e Faraday]] se cambia l'intensità del campo elettrico, come succede per questo circuito, abbiamo che si ha una densità di corrente di spostamento.

Calcoliamo la circuitazione in una parte del filo (intorno a un punto, in modo classici diciamo) e allora abbiamo
$$
\oint_{\Gamma} \vec{B} \cdot d\vec{r} 
= \mu_{0} i(t)
= \mu_{0} \int _{\Sigma(\Gamma)} \vec{J} \cdot d\vec{s} = \mu_{0}(\frac{\varepsilon}{R} e^{-t/RC})
$$
Questo scegliendo la superficie più semplice che esisteva.
Posso però scegliere una altra superficie che passa dalle facce del condensatore, in questo caso io non ho corrente! Ecco che entra in gioco la correzione di Maxwell, per la corrente di spostamento.
E facendo i calcoli si è scoperto che la predizione era corretta, e il valore è esattamente lo stesso.

