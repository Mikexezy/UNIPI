---
MOC: "[[Lab Fondamenti di Programmazione]]"
---
$N = (1010111)_2$ , dobbiamo convertirlo in base 10.

# 1. (utilizzando l'algoritmo della sommatoria)
$$(1010111)_{2} = 1*2^6 + 0 + 1*2^4 + 0 + 1*2^2 + 1*2^1 + 1*2^0 =$$
$$= 64 + 16 + 4 + 2 + 1 = (87)_{10}$$
---

$N = (87)_{10}$ , dobbiamo convertirlo in base 2.

# 1. (utilizzando l'algoritmo DIV&MOD)

- Se N = 0 => $a_0 = 0$
- Altrimenti 
	$q_0 = N$ e procedo iterativamente:
		$q_1 = q_0 \ DIV \ \beta$
		$q_2 = q_1 \ DiV \ \beta$
		$q_3 = q_2 \ DIV \ \beta$
		fino a quando $q_p$ = 0
		
		$a_0 = q_0 \ MOD \ \beta$
		$a_1 = q_1 \ MOD \ \beta$
		$a_2 = q_2 \ MOD \ \beta$

$$q_0 = 87$$

$$q_1 = q_0 \ DIV \ 2 = 87 \ DIV \ 2 = 43$$
$$q_2 = q_1 \ DIV \ 2 = 43 \ DIV \ 2 = 21$$
$$q_3 = q_2 \ DIV \ 2 = 21 \ DIV \ 2 = 10$$
$$q_4 = q_3 \ DIV \ 2 = 10 \ DIV \ 2 = 5$$
$$q_5 = q_4 \ DIV \ 2 = 5 \ DIV \ 2 = 2$$
$$q_6 = q_5 \ DIV \ 2 = 2 \ DIV \ 2 = 1$$


$$a_0 = q_0 \ MOD \ 2 = 87 \ MOD \ 2 = 1$$
$$a_1 = q_1 \ MOD \ 2 = 43 \ MOD \ 2 = 1$$
$$a_2 = q_2\ MOD \ 2 = 21 \ MOD \ 2 = 1$$
$$a_3 = q_3 \ MOD \ 2 = 10 \ MOD \ 2 = 0$$
$$a_4 = q_4 \ MOD \ 2 = 5 \ MOD \ 2 = 1$$
$$a_5 = q_5 \ MOD \ 2 = 2 \ MOD \ 2 = 0$$
$$a_6 = q_6 \ MOD \ 2 = 1 \ MOD \ 2 = 1$$

$$(87)_{10} = (1010111)_2$$

---

# Conversione fra basi $\beta$

$$(01011101)_2 = (?)_{16}$$

- Soluzione 1 :
	1. Uso base 10 come "BASE DI APPOGGIO"
	2. Converto da $\beta_1 \ -> 10$
	3. Converto da $10 \ -> beta_2$

- Soluzione 2 :
	1. Notiamo che $\beta_2 = 2^4 = \beta_1^4$
	2. ![[Pasted image 20250925151446.png]]
	
	3. $(1101)_2 = 1*2^0 + 0*2^1 + 1*2^2 + 1*2^3$
	4. $= 1 + 0 + 4 + 8 = (13)_{10} = (D)_{16}$
	
	5. $(0101)_2 = 1*2^0 + 0*2^1 + 1*2^2 + 0*2^3$
	6. $= 1 + 0 + 4 + 0 = (5)_{10} = (5)_{16}$