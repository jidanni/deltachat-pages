---
title: FAQ
lang: it
render_toc: true
header: Frequently Asked Questions
---


## Cos'è Delta Chat? 

Delta Chat è una nuova app di chat che invia messaggi tramite e-mail, se possibile crittografati, con Autocrypt. 
**Non devi registrarti da nessuna parte, usa semplicemente il tuo account e-mail esistente con Delta Chat.**

<img style="float:right; width:50%; max-width:360%; margin:1em;" src="../assets/home/delta-what-optim.png" />


### Come posso trovare persone con cui messaggiare? 

Con Delta Chat puoi scrivere a qualsiasi indirizzo e-mail esistente, anche
se il destinatario non sta utilizzando l'app Delta Chat. Non c'è bisogno per il
destinatario di installare la tua stessa app, come con altri messenger.


### Quali sono i vantaggi di Delta Chat rispetto ad altri messenger?

- _Indipendente_ da qualsiasi azienda o servizio. _Tu_ possiedi i tuoi dati.
- I tuoi dati non vengono salvati su un server centrale a meno che non vengano utilizzati da tutti gli utenti
gli stessi server e-mail
- Non distribuisce la tua rubrica a nessuno.
- _Veloce_ grazie all'uso di Push-IMAP.
- _Base utenti più numerosa_: è possibile raggiungere anche i destinatari che _non_ utilizzano Delta Chat.
- _No Spam_: per impostazione predefinita vengono visualizzati solo i messaggi di utenti conosciuti.
- _Crittografia end-to-end_ tramite Autocrypt.
- Software libero basato su _Copyleft_ e _Standards_.
- _Identità flessibile_ con supporto integrato per [più account](#multiple-accounts)


### Quali messaggi vengono mostrati in Delta Chat?

Per impostazione predefinita, Delta Chat mostra tutte le e-mails.

In "Impostazioni -> Chat e
Media -> Mostra E-mail Tradizionali", puoi modificare questa impostazione. Hai queste opzioni:

- "No, solo chat": solo i messaggi inviati da altri utenti di Delta Chat e le "risposte a"
vengono visualizzati i tuoi messaggi di Delta Chat. Questo ha più senso se usi lo stesso
account di posta elettronica anche per le normali e-mail.
- "Per i contatti accettati": Delta Chat mostra tutte le e-mail dei contatti con cui
hai già una chat, ma le nuove chat vengono visualizzate solo per i messaggi di Delta Chat.
Questo aiuta a decidere caso per caso se si desidera avere una
conversazione in Delta Chat o in una "normale" app di posta elettronica.
- "Sì": Delta Chat mostra tutte l'e-mail inviate al tuo indirizzo e-mail. Questo
ha senso se vuoi usare Delta Chat per tutte le tue e-mail, quindi nessun messaggio
si perde. Questa è l'impostazione predefinita.


### Cosa succede se aspetto un messaggio da qualcuno a cui non ho scritto in passato?

- Se un messaggio proviene da un contatto sconosciuto, appare come una **richiesta**. È necessario
accettare la richiesta prima di poter rispondere.
- Si può anche "cancellare" il messaggio se non si vuole più chattare con esso. Questo
non cancella il messaggio sul server, ma solo sul dispositivo. Quindi è possibile
continuare a gestire il messaggio in un'altra applicazione di posta.
- Se si elimina una richiesta, i futuri messaggi di quel contatto continueranno a essere visualizzati come richieste di contatto
in modo da poter cambiare idea. Se non si vuole davvero ricevere
messaggi da questa persona, prendete in considerazione la possibilità di *bloccarla*.


### Delta Chat supporta immagini, video e altri allegati?

- Sì. Oltre al testo normale, tutti gli allegati e-mail vengono visualizzati come messaggi separati. I messaggi in uscita ricevono automaticamente gli allegati necessari.

- Per le prestazioni, le immagini sono ottimizzate e inviate in dimensioni inferiori per impostazione predefinita, ma è possibile inviarle come "file" per preservare l'originale.

<h3 id="multiple-accounts">Come posso aggiungere o passare da un account all'altro?</h3>

Puoi facilmente lavorare con account aggiuntivi sui client mobili e desktop di Delta Chat facendo clic su:
- sul pulsante del menu e poi su "Cambia Account" (Android e desktop)
- o l'icona del profilo e poi 'Aggiungi account' (iOS)

Potresti anche voler imparare [come aggiungere account a più dispositivi](#multiclient).

### Chi vede la mia immagine del profilo?

- Puoi aggiungere un'immagine del profilo nelle tue impostazioni. Se scrivi ai tuoi contatti
o li aggiungi tramite codice QR, la vedranno automaticamente come immagine del tuo profilo.

- I contatti che non usano Delta Chat non vedono l'immagine del profilo (tuttavia, ovviamente, possono installare Delta Chat :)

- Per motivi di privacy, nessuno vede la tua immagine del profilo finché non scrivi un
messaggio a loro.

- L'immagine del tuo profilo non viene inviata con ogni messaggio, ma abbastanza regolarmente che
i tuoi contatti riceveranno nuovamente la tua immagine del profilo, anche se aggiungono un nuovo
dispositivo.


### Delta Chat supporta le e-mail HTML?

Sì, i messaggi HTML in arrivo sono dotati di un pulsante "Mostra messaggio completo".
I messaggi in uscita utilizzano sempre testo normale.


### Perché devo inserire la mia password E-Mail in Delta Chat? È sicuro?

Come con altri programmi di posta elettronica quali Thunderbird, K9-Mail o Outlook,il
programma ha bisogno della password in modo da poterla utilizzare per inviare mail. Naturalmente, la
password è memorizzata solo sul tuo dispositivo. La password viene trasmessa solo a
il tuo fornitore E-Mail (quando effettui il login), che ha comunque accesso alla tua posta.

Se utilizzi un provider E-Mail con supporto OAuth2 come gmail.com o yandex.ru,
non è necessario memorizzare la password sul dispositivo. In questo caso, solo un
token di accesso viene utilizzato.

Poiché Delta Chat è Open Source, puoi controllare il [Codice
Sorgente](https://github.com/deltachat/deltachat-core-rust/blob/master/src/login_param.rs)
se vuoi verificare che le tue credenziali siano gestite in modo sicuro. Siamo felici dei feedback che rendono l'app più sicura per tutti i nostri utenti.


### Di quali autorizzazioni ha bisogno Delta Chat?

A seconda del sistema operativo in uso,
potrebbe esserti chiesto di concedere le autorizzazioni all'app.
Questo è ciò che fa Delta Chat con queste autorizzazioni:

- Fotocamera *(può essere disabilitata)*
- scattare foto e video: per l'invio di foto
- Contatti *(possono essere disabilitati)*
- leggi i tuoi contatti: per scoprire i contatti con cui chattare
- Posizione *(può essere non consentita)*
- accedere alla posizione approssimativa (fonti di posizione di rete): per la funzione di trasmissione della posizione
- accedere alla posizione precisa (GPS e fonti di localizzazione di rete): per la funzione di trasmissione della posizione
- Microfono *(può essere disattivato)*
- registra audio: per i messaggi audio
- Memoria *(può essere disabilitata)*
- modificare o eliminare il contenuto della scheda SD: per scaricare gli allegati dei messaggi
- leggere il contenuto della tua scheda SD: per condividere file con i tuoi contatti
- Altre funzionalità dell'app
- modificare le impostazioni audio: così puoi scegliere suonerie e volume per notifiche e messaggi audio
- esegui all'avvio: così non devi avviare Delta Chat manualmente
- controllo vibrazione: per le notifiche
- visualizzare le connessioni di rete: per connettersi al proprio fornitore E-Mail
- impedisce al telefono di andare in sospensione: così puoi copiare più facilmente il codice di sicurezza durante il messaggio di configurazione di Autocrypt
- avere pieno accesso alla rete: per connettersi al proprio fornitore E-Mail
- visualizzare le connessioni Wi-Fi: per connettersi al proprio fornitore E-Mail
- chiedi di ignorare le ottimizzazioni della batteria: per gli utenti che vogliono ricevere immediatamente i messaggi

### Cosa significa Fissare, Silenziare, Archiviare?

Usa questi strumenti per organizzare le tue chat e tenere tutto in ordine:

- **Chat fissate** restano sempre in cima all'elenco. Puoi usarlo per accedere velocemente alle tue chat preferite o temporaneamente per non dimenticare alcune cose.

- **Silenzia chat** se non vuoi ricevere notifiche da queste. Le chat silenziate restano al loro posto e puoi anche fissare una chat silenziata.

- **Archivia chats** se non vuoi più vederle nel tuo elenco chat.
Le chat archiviate rimangono accessibili sopra l'elenco delle chat o tramite la ricerca.

- Quando una chat archiviata riceve un nuovo messaggio, a meno che non sia silenziata, **salterà fuori dall'archivio** e tornerà nell'elenco delle chat.
**Le chat silenziate restano archiviate** fino a che non le estrai manualmente.

Per archiviare o fissare una chat, premi a lungo (Android), usa il menu della chat (Android/Desktop) o striscia verso sinistra (iOS);
per silenziare una chat, usa il menu della chat (Android/Desktop) o il profilo della chat (iOS).


### Cosa significa il punto verde?

- A partire da Delta Chat 1.34 a volte puoi vedere un "punto verde" accanto all'avatar
  di un contatto. Significa che è stato "visto di recente".
- Nel dettaglio: significa che negli ultimi 10 minuti Delta Chat lo ha visto:
- o perché ti ha inviato un messaggio direttamente,
- perché ha scritto qualcosa a un gruppo di cui siete entrambi membri,
- perché ti ha inviato una conferma di lettura per un messaggio che hai scritto,
- o perché ha inviato dati alla tua app Delta Chat utilizzando l'
[applicazione webxdc](#webxdc).
- Quindi questo non è uno stato online in tempo reale - e se qualcuno non risponde
subito anche se sembra online, non preoccuparti e dagli un po'
di spazio ;-)
- D'altra parte, non sempre gli altri "vedranno che sei online". Se tu
hai disattivato le conferme di lettura, non vedranno il punto verde finché non lo farai tu
invia loro un messaggio o scrivi anche a un gruppo a cui appartengono.


### Come funzionano i messaggi a scomparsa? {#ephemeralmsgs}

Puoi attivare i "messaggi che scompaiono"
nelle impostazioni di una chat,
in alto a destra nella finestra della chat,
selezionando un intervallo di tempo
tra 1 minuto e 5 settimane.

Fino a quando l'impostazione non viene nuovamente disattivata,
l'app Delta Chat di ogni membro della chat si prende cura
di eliminare i messaggi
dopo l'intervallo di tempo selezionato.
Inizia il lasso di tempo
quando il destinatario vede per la prima volta il messaggio in Delta Chat.
I messaggi vengono eliminati
entrambi in ciascun account di posta elettronica sul server,
e nell'app stessa.

Tieni presente che puoi fare affidamento sui messaggi che scompaiono
solo finché ti fidi dei tuoi partner di chat;
i partner di chat dannosi possono scattare foto,
o altrimenti salvare, copiare o inoltrare messaggi prima della cancellazione.

A parte quello,
se un partner di chat disinstalla Delta Chat,
i messaggi non verranno eliminati dal loro account di posta elettronica.
Molto probabilmente non saranno più decifrabili
(a patto che siano stati crittografati in primo luogo).


### Come posso eliminare il mio account?

Poiché utilizzi un account e-mail per Delta Chat,
il modo in cui puoi eliminare il tuo account dipende dal tuo provider e-mail.
Non abbiamo alcun controllo sul tuo account e-mail,
quindi purtroppo non possiamo aiutarti in questo.

Se vuoi mantenere l'account,
ma disinstallare Delta Chat,
si consiglia di uscire da qualsiasi chat di gruppo prima di disinstallare Delta Chat.


## Gruppi

### Creazione di un gruppo

- Seleziona **Nuova chat** e poi **Nuovo gruppo** dal menu nell'angolo in alto a destra o premi il pulsante corrispondente su Android/iOS.
- Nella schermata successiva, seleziona i **membri del gruppo** e definisci un **nome del gruppo**. Puoi anche selezionare un **avatar di gruppo**.
- Non appena scrivi il **primo messaggio** nel gruppo, tutti i membri vengono informati del nuovo gruppo e possono rispondere nel gruppo (finché non scrivi un messaggio nel gruppo il gruppo è invisibile ai membri).


### Aggiungi membri a un gruppo

- Ogni componente del gruppo ha gli **stessi diritti** di ogni altro. Per questo motivo chiunque può rimuovere chiunque o aggiungere nuovi componenti.
- Per aggiungere o rimuovere i membri, fai clic sul nome del gruppo nella conversazione.


### Mi sono cancellato per sbaglio.

- Poiché non sei più un membro del gruppo, non puoi aggiungerti di nuovo.
Tuttavia, nessun problema, chiedi a qualsiasi altro membro del gruppo in una normale chat di aggiungerti nuovamente.


### Non desidero più ricevere i messaggi di un gruppo.

- Elimina te stesso dall'elenco dei membri o elimina l'intera chat.
Se vuoi unirti di nuovo al gruppo in un secondo momento, chiedi a un altro membro del gruppo di aggiungerti di nuovo.

- In alternativa, puoi anche "Silenziare" un gruppo - così facendo riceverai tutti i messaggi e
puoi ancora scrivere, ma non viene più notificato alcun nuovo messaggio.


### Cosa significano i segni di spunta visualizzati accanto ai messaggi in uscita?

- **Un segno di spunta** significa che il messaggio è stato inviato con successo al tuo fornitore.
- **Due segni di spunta** significano che almeno un dispositivo del destinatario
ha riferito di aver ricevuto il messaggio.
- I destinatari possono avere le conferme di lettura disabilitate,
quindi anche se vedi solo un segno di spunta, il messaggio potrebbe essere stato letto.
- Al contrario, due segni di spunta non significano automaticamente
che un essere umano abbia letto o compreso il messaggio ;)


### Cosa succede se attivo "Elimina Messaggi dal Server"?

- Per impostazione predefinita, Delta Chat memorizza tutti i messaggi in locale sul dispositivo. Se
ad esempio, si vuole risparmiare spazio di archiviazione presso il proprio provider di posta elettronica, è possibile scegliere di
eliminare automaticamente i vecchi messaggi. I messaggi rimangono comunque sul dispositivo finché non li si cancella anche lì.

- Per attivarlo, vai su **Elimina i vecchi messaggi → Elimina messaggi dal server**
nelle impostazioni "Chat e Media".
Puoi impostare un intervallo di tempo compreso tra "Subito" e "Dopo 1 anno".
Tutte le e-mail ricevute da Delta Chat verranno eliminate dal server dopo questo periodo di tempo.

- Tieni presente che se utilizzi Delta Chat su più di un dispositivo, è necessario lasciare il messaggio sul server con un tempo sufficiente
in modo che anche gli altri dispositivi(o) possano scaricarli.


### Cosa succede se attivo "Elimina Messaggi dal Dispositivo"? {#delold}

- Se si desidera risparmiare spazio sul dispositivo, è possibile scegliere di eliminare i vecchi
messaggi automaticamente.
- Per attivarla, andare su "Elimina Messaggi dal Dispositivo" nelle impostazioni di "Chat e Media".
È possibile impostare un intervallo di tempo compreso tra "Dopo 1 ora" e "Dopo 1 anno";
in questo modo, *tutti* i messaggi saranno eliminati dal dispositivo non appena saranno
più vecchi di quel periodo.


## Crittografia e Sicurezza

### Quali standards vengono utilizzati per la crittografia end-to-end?

[Autocrypt](https://autocrypt.org) viene utilizzato automaticamente per stabilire la crittografia end-to-end con contatti e chat di gruppo. Autocrypt utilizza un [sottoinsieme limitato e sicuro dello standard OpenPGP](#openpgp-secure). I messaggi crittografati end-to-end sono contrassegnati da un lucchetto 
<img style="vertical-align:middle; width:1.2em; margin:1px" src="../assets/help/lock-icon.png" alt="padlock"/>.

[Protocolli Secure-Join](https://securejoin.delta.chat/en/latest/new.html)
vengono utilizzati per stabilire chat con crittografia end-to-end garantita
che protegge dagli attacchi di rete e dai server compromessi.
Chat contrassegnata da un segno di spunta verde
<img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark"/>
garantisce messaggi crittografati end-to-end.

### Come posso sapere se i messaggi sono crittografati end-to-end?  {#whene2e}

Tutti i messaggi crittografati end-to-end portano un lucchetto:

<img style="width:160px; margin:1px" src="../assets/help/lock-screenshot.png" alt="padlock in bubble"/>

La crittografia end-to-end è garantita se è presente un segno di spunta verde accanto al titolo della chat:

<img style="width:211px; margin:1px" src="../assets/help/green-checkmark-screenshot.png" alt="green checkmark in title"/>


### Come posso ottenere la crittografia end-to-end garantita e i segni di spunta verdi? {#howtoe2ee}

Incontra il tuo partner di chat fuori Delta Chat, preferibilmente di persona
ma un secondo canale come una chat video
oppure va bene anche un altro messenger.
Esegui la seguente procedura di presentazione/scansione QR con il tuo partner di chat.
Uno di voi è l'"Invitante", l'altro è l'"Invitato".

**Lato invito**:

- Invito di gruppo:
Tocca il titolo del gruppo di chat per visualizzare l'elenco dei membri e seleziona "Codice QR di invito".
Condividi l'immagine QR con l'altra parte di persona o tramite un secondo canale.

- Invito diretto alla chat 1:1:
  Tocca l'icona del Codice QR <img style="vertical-align:middle; width:1.8em; margin:1px" src="../assets/help/qr-icon.png" />
  nella schermata principale dell'app Delta Chat -- 
  sul desktop l'icona QR si trova nel menu a sandwich sul lato sinistro.
  Condividi l'immagine QR con l'altra parte di persona o tramite un secondo canale.

**Lato invitato**:

- Tocca l'icona del Codice QR <img style="vertical-align:middle; width:1.8em; margin:1px" src="../assets/help/qr-icon.png" /> 
   nella schermata principale dell'app Delta Chat --
   sul desktop l'icona QR si trova nel menu a sandwich sul lato sinistro.

- Scegli "SCANSIONE CODICE QR" e scansiona il Codice QR
  che vedi dal tuo partner di chat in un secondo canale.

- Tocca "OK".


**Sia Invitante che Invitato**:

Attendere mentre [i messaggi di rete Secure-Join vengono scambiati](https://securejoin.delta.chat/en/latest/new.html#setup-contact-protocol) tra entrambi i dispositivi.

- Se entrambi i dispositivi sono online,
  entrambe le parti vedranno eventualmente una chat (di gruppo o diretta) con un segno di spunta verde
  <img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark"/>
  accanto al titolo.

- Se uno dei dispositivi è offline, verranno visualizzati solo i segni di spunta verdi
  verranno visualizzati in seguito quando il dispositivo sarà nuovamente connesso a Internet
  e il protocollo di rete Secure-Join è stato completato.

Congratulazioni!
Ora utilizzerai automaticamente la crittografia end-to-end garantita
con questo contatto potete aggiungervi a vicenda nei gruppi contrassegnati da un segno di spunta verde
<img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark"/>,
diffondendo così automaticamente la crittografia end-to-end garantita tra i suoi membri.


### Cosa significano il segno di spunta verde e la "crittografia end-to-end garantita"? {#e2eeguarantee}

Titoli di chat con segni di spunta verde
<img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark" />
significa che tutti i messaggi nella chat saranno crittografati end-to-end
e non possono essere letti o modificati da server di e-mail o provider Internet compromessi.
Partecipare alle chat di gruppo contrassegnate da un segno di spunta verde diffonde in modo sicuro le informazioni di crittografia di tutti (e i segni di spunta verdi)
in modo da garantire la crittografia end-to-end nel gruppo e tra i membri.

Profili di contatto con segni di spunta verdi
<img style="vertical-align:middle; width:1.5em; margin:1px" src="../assets/help/green-checkmark.png" alt="green checkmark" />
significa che attualmente è garantita la crittografia end-to-end dei messaggi a un contatto.
Ogni contatto contrassegnato dal segno di spunta verde ha effettuato una [scansione QR](#howtoe2ee) diretta con te
o è stato presentato da un altro contatto contrassegnato da un segno di spunta verde.
Le presentazioni avvengono automaticamente quando si aggiungono membri ai gruppi.
Chi aggiunge un contatto a un gruppo contrassegnato da un segno di spunta verde diventa un introduttore
a quei membri che non erano ancora a conoscenza del contatto aggiunto. In un profilo di contatto è possibile toccare ripetutamente il testo "Presentato da...".
fino ad arrivare a quello con cui hai effettuato direttamente una [scansione QR](#howtoe2ee).

Tieni presente che nel profilo di un contatto potresti vedere e toccare gli introduttori
ma non c'è il segno di spunta verde nel titolo del profilo.
Questo di solito significa che il contatto ["ha inviato un messaggio da un altro dispositivo"](#nocryptanymore).

Per una discussione più approfondita sulla "crittografia end-to-end garantita"
consultare [Protocolli Secure-Join](https://securejoin.delta.chat/en/latest/new.html)
e leggi nello specifico i "Gruppi Verificati", il termine tecnico
di quelle che qui vengono chiamate chat "con segno di spunta verde" o "crittografate end-to-end garantite".


### Un contatto "ha inviato un messaggio da un altro dispositivo", cosa posso fare? {#nocryptanymore}

La tua chat con un contatto che ha perso la crittografia end-to-end garantita.
Il segno di spunta verde è stato rimosso per questa chat e per questo contatto quando vedi questo avviso.
**Se riscontri l'improvvisa rimozione della crittografia end-to-end garantita
inaspettatamente per questo contatto allora non accettare l'avviso!**
Verifica invece con il tuo contatto attraverso un secondo canale
come una videochiamata, un altro messenger o una telefonata,
per scoprire cosa è successo.

Se il tuo contatto ha effettivamente causato la rimozione della crittografia end-to-end garantita
consultare i paragrafi successivi per i motivi comuni e le relative attenuazioni.
Indipendentemente da ciò, tutte le altre chat contrassegnate da un segno di spunta verde rimangono garantite con crittografia end-to-end
anche se il contatto è un membro.

**Il tuo contatto sta utilizzando Delta Chat su un secondo dispositivo (telefono o laptop)**

Se hanno un altro dispositivo con l'app Delta Chat in esecuzione,
dovrebbero rimuovere l'account dal nuovo dispositivo
e aggiungerlo [come secondo dispositivo come descritto qui](#multiclient).
Non appena ti invieranno un messaggio, l'avviso scomparirà
e la crittografia garantita viene stabilita con entrambi i dispositivi del tuo contatto.

**Il tuo contatto ha reinstallato Delta Chat utilizzando il vecchio login dell'account**
 
Se hanno [un file di backup](#backup),
dovrebbero rimuovere l'account dal nuovo dispositivo
e piuttosto importare il file di backup per ricreare il proprio account.
Non appena ti invieranno un messaggio, l'avviso scomparirà
e la crittografia garantita viene ristabilita per questo contatto.

Se non hanno un file di backup, è meglio eseguire una [scansione QR](#howtoe2ee)
con il tuo partner di chat per ristabilire la crittografia end-to-end garantita.

**Il tuo contatto ha inviato un'e-mail tramite un'interfaccia webmail o un'altra app di posta elettronica
e presto tornerà a utilizzare Delta Chat.**

Se sei sicuro che il contatto a volte utilizza la webmail,
o un'altra app di posta priva di crittografia end-to-end,
allora puoi accettare l'avvertimento.
Non appena il tuo contatto utilizzerà nuovamente Delta Chat,
la crittografia end-to-end garantita verrà ristabilita automaticamente.

**Il tuo contatto ha smesso completamente di utilizzare Delta Chat**

A volte rimanere in contatto è più importante della crittografia end-to-end.
["Transport Layer Encryption" (TLS)](#tls) può comunque proteggere in modo significativo
la riservatezza dei tuoi messaggi tra il tuo dispositivo e il server di posta elettronica.
Ma senza la crittografia end-to-end tu e il tuo contratto vi fidate del vostro server di posta elettronica
a non leggere o manipolare i tuoi messaggi e a non trasmetterli a terzi.

In ogni caso, non puoi fare molto altro che accettare l'avvertimento.
Rimuovi anche il contatto da qualsiasi gruppo attivo contrassegnato da un segno di spunta verde
che puoi trovare in "Chat condivise" nel profilo dei contatti.
Ciò evita che il tuo contatto riceva messaggi "illeggibili".

Se il contatto ha rimosso Delta Chat a causa di bug o di comportamenti indesiderati,
ti invitiamo a pubblicare post sul nostro [forum di supporto](https://support.delta.chat)
per aiutarci a identificare e affrontare i problemi comuni. Grazie!


### Gli allegati (immagini, file, audio, ecc.) sono crittografati end-to-end?

Sì.

Quando parliamo di "messaggio crittografato end-to-end"
intendiamo sempre che l'intero messaggio è crittografato,
compresi tutti gli allegati
e metadati degli allegati come i nomi dei file.


### OpenPGP è sicuro? {#openpgp-secure}

Sì, Delta Chat utilizza un sottoinsieme sicuro di OpenPGP
e visualizza solo un indicatore di sicurezza lucchetto su un messaggio
se l'intero messaggio è crittografato e firmato correttamente.
Ad esempio, le "Firme distaccate" non sono considerate sicure.

OpenPGP non è insicuro di per sé.
I problemi di sicurezza di OpenPGP più discussi pubblicamente
in realtà derivano da una cattiva usabilità o da cattive implementazioni di strumenti o app (o entrambi).
È particolarmente importante distinguere tra OpenPGP, lo standard di crittografia IETF,
e GnuPG (GPG), uno strumento da riga di comando che implementa OpenPGP.
Molte critiche pubbliche di OpenPGP in realtà discutono di GnuPG che Delta Chat non ha mai utilizzato.
Delta Chat utilizza piuttosto l'implementazione OpenPGP Rust [rPGP](https://github.com/rpgp/rpgp),
disponibile come [un pacchetto "pgp" indipendente](https://crates.io/crates/pgp),
e [controllato sulla sicurezza nel 2019](https://delta.chat/assets/blog/2019-first-security-review.pdf).

Puntiamo, insieme ad altri implementatori di OpenPGP,
per migliorare ulteriormente le caratteristiche di sicurezza implementando il
[nuovo aggiornamento crittografico IETF OpenPGP](https://datatracker.ietf.org/doc/draft-ietf-openpgp-crypto-refresh/) che per fortuna è stato adottato nell’estate 2023.


### Avete considerato l'utilizzo di alternative a OpenPGP per la crittografia end-to-end? {#openpgp-alternative}

Sì, stiamo seguendo iniziative come [MLS](https://en.wikipedia.org/wiki/Messaging_Layer_Security)
o [Saltpack](https://saltpack.org/)
ma adottarli significherebbe rompere l’interoperabilità della crittografia end-to-end
con tutte le altre app di posta elettronica che in genere supportano la crittografia OpenPGP.
Quindi non sarebbe una decisione facile da prendere
e devono esserci miglioramenti tangibili per gli utenti.

Delta Chat adotta un approccio olistico di "sicurezza utilizzabile".
e lavora anche con una vasta gamma di gruppi di attivisti
ricercatori rinomati come [TeamUSEC](https://teamusec.de)
per migliorare i risultati effettivi degli utenti contro le minacce alla sicurezza.
Il protocollo dei messaggi e lo standard per stabilire la crittografia end-to-end è
solo una parte dei "risultati utente",
vedi anche le nostre risposte a [device-seizure](#device-seizure)
e domande su [metadati-messaggio](#message-metadata).


### Delta Chat è vulnerabile agli EFAIL?

No, [Delta Chat non è mai stato vulnerabile all'EFAIL](https://delta.chat/en/2018-05-15-delta-chat-not-vulnerable-to-efail)
perché la sua implementazione OpenPGP [rPGP](https://github.com/rpgp/rpgp)
utilizza il codice di rilevamento delle modifiche durante la crittografia dei messaggi
e restituisce [un errore](https://docs.rs/pgp/latest/pgp/errors/enum.Error.html#variant.MdcError)
se il codice di rilevamento della modifica non è corretto.

Inoltre, Delta Chat non è mai stata vulnerabile all'attacco EFAIL "Direct Exfiltration"
perché decodifica solo i messaggi "multipart/encrypted".
che contengono esattamente una parte crittografata e firmata,
come definito dalla specifica Autocrypt Level 1.


### Un messaggio viene esposto in chiaro se la crittografia end-to-end non è disponibile? {#tls}

Anche se non è garantito che i tuoi messaggi siano crittografati end-to-end,
sono ancora protetti dai fornitori di Internet come le società di telefonia mobile o via cavo.
Tuttavia, i provider di posta elettronica tuoi e del destinatario
potranno leggere, analizzare o addirittura modificare i tuoi messaggi,
compresi eventuali allegati,
se non sono crittografati end-to-end.

Delta Chat per impostazione predefinita utilizza
[Crittografia TLS] rigorosa (https://en.wikipedia.org/wiki/Transport_Layer_Security)
che protegge le connessioni tra il tuo dispositivo e il tuo provider e-mail.
Tutta la gestione TLS di Delta Chat è stata sottoposta a [controlli di sicurezza](#security-audits) in modo indipendente.
Inoltre, la connessione tra il tuo provider e-mail e quello del destinatario
sarà in genere anche crittografato per il trasporto.
Se i server e-mail coinvolti supportano [MTA-STS](https://datatracker.ietf.org/doc/html/rfc8461)
verrà applicata la crittografia del trasporto tra i provider e-mail
in tal caso le comunicazioni Delta Chat non verranno mai esposte in chiaro su Internet
anche se il messaggio non sarà crittografato end-to-end.

Tieni presente che [mantenere la crittografia end-to-end garantita](#howtoe2ee) oltre alla crittografia TLS
fornisce una sicurezza pervasiva tra i tuoi dispositivi e quelli del destinatario.
Nemmeno il tuo provider e-mail o Internet sarà in grado di leggere o modificare i tuoi messaggi.


### In che modo Delta Chat protegge i metadati nei messaggi? {#message-metadata}

Delta Chat protegge la maggior parte dei metadati dei messaggi inserendo le seguenti informazioni
nella parte crittografata end-to-end dei messaggi:

- Linea oggetto
- Avatar e nome del gruppo
- Richieste MDN (conferma di lettura) ("Chat-Disposition-Notification-To")
- Temporizzatore dei messaggi che scompaiono ("Ephemeral-Timer")
- "Membro del gruppo chat rimosso", "Membro del gruppo chat aggiunto".
- Intestazione "Secure-Join" contenente comandi di join sicuri
- Notifica sull'attivazione dello streaming della posizione
- URL della stanza WebRTC

I server E-Mail non hanno accesso a questi metadati protetti
ma vedono la data del messaggio e la dimensione del messaggio,
e, cosa ancora più importante, gli indirizzi del mittente e del destinatario.
I server E-Mail necessitano di indirizzi di destinatari per instradare e
consegnare messaggi ai dispositivi del destinatario.


### Come proteggere i metadati e contatti quando un dispositivo viene sequestrato? {#device-seizure}

Entrambi per la protezione dai server e-mail che raccolgono metadati
nonché contro il pericolo di sequestro del dispositivo
consigliamo di utilizzare un'[istanza del server e-mail](https://delta.chat/serverguide) ottimizzata per Delta Chat
per creare account temporanei pseudonimi tramite scansioni di codici QR.
Tieni presente che le app Delta Chat su tutte le piattaforme supportano più account
in questo modo puoi utilizzare facilmente account "1 settimana" o "1 mese" specifici per azioni accanto al tuo account "principale".
con la consapevolezza che tutti i dati temporanei dell'account, insieme a tutti i metadati, verranno cancellati.
Inoltre, se un dispositivo viene sequestrato, i contatti utilizzano account di posta elettronica temporanei
non possono essere identificati facilmente, rispetto ai messaggeri che rivelano
numeri di telefono nei gruppi di chat che a loro volta sono spesso associati a identità legali.


### Come posso verificare le informazioni di crittografia?

È possibile verificare manualmente lo stato della crittografia end-to-end nella finestra di dialogo "Crittografia".
(profilo utente su Android/iOS o clic con il pulsante destro del mouse sull'elemento dell'elenco chat di un utente sul desktop).
Delta Chat mostra due impronte digitali.
Se sul tuo dispositivo e su quello del tuo contatto vengono visualizzate le stesse impronte digitali,
la connessione è sicura.


### Come posso verificare lo stato di crittografia dei messaggi?

Un piccolo **lucchetto** in un fumetto denota
che il messaggio è stato correttamente crittografato end-to-end dal mittente specificato.
Se **non è presente alcun lucchetto**, il messaggio non è stato crittografato correttamente end-to-end
molto probabilmente perché il mittente utilizza un'app o un'interfaccia webmail
senza supporto per la crittografia end-to-end.


### Perché vedo messaggi non crittografati?

Se un contatto utilizza un'app e-mail non Autocrypt,
tutti i messaggi che coinvolgono questo contatto (in un gruppo o in una chat 1:1)
non sarà crittografato end-to-end e quindi non mostrerà un "lucchetto" con i messaggi.
Tieni presente che anche se i tuoi contatti utilizzano Delta Chat sul proprio account,
potrebbero anche utilizzare un'app di posta elettronica non Autocrypt su quell'account
che quindi potrebbe causare messaggi non crittografati in modo intermittente.
La risposta non crittografata a messaggi non crittografati è richiesta da Autocrypt
per evitare messaggi illeggibili tra i tuoi contatti
e la loro app e-mail non Autocrypt.

### Come posso ottenere una chat crittografata end-to-end con un contatto Delta Chat che a volte utilizza la webmail o un'altra app e-mail non Autocrypt?

Se hai bisogno di una chat crittografata end-to-end sicura con un contatto
chi utilizza il proprio account sia con Delta Chat che con app non Autocrypt (ad esempio webmail),
è meglio configurare [la crittografia end-to-end garantita con loro](#howtoe2ee)
e quindi crea una chat di gruppo crittografata end-to-end garantita con voi due come membri.
In questa chat di gruppo tutti i messaggi verranno crittografati end-to-end
anche se la chat diretta tra voi due ha a
["... inviato un messaggio da un altro dispositivo"](#nocryptanymore) avviso.


### Come posso garantire la crittografia e l'eliminazione end-to-end dei messaggi?

Il modo migliore per garantire che ogni messaggio sia crittografato end-to-end,
e i metadati vengono eliminati il ​​più rapidamente possibile
è [utilizzare chat con crittografia end-to-end garantita](#howtoe2ee)
e l'attivazione dei [messaggi a scomparsa](#ephemeralmsgs).

Le chat crittografate end-to-end garantiscono la protezione dagli [attacchi MITM](https://en.wikipedia.org/wiki/Man-in-the-middle_attack)
e l'attivazione dei "messaggi che scompaiono" elimina i messaggi
sul server dopo un tempo configurato dall'utente.

Se non hai bisogno di una copia più longeva dei tuoi messaggi sul server,
puoi anche attivare ["elimina messaggi dal server"](#delold).


### Delta Chat supporta Perfect Forward Secrecy? {#pfs}

No, Delta Chat non supporta Perfect Forward Secrecy (PFS).
Ciò significa che se la tua chiave di decrittazione privata Delta Chat viene divulgata,
e qualcuno ha raccolto i tuoi precedenti messaggi in transito,
sarà in grado di decrittografarli e leggerli utilizzando la chiave di decrittazione trapelata.

Tieni presente, tuttavia, che se qualcuno ottiene le tue chiavi di decrittazione,
in genere saranno anche in grado di ricevere i tuoi messaggi,
indipendentemente dal fatto che Perfect Forward Secrecy sia attivo o meno.
La tipica situazione reale in caso di fuga di chiavi di decrittazione è il sequestro del dispositivo
di cui discutiamo nella nostra risposta [sui metadati e sul sequestro dei dispositivi](#device-seizure).

È possibile che Delta Chat si evolva per supportare Perfect Forward Secrecy,
perché OpenPGP è solo un contenitore per messaggi crittografati
ma la gestione delle chiavi di crittografia (e quindi la rotazione delle chiavi o "cricchetto")
potrebbero essere organizzati in modo flessibile.
Vedi [prototipo PFS di Seqouia](https://gitlab.com/sequoia-pgp/openpgp-dr)
per gli esperimenti esistenti nella comunità degli implementatori di OpenPGP.


### La crittografia end-to-end di Delta Chat è sicura quanto quella di Signal?

Dipende da cosa è importante per te.
Delta Chat [non supporta PFS](#pfs) come fa Signal
ma fornisce [chat crittografate end-to-end garantite](#e2eeguarantee)
che sono sicuri contro server compromessi o reti danneggiate.
Signal e la maggior parte degli altri servizi di messaggistica che supportano PFS non forniscono
uno schema pratico per proteggere i gruppi di chat dagli attacchi di rete
che sono probabilmente più preoccupanti
di un potenziale utente malintenzionato che si impadronisce del tuo telefono e della configurazione di crittografia privata
ma in qualche modo non i tuoi messaggi, ma ha un registro completo di tutti
messaggi crittografati precedenti.

In ogni caso, la crittografia end-to-end di Delta Chat utilizza un [sottoinsieme sicuro di OpenPGP](#openpgp-secure)
che è stato [controllato in modo indipendente sulla sicurezza](../assets/blog/2019-first-security-review.pdf).

### Posso riutilizzare la mia chiave privata esistente?

Sì.
The best way is to send an Autocrypt Setup Message from the other e-mail client.
Look for something like **Start Autocrypt Setup Transfer** in the settings of the other client and follow the instructions shown there.

In alternativa è possibile importare manualmente la chiave in "Impostazioni -> Avanzate -> Gestisci Chiavi -> Importa Chiavi Segrete".
Attenzione: assicurarsi che la chiave non sia protetta da password oppure rimuovere prima la password.

Se non hai una chiave o non sai nemmeno che ne avrai bisogno - non preoccuparti: Delta Chat genera le chiavi secondo necessità, non devi premere un pulsante per ottenerle.

### Non riesco a importare la mia chiave PGP esistente in Delta Chat.

Con molta probabilità, il problema sta nel fatto che la tua chiave è cifata e/o usa
una password. Queste chiavi non sono supportate da Delta Chat. Rimuovi la
cifratura e la password e prova ad importarla nuovamente.

Un altro errore comune è avere la fine del file sbagliata.
Utilizza il formato corazzato ASCII e l'estensione del file ".asc".

Delta Chat supporta i formati di chiave privata OpenPGP comuni, tuttavia,
è improbabile che le chiavi private di tutte le fonti siano completamente supportate. Questo
non è l'obiettivo principale di Delta Chat. In effetti, la maggior parte dei nuovi utenti
non avrà alcuna chiave prima di utilizzare Delta Chat.
Tuttavia, cerchiamo di supportare le chiavi private dal maggior numero possibile di fonti.

La rimozione della password dalla chiave privata dipenderà dal
software che usi per gestire le tue chiavi PGP. Con Enigmail puoi impostare la tua
password su un valore vuoto nella finestra Gestione chiavi. Con GnuPG puoi impostarla
[tramite la linea
di comando](https://github.com/deltachat/deltachat-android/issues/98#issuecomment-378383429).
Per altri programmi, dovresti essere in grado di trovare una soluzione online.

## Multi-client {#multiclient}

### Posso utilizzare Delta Chat su più dispositivi contemporaneamente?

Sì. Delta Chat 1.36 comes with a new, experimental function for using the same account on different devices:

- Assicurati che entrambi i dispositivi siano collegati alla stessa rete Wi-Fi o network

- Sul primo dispositivo, andare su **Impostazioni → Aggiungi Secondo Dispositivo**, sbloccare lo schermo se necessario
  e attendere un attimo fino a quando non viene visualizzato un codice QR

- Sul secondo dispositivo, [installare Delta Chat](https://get.delta.chat)

- Sul secondo dispositivo, avviare Delta Chat, selezionare **Aggiungi Come Secondo Dispositivo** e scansionare il codice QR del vecchio dispositivo.

- Il trasferimento dovrebbe iniziare dopo pochi secondi e durante il trasferimento entrambi i dispositivi mostreranno il **progresso**.
 Attendere il termine del trasferimento su entrambi i dispositivi.

A differenza di molti altri messengers, dopo un trasferimento riuscito,
entrambi i **dispositivi sono completamente indipendenti.**
Un dispositivo non è necessario perché l'altro funzioni.


### Risoluzione dei problemi

- Verificare che entrambi i dispositivi siano nella **stessa rete o Wi-Fi**.

- Il sistema potrebbe avere un "personal firewall",
  che è noto per causare problemi (soprattutto su Windows).
  **Disattivare il firewall personale** per Delta Chat su entrambe le estremità e riprovare.

- Assicurarsi che sul dispositivo di destinazione ci sia **disponibilità di memoria sufficiente**.

- Se il trasferimento è iniziato, assicurarsi che i dispositivi **rimangano attivi** e non si addormentino.
  Non uscire da Delta Chat.
  (cerchiamo di far funzionare l'applicazione in background, ma [i sistemi tendono a uccidere le applicazioni](https://dontkillmyapp.com), purtroppo).

- Delta Chat è **già connesso** sul dispositivo di destinazione?
  È possibile utilizzare più account per dispositivo, basta [aggiungere un altro account](#multiple-accounts)

- Se si riscontrano ancora problemi o se **non si riesce a scansionare un codice QR**
  provate il **trasferimento manuale** descritto di seguito


### Trasferimento manuale {#backup}

Questo metodo è consigliato solo se "Aggiungi Secondo Dispositivo" come descritto sopra non funziona.

- Sul vecchio dispositivo, vai su "Impostazioni -> Chat e Media -> Backup Chat su Memoria Esterna". Inserisci il tuo
PIN, sequenza o password di sblocco dello schermo. Quindi puoi fare clic su "Avvia
Backup". Questo salva il file di backup sul tuo dispositivo. Ora devi trasferirlo
in qualche modo all'altro dispositivo.
- Sul nuovo dispositivo, nella schermata di accesso, invece di accedere alla tua email
account, seleziona "Importa backup". Dopo l'importazione, le tue conversazioni, la crittografia
i tasti e i supporti devono essere copiati sul nuovo dispositivo.
- **Se usi iOS:** e incontri difficoltà, forse
[questa guida](https://support.delta.chat/t/import-backup-to-ios/1628)
Aiutarti.
- Ora sei sincronizzato e puoi utilizzare entrambi i dispositivi per inviare e ricevere
messaggi crittografati end-to-end con i tuoi partner di comunicazione.

### Sono previsti piani per l'introduzione di un client Web Delta Chat?

- Non ci sono piani immediati ma alcune riflessioni preliminari.
- Ci sono 2-3 strade per introdurre un client Web Delta Chat, ma tutte sono
lavoro significativo. Per ora, ci concentriamo sull'ottenere versioni stabili in tutti
gli app store (repository Google Play/iOS/Windows/macOS/Linux) come app native.
- Se hai bisogno di un Client Web, perché non sei autorizzato a installare software sul
computer con cui lavori, puoi utilizzare il client Desktop Windows Portatile,
o l'AppImage per Linux. Le trovi su
[get.delta.chat](https://get.delta.chat).


### A cosa serve l'impostazione "Invia copia a se stessi"?

L'invio di una copia dei tuoi messaggi a te stesso ti assicura di ricevere i tuoi
messaggi su tutti i dispositivi. Se disponi di più dispositivi e non lo attivi,
vedrai solo i messaggi di altre persone e i messaggi che invii dal
dispositivo attuale.

La copia viene inviata alla Posta in arrivo, quindi spostata nella cartella DeltaChat; non è
messa nella cartella "Inviata". Delta Chat *non* carica mai nulla su Posta
Inviata perché questo significherebbe caricare un messaggio due volte (una volta tramite SMTP,
e una volta tramite IMAP nella cartella Posta Inviata).

L'impostazione predefinita per la copia su se stesso è "no".

### Perché posso scegliere di guardare la cartella "Inviata"?

L'unico motivo per cui si vuole guardare la cartella Inviata è se ne stai usando un'altro
programma di posta (come Thunderbird) accanto alla tua app Delta Chat e desideri il tuo MUA
per partecipare a conversazioni in chat.

Tuttavia, consigliamo di utilizzare il client desktop Delta Chat; puoi scaricarlo
su [get.delta.chat](https://get.delta.chat). L'opzione per guardare la cartella
"Inviata" potrebbe scomparire in futuro. È stato introdotto in un momento in cui non c'era
nessun client Delta Chat Desktop disponibile su tutte le piattaforme.

### Perché posso scegliere di non guardare la cartella DeltaChat?

Alcune persone usano Delta Chat come un normale client di posta elettronica e desiderano utilizzare la cartella Posta in arrivo
per la loro posta, invece della cartella DeltaChat. Se disabiliti "Controlla
cartella DeltaChat", dovresti anche disabilitare "sposta messaggi chat in DeltaChat".
In caso contrario, l'eliminazione dei messaggi o configurazioni multi-dispositivo potrebbero non funzionare correttamente.


## apps webxdc {#webxdc}

In Delta Chat, puoi condividere [app webxdc](https://webxdc.org), allegati file con estensione `.xdc`.
Possono fare cose molto diverse e rendere Delta Chat davvero
un messenger estensibile.


### Quanto sono private le apps webxdc?

- Le apps webxdc non possono inviare dati a Internet o scaricare nulla.
- Un'app webxdc può scambiare dati solo all'interno di una chat Delta Chat, con la sua
copia sui dispositivi dei tuoi partner di chat. A parte questo, è completamente
isolato da Internet.
- La privacy offerta da un'app webxdc è la privacy della tua chat, purché tu
ti fidi delle persone con cui chatti e quindi puoi fidarti anche dell'app webxdc.
- Ciò significa anche: può essere un rischio per la privacy aprire le app webxdc nelle chat dove
non ti fidi dei membri, come sai dagli allegati di posta elettronica, dove
apri solo gli allegati provenienti dai mittenti di cui ti fidi e non da spammer.


### Dove posso trovare le apps webxdc?

- In generale, chiunque può condividere apps webxdc con ciascun
  altro senza restrizioni.
- Puoi [inviare 'ciao' a xstore@testrun.org](https://delta.chat/en/2023-08-11-xstore)
  per vedere un app store webxdc sperimentale.
  Tutte le app sono open source e gratuite.
- Molte persone scrivono le proprie app webxdc e le pubblicano su [Delta Chat
  forum](https://support.delta.chat/c/webxdc/20).


### Come posso creare le mie apps webxdc?

- Le app webxdc sono solo file zip contenenti codice html, css e javascript.
- Puoi estendere l'[app di esempio Hello World](https://github.com/webxdc/hello)
  per iniziare.
- Tutto il resto che devi sapere è scritto nella
  [documentazione](https://docs.webxdc.org/).
- Se hai domande, puoi chiederle ad altri con esperienza nel [Delta Chat
  Forum](https://support.delta.chat/c/webxdc/20).


## Caratteristiche Sperimentali

Siamo molto grati per il feedback su queste funzionalità: vuoi condividere
le tue idee? Partecipa al [Forum](https://support.delta.chat) per contribuire.
Puoi accedere comodamente tramite Delta Chat e una scansione del codice QR,
un altro esperimento piuttosto stabile che eseguiamo a parte (sic!).

### Come posso utilizzare le chiamate audio/video con Delta Chat?

- Per attivare le chiamate audio/video vai alla sezione "funzionalità sperimentali" in
le impostazioni avanzate e scegli una "Istanza di chat video".
- Quando inviti altri a una chat video, questa viene aperta nel tuo browser/app all'indirizzo
una volta. Gli altri ricevono un'e-mail con un collegamento alla chat video.
In questo modo è compatibile anche se i tuoi partner di chat non utilizzano Delta Chat.
- Tieni presente che non c'è suoneria dall'altra parte e dai tuoi partner di chat
non verrà interrotto da un invito alla chat video.
- Puoi utilizzare qualsiasi servizio di chat video che consenta l'accesso tramite collegamento. Basta aggiungere il
collegamento nelle impostazioni.
- Ad esempio, per utilizzare l'istanza Jitsi Meet di punta, potresti inserire
`https://meet.jit.si/$ROOM`. La variabile "$ROOM" sarà un valore casuale;
in questo modo, avrai una nuova stanza jitsi casuale ogni volta che chiami qualcuno.


### Cosa sono le Liste di Trasmissione e come si possono usare?

- Con una Lista di Trasmissione è possibile inviare un messaggio a molti destinatari contemporaneamente; quando questi vi rispondono, ricevete la risposta nella vostra chat diretta 1:1 con loro.
I destinatari non possono vedersi a vicenda.
- Tecnicamente, si tratta di un messaggio di posta elettronica con molti destinatari in BCC.
- È possibile attivare questa funzione nella sezione "Funzionalità Sperimentali" delle impostazioni avanzate.
Quindi è possibile creare una Lista di Trasmissione dalla finestra di dialogo "Nuova chat".
- Nel caso in cui si utilizzi più di un dispositivo, le Liste di Trasmissione non sono attualmente sincronizzate tra loro.
- I messaggi inviati alle Liste di Trasmissione non sono crittografate. La crittografia romperebbe l'anonimato, perché
tutti i destinatari saprebbero chi altro ha ricevuto il messaggio.
(l'invio di singoli messaggi di posta elettronica a tutti sarebbe peggiore per il limite di velocità e il
consumo di rete).


### Come posso condividere la mia posizione con i miei partner di chat?

- Puoi attivare la trasmissione della posizione nella sezione "Funzionalità Sperimentali" nelle
impostazioni avanzate.
- Ora, se vuoi condividere la tua posizione in una chat, vai su "allega" e seleziona
"Posizione". Ora puoi impostare un intervallo di tempo in cui verrà trasmessa la tua posizione
ai tuoi partner di chat, tra 5 minuti e 6 ore.
- Quando la tua posizione cambia, gli altri nella chat possono visualizzarla su una mappa nella
chat.
- Per vedere la mappa e visualizzare le posizioni degli altri, devi attivare la funzione
nelle impostazioni avanzate.
- Questa funzione non condividerà la tua posizione con nessuno tranne che con i tuoi partner di chat.
*Ma:* per mostrare la mappa, dobbiamo scaricare i riquadri della mappa da
mapbox.com, quindi se *visualizzi* la mappa, a mapbox.com viene richiesta la mappa di un
area specifica. Se questo è un rischio per la privacy per te, questa funzione potrebbe non esserlo più.
Stiamo lavorando per trovare un'alternativa decentralizzata per Mapbox.
- Su desktop, il sistema operativo in genere non è in grado di determinare la tua posizione. Invece puoi
fare clic con il tasto destro sulla mappa e descrivere una posizione, che viene inviata alla chat come
un messaggio, ma appare anche sulla mappa.


### Cosa protegge effettivamente la crittografia sperimentale del database?

- In questo momento, la crittografia del database è ancora molto sperimentale.  Non affidarti su di essa
 per sicurezza, dovresti inoltre utilizzare la crittografia del tuo sistema
 operativo, se ne prevede una.
 - La crittografia del database non crittografa ancora i BLOB, solo le righe e le
colonne del database. Questo più o meno significa che i tuoi messaggi sono al sicuro,
ma non i tuoi allegati.
- Per iOS e Android, le chiavi di crittografia sono memorizzate nel portachiavi di sistema.
Ciò significa che la crittografia è sicura quanto il sistema operativo
in esecuzione.
- Il client desktop Delta Chat non offre ancora la crittografia del database, come qui
non c'è un modo standard per memorizzare le chiavi di crittografia sulle diverse piattaforme
supportate.


### Perché posso scegliere di guardare solo la cartella DeltaChat?

Questa è un'impostazione sperimentale per alcune persone che stanno sperimentando
regole lato server. Non tutti i provider supportano questo, ma con alcuni puoi spostare
tutti i messaggi con un'intestazione "Chat-Version" nella cartella DeltaChat. Normalmente, questo
verrebbe eseguito dall'app Delta Chat.

Abilitare "Recupera dalla Cartella DeltaChat" ha senso se hai **entrambi**:

- abilitato una regola lato server per spostare tutti i messaggi con l'intestazione Chat-Version nella cartella DeltaChat, e
- aver impostato l'impostazione "Mostra email classiche" su "no, solo chat".

In questo caso, Delta Chat non ha bisogno di guardare la Posta in arrivo ed è sufficiente guardare solo la cartella DeltaChat.


### Come posso cambiare il mio account con un indirizzo e-mail diverso?

1. Cambia il tuo indirizzo in “Impostazioni - Password e Account” e
inserisci la password del tuo nuovo account (e se necessario, le impostazioni del server).
Riceverai un avviso informativo sul fatto che ti trasferirai ad un nuovo indirizzo.
Un ulteriore avviso verrà visualizzato anche nella chat "Messaggi del dispositivo".

2. Se possibile, lascia che il tuo vecchio provider e-mail inoltri tutti i messaggi al tuo nuovo indirizzo.

3. Dì ai tuoi contatti che hai cambiato il tuo indirizzo.
Scrivere a chat e gruppi crittografati end-to-end garantiti,
farà loro notare automaticamente la tua azione
e continueranno a chattare con te utilizzando il tuo nuovo indirizzo.

Tieni presente che Delta Chat non recupererà più i messaggi dal tuo vecchio provider e-mail.
Se non hai configurato il tuo provider e-mail per inoltrare i messaggi (passaggio 2.)
solo i contatti a cui hai inviato un messaggio in una chat crittografata end-to-end garantita
invieranno messaggi al tuo nuovo indirizzo.

Per saperne di più su questi dettagli, [leggi il nostro post sul blog
it](https://delta.chat/en/2022-09-14-aeap).


## Varie

### Delta Chat funziona con il _mio_ fornitore e-mail?

- Con buona possibilità: Sì :)
Tuttavia, alcuni provider necessitano di opzioni speciali per funzionare correttamente,
vedi [Panoramica fornitore](https://providers.delta.chat)


### Voglio gestire il mio server di posta elettronica per Delta Chat. Che cosa mi consigliate?

- La maggior parte dei server di posta funzionerà bene. Ma quello che raccomandiamo personalmente è una
combinazione di mailcow e mailadm, come descritto [in questo
blogpost](https://delta.chat/en/2023-01-27-upcoming-mail-server-workshops).
- È possibile trovare una [guida all'installazione sul nostro sito Web](serverguide).


### Se Delta Chat utilizza l' E-Mail, è davvero una Messaggistica _Istantanea_?

- L'invio e la ricezione dei messaggi richiedono generalmente alcuni secondi. Qualche volta
ci sono casi in cui ci vuole più tempo, ma questo è probabilmente vero anche per
qualsiasi altro messenger.
- La chat istantanea funziona velocemente se entrambe le parti utilizzano attivamente l'app. È
a volte più lento se l'app è in esecuzione in background.
- La ricezione dei messaggi può richiedere minuti perché spesso sia Android che iOS
interrompono l'esecuzione di Delta Chat in background e riattivandola solo
occasionalmente. Questo ritardo artificiale è solitamente peggiore su iOS che su Android.
- Tuttavia, Android e iOS uccidono le app in esecuzione in background ed è un
problema per molte app legittime. Per ulteriori informazioni, vedi
[dontkillmyapp.com](https://dontkillmyapp.com/).


### Delta Chat è compatibile con Protonmail / Tutanota / Criptext?

- Sì e no.
- No, non puoi utilizzare il tuo account Protonmail, Tutanota o Criptext con Delta
  Chat; non offrono la ricezione di posta tramite IMAP.
- In ogni caso puoi utilizzare Delta Chat per inviare messaggi alle persone che lo utilizzano
  Protonmail, Tutanota o Criptext. Tali messaggi non saranno end-to-end
  crittografato, però. La crittografia end-to-end offerta da questi provider non è
  compatibile con [Autocrypt](https://autocrypt.org/), gli standard Delta Chat
che usa.
- Delta Chat può crittografare end-to-end tramite qualsiasi provider e-mail con qualsiasi
[App di posta elettronica abilitata per Autocrypt](https://autocrypt.org/dev-status.html).


### Sono interessato ai dettagli tecnici. Mi puoi dire di più?

- Vedi [Standard usati in Delta Chat]({% include standards-url %}).

### Delta Chat è stata verificata in modo indipendente per le vulnerabilità di sicurezza? {#security-audits}

Il progetto Delta Chat è stato sottoposto a quattro verifiche di sicurezza indipendenti negli ultimi anni:

- Nel 2019, [Include Security](https://includesecurity.com) ha analizzato le librerie
[PGP](https://github.com/rpgp/rpgp) e
[RSA](https://github.com/RustCrypto/RSA) di Delta Chat.
Non ha riscontrato criticità,
ma due problemi di elevata gravità che abbiamo successivamente risolto.
Ne sono emersi anche uno di media gravità e alcuni problemi meno gravi,
ma non c'era modo di sfruttare queste vulnerabilità nell'implementazione di Delta Chat.
Alcuni di essi sono stati comunque corretti dopo la conclusione dell'audit.
Puoi leggere il [rapporto completo qui](../assets/blog/2019-first-security-review.pdf).

- Nel 2020, [Include Security](https://includesecurity.com) ha analizzato il Delta
Chat's Rust [core](https://github.com/deltachat/deltachat-core-rust/),
[IMAP](https://github.com/async-email/async-imap),
[SMTP](https://github.com/async-email/async-smtp) e
[TLS](https://github.com/async-email/async-native-tls) librerie.
Non ha rilevato problemi critici o di elevata gravità.
Il rapporto ha sollevato alcuni punti deboli di media gravità:
da soli non rappresentano una minaccia per gli utenti di Delta Chat
perché dipendono dall'ambiente in cui viene utilizzato Delta Chat.
Per motivi di usabilità e compatibilità,
non possiamo mitigarli tutti
e ha deciso di fornire consigli sulla sicurezza agli utenti minacciati.
Puoi leggere il [rapporto completo qui](../assets/blog/2020-second-security-review.pdf).

- A partire dal 2023, [Cure53](https://cure53.de) ha analizzato sia la crittografia del trasporto delle
Connessioni di rete di Delta Chat e una configurazione del server di posta riproducibile come
[consigliato su questo sito](serverguide).
Puoi leggere ulteriori informazioni sull'audit [sul nostro blog](https://delta.chat/en/2023-03-27-third-independent-security-audit)
o leggere il [rapporto completo qui](../assets/blog/MER-01-report.pdf).

- A partire dal 2023, abbiamo risolto i problemi di sicurezza e privacy con il servizio "web
app condivise in una chat", relativa ai guasti del sandboxing
soprattutto con Chromium. Successivamente abbiamo ottenuto una sicurezza indipendente
audit da Cure53 e tutti i problemi rilevati sono stati risolti nella serie di app 1.36 rilasciata nell'aprile 2023.
Vedi [qui per la storia completa sulla sicurezza end-to-end nel web](https://delta.chat/en/2023-05-22-webxdc-security).


### Come viene finanziato lo sviluppo di Delta Chat?

Delta Chat non riceve alcun capitale di rischio e
non è indebitato e non è sotto pressione per produrre enormi profitti, o per farlo
vendere utenti e i loro amici e familiari agli inserzionisti (o peggio).
Utilizziamo piuttosto fonti di finanziamento pubblico, così lontane dalle origini dell'UE e degli Stati Uniti, per aiutare
i nostri sforzi nell'istigare un ecosistema di messaggistica di chat decentralizzato e diversificato
basato sugli sviluppi della comunità Free e Open-Source.

Concretamente, gli sviluppi di Delta Chat finora sono stati finanziati da queste fonti:

- Il progetto UE [NEXTLEAP](https://nextleap.eu) ha finanziato la ricerca
  e implementazione di gruppi verificati e impostazione di protocolli di contatto
  nel 2017 e nel 2018 e ha anche contribuito a integrare la crittografia end-to-end
  tramite [Autocrypt](https://autocrypt.org).

- L'[Open Technology Fund](https://opentechfund.org) ci ha dato una
prima sovvenzione 2018/2019 (~$200K) durante la quale abbiamo notevolmente migliorato l'app Android
e ha rilasciato una prima versione beta dell'app desktop, e che inoltre
ancorato i nostri sviluppi delle funzionalità nella ricerca sulla UX nei contesti dei diritti umani,
vedete il nostro [Rapporto Needfinding e UX] conclusivo (https://delta.chat/en/2019-07-19-uxreport).
La seconda sovvenzione 2019/2020 (~$300K) ci ha aiutato a farlo
rilasciare nelle versioni Delta/iOS, per convertire la nostra libreria principale in Rust, e
per fornire nuove funzionalità per tutte le piattaforme.

- La [fondazione NLnet](https://nlnet.nl/) ha concesso nel 2019/2020 46.000 EUR per
  completando i collegamenti Rust/Python e avviando un ecosistema Chat-bot.

- Nel 2021 abbiamo ricevuto ulteriori finanziamenti dell'UE per due Next-Generation-Internet
proposte, in particolare per [EPPD - directory di portabilità del provider di posta elettronica](https://dapsi.ngi.eu/hall-of-fame/eppd/) (~97K EUR) e [AEAP - portabilità dell'indirizzo e-mail](https://nlnet.nl/project/EmailPorting/) (~90K EUR) che ha portato a un migliore supporto multi-account, contatti QR-code migliorati e configurazioni di gruppo e molti miglioramenti della rete su tutte le piattaforme.

- Dalla fine del 2021 fino a Marzo 2023 abbiamo ricevuto finanziamenti *Internet Freedom* (500.000 USD) dall'Ufficio per la democrazia, i diritti umani e il lavoro degli Stati Uniti (DRL). Questo finanziamento ha supportato i nostri obiettivi a lungo termine per rendere Delta Chat più utilizzabile e compatibile con un'ampia gamma di server di posta elettronica in tutto il mondo e più resiliente e sicuro in luoghi spesso colpiti dalla censura e dalla chiusura di Internet.

- A partire dal 2023 siamo stati accettati nel programma Next Generation Internet (NGI) Affidamento per le nostre proposte di "App private decentralizzate". L'importo esatto è da definire (circa 100.000 euro). Questo finanziamento supporta ulteriori sviluppi di [webxdc "app condivise in una chat"](https://webxdc.org). 

- A volte riceviamo donazioni una tantum da privati.
Ad esempio, nel 2021 un generoso individuo ci ha trasferito in banca 4K EUR
con l'oggetto "mantenete il buoni sviluppi!". 💜
Usiamo questi soldi per finanziare incontri di sviluppo o per sostenere spese ad hoc
che non possono essere facilmente previsti o rimborsati da finanziamenti pubblici.
Ricevere più donazioni ci aiuta anche a diventare più indipendenti e vitali a lungo termine
come comunità di contributori.

[Dona denaro](donate){: .cta-button}

- Ultimo ma non meno importante, hanno contribuito diversi esperti e appassionati pro-bono
e contribuito allo sviluppo di Delta Chat senza ricevere denaro, o solo
piccole quantità. Senza di loro, Delta Chat non sarebbe dove è oggi, nemmeno
vicino.

Il finanziamento monetario di cui sopra è per lo più organizzato da merlinux GmbH in
Friburgo (Germania) ed è distribuito a più di una dozzina di contributori in tutto il mondo.

Consulta [Canali contribuzione di Delta Chat](contribute)
sia per le possibilità monetarie che contributive.
