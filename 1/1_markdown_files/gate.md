# Gate con 1 ingresso
- il numero di funzioni diverse di n ingressi binari con uscita binaria è $$2^{2^n}$$
- i componenti elementari (funzioni) sono quindi 4.
- tolte identità e costanti, rimane una funziona: l'operatore NOT

## Gate NOT
![[Pasted image 20230223223123.png]]
# Gate con 2 ingressi
$2^{2^n}$ con $n=2$, dunque 16 possibili funzioni elementari

## Gate AND
- [[astrazione]] di due [[interruttore|interruttori]] in **serie**:
	![[Pasted image 20230223223316.png]]
- ![[Pasted image 20230223223343.png]]

## Gate OR
- [[astrazione]] di due [[interruttore|interruttori]] in **parallelo**:
	![[Pasted image 20230223223544.png]]
- ![[Pasted image 20230223223556.png]]

## Gate EXOR
- EXCLUSIVE OR
- astrazione di due deviatori
- assume valore 1 se un ingresso ha valore 1 ma non entrambi
- ![[Pasted image 20230223223757.png]]
- anche detto **somma a modulo 2** (output interpretato come risultato somma dei due bit)
# Gate con più ingressi
- AND vale 1 se tutti gli ingressi hanno valore 1
- OR vale 1 se almeno un ingresso ha valore 1
- EXOR vale 1 se se e solo se il numero di '1' in ingresso è dispari

# Gate negati:
## NAND
## NOR
## EXNOR

![[Pasted image 20230223224204.png]]

- EXNOR anche chiamato EQUIVALENCE perchè in **due ingressi** ha uscita 1 solo se entrambi gli ingressi sono uguali (non vale per più ingressi)

Tutti ottenibili da un NOT a cascata:
	![[Pasted image 20230223224338.png]]