---
MOC: "[[Fondamenti di Programmazione]]"
---
# Struttura di un programma

![[Struttura di un programma.png]]

### ==es.==
``` C++
int main() {         // compund-statement
	int a = ...;        // definition-statement
	int _b1 = ...;       
	
	
	(a + b) * 3;        // expression-statement
 }
```

---

### Teorema di Bohm Jacopini
==Qualunque problema può essere risolto utilizzando solamente istruzioni strutturate.==

NON SI CAPISCE UN CAZZO QUANDO SPIEGA

---

# Operazioni di confronto

![[Operatori di confronto.png]]

``` C++
float f1 = 3.5f
bool b2 = f1 < 7.4f;        // < è l'operatore di confronto, che in questo caso
                            // assegnerà il valore true a b2
```

L'unità hardware ALU (Arithmetic Logic Unit), ci permette di effettuare sia le operazione aritmetiche, ma anche le logiche.

L'FPU invece si occupa di effettuare le operazioni aritmetiche fra numeri decimali.

---

# selection-statement

questo statement contiene al suo interno:
- if-statement
- switch-statement

#### ==if-statement==
```C++
if (condition) {
	statement
}

//oppure 

if (condition) {
	statement
} else {
	statement
}
```

esempio
```C++
int a, b;
cin >> a >> b;

if( a > b ){
	cout << "A è maggiore di B";
}else{
	cout << "A è minore di B";
}
```

---

# Diagramma di flusso

![[sticker whatsapp 1.png]]


---
