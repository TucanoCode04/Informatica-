##Interazioni tra processi
Si classifica la modalità di interazione tra due processi in vase alla consapevolezza l'uno dell'altro:
- ignari(indipendenti) : competono per le risorse, il sistema operativo deve fornire meccanismi di sincronizzazione per risolvere la competizione
- indirettamente a conoscenza(condividono risorse al fine di scambiarsi informazioni): cooperano, il sistema operativo fornisce meccanisci per la sincronizzazione
- direttamente a conoscenza(comunicano tramite id): cooperano, il sistema operativo fornisce meccanisci di comunicazione

#####Proprietà di un programma concorrente(attributo vero per ogni storia di esecuzione)
- <b>Safety</b>: il programma se avanza va nella direzione voluta. Consensus: un processo deve decidere un valore proposto, se sono due processi devono scegliere lo stesso
- <b>Liveness</b>: il programma avanza, non si ferma. Consensus: prima o poi ogni processo prenderà una decisione

Consensus: ogni processo propone un valore, tutti i processi alla fine si devono accordare su uno dei valori proposti

#####Programmi sequenziali:
- la safety esprime correttezza dello stato finale
- la liveness esprime la terminazione
#####Programmi concorrenti:
- 