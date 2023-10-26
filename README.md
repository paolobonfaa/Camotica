# Camotica
Documento di analisi del problema ed elenco funzionalità dell'applicazione Camotica

1. Introduzione:

La domotica è un campo in rapida crescita che combina tecnologia e comfort domestico. Il tipo di domotica che utilizzerò in questa applicazione è di tipo Centralizzato perchè è presente un'unità di controllo.
L’obiettivo è sviluppare un’applicazione client-server che permetta agli utenti di controllare tutti gli elettrodomestici, luci, termostati e sistemi di sicurezza direttamente dal dispositivo mobile e da remoto. 

2. Definizione del Problema:

Chiunque ha bisogno di essere in casa per poter utilizzare i propri elettrodomestici, svolgere le mansioni casalinghe, poter accendere o spegnere le luci o accedere alla videosorveglianza.
Sprechiamo anche molti soldi per la bolletta, a causa delle luci lasciate accesse o inquiniamo l'ambiente con elettrodomestici datati e non più funzionali.
Con Camotica e il collegamento da remoto tutte queste cose si possono evitare.

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

Regsitrazione ed Acquisti:
<img src="http://yuml.me/diagram/scruffy/usecase/[Utente]-(Registrazione), (Registrazione)>(Inserire Mail di Recupero), (Registrazione)>(Inserire Password e Nome Utente), [Utente]-(Login), (Login)>(Inserire Password e Nome Utente), (Registrazione)>(Account creato), (Registrazione)<(Navigazione), (Registrazione)<(Inserire Password Efficace), (Registrazione)<(Autenticazione Sicura a 2 Fattori), (Login)<(Nome Utente Errato), (Login)<(Password Errata), (Login)<(Recupero Nome Utente),(Login)<(Recupero Password), [Sistema Helper]-(Invio Mail Recupero Nome Utente), [Sistema Helper]-(Invio Mail Recupero Password), (Invio Mail Recupero Nome Utente)>(Recupero Nome Utente), (Invio Mail Recupero Password)>(Recupero Password), (Account Creato)<(Collegamento a Google/Facebook), [Utente]-(Acquista Prodotti), (Acquista Prodotti)>(Autenticazione), (Acquista Prodotti)<(Acquisto Abbonamento), (Acquisto Abbonamento)>(Scelta Livello Abbonamento), (Acquisto Abbonamento)>(Account Servizi Abbonato), (Acquista Prodotti)<(Acquisto Unità Centrale ed Adattatori), (Acquisto Unità Centrale ed Adattatori)>(Aggiungere Carta), (Acquisto Abbonamento)>(Aggiungere Carta), (Aggiungere Carta)>(Transazione), [Staff]-(Riceve Ordine), (Riceve Ordine)>(Transazione), [Staff]-(Rifiuta Ordine), (Rifiuta Ordine)>(Prodotto non Disponibile), [Staff]-(Spedisce Ordine), (Spedisce Ordine)>(Imballaggio Unità Principale ed Adattatori), [Sistema Bancario]-(Accetta Transazione), [Sistema Bancario]-(Rifiuta Transazione), (Accetta Transazione)>(Effettua Pagamento), (Rifiuta Transazione)>(Comunica Errore), (Comunica Errore)<(Carta Scaduta)">

Unità Centrale e Software Gestionale:
<img src="http://yuml.me/diagram/scruffy/usecase/[Corriere]-(Consegna Pacco), (Consegna Pacco)>(Arrivo Ordine Utente), [Utente]-(Installazione Unità Centrale), [Utente]-(Installazione Adattatori), [Utente]-(Richiede Supporto), [Utente]-(Scaricare Software Gestionale),[Utente]-(Inserisce Codice Software), (Installazione Adattatori)>(Compatibilità Universale),(Installazione Unità Centrale)<(Lettura Tutorial), (Installazione Adattatori)<(Lettura Tutorial), (Arrivo Ordine Utente)>(Codice Software Gestionale),(Scaricare Sofware Gestionale)>(Inserisce Codice Software),[Software Gestionale]-(Connesso Unità Principale), (Connesso Unità Principale)>(Scaricare Software Gestionale), [Software Gestionale]-(Gestione Unità Principale), (Gestione Unità Principale)>(Scaricare Software Gestionale), [Software Gestionale]-(Supervisione Adattatori),(Supervisione Adattatori)>(Scaricare Software Gestionale), [Staff]-(Fornisce Supporto Tecnico Online), (Fornisce Supporto Tecnico Online)>(Richiede Supporto)">

Gestione Abbonamento:
<img src="http://yuml.me/diagram/scruffy/usecase/[Utente]-(Acquisto Abbonamento), (Acquisto Abbonamento)>(Autenticazione), (Acquisto Abbonamento)>(Scelta Livello Abbonamento), (Acquisto Abbonamento)>(Account Servizi Abbonato), (Acquisto Abbonamento)>(Aggiungere Carta), (Aggiungere Carta)>(Transazione), [Utente Abbonato]-(Abbonamento Livello 1), [Utente Abbonato]-(Abbonamento Livello 2), [Utente Abbonato]-(Abbonamento Livello 3), [Utente Abbonato]-(Gestione Adattatori),(Abbonamento Livello 1)>(Controllo 3 Dispositivi), (Abbonamento Livello 1)>(Controllo da Remoto 1 Dispositivo), (Abbonamento Livello 1)>(Adattatore Regalo), (Abbonamento Livello 2)>(Controllo 5 Dispositivi), (Abbonamento Livello 2)>(Controllo da Remoto 3 Dispositivi), (Abbonamento Livello 2)>(2 Adattatori Regalo), (Abbonamento Livello 2)>(Sconti Pezzi), (Abbonamento Livello 3)>(Controllo Dispositivi), (Abbonamento Livello 3)>(Controllo da Remoto 6 Dispositivi),(Abbonamento Livello 3)>(3 Adattatori Regalo), (Abbonamento Livello 3)>(Sconti Pezzi),(Abbonamento Livello 3)>(Supporto Tecnico a Casa)">

Collegamento Remoto e Helper:
<img src="http://yuml.me/diagram/scruffy/usecase/[Utente Abbonato]-(Collegamento da Remoto),(Collegamento da Remoto)>(Autenticazione), (Collegamento da Remoto)>(Acquisto Abbonamento),(Collegamento da Remoto)<(Controllo Parametri Funzionali Dispositivi), (Controllo Parametri Funzionali Dispositivi)>(Acquisto Abbonamento), [Sistema Helper]-(Aiuta Collegare Unità Centrale), [Sistema Helper]-(Aiuta Scollegare Dispositivi), [Sistema Helper]-(Aiuta Collegare Adattatori), [Sistema Helper]-(Aiuta Collegare Dispositivi), [Sistema Helper]-(Aiuta Installare Software)"> 

5. Conclusione:

Lo sviluppo di un’applicazione per la domotica presenta molti vantaggi dal punto di vista tecnologico ma allo stesso tempo della sostenibilità.
Offre l’opportunità di migliorare significativamente il comfort e l’efficienza delle case moderne. 
Perchè usare la mia app? Questa scelta, anche se può risultare costosa, comporta il risparmio di energia e l'ecosostenibilità a sostegno dell'ambiente. Inoltre è una scelta che rende smart la propria vita, svolgendo vari compiti con dei semplici tocchi.
