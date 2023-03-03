## rete logica definizione:
![[rete logica#definizione]]

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

# Rete logica combinatoria
I valori delle variabili di uscita dipendono solo dai valori contemporanei delle variabili di ingresso

# Composizione e decomposizione
La disposizione in **serie** e/o in **parallelo** di reti logiche combinatorie è ancora una rete logica combinatoria $\implies$ per progettare rete con m uscite, si possono progettare m reti con una sola uscita, operanti in parallelo

# Funzioni complete ed incomplete
![[funzione completa]]
![[funzione incompleta]]

# Tabella della verità
![[tabella della verità]]

## Convertitore BCD/7 segmenti
-  sono in realtà 7 funzioni in parallelo di 4 ingressi
- la descrizione a parole NON è univoca (esempio come scrivere 6?)
Solo la [[tabella della verità]] ci permette di descrivere il **comportamento** di una **macchina combinatoria** in modo NON ambiguo
 
# Funzioni complete di n variabili
il numero di distinte funzioni di n variabili binarie è: $$\phi(n)=2^{2^n}$$
aumenta esponenzialmente con n.

è dunque il progettista a dover realizzare ogni funzione tramite composizione di [[gate]] disponibili in forma di circuiti integrati

# Fase di sintesi: da comportamento a struttura
![[Pasted image 20230303154232.png]]

![[algebre binarie]]

## Schema logico
![[schema logico]]


## [[schema logico|schemi logici]] $\to$ [[espressione|espressioni]]
1. relazione 1: ogni struttura formata da [[gate]] connessi in serie e/o in parallelo è descritta da una sola [[espressione]] 

#esempio 
![[Pasted image 20230303150937.png]]

## [[espressione|espressioni]] $\to$ [[schema logico|schemi logici]]
2. relazione 2: ogni [[espressione]] descrive una sola struttura formata da [[gate]] connessi in serie e/o in parallelo

### per indiividuare lo schema di un'espressione:
1. si parte da *parentesi più interne* e si traccia il simbolo del [[gate]] corrispondente all’operazione, collegandone gli ingressi ai segnali esterni
2.  modo analogo con le altre coppie di parentesi, considerando via via come ingressi dei nuovi gate anche le uscite di quelli già tracciati.

#esempio 
![[Pasted image 20230303151012.png]]

#esempio 
![[Pasted image 20230303152410.png]]

### [[espressione]] = [[schema logico]]
- relazione **biunivoca** tra schemi ed espressioni
- per esprimere la struttura sono indifferenti
- [[espressione]] è più compatta

#### Valutazione di un'[[espressione]]
(di n variabili per una n-upla di valori)
1. si sostituisce ad ogni variabile il valore che ha nella n-upla
2. dalle parantesi più interne, si sostituisce ogni operazione con il suo risultato fino ad ottenere o 0 o 1

#esempio 
![[Pasted image 20230303153542.png]]

#### numero di valutazioni
una [[espressione]] di n variabili, può essere valutata in $2^n$ modi diversi
$\implies$ valutando un'espressione per tutte le $2^n$ configurazioni, ottengo la [[tabella della verità]] (**comportamento**).

3. relazione 3: Ogni espressione descrive una e una sola [[tabella della verità]] **completamente specificata**

# Fase di analisi
- risultato univoco: partendo da un dato [[schema logico]] o da un’[[espressione]], si può determinare in modo univoco il **comportamento** (la [[tabella della verità]]) che realizzano 
![[Pasted image 20230303154205.png]]

Relazione 4: Una **funzione** può essere descritta da una molteplicità di [[espressione|espressioni]]

