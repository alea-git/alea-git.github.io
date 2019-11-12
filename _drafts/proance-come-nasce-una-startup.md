---
author: Alessandro Trezza
title: "[Proance] Come nasce una startup"
date: 2019-11-13 09:00:00 +0000
description: In questo articolo troverai come siamo arrivati ad ideare Proance e il
  racconto del primissimo giorno in cui abbiamo iniziato a lavorarci.
featured_image: ''

---
Una startup di successo nasce sempre dalla volontà di **risolvere un problema**. Succede che si incontra una difficoltà mentre si sta facendo un qualcosa e si intuisce che, grazie alle proprie competenze, si è in grado di aiutare le altre persone ad evitare le stesse complicazioni. È così che, da qualche mese, io e Gabriel siamo entrati nell’ottica di creare più side-project, anche contemporaneamente ([_sul nostro sito_](https://www.aleamakers.com "Homepage Alea Makers") abbiamo pubblicato i tre più significativi).

Questa è una premessa necessaria per introdurre la nascita di Proance.

Per entrare nel vivo dell’articolo, tutto è iniziato quando ci siamo ritrovati ad avere dei **conti da gestire**: segnarci tutte l’entrate, uscite, quanti soldi personali avessimo investito, capire il margine per ogni conversione in relazione alle spese effettuate. Avere sotto controllo questo tipo di informazioni è importante per chiunque faccia impresa; per chi lavora nel mondo digital come noi, che ogni giorno si sforza di essere data driven, ovvero di basare le proprie scelte strategiche sui dati ricevuti dai test effettuati ciclicamente, lo è in modo particolare.

Quasi d’impulso, per risolvere questa necessità, ho iniziato ad utilizzare il classico foglio di calcolo stile Excel, su Google Drive. Richiede un po’ di tempo per impostare tutte le formule, però è gratuito, personalizzabile e svolge bene il suo dovere.

Ovviamente, l’aggiornamento dei dati avveniva in modo manuale: ad ogni vendita o ad ogni spesa effettuata, dovevo ricordarmi di accedere al mio Drive, aprire il file, scegliere la tabella giusta, inserire la data, la descrizione e l’importo. È bastato poco tempo per capire che urgeva una soluzione per automatizzare questo processo.

Ho iniziato a fare delle ricerche sui servizi già presenti sul mercato, fino a quando ho trovato Zapier. Mi ha convinto poiché serve proprio per far comunicare servizi differenti (come Google Drive e Stripe, il nostro gestore di pagamenti), in modo da aggiornare in autonomia determinati parametri.  Ad esempio, nel nostro caso è stato utile per aggiungere una riga nella tabella delle entrate ogni volta che Stripe registrava una vendita.

Tutto è filato liscio finché, un bel giorno, il periodo di prova gratuita di Zapier è scaduto. È un servizio necessario perché permette di risparmiare molto tempo, quindi decido di volerlo utilizzare, anche pagando. Scopro, però, che le automatizzazioni che avevo creato, nonostante fossero basilari, mi sarebbero costate almeno € 20 al mese. Sicuramente l’avrei acquistato se avessi avuto delle entrate fisse maggiori; per gestire un piccolo side-project, però, non mi è sembrato il caso spendere quella cifra.

Un breve riepilogo per tirare le somme: dobbiamo gestire abbastanza informazioni economico/finanziare da rendere opportuna l’aggiornamento automatico dei dati ma non a sufficienza da poter investire la cifra richiesta dai servizi già presenti sul mercato. Con queste premesse, abbiamo deciso di iniziare a lavorare su Proance.

In realtà non è stata una scelta così sequenziale come potrebbe sembrare: per diverse settimane mi sono portato dentro una sensazione di insoddisfazione, finché, in modo del tutto inaspettato, è uscita fuori l’idea di un servizio che potesse risolvere questo problema a noi e a chiunque altro si fosse trovato nella stessa situazione.

Dopo le prime impressioni tramite diverse telefonate e scambi di messaggi su Telegram, ci siamo riuniti e abbiamo iniziato a parlarne davanti ad una lavagna bianca attaccata al muro del nostro (temporaneo e ormai ex) ufficio.

Per prima cosa, ci siamo raccontati, senza interromperci, come ci immaginavamo il servizio, per capire se ci fossero dei punti in comune, dopodiché abbiamo iniziato a scrivere.

_Ci tengo a far notare che, se non avessimo abbracciato il movimento Open Startup, per me sarebbe stato impensabile riportare le lavagne, peraltro con l’aggiunta della spiegazione. Di seguito, non solo racconterò l’idea ma anche tutti ragionamenti che abbiamo fatto, così da poter seguire il filo logico che porta alle nostre scelte. Questo è possibile per via dei principi introdotti nel_ [_primo articolo del nostro blog_](https://www.aleamakers.com/blog/ci-uniamo-al-movimento-open-startup-we-grow-we-make-we-share 'Articolo "Ci uniamo al movimento Open Startup" dal blog di Alea Makers')_, che ti invito a leggere._

![](../board1.jpeg)

Ci siamo trovati d’accordo sul fatto che dovesse essere un servizio immediato, dunque, un’app mobile. Abbiamo comunque valutato la versione desktop e web, trovandole sconvenienti in questa prima fase del progetto, sopratutto tenendo presente che Gabriel è specializzato in Flutter (_framework creato da Google che permette di sviluppare app native per Android e iOs con un unico codice_).

Dopodiché, abbiamo definito il target: startuppers, makers, ma anche chi vende online prodotti non digitali. In una parola, digital entrepreneurs.

Per essere più specifici, poiché non avrebbe senso creare un’app per gestire le finanze di grosse aziende dato che esistono software strutturati e molto complessi che già soddisfano i loro bisogni, vogliamo rivolgerci in particolare ad imprenditori digitali con progetti in fase iniziale, gli early stage project. Vogliamo che sia un servizio utilizzabile anche gratuitamente se l’ammontare delle transazioni rientra in un certo limite, proprio per essere utili a chi dovesse trovarsi nella situazione che ho descritto nell’introduzione di questo articolo.

Determinata la piattaforma e il nostro pubblico, abbiamo iniziato a definire le macro-funzionalità del servizio, suddividendoli in due categorie: gestore finanze e analytics.

La prima è la classica app bancaria, con cui controllare le entrate/uscite, mentre la seconda riguarda tutta la parte di elaborazione dati, con cui creare grafici e indicatori utili all’imprenditore per capire l’andamento del proprio progetto.

In generale, in questa prima lavagna, è uscito il concetto di un’app che potesse diventare il centro di controllo sul proprio progetto, con tutti i dati utili e necessari in primo piano.

![](../board2.jpeg)

Nella seconda lavagna, abbiamo iniziato ad analizzare il gestore delle finanze, cercando gli attributi necessari per avere i dati giusti da poter elaborare nell’analytics.

La base degli attributi sono i tag, alcuni obbligatori (come il customer) e altri facoltativi e personalizzabili (molte di quelle chiavi, allo stato attuale, non sono state implementate perché ritenute, in un secondo momento, superflue).

L’appunto in alto a sinistra sull’account, indica che un progetto può avere solo un account, dunque non è prevista, al momento, la condivisione tra membri; dato che sarebbe dispendioso, in termini di tempo, implementare il multi account,  si utilizzano le stesse credenziali su vari dispositivi.

![](../board3.jpeg)

Nel terza lavagna abbiamo cercato di identificare e definire quali indicatori inserire nel monitor, ovvero il gestore delle finanze, e nell’analytics.

Nel monitor sono presenti i dati grezzi mentre nell’analytics forniamo grafici sulla base di informazioni elaborate (come elencato sulla lavagna).

Abbiamo anche definito la necessità di gestire i prodotti venduti, così da poter calcolare grafici più precisi. In generale, a tutti i dati si potranno applicare dei filtri temporali, oltre che poterli comparare tra loro.

![](../board4.jpeg)

Nella quarta lavagna, forse la più importante, abbiamo definito la value proposition, ovvero ciò che offriamo e che ci contraddistingue sul mercato. Il nostro approccio è stato quello di esplorare più possibilità, scegliendo poi, alla fine, quella a noi più congeniale.

La prima proposta è stata quella di offrire l’integrazione con i servizi più utilizzati da chi vende online,  come Stripe e Shopify, in modo da permettere l’importazione automatica dei propri dati.

Un’altra strada potrebbe essere quella di predisporre il servizio all’Open Startup, così da offrire un servizio specifico per una particolare nicchia facente parte del nostro target.

Una necessità che ho riscontrato personalmente è quella di avere uno strumento che aiuti nella gestione dei conti tra i fondatori di un progetto, per capire quanti soldi personali sono stati investiti da ognuno e tutti i dati che ne conseguono nel momento della suddivisione di eventuali utili.

In fine, un assistente personale che riesca a dare dei consigli in base all’andamento del progetto e la possibilità di creare e gestire dei budget, ad esempio per il marketing o per lo sviluppo di un prodotto.

Dopo aver scritto tutte le proposte, che saranno tutte implementate in futuro, abbiamo scelto quelle da inserire nell’MVP, ovvero l’integrazione con Stripe e una versione base dell’assistente personale.

![](../board5.jpeg)

Inizia il caos. Quando ci si trova sulla stessa lunghezza d’onda e delle cose interessanti iniziano a venire a galla, succede che si parla di più argomenti insieme.

In questa lavagna si è cercato di entrare nel dettaglio sui tabs da inserire all’interno dell’app, iniziando ad abbozzare un principio di grafica, per farci un’idea. Intanto, si è parlato del business model (in alto a destra), di quali grafici dovesse avere il compare (l’analytics) e quali informazioni chiedere durante la creazione di un nuovo account.

È uscita anche l’idea di inserire delle scorciatoie nella prima schermata, così da velocizzare l’aggiunta di quelle entrate o uscite ripetitive.

![](../board6.jpeg)

Come da titolo, abbiamo approfondito il tab del monitor, scegliendo quali informazioni inserire e in che ordine. È stato definito il concept grafico della schermata principale, scegliendo di inserire in alto uno spazio riservato alla cassa, poi quattro tasti per le shortcuts (di cui uno per iniziare una chat per inviare richieste/feedback) e sotto i diversi grafici delle voci scelte e riportate sulla sinistra della lavagna.

Nella parte centrale inferiore è accennato un piccolo algoritmo di prova per l’assistente personale.

La sensazione che si prova durante questi momenti iniziali è uno dei motivi per cui, molto probabilmente, le persone come noi continuano a sfornare progetti. Amiamo il processo di creazione, è uno stimolo fortissimo alla propria creatività e intraprendenza ed è ciò che principalmente vorrei comunicare con il blog di Alea Makers.

Nel prossimo articolo approfondirò la strategia di comunicazione, basandomi sull’ultima lavagna fatta in questo giorno.

Seguici su [Instagram](https://www.instagram.com/aleamakers/ "Profilo Instagram di Alea Makers") per scoprire il dietro le quinte in presa diretta e su [LinkedIn](https://www.linkedin.com/company/aleamakers/ "Profilo LinkedIn di Alea Makers") per restare aggiornato sui nuovi articoli, grazie!