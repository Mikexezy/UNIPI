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

Mi dispiace prof per non aver seguito, però mi somiglia troppo a La Placa.
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


