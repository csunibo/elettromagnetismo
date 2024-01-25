### Introduzione al vettore potenziale
#### Definizione vettore potenziale 
Possiamo sempre scrivere il campo $\vec{B}$ come 
$$
\vec{B} = \vec{\nabla} \times \vec{A}
$$
Con un campo vettoriale a caso $\vec{A}$, vedremo che questo campo avrà qualche utilità per fare i calcoli.

Possiamo notare che soddisfa la proprietà dell **campo solenoidale** citato in [[Magnetismo]], infatti

$$
\vec{\nabla} \cdot \vec{B} = \vec{\nabla} \cdot (\vec{\nabla} \times \vec{A}) = 0
$$
Perché sappiamo che la divergenza del rotore  (questo operatore dico) è sempre nullo per ragioni di Cauchy, se ne parla in [[Divergenza e Circuitazione]].

#### Unicità del campo 
Proviamo ad analizzarlo matematicamente, ci stiamo chiedendo, è **unica**?
> Lo è a **meno di un gradiente di una funzione scalare**

Definiamo 
$$
\vec{A}' = \vec{A} + \vec{\nabla}F
$$
Abbiamo:

$$
\vec{\nabla} \times \vec{A}' = \vec{\nabla} \times \vec{A} + \vec{\nabla} \times (\vec{\nabla}F) = \vec{\nabla} \times \vec{A} + 0
$$

Dove il gradiente di $F$, si ricorda è vettoriale, ed è utilizzato per rappresentare un vettore qualunque, basta che esista $F$ che lo generi, che lo abbiamo in ipotesi.

Simile con il potenziale, che è una **funzione definita a meno di una costante** perché possiamo mettere un punto (che scegliamo noi) in un certo punto, o potenziale del sistema che sono contati in quella costante, ne parliamo in [[Campo elettrico]]. (in questo capo la nostra costante è un vettore in un certo senso :P)

#### Scelta del campo A 
Per la divergenza abbiamo invece:

$$
\vec{\nabla} \cdot \vec{A}' = \vec{\nabla} \cdot(\vec{A} + \vec{\nabla}F) = \vec{\nabla} \cdot \vec{A} + \nabla^{2}F
$$

Lo scalare $F$ lo posso scegliere io, e mi può semplificare molti conti (si dovrebbe dimostrare che questo $F$ che me lo annulli esista sempre, probabilmente è vero).
Allora possiamo scegliere come il campo $A$ vettore potenziale tale per qui valnga
$$
\vec{\nabla} \cdot \vec{A} = 0
$$
Per qualche motivo questa cosa **vale solo nel caso stazionario (con $\vec{J}$ stabile)**.

### Comodità del vettore potenziale
#### Ampere Max-well con vettore potenziale 

Abbiamo quindi

$$
\vec{\nabla} \times (\vec{\nabla} \times \vec{A}) = \mu_{0}\vec{J}
$$

Questa espressione si può semplificare tenendo conto che $a\times b\times c = b (a \cdot c) - (a\cdot b) c$
Da cui abbiamo:

$$
\vec{\nabla} \cdot (\vec{\nabla} \cdot \vec{A}) - (\vec{\nabla} \cdot \vec{\nabla})\vec{A} = \mu_{0}\vec{J}
$$
Utilizzando l'approssimazione sopra presente abbiamo ancora un laplaciano per rappresentare questa legge, in modo simile a quanto presente al differenziale potenziale per la quantità di carica.
$$
\nabla^{2}\vec{A} = -\mu_{0}\vec{J}
$$
Possiamo notare che $A$ ha la  **stessa direzione della corrente**! seguendo la soluzione dell'equazione di Poisson per campo elettrico abbiamo che

$$
A(x, y, z) = \frac{\mu_{0}}{4\pi} \int _{\Sigma} \frac{J(x', y', z')\, dx'dy'dz'}{\sqrt{ (x - x')^{2} + (y - y')^{2} + (z - z') ^{2} }}  
$$

Se applichiamo questo su un filo allora diventa in un certo senso:
$$
\vec{A} = \frac{\mu_{0}}{4\pi} \int \frac{\vec{J} d\Sigma \, dl}{r} 
=  \frac{\mu_{0}}{4\pi} \int \frac{i \, dl}{r} 
$$
Quindi quantità di corrente lungo un certo tratto di filo!

#### Faraday con vettore potenziale --

$$
\vec{\nabla} \times \vec{E} = - \frac{\delta \vec{B}}{\delta t} = \frac{\delta (\vec{\nabla} \times \vec{A})}{\delta t}
$$

E abbiamo:

$$
\vec{\nabla} \times \left( \vec{E} + \frac{\delta \vec{A}}{\delta t} \right) = 0
$$
Quindi abbiamo che vale:

$$
\vec{E} = -\frac{\delta A}{\delta t} \implies \vec{\nabla}V = \frac{\delta A}{\delta t}
$$

#### Circuitazione del vettore potenziale 
Consideriamo il flusso del vettore su una superficie

$$
	\int_{\Sigma} \vec{B} \hat{u}_{n}  \, ds =  \int_{\Sigma} \vec{\nabla} \times \vec{A} \hat{u}_{n}  \, ds = 
	\int_{\Gamma(\Sigma)} \vec{A} \cdot\, d\vec{l}
$$
Dove l'ultima vale per **Stokes** in [[Divergenza e Circuitazione]], quindi possiamo calcolare il flusso su un campo andando a considerare la **circuitazione** del potenziale vettore!

### Esempi di applicazione

#### Studio del vettore potenziale in un solenoide 
Possiamo poi scoprire che
$$
\vec{A} = B \frac{r}{2} \hat{u}_{c}
$$
Quando $r$ è minore del raggio del solenoide, se è maggiore abbiamo
$$
\vec{A} = B \frac{R^{2}}{2r} \hat{u}
$$
