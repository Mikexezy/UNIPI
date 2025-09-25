---
MOC: "[[Lab Fondamenti di Programmazione]]"
---
# Basi C++

### Inizio del programma

Tutti i comandi che cominciano con # sono comandi facenti parte del ==pre-processore==.
```C++
#include<...>;
```
>#include serve ad includere nel nostro progetto certe librerie.

---

### Funzione Main

La funzione principale del nostro programma è il main, definita di default come:
```C++
int main(){
	//blocco di codice
}
```

---

### Output

Il comando base di output della libreria iostream è:
```C++
cout << "stringa"; //stampa la stringa

cout << endl; //va a capo

cout << endl << "stringa"; //va a capo e successivamente stampa la stringa

cout << "stringa" << endl; //stampa la stringa e successivamente va a capo

cout << "stringa1" << "stringa2"; // stamperà "stringa1stringa2"
```
>Siamo noi a comporre il comando cout come preferiamo utilizzando le parentesi angolari "<<".

---

### Commenti

Possiamo scrivere alcune righe che non verranno prese in considerazione una volta che il nostro programma verrà avviato.
Queste prendono il nome di "Commenti":
```C++
//Questo è un commento e non verrà minimamente considerato all'avvio =)

/*
Io sono pure un commento,
però posso prendere più righe =)
*/

```

---

### CMakeLists.txt

```txt
cmake_minimum_required(VERSION 4.0)       //Versione minima di cmake richiesta
project(PrimaEsercitazione)               //Nome del nostro progetto
  
set(CMAKE_CXX_STANDARD 20)                //Imposta il CXX di CMake minimo a 20
  
add_executable(PrimaEsercitazione main.cpp)    //Specifica il nostro eseguibile
```

---

![[lab01.pdf]]

---

# 1.1
![[Esercizio 1.1 25-09-25.png]]

---

# 1.2

![[Esercizio 1.2 25-09-25.png]]

---

# 1.3

![[Esercizio 1.3 25-09-25.png]]

---

# 1.4

![[Esercizio 1.4 25-09-25.png]]

---

# 1.5

![[Esercizio 1.5 25-09-25.png]]

---

# 1.6

![[Esercizio 1.6 25-09-25.png]]