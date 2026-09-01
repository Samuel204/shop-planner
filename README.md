# Purchase Planner

**Purchase Planner** è una dashboard web personale, che permette di pianificare e organizzare nel tempo gli acquisti di beni secondari o non essenziali.

L'obiettivo non è creare una semplice wishlist, ma **gestire quando effettuare un acquisto**, evitando di concentrare troppe spese nello stesso periodo.

La dashboard presenta i mesi in ordine cronologico, organizzati verticalmente. Non è necessario mostrare i singoli giorni del mese: ogni mese rappresenta semplicemente una finestra temporale nella quale pianificare determinati acquisti.

## Funzionamento

Per ogni mese è possibile aggiungere gli oggetti che si desidera acquistare.

Ogni elemento può contenere:

* nome del prodotto;
* breve descrizione o nota;
* prezzo stimato;
* URL del sito in cui acquistarlo;
* stato dell'acquisto;
* eventuali note aggiuntive.

Gli elementi vengono salvati direttamente nel **Local Storage del browser**, quindi i dati rimangono disponibili anche dopo aver chiuso o ricaricato la pagina.

## Il problema da risolvere

Il sistema non deve trasformarsi in una wishlist infinita.

Un problema possibile è che, ogni volta che viene in mente qualcosa da acquistare, si finisca per inserirlo immediatamente nel mese corrente o in quello successivo. In questo modo la dashboard perderebbe il suo scopo principale: aiutare a distribuire le spese.

Per questo motivo il progetto deve introdurre un sistema di **controllo degli acquisti mensili**.

### Limite mensile

Ogni mese dovrebbe avere un numero massimo di acquisti programmabili, ad esempio **3 acquisti**.

Quando il limite viene raggiunto, il sistema dovrebbe suggerire di:

* spostare l'acquisto a un mese successivo;
* scegliere quale acquisto ha maggiore priorità;
* oppure inserire l'oggetto in una sezione separata di **idee future**, che non occupa uno slot del mese.

In questo modo un nuovo prodotto che viene in mente non viene automaticamente trasformato in un acquisto imminente.

## Priorità degli acquisti

Ogni elemento potrebbe avere un livello di priorità, ad esempio:

* **Alta** — acquisto che voglio effettuare nel periodo stabilito;
* **Media** — acquisto desiderato, ma rimandabile;
* **Bassa** — acquisto secondario da valutare in futuro.

La priorità può aiutare a decidere quali elementi mantenere nei mesi più vicini e quali spostare più avanti.

## Sezione "Future Ideas"

Per evitare che ogni nuova idea venga immediatamente assegnata a un mese, dovrebbe essere presente una sezione separata per gli acquisti futuri.

Questa sezione funziona come un **parcheggio temporaneo delle idee**.

Esempio:

> Mi viene in mente che vorrei comprare delle cuffie.

Invece di inserirle automaticamente ad agosto, posso salvarle nelle **Future Ideas**.

Successivamente, quando pianifico i mesi successivi, posso decidere se e quando assegnarle a un mese.

In questo modo il sistema distingue chiaramente tra:

**"Mi piacerebbe avere questa cosa"**

e

**"Ho deciso di comprarla in questo periodo."**

## Obiettivo

Il progetto deve quindi aiutare a rispondere a tre domande:

1. **Cosa voglio acquistare?**
2. **Quando voglio acquistarlo?**
3. **Quanti acquisti posso permettermi di programmare in quel mese?**

L'obiettivo finale è creare uno strumento semplice per **pianificare gli acquisti, distribuire le spese e ridurre gli acquisti impulsivi**, senza trasformare il progetto in un sistema di gestione finanziaria complesso.

## Tecnologie

* HTML
* CSS
* JavaScript
* Local Storage API (github git)

Non è previsto un backend: tutti i dati vengono memorizzati localmente nel browser.
