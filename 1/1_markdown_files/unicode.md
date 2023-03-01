- problema: architetture e linguaggi programmazione operano su gruppi di byte (8 [[bit]]).
Dunque 3 standard per mappare carattere unicode da 21 bit in una sequenza di byte **non ridondanti**.

1. UTF-32
	usa 32 [[bit]] (**4 byte**) per ogni carattere $\to$ aggiunge 11 volte 0 a sinistra
1. UTF-16
	usa **2 byte** per caratteri più comuni (63000) e **4 byte** per i restanti
2. UTF-8
	**1 byte** per 128 [[codice ASCII|ascii]], **2 byte** per altri 1920, **3-4byte** per gli altri