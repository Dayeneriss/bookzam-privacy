# Informativa sulla Privacy — BookZam

Ultimo aggiornamento: 3 aprile 2026

BookZam rispetta la tua privacy. Questa informativa spiega quali dati vengono raccolti, come vengono utilizzati e quali sono i tuoi diritti.

## 1. Dati Raccolti

### 1.1 Dati dell'account

- Indirizzo email e nome (durante la creazione dell'account)
- Identificatore di accesso tramite Google Sign-In o Sign in with Apple
- Foto del profilo (se fornita tramite Google o Apple)

### 1.2 Dati della biblioteca

- Cronologia dei libri scansionati, cercati e aggiunti
- Coordinate geografiche associate a ogni scansione (latitudine, longitudine, citta, paese), se hai autorizzato l'accesso alla posizione. Questi dati vengono memorizzati nel tuo profilo sui nostri server (Cloud Firestore) e servono ad alimentare la tua mappa delle scoperte.
- Preferiti, note personali, stati di lettura
- Progressi di lettura e obiettivi
- Sfide di lettura e badge ottenuti

### 1.3 Dati di ascolto (audiolibri)

- Sessioni di ascolto (inizio, fine, durata, velocita di riproduzione)
- Progressi per capitolo e per audiolibro
- Feedback post-ascolto (abbandono o completamento)

### 1.4 Dati sociali

- Profilo pubblico: nome utente, livello di lettura, generi preferiti, numero di libri, badge
- Attivita condivisa: libri aggiunti, sfide completate, badge ottenuti
- Messaggi nei club di lettura

### 1.5 Dati relativi all'IA

Quando utilizzi le funzionalita di intelligenza artificiale (ricerca per umore, ricerca per citazione, DNA Letterario, chat Libro Dimenticato, quiz, raccomandazioni), i testi che inserisci insieme al contesto della tua biblioteca vengono inviati ai server di Google (Gemini) per l'elaborazione. Nessuna immagine di copertina viene inviata per il riconoscimento del testo (OCR), che viene effettuato interamente sul tuo dispositivo.

### 1.6 Dati tecnici

- Modello del dispositivo, versione del sistema operativo, versione dell'applicazione
- Log di crash anonimi (tracce di errore, senza dati personali)
- Eventi di utilizzo anonimizzati (schermate visitate, funzionalita utilizzate)
- Proprieta utente anonimizzate trasmesse a Firebase Analytics: piattaforma (Android/iOS/Web), fonte di installazione (Google Play, App Store...), tipo di account (anonimo, gratuito, premium), anzianita di installazione, numero di sessioni, numero di libri, funzionalita scoperte, livello di coinvolgimento
- Contatori di utilizzo locali (numero di scansioni, ricerche IA, quiz, ecc.) memorizzati sul dispositivo e sincronizzati periodicamente
- Token di notifica push (FCM token)

### 1.7 Dati di localizzazione

- Posizione geografica (solo se lo autorizzi), utilizzata per:
  - **Mappa delle scoperte**: le coordinate GPS (latitudine, longitudine) e la localizzazione inversa (citta, paese) vengono salvate con ogni scansione di libro nel tuo profilo Firestore. Puoi eliminare questa cronologia in Impostazioni > Cancella cronologia.
  - **Link di acquisto**: il tuo paese viene rilevato per reindirizzarti al negozio Amazon corrispondente. Il codice paese viene memorizzato nella cache locale del dispositivo (SharedPreferences), ma non viene inviato ai nostri server.
- Puoi revocare l'accesso alla posizione in qualsiasi momento nelle impostazioni del telefono. L'applicazione continuera a funzionare normalmente senza questo permesso.

### 1.8 Dati multimediali

- Accesso alla fotocamera (per scansionare copertine di libri e scaffali)
- Accesso alle foto (per selezionare immagini di libri)
- Accesso al microfono (per la ricerca vocale)
- Questi dati vengono elaborati localmente o trasmessi temporaneamente per il riconoscimento. Non vengono memorizzati sui nostri server.

## 2. Utilizzo dei Dati

- Fornire le funzionalita principali dell'applicazione (biblioteca, ricerca, raccomandazioni, audiolibri, quiz, club di lettura)
- Personalizzare la tua esperienza (raccomandazioni IA, DNA Letterario, profilo di lettura)
- Gestire il tuo abbonamento Premium
- Mostrare pubblicita rilevanti (solo per gli utenti gratuiti)
- Migliorare l'applicazione (statistiche di utilizzo anonimizzate, correzione di bug)
- Inviare notifiche di promemoria e progresso (disattivabili nelle impostazioni)
- Offrire link di acquisto su Amazon tramite link di affiliazione (programma Amazon Associates, tag `bookzam0cf-21`). BookZam riceve una commissione sugli acquisti effettuati tramite questi link. Nessun dato personale viene trasmesso ad Amazon da BookZam; solo la tua posizione (paese) viene utilizzata localmente per indirizzarti al negozio Amazon corretto.
- **Nessun dato viene venduto a terze parti**

## 3. Servizi di Terze Parti

BookZam utilizza i seguenti servizi di terze parti:

| Servizio | Finalita | Dati trasmessi |
|----------|----------|----------------|
| **Firebase Authentication** | Accesso sicuro | Email, nome, ID di accesso |
| **Cloud Firestore** | Archiviazione dati | Biblioteca, profilo, progressi |
| **Firebase Analytics** | Statistiche di utilizzo | Eventi anonimizzati, proprieta utente |
| **Firebase Crashlytics** | Rapporti di crash | Tracce di errore, info dispositivo |
| **Firebase Cloud Messaging** | Notifiche push | Token FCM |
| **Firebase Remote Config** | Configurazione dinamica | Nessun dato personale |
| **Firebase App Check** | Protezione anti-frode | Attestazione del dispositivo |
| **Google Generative AI (Gemini)** | Funzionalita IA | Testi di ricerca, contesto biblioteca |
| **RevenueCat** | Gestione abbonamenti | ID utente, stato abbonamento |
| **Google AdMob** | Pubblicita | Identificatore pubblicitario (GAID/IDFA) |
| **Google Books API** | Ricerca libri | Termini di ricerca (titolo, autore, ISBN) |
| **Open Library** | Ricerca libri | Termini di ricerca |
| **Library of Congress** | Ricerca libri (fallback) | Termini di ricerca |
| **LibriVox** | Audiolibri gratuiti | Titolo, autore |
| **Google ML Kit** | OCR (sul dispositivo) | Nessuno — elaborazione locale unicamente |

In caso di attivazione di test comparativi (shadow testing), le tue richieste IA possono essere elaborate anche da Anthropic (Claude) in parallelo con Gemini.

## 4. Archiviazione e Sicurezza

- I dati sono archiviati su **Google Firebase** (infrastruttura sicura, crittografia in transito e a riposo)
- I dati locali (cache, preferenze) sono archiviati sul tuo dispositivo tramite SharedPreferences e sqflite (non crittografati)
- Le immagini catturate dalla fotocamera sono archiviate temporaneamente sul tuo dispositivo e non vengono inviate ai nostri server

## 5. Pubblicita

- Gli utenti **gratuiti** vedono banner pubblicitari forniti da Google AdMob
- Gli utenti possono guardare **annunci premiati** (rewarded ads) per ottenere ricerche IA aggiuntive
- Gli utenti **Premium** non vedono alcuna pubblicita
- Google AdMob puo raccogliere identificatori pubblicitari (GAID su Android, IDFA su iOS) per personalizzare gli annunci
- Su iOS, ti verra presentata una richiesta di consenso (App Tracking Transparency) prima di qualsiasi raccolta di identificatore pubblicitario

## 6. Notifiche

- BookZam puo inviare notifiche push per promemoria di lettura, serie, sfide, raccomandazioni e aggiornamenti
- Puoi disattivare ogni categoria di notifica individualmente nelle impostazioni dell'applicazione
- Puoi annullare completamente l'iscrizione alle notifiche in qualsiasi momento

## 7. Profilo Pubblico e Dati Sociali

- Alcune informazioni del tuo profilo sono visibili agli altri utenti: nome utente, livello di lettura, generi preferiti, numero di libri, badge
- Il feed di attivita (libri aggiunti, sfide completate, badge) e visibile a tutti gli utenti connessi
- I messaggi dei club di lettura sono visibili ai membri del club
- Puoi controllare la visibilita del tuo profilo nelle impostazioni

## 8. Diritti dell'Utente

In conformita con il GDPR e le leggi applicabili, puoi:

- **Accedere** ai tuoi dati personali
- **Rettificare** le tue informazioni
- **Cancellare** il tuo account e tutti i tuoi dati — disponibile direttamente nell'applicazione (Impostazioni > Account > Elimina il mio account)
- **Esportare** i tuoi dati — disponibile direttamente nell'applicazione (Impostazioni > Account > Esporta i miei dati) in formato JSON
- **Revocare il tuo consenso** per notifiche e localizzazione tramite le impostazioni dell'applicazione

Per esercitare questi diritti, puoi utilizzare le funzionalita integrate nell'applicazione o contattarci a **contact@bookzam.io**

## 9. Conservazione dei Dati

- I dati del tuo account vengono conservati finche il tuo account e attivo
- In caso di cancellazione dell'account, i tuoi dati vengono eliminati entro 30 giorni
- I log di crash vengono conservati per 90 giorni
- Gli eventi di analytics vengono conservati secondo la politica di conservazione di Firebase (14 mesi per impostazione predefinita)

## 10. Minori

BookZam non e destinato ai minori di 13 anni. Non raccogliamo consapevolmente dati personali di minori. Se sei un genitore e ritieni che tuo figlio ci abbia fornito dei dati, contattaci a contact@bookzam.io.

## 11. Modifiche

BookZam puo aggiornare questa informativa. In caso di modifiche importanti, ti informeremo tramite l'applicazione o via email. La data dell'ultimo aggiornamento e indicata in cima a questo documento.

## 12. Contatto

Per qualsiasi domanda o richiesta riguardante i tuoi dati:

- Email: **contact@bookzam.io**
- Puoi anche utilizzare la funzione di feedback nell'applicazione (Impostazioni > Feedback)
