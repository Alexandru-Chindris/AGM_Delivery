#AGM Express

AGM Express Delivery Service è una nuova realtà imprenditoriale motivata ad entrare nel
mercato delle spedizioni e consegne veloci.

Premessa
La compagnia :
  1. si avvale di un magazzino centrale per le giacenze ubicato in Via Dante Chiasserini, 15 a
  Milano
  2. ha a disposizione vari modelli di furgone per ritiri e consegne, per un totale di 10
  autovetture
  Ogni vettura esce quotidianamente per ritirare colli ed effettuare consegne, passando
  mediamente per circa 20 indirizzi differenti, sulla città di Milano
  AGM Express si avvale di un gestionale con le seguenti entità:
  - Colli
  - Veicoli
  - Clienti (indirizzi)

#Obiettivo #1: Ogni entità deve avere un’interfaccia di pagine Web che implementa le
funzioni CRUD (Create, Read, Update, Delete) con cui è possibile listare, vedere il dettaglio,
aggiungere, modificare e cancellare gli elementi
Esempio:

Relazioni tra entità:
1. Ad ogni collo corrispondono due indirizzi, uno di ritiro (inbound) ed uno di
consegna (outbound)
2. Ogni furgone esce quotidianamente con un determinato numero di colli da consegnare
3. Ogni furgone rientra ogni sera con un determinato numero di colli ritirati (da
consegnare il giorno seguente)
4. Ad ogni ritiro / consegna corrisponde un indirizzo di un cliente (oppure l’indirizzo del
magazzino di AGM Express)


#Obiettivo #2: modificare le pagine di dettaglio di ogni entità per visualizzare le entità
collegate, ed implementare le funzioni “incrociate”

Furgone
- lista colli assegnati
- assegna nuova spedizione / ritiro per il giorno corrente (creazione nuovo collo)

Collo
- assegna cliente esistente (e relativo indirizzo) per ritiro o consegna
- inserisci nuovo cliente (con relativo indirizzo) per ritiro o consegna
- assegna ad un furgone per la consegna (visualizza furgone assegnato)

#Obiettivo #3:
Nella pagina di dettaglio del Furgone:
  1. Visualizzare una mappa dei punti di passaggio per ciascun furgone (ad es: usando
     le API di google maps)
  2. Per ciascun furgone, calcolare la route migliore per ritiri e consegne. La route
     migliore è quella che passa per tutti i punti di ritiro/consegna, prediligendo i punti
     successivi più vicini a quello attuale. In breve, il furgone deve seguire un tracciato
     consumando il minor tempo/carburante possibile.


Strumenti / tecnologie a disposizione:
  - Java
  - Spring / MVC / Thymeleaf / Javascript / CSS
  - MySQL/ MariaDB
  
  
  #Pianificazione
![IMG-20220613-WA0076](https://user-images.githubusercontent.com/89776299/173372184-3564ff2d-0f75-4bbb-93d0-a33aea5f02e0.jpg)
![IMG-20220613-WA0074](https://user-images.githubusercontent.com/89776299/173372199-3595a728-8fca-4c1a-b604-e8bcd64bbbb6.jpg)
![IMG-20220613-WA0075](https://user-images.githubusercontent.com/89776299/173372208-be657a5f-ce62-4128-b3e0-a222947108ff.jpg)
