# Camotica
Documento di analisi del problema ed elenco funzionalità dell'applicazione Camotica

1. Introduzione:

La domotica è un campo in rapida crescita che combina tecnologia e comfort domestico. Il tipo di domotica che utilizzerò in questa applicazione è di tipo Centralizzato perchè è presente un'unità di controllo.
L’obiettivo è sviluppare un’applicazione client-server che permetta agli utenti di controllare tutti gli elettrodomestici, luci, termostati e sistemi di sicurezza direttamente dal dispositivo mobile e da remoto. 

Gli ambiti e i prodotti applicativi alla domotica sono:

lavatrici, forni e frigoriferi smart, robot da cucina
sistemi di termoregolazione
sistemi di illuminazione
sistemi di videosorveglianza e gestione degli accessi (porte, finestre, tapparelle, cancelli e così via)
sistemi audio/video (entertainment)
sistemi di irrigazione

2. Definizione del Problema:

Chiunque ha bisogno di essere in casa per poter utilizzare i propri elettrodomestici, svolgere le mansioni casalinghe, poter accendere o spegnere le luci o accedere alla videosorveglianza.
Sprechiamo anche molti soldi per la bolletta, a causa delle luci lasciate accesse o inquiniamo l'ambiente con elettrodomestici datati e non più funzionali. 

3. Requisiti dell’Applicazione:

Utente Registrato: Per accedere all'applicazione bisognerà registrarsi con un account che potrà essere collegato a Google o Facebook, tramite email e password. (Funzionale ed Utente)

Semplice Connesione: L'applicazione, una volta configurata, visualizzerà sul vostro dispositivo tutti gli apparecchi a cui è possibile connettersi grazie all'impianto domotico. (Funzionale e Sistema)

Produzione Unità Centrale e Adattatori: L'applicazione si occupa di produrre un home automation per rendere realizzabile il progetto, questo consiste nella produzione di un'unità centrale insieme a vari tipi di adattatori (sensori temparatura, luci, valvole) acquistabili separatamente sull'app. (Funzionale e Sistema) 

Software Gestionale: Nel pacchetto dell'applicazione è  compresa e necessaria l'installazione di un software su pc, che permette il controllo dell'unità centrale per poter supervisionare gli adattatori che saranno controllati a loro volta dall'applicazione, per poter utilizzare i servizi desiderati. (Funzionale e Utente) 

Interfaccia Utente Intuitiva: L’applicazione avrà un’interfaccia facile da usare, ovvero che permetta agli utenti di controllare i loro dispositivi con pochi tocchi. (Non funzionale ed Utente)

Abbonamento per l'utilizzo: L'applicazione presenterà 3 livelli di abbonamento, ogni livello presenta dei vantaggi e più dispotivi da remoto a cui si può accedere. (Funzionale ed Utente)

Compatibilità con Diversi Dispositivi: L’applicazione deve essere compatibile con una varietà di dispositivi domestici di diversi produttori. (Funzionale e Sistema)

Sicurezza: Poiché l’applicazione avrà accesso a dispositivi che potrebbero compromettere la sicurezza domestica, deve avere robuste misure di sicurezza per proteggere contro accessi non autorizzati. (Dominio e Sistema)

Personalizzazione: Gli utenti saranno in grado di personalizzare le impostazioni in base alle loro preferenze individuali. (Funzionale ed Utente)

Sostenibilità: I prodotti sponsorizzati sono sostenibili per l'ambiente e permettono il risparmio energetico tramite il controllo dei parametri funzionali dei dispositivi. (Dominio e Sistema)

Collegamento da Remoto: Gli utenti potranno ovviamente collegarsi ai loro elettrodomestici e controllare la loro casa anche se si trovano a migliaia di kilometri di distanza. (Funzionale ed Utente)

Tutorial: La mia applicazione avrà un tutorial disponibile a tutti per permettere la facile installazione dei dispositivi che permettono il collegamento domotico: (Non funzionale ed Utente)
- collega l’unità centrale a una presa e segui la configurazione
- scollega dispositivi ed elettrodomestici che vuoi controllare
- collega gli adattatori
- collega i dispositivi e gli elettrodomestici al proprio adattatore
- accedi all’unità centrale e attendi che si connetta agli adattatori e dunque ai dispositivi ad essi collegati
- procedi con l’installazione del programma che ti permette di interagire con i dispositivi

<img src="http://yuml.me/diagram/scruffy/usecase/[Utente]-(Registrazione), (Registrazione)>(Account creato), (Registrazione)>(Navigazione), (Account creato)<(Collegamento a Google/Facebook), [Utente]-(Acquista prodotti), (Acquista prodotti)>(Autenticazione), (Acquista prodotti)<(Acquisto abbonamento), (Acquista prodotti)<(Acquisto Unità centrale ed Adattatori), (Acquista prodotti)>(Checkout), (Checkout)<(Aggiungere carta), (Aggiungere Carta)>(Transizione)">



4. Conclusione:

Lo sviluppo di un’applicazione per la domotica presenta molti vantaggi dal punto di vista tecnologico ma allo stesso tempo della sostenibilità.
Offre l’opportunità di migliorare significativamente il comfort e l’efficienza delle case moderne. 
Perchè usare la mia app? Questa scelta, anche se può risultare costosa, comporta il risparmio di energia e l'ecosostenibilità a sostegno dell'ambiente. Inoltre è una scelta che rende smart la propria vita, svolgendo vari compiti con dei semplici tocchi.
