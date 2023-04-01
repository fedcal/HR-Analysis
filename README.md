# HR analysis

Questo progetto nasce con l'intenzione di creare un programma per la gestione del personale di un'azienda informatica e 
dei relativi progetti. L'utente finale sarà una persona qualificata nella ricerca del personale, la quale dovrà interrogare 
la base dati per poter visualizzare i progetti attivi e il personale assunto. 

Tramite il sistema potrà quindi stabilire se:

1. Vi è un esubero di personale, ovvero se ci sono molte più persone rispetto ai progetti attivi
2. Se vi è la necessità di assumere personale da impiegare in vari progetti
3. Se vi è una situazione normale, ovvero in cui tutto il personale è impiegato nei vari progetti

Inoltre vi è la possibilità di interrogare il sistema in merito:
1. Alle competenze del singolo lavoratore
2. Le relazioni tra i vari lavoratori
3. Verificare se un determinato soggetto ha bisogno di formazione per migliorare alcune skill
4. Verificare se un progetto può essere preso in carico in base alle persone presenti ed eventualmente avviare un percorso 
di assunzione
5. Collocare in un progetto le persone appena assunte


Per navigare il sistema si pensa di utilizzare un'interfaccia grafica, mentre i dati verranno storicizzati in un database 
relazionale. I dati verranno caricati in memoria attraverso una struttura dati chiamata grafo. Ogni nodo del grafo sarà 
costituito da un dipendente e le relazioni tra i dipendenti saranno rappresentate dagli archi tra i nodi. Non ci saranno 
nodi isolati in quanto ogni dipendente avrà un responsabile e farà parte di un team di sviluppo o di una classe di formazione. 

Ogni progetto, per essere preso in carico, dovrà rispettare le seguenti caratteristiche:
- Deve essere disponibile un Product Manager
- Deve essere presente un analista funzionale, il cui compito è quello di formalizzare le richieste del cliente
- Deve essere presente un UX designer per la gestione delle interfacce grafiche+
- Un gruppo di sviluppatori così diviso:
  - 2 sviluppatori senior
  - 2 sviluppatori middle
  - 2 sviluppatori junior

UnProduct Manager può curare gli aspetti relativi di due progetti contemporaneamente, mentre tutti le altre figure possono 
partecipare allo sviluppo di un solo progetto.
Se non sono rispettate queste caratteristiche l'HR può riservarsi di inserire il progetto in uno stato di pending della 
durata di due settimane, al fine di poter assumere le figure professionali coinvolte.
