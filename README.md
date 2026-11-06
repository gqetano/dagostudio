# DAGOSTUDIO — GitHub Pages

Pacchetto **completo e pronto alla pubblicazione**, con risorse locali separate.

## Contenuto

- `index.html` — sito e animazioni (il font Ronzino Medium è incorporato direttamente nel file)
- `images/` — 11 fotografie della Home, ritratto About e immagini di riserva degli hover
- `assets/logo-originale.svg` — logo vettoriale originale
- `.nojekyll` — configurazione GitHub Pages

## Pubblicazione

1. Apri lo ZIP ed estrai i file.
2. Carica **tutto il contenuto estratto** nella directory principale del repository GitHub (non la cartella contenitore, non soltanto `index.html`).
3. In GitHub apri **Settings → Pages → Build and deployment**, imposta **Deploy from a branch**, `main` e `/ (root)`.
4. Attendi che GitHub abbia concluso la pubblicazione. Apri l'indirizzo mostrato in Pages e ricarica la pagina dopo l'aggiornamento.

**Non rinominare** le cartelle `images` e `assets`. I percorsi nell'HTML sono relativi, adatti sia a un sito GitHub Pages alla radice sia a un sito sotto il nome del repository.

## Pannello Contatti

Il cerchio apre il pannello Contatti, speculare all'About: su desktop entra da destra e il cerchio, ruotando e aprendosi, segue il suo bordo; su mobile copre tutto lo schermo e il cerchio aperto va nell'angolo in basso a sinistra. Un nuovo clic lo fa ruotare indietro e richiudere. Si apre un solo pannello alla volta.

### Attivare l'invio dei messaggi

GitHub Pages non può inviare email da solo: serve un servizio esterno gratuito. Finché non è configurato, il modulo mostra "Il modulo è in fase di attivazione".

**Web3Forms (consigliato, gratuito):**
1. Vai su web3forms.com, inserisci l'email che deve ricevere i messaggi e ricevi la *Access Key*.
2. In `index.html` cerca `CONTACT_CONFIG` e compila:
   - `endpoint: 'https://api.web3forms.com/submit',`
   - `accessKey: 'LA-TUA-ACCESS-KEY',`

**In alternativa Formspree:** crea un form su formspree.io e incolla l'indirizzo in `endpoint` (es. `'https://formspree.io/f/abcdwxyz'`), lasciando `accessKey` vuoto.

**Senza servizio:** compilando solo `fallbackEmail` il pulsante apre il programma di posta del visitatore con il messaggio già scritto.

Prima della pubblicazione definitiva conviene collegare il testo del consenso a una pagina di informativa privacy.

## Font

Ronzino Medium (peso 500) è incorporato in base64 dentro `index.html`: non dipende da nessun file esterno, quindi non può andare in 404 su GitHub Pages. Per aggiornarlo va sostituito il blocco `@font-face` nell'HTML.

## Verifiche

Confermati in test locale da server HTTP: Home e 11 foto, navigazione, apertura di About e font Medium senza file mancanti. Il sito usa immagini reali remote per alcuni hover quando raggiungibili e, in caso contrario, immagini di riserva locali. La versione Safari va verificata anche sul dispositivo di destinazione.

## Da completare prima della pubblicazione definitiva

Nell'About e nel pannello Contatti è ancora presente il testo segnaposto per email e social: sostituirlo quando disponibili. Va inoltre attivato l'invio del modulo (vedi sopra).
