Definizione [[rete logica]] (struttura e comportamento, analisi e sintesi)
![[Pasted image 20230301223806.png]]

#esempio 
esempio di **macchina combinatoria**:
- [[trascodifica]] codice BCD/7 segmenti
	7 uscite univocamente determinate dal valore corrente dei 4 ingressi che codificano un numero senza segno tra 0 e 9.
- il dizionario

## Cassaforte
- macchina con due ingressi (x,y) ed un uscita (z)
- z = 0/1 cassaforte chiusa/aperta
- se ad esempio si apre solo con una sequenza corretta $\implies$ dipende dalla *storia*:
	**macchina sequenziale**
		l'[[informazione]] è insufficiente a determinare il comportamento della macchina, dipende dalla storia

# Combinatoria vs Sequenziale
1. Rete **combinatoria**: uscita dipende unicamente dagli ingressi correnti.
2. Rete **sequenziale**: uscita dipende anche dalla storia passata (ingressi precedenti o scorrere del tempo) 

Se in presenza di una stessa configurazione di ingressi la rete deve fornire più uscite diverse, allora è sequenziale.

#finisci (fai nota per reti combin e seq).