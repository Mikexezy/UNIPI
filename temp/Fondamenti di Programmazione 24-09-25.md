---
MOC: "[[Fondamenti di Programmazione]]"
---
"Rappresentazione dell'informazione (2/2)" - [[Fondamenti di programmazione PDF1.pdf]]

Spiega come funzionano i bit e come funziona il byte, facendo capire quante combinazioni è possibile avere con $2^8$.

Un byte a seconda del contesto può descrivere elementi diversi, come:
- Un carattere, tipo "A".
- Un pixel sullo schermo.

---

### Codifica ASCII 7 bit

La codifica utilizza 7 bit per identificare vari caratteri, la tabella classica contiene 128 caratteri, mentre esiste un'estensione che aggiunge ulteriori 128 caratteri per un totale di 256.

Il byte che riceverà il calcolatore sarà formato da uno 0 iniziale, a seguire le 3 cifre più significative che identificano la colonna della tabella e successivamente le 4 meno significative che identificano le righe.

![[TabellaASCII.png]]

---

### Mi dispiace professore

"O ora vi spiego come funziona la rappresentazione posizionale della base decimale e binaria"

| Binario | Decimale |
| ------- | -------- |
| 000     | 0        |
| 001     | 1        |
| 010     | 2        |
| 011     | 3        |
| 100     | 4        |
| 101     | 5        |
| 110     | 6        |

Mi dispiace prof per non aver seguito, non riesco 😔.
Si è messo a spiegare tutte le basi...

---

### Conversioni 

(pag. 44 - [[Fondamenti di programmazione PDF1.pdf]])
![[Formula della sommatoria.png]]
Ed eccoci qua con la formula della sommatoria...

Praticamente per convertire un numero in base beta in un numero in base dieci bisogna semplicemente applicare questa formula.
 $$(160)_{6} = 1\cdot6^2 + 6\cdot6^1 + 6\cdot6^0 = 36 + 36 + 6 = (78)_{10}$$

Invece per convertire dalla base dieci ad una qualsiasi altra base bisogna dividere il numero di partenza per la base di destinazione fino a raggiungere quoziente 0.

![[Conversione Da Base 10.png]]

$$(23)_{10} = (113)_{4}$$

---

### Procedimento Div & Mod 

Questo è proprio il procedimento che serve a convertire da base 10 ad un altra base.

Div è l'operazione che ci permette di ottenere il quoziente intero derivante da una divisione.
Mod invece ci permette di ottenere il resto di una divisione.

Queste due operazioni le troviamo nei vari linguaggi di programmazione.

---

### Inizializzazione di una variabile int senza segno

In C++ possiamo allocare numeri reali in variabili da 16 bit utilizzando il tipo:
```C++ 
unsigned short int nome_variabile;
```

, in una variabile da 32 bit utilizzando:
```C++
unsigned int nome_variabile;
```

, e una variabile da 64 bit utilizzando:
```C++
unsigned long int nome_variabile;
```

>"non è detto che vengano allocati 64 bit, potrebbe allocare ugualmente 32 bit".

---

### Inizializzazione di una variabile booleana

In C++ possiamo inizializzare una variabile booleana utilizzando il tipo:
```C++
bool nome_variabile;
```

>Il tipo bool può assumere soltanto i valori 0 e 1, oppure true e false.

E' possibile effettuare operazioni logiche come OR, AND, NOT ecc.

| Operazione | Simbologia |     | Valore 1 | Valore 2 | Risultato |
| :--------: | :--------: | --- | :------: | :------: | :-------: |
|     OR     |    \|\|    |     |  false   |  false   |   false   |
|     OR     |    \|\|    |     |  false   |   true   |   true    |
|     OR     |    \|\|    |     |   true   |  false   |   true    |
|     OR     |    \|\|    |     |   true   |   true   |   true    |
|            |            |     |          |          |           |
|    AND     |     &&     |     |  false   |  false   |   false   |
|    AND     |     &&     |     |  false   |   true   |   false   |
|    AND     |     &&     |     |   true   |  false   |   false   |
|    AND     |     &&     |     |   true   |   true   |   true    |
|            |            |     |          |          |           |
|    NOT     |     !      |     |   true   |          |   false   |
|    NOT     |     !      |     |  false   |          |   true    |

---

### Principali oggetti della libreria IO 

In C++ nella libreria standard IO (iostream), troviamo i due principali oggetti...

output per stampare qualcosa sul terminale:
```C++
cout << "Hello World" << endl;
```
![[cout C++.png]]

, per richiedere un input da terminale:
```C++
unsigned int input;

cout << "Inserisci un numero: ";
cin >> input;
```
![[cin C++.png]]