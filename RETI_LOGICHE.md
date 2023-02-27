# Macchina Digitale
![[macchina digitale]]

# Segnali Digitali ed Analogici

## segnali analogici
![[segnali analogici]]
## segnali digitali
![[segnali digitali]]
## segnali binari
![[segnali binari]]

# Bit
Per descrivere a livello logico un [[segnali binari|segnale binario]], uso una variabile binaria: **bit**.
![[bit]]

# Codici binari
Per manetenere la robustezza del segnale binario ma rappresentare anche più informazioni, uso un [[codice binario]].
![[codice binario]]

# Livelli di Astrazione
Un sistema complesso è articolati su più livelli, dunque è necessario **astrarre**.
![[astrazione]]

# Reti Logiche
![[rete logica]]

## Gate
![[gate]]


# Diagrammi ad occhio
per rappresentare l'evoluzione di gruppi di [[segnali binari]] in forma compatta.
Dato che i segnali analogici non cambiano valore istantaneamente, vengono riportati anche i transitori alla successiva configurazione.

# Bus di segnali
bus:  insieme di segnali

# Ritardi di propagazione

Dato che i [[gate]] sono componenti reali, esiste un ritardo di propagazione.
Quando cambia un ingresso di un gate, l'uscita non cambia istantaneamente, ma dopo un tempo $t_p$ che dipende dalla tecnologia usata.

Questo ritardo è un ritardo "inerziale": un impulso di durata $< t_p$ su uno degli ingressi non appare in uscita.
Dunque esiste un limite superiore per la velocità di funzionamento di ogni gate.
![[Pasted image 20230225124255.png]]

# Montaggi gate
Dati due [[gate]], è possibile montarli:
1. in **serie**
2. in **parallelo**
3. in **retroazione** (uscita di un gate è ingresso dell'altro e viceversa)

# Conversione A/D e D/A
Se input ed output sono [[segnali analogici]], è possibile convertirli in [[segnali binari|binari]] e viceversa.
#esempio 
	scena reale, è possibile convertirla in un immagine digitale.

# Informazione
![[informazione]]

Guarda definizione [[codice binario]].

# Proprietà di un codice
Un codice è una rappresentazione convenzionale dell'[[informazione]].
La scelta di un codice deve essere condivisa da sorgente e destinazione, ed ha due gradi di libertà:
1. il numero di bit
2. l'associazione tra configurazioni ed informazioni

A parità di n ed M, le configurazioni possibili sono 
$$C = 2^n!/(2^n-M)!$$

## Codici ridondanti
Dato che la condizione per rendere necessaria la codifica è $2^n\geq M$, allora il numero minimo di [[bit]] è: $n_{min} = [log_2{M}]$
- un codice che usa un numero $n> n_{min}$ è detto **codice ridonante**.

Gli umani preferiscono il ridondante, da maggiore robustezza.

### Codice a 7 segmenti 
Il codice per visualizzare a schermo i numeri decimali, è **ridondante**.
	(0 acceso, 1 spento)

### Universal Product Code
è un codice ridondante per associare un valore numerico ad un prodotto.
![[Pasted image 20230227193119.png]]
Per essere più leggibile dalla macchina inizia col bianco e finisce col nero sempre.

![[rappresentazione dei numeri]]

