# Camotica
Documento di analisi del problema ed elenco funzionalità dell'applicazione Camotica

1. Introduzione:

La domotica è un campo in rapida crescita che combina tecnologia e comfort domestico. Il tipo di domotica che utilizzerò in questa applicazione è di tipo Centralizzato perchè è presente un'unità di controllo.
L’obiettivo è sviluppare un’applicazione client-server che permetta agli utenti di controllare tutti gli elettrodomestici, luci, termostati e sistemi di sicurezza direttamente dal dispositivo mobile e da remoto. 

2. Definizione del Problema:

Chiunque ha bisogno di essere in casa per poter utilizzare i propri elettrodomestici, svolgere le mansioni casalinghe, poter accendere o spegnere le luci o accedere alla videosorveglianza.
Sprechiamo anche molti soldi per la bolletta, a causa delle luci lasciate accesse o inquiniamo l'ambiente con elettrodomestici datati e non più funzionali. Con Camotica e il collegamento da remoto tutte queste cose si possono evitare. 
L'applicazione è supportata da un'unità centrale e da vari adattatori universali che permettono il collegamento da app a dispositivi domestici, questi prodotti fisici vengono spediti e consegnati al cliente.
Una volta installata l'unità centrale che poi sostiene gli adattatori, l'applicazione sarà utilizzabile tramite l'acquisto di un abbonamento, con vari livelli disponibili, che permettono di gestire i dispositivi

3. Requisiti dell’Applicazione:

Utente Registrato: Per accedere all'applicazione bisognerà registrarsi con un account che potrà essere collegato a Google o Facebook, tramite email e password. (Funzionale ed Utente)

Semplice Connessione: L'applicazione, una volta configurata, visualizzerà sul vostro dispositivo tutti gli apparecchi a cui è possibile connettersi grazie all'impianto domotico. (Funzionale e Sistema)

Produzione Unità Centrale e Adattatori: L'applicazione si occupa di produrre un home automation per rendere realizzabile il progetto, questo consiste nella produzione di un'unità centrale insieme a vari tipi di adattatori (sensori temparatura, luci, valvole) acquistabili anche separatamente sull'app. Insieme all'Unità centrale viene fornito un adattatore. (Funzionale e Sistema) 

Software Gestionale: Nel pacchetto dell'applicazione è  compresa e necessaria l'installazione di un software su pc, che permette il controllo dell'unità centrale per poter supervisionare gli adattatori che saranno controllati a loro volta dall'applicazione, per poter utilizzare i servizi desiderati. Il software è gratuito e si può installare tramite un codice che viene fornito insieme all'unità centrale. (Funzionale e Utente) 

Interfaccia Utente Intuitiva: L’applicazione avrà un’interfaccia facile da usare, ovvero che permetta agli utenti di controllare i loro dispositivi con pochi tocchi. (Non funzionale ed Utente)

Abbonamento per l'utilizzo: L'applicazione presenterà 3 livelli di abbonamento:
Livello 1: Si ottiene la possibilità di connettersi, tramite gli adattatori,  a 3 dispositivi in casa, utilizzandone 1 da remoto, un adattatore in regalo. 

Livello 2: Si ottiene la possibilità di connettersi, tramite gli adattatori,  a 5 dispositivi in casa, utilizzandone 3 da remoto, ci sono 2 adattatori in regalo e sconti su pezzi nuovi o da sostituire  

Livello 3: Si ottiene la possibilità di connettersi, tramite gli adattatori,  a tutti i dispositivi in casa, utilizzandone 6 da remoto, ci sono 3 adattatori in regalo, sconti su pezzi nuovi o da sostituire, qualsiasi supporto tecnico anche a casa. (Funzionale ed Utente)

Compatibilità con Diversi Dispositivi: L’applicazione deve essere compatibile con una varietà di dispositivi domestici di diversi produttori. (Funzionale e Sistema)

Sicurezza: Poiché l’applicazione avrà accesso a dispositivi che potrebbero compromettere la sicurezza domestica, deve avere robuste misure di sicurezza per proteggere contro accessi non autorizzati. (Dominio e Sistema)

Sostenibilità: I prodotti venduti sono sostenibili per l'ambiente e permettono il risparmio energetico tramite il controllo dei parametri funzionali dei dispositivi. (Dominio e Sistema)

Collegamento da Remoto: Gli utenti potranno ovviamente collegarsi ai loro elettrodomestici e controllare la loro casa anche se si trovano a migliaia di kilometri di distanza. (Funzionale ed Utente)

Tutorial: La mia applicazione avrà un tutorial disponibile a tutti per permettere la facile installazione dei dispositivi che permettono il collegamento domotico: 
- collega l’unità centrale a una presa e segui la configurazione
- scollega dispositivi ed elettrodomestici che vuoi controllare
- collega gli adattatori
- collega i dispositivi e gli elettrodomestici al proprio adattatore
- accedi all’unità centrale e attendi che si connetta agli adattatori e dunque ai dispositivi ad essi collegati
- procedi con l’installazione del programma che ti permette di interagire con i dispositivi
A disposizione sarà sempre disponibile il supporto tecnico da parte dello staff nel caso in cui ci siano difficoltà nell'installazione. (Non funzionale ed Utente)

4. USE CASE DIAGRAMS

Regsitrazione:
<img src="http://yuml.me/diagram/scruffy/usecase/[Utente]-(Registrazione), (Registrazione)>(Inserire Mail di Recupero), (Registrazione)>(Inserire Password e Nome Utente), [Utente]-(Login), (Login)>(Inserire Password e Nome Utente), (Registrazione)>(Inserire Telefono), (Inserire Telefono)>(Verifica con SMS), (Registrazione)>(Inserire Cognome), (Registrazione)>(Inserire Nome), (Registrazione)>(Inserire Mail), (Registrazione)>(Inserire Nome Utente), (Registrazione)<(Inserire Password Efficace), (Registrazione)<(Autenticazione Sicura a 2 Fattori), (Login)<(Nome Utente Errato), (Login)<(Password Errata), (Login)<(Recupero Nome Utente), (Login)<(Recupero Password)">

Acquistare:
 <img src="http://yuml.me/diagram/scruffy/usecase/[Utente]-(Acquista Unità Centrale ed Adattatori), (Acquista Unità Centrale ed Adattatori)>(Autenticazione), [Utente]-(Acquista Abbonamento), (Acquista Abbonamento)>(Scegliere Livello Abbonamento), (Acquista Unità Centrale ed Adattatori)>(Pagamento), (Acquista Abbonamento)>(Pagamento), (Pagamento)>(Inserire Dati Pagamento), [Staff]-(Riceve Ordine), (Riceve Ordine)>(Pagamento), [Staff]-(Rifiuta Ordine), [Staff]-(Spedisce Ordine), (Spedisce Ordine)>(Imballaggio Unità Principale ed Adattatori), [Sistema Bancario]-(Accetta Pagamento), [Sistema Bancario]-(Rifiuta Pagamento), (Rifiuta Pagamento)>(Comunica Errore)">

Software Gestionale:

 <img src="http://yuml.me/diagram/scruffy/usecase/[Utente]-(Inserisce Codice Software Gestionale),[Utente]-(Scaricare Sofware Gestionale),[Software Gestionale]-(Connesso Unità Principale), (Connesso Unità Principale)>(Scaricare Software Gestionale), [Software Gestionale]-(Gestione Unità Principale), (Gestione Unità Principale)>(Scaricare Software Gestionale), [Software Gestionale]-(Supervisione Adattatori),(Supervisione Adattatori)>(Scaricare Software Gestionale)">

Unità Centrale:

<img src="http://yuml.me/diagram/scruffy/usecase/[Corriere]-(Consegna Pacco),[Utente]-(Installazione Unità Centrale), [Utente]-(Installazione Adattatori), (Installazione Adattatori)>(Compatibilità Universale),(Installazione Unità Centrale)<(Lettura Tutorial), (Installazione Adattatori)<(Lettura Tutorial)">

Gestione Abbonamento:
<img src="http://yuml.me/diagram/scruffy/usecase/[Utente]-(Acquisto Abbonamento), (Acquisto Abbonamento)>(Autenticazione), (Acquisto Abbonamento)>(Scelta Livello Abbonamento), (Acquisto Abbonamento)>(Account Servizi Abbonato), (Acquisto Abbonamento)>(Aggiungere Carta), (Aggiungere Carta)>(Transazione)">

Collegamento Remoto: 
<img src="http://yuml.me/diagram/scruffy/usecase/[Utente]-((Acquisto Abbonamento),((Acquisto Abbonamento)>(Autenticazione), (Acquisto Abbonamento)<(Collegamento da Remoto),(Collegamento da Remoto)<(Controllo Parametri Funzionali Dispositivi)">

Supporto:

 <img src="http://yuml.me/diagram/scruffy/usecase/ [Utente]-(Richiede Supporto Online), [Utente]-(Richiede Supporto Fisico), [Staff]-(Fornisce Supporto Fisico), [Staff]-(Fornisce Supporto Online)">

Helper:

<img src="http://yuml.me/diagram/scruffy/usecase/ [Sistema Helper]-(Aiuta Collegare Unità Centrale), [Sistema Helper]-(Aiuta Scollegare Dispositivi), [Sistema Helper]-(Aiuta Collegare Adattatori), [Sistema Helper]-(Aiuta Collegare Dispositivi), [Sistema Helper]-(Aiuta Installare Software), [Sistema Helper]-(Invio Mail Recupero Nome Utente), [Sistema Helper]-(Invio Mail Recupero Password), (Invio Mail Recupero Nome Utente)>(Recupero Nome Utente), (Invio Mail Recupero Password)>(Recupero Password)"> 

5. Work Breakdown Structure (WBS):

1. CAMOTICA
├── 1.1 Registrazione Utente 10%<br>
│   ├── 1.1.1 Implementazione Accesso tramite Account Social (Google, Facebook) 
│   ├── 1.1.2 Accesso tramite Email e Password
│   ├── 1.1.3 Configurazione Iniziale dell'Applicazione
│   └── 1.1.4 Implementazione Nome Utente
├── 2.1 Produzione Unità Centrale, Adattatori 25%
│   ├── 2.1.1 Progettazione dell'Unità Centrale 
│   ├── 2.1.2 Produzione dell'Unità Centrale
│   ├── 2.1.3 Progettazione di Adattatori (sensori temperatura, luci, valvole) 
│   ├── 2.1.4 Produzione di Adattatori (sensori temperatura, luci, valvole) 
│   └── 2.1.5 Acquisto Separato degli Adattatori sull'App
├── 3.1 Software Gestionale 20% 
│   ├── 3.1.1 Creazione e Distribuzione del Software per PC 
│   └── 3.1.2 Integrazione con l'Unità Centrale e l'Applicazione Mobile
├── 4.1 Abbonamento 10%
│   ├── 4.1.1 Definizione dei Livelli di Abbonamento 
│   ├── 4.1.2 Implementazione e Gestione dei Livelli di Abbonamento
│   └── 4.1.3 Visualizzazione Dispositivi Domotici Disponibili
├── 5.1 Compatibilità e Sicurezza 20%
│   ├── 5.1.1 Test di Compatibilità con Dispositivi di Produttori Diversi
│   ├── 5.1.2 Implementazione Misure di Sicurezza Robuste 
│   ├── 5.1.3 Test Misure di Sicurezza
│   ├── 5.1.4 Valutazione Misure di Sicurezza
│   └── 5.1.5 Autenticazione a 2 Fattori
├── 6.1 Sostenibilità 5%
│   ├── 6.1.1 Analisi dell'Impatto Ambientale dei Prodotti
│   └── 6.1.2 Implementazione dei Controlli per il Risparmio Energetico
├── 7.1 Collegamento Remoto 5%
└── 8.1 Staff Helper 5%
    ├── 8.1.1 Aiuto Utente 
    └── 8.1.2 Recupero Dati Utente


6. Conclusione:

Lo sviluppo di un’applicazione per la domotica presenta molti vantaggi dal punto di vista tecnologico ma allo stesso tempo della sostenibilità.
Offre l’opportunità di migliorare significativamente il comfort e l’efficienza delle case moderne. 
Perchè usare la mia app? Questa scelta, anche se può risultare costosa, comporta il risparmio di energia e l'ecosostenibilità a sostegno dell'ambiente. Inoltre è una scelta che rende smart la propria vita, svolgendo vari compiti con dei semplici tocchi.
