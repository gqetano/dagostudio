# DAGOSTUDIO — sito per GitHub Pages | V60

Questa cartella contiene **la versione V60** approvata, con tutte le 11 fotografie della Home e il ritratto About inclusi come file locali. Le quattro immagini concept di riserva per gli hover sono incluse localmente. Le foto reali dei riferimenti culturali vengono richieste a Wikimedia Commons; se non disponibili viene mostrata l’immagine concept corrispondente.

## Pubblicazione su GitHub Pages

1. Crea un repository GitHub (oppure usa quello del sito).
2. Carica **il contenuto di questa cartella** nella radice del repository, non la cartella contenitore. La radice deve avere `index.html`, `images/` e `assets/`.
3. In Settings → Pages, seleziona Deploy from a branch, branch `main`, folder `/ (root)`; salva.
4. Apri l’URL GitHub Pages mostrato nelle impostazioni.

Puoi anche caricare lo ZIP tramite un programma che lo estragga prima: GitHub Pages non pubblica automaticamente un archivio ZIP caricato come singolo file.

## Note di pubblicazione

- **Font:** il file `Ronzino-Medium.woff2` non era presente nei file forniti. Aggiungilo in `assets/` se ne disponi con licenza. Senza, il sito userà un fallback, con aspetto tipografico diverso. Vedi `assets/INSTALLARE-FONT.txt`.
- **Contatti:** la dicitura “email e social da inserire” è ancora un segnaposto; sostituiscila prima di pubblicizzare il sito.
- **Hover desktop:** immagini culturali via Wikimedia con fallback concept locale; collegamenti cliccabili ai video ufficiali Depeche Mode e Joy Division. Gli effetti sonori hover sono dimostrativi, non brani commerciali.
- **Versione:** V60, con About scorrevole, colophon al bordo inferiore, +/X fisso durante lo scroll e colophon a colonna singola su iPhone. Lo switch On/Off è stato rimosso.
- Il sito è statico: non richiede build, Node.js o dipendenze esterne.

Crediti delle fotografie di riferimento in `CREDITI-IMMAGINI.md`.
