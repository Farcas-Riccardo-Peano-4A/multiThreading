# multiThreading
## Teoria
Un thread è molto simile ad un programma sequenziale ma non può essere eseguito in modo indipendente, deve essere eseguito all'interno di un programma. Si  possono  utilizzare  più threads  all’interno  di  un singolo programma; essi  eseguiranno  allo  stesso  tempo  ma  eseguono tasks differenti.
Nella classe che estende il thred si crea un metodo run() che il main non chiamerà direttamente, se si vuole avviare un thread t bisogna fare una chiamata "t.start". Il multithreading è l'esecuzione contemporanea di diversi thread nell’ambito di uno stesso processo.

## Esercizio 1 
Abbiamo creato un progetto contenente due classi che stampano **"Hello"** e **"Hi"** 10 volte per ciascuno. L'output stampa le parole in ordine casuale ad ogni esecuzione poichè è il sistema operativo che in base al protocollo li esegue prima.

Esecuzione 1:

Hi
Hi
Hi
Hi
Hi
Hi
Hi
Hi
Hi
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hi

Esecuzione 2:

Hi
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hi
Hi
Hi
Hi
Hi
Hi
Hi
Hi
Hi

Esecuzione 3:

Hi
Hi
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hi
Hi
Hi
Hi
Hi
Hi
Hi
Hi

## Esercizio 2
Abbiamo creato una nuova classe **"Say"** che riceve un parametro Stringa e lo stampa 10 volte, il main crea 2 variabili di tipo "Say" e chiama la classe tramite la chiamata "nomeVariabile.start"; la classe "Say" stampa i due parametri in ordine casuale come l'esecizio 1.
Questo esercizio ci fa comprendere come sia possibile ricreare l'esercizio 1 usando una classe unica anzichè dover creare una classe per ogni parametro che vogliamo passare.

Esecuzione 1:

Hi
Hi
Hi
Hi
Hi
Hi
Hi
Hi
Hi
Hello
Hello
Hello
Hello
Hi
Hello
Hello
Hello
Hello
Hello
Hello

Esecuzione 2:

Hi
Hi
Hi
Hi
Hi
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hi
Hi
Hi
Hi
Hi

Esecuzione 3:

Hi
Hi
Hi
Hi
Hi
Hi
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hello
Hi
Hi
Hi
Hi
