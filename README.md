# DAGOSTUDIO — Versione 14 per GitHub Pages (pacchetto ricreato)

Questo pacchetto conserva **esattamente il codice e le immagini della V14 già approvata**, senza cambiare layout, logo, animazioni, colori o fotografie. Il README è stato riscritto e la struttura ricontrollata.

## Contenuto

```
index.html                 ← homepage (HTML, CSS e JavaScript in un file)
.nojekyll                  ← disattiva l'elaborazione Jekyll su GitHub Pages
README.md                  ← queste istruzioni
assets/logo-originale.svg ← logo vettoriale originale
images/foto-01.webp       ← 11 fotografie, numerate fino a foto-11.webp
...
```

Non è richiesta alcuna installazione, build o backend. **Le cartelle `assets` e `images` devono rimanere allo stesso livello di `index.html`.**

## Caricamento tramite GitHub dal browser

1. **Estrai lo ZIP** sul tuo Mac; NON trascinare lo ZIP direttamente dentro il repository.
2. Apri il repository su github.com, sulla branch `main`.
3. Fai clic su **Add file → Upload files**.
4. Trascina il contenuto della cartella estratta (non la cartella esterna): `index.html`, `README.md`, `.nojekyll`, `assets`, `images`.
5. Controlla che la lista mostri `index.html`, `assets/logo-originale.svg` e `images/foto-01.webp` … `images/foto-11.webp`, poi conferma con **Commit changes**.
6. Nelle impostazioni del repository vai su **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: main → / (root) → Save**.
7. L'indirizzo sarà normalmente `https://TUO-USERNAME.github.io/NOME-REPOSITORY/` (salvo repository speciale username.github.io o dominio personalizzato).

Se carichi i file con **GitHub Desktop**, procedi come qui sotto; è la soluzione consigliata se compare di nuovo l'errore *“Something went really wrong, and we can't process that file”*.

## Alternativa più affidabile: GitHub Desktop (Mac)

1. Installa GitHub Desktop, accedi e apri **File → Clone repository** (scegli il repository DAGOSTUDIO).
2. Apri la cartella locale del repository (**Repository → Show in Finder**).
3. Copia nella root i file e le cartelle estratti dallo ZIP V14. Accetta la sostituzione dei file della versione precedente.
4. Torna in GitHub Desktop: vedrai le modifiche nella scheda **Changes**.
5. Scrivi ad esempio `Aggiornamento DAGOSTUDIO V14`, fai clic su **Commit to main**, poi su **Push origin**.
6. GitHub Pages pubblicherà la nuova versione secondo le impostazioni Pages del repository.

**Importante:** il messaggio di errore in fase di upload mostrato da GitHub è generato prima del commit. Reimpacchettare i file NON garantisce di risolvere un problema del caricamento via browser. Per questo è inclusa anche una seconda confezione denominata **FILE-UNICO**, con un solo `index.html` contenente tutte le foto.

## Versione FILE-UNICO

In questa alternativa le fotografie sono convertite in `data:image/webp;base64,...` **all'interno** dell'HTML. Non servono `images/` né `assets/`; il logo SVG usato per le animazioni è già incorporato nel markup. Si pubblica caricando solo `index.html` (più il README facoltativo). L'aspetto e il comportamento sono identici, ma l'HTML pesa di più.

## Comportamenti della V14 (non alterati)

- Carousel di 11 foto fullscreen visibili dal primo istante, ogni 5 secondi, in loop, cambi netti senza fade.
- Click sulla metà sinistra/destra del sito oppure swipe orizzontale per cambiare fotografia; su desktop il cursore è una freccia rossa a due segmenti.
- Logo originale scomposto che si ricompone tramite scroll; su mobile il gesto rapido ha inerzia con rallentamento. Dopo la composizione il logo rimane fermo.
- Tre modalità di intro **V1 / V2 / V2+**, selezionabili a metà del bordo destro; V2+ è il default.
- Barra stories in basso su desktop, in alto su mobile; croce e cerchio rossi (`#FF0000`) in alto su desktop, in basso su mobile.
- Margini logo mobile allineati alle icone, e logo leggermente abbassato rispetto alla barra stories (modifiche originali della V14).

## Risoluzione problemi

- **“Something went really wrong, and we can't process that file” durante Upload files:** prova GitHub Desktop; il messaggio non dimostra che l'HTML sia sbagliato. Se fallisce anche `index.html` da solo, è particolarmente probabile che riguardi l'interfaccia web, la sessione o la connessione.
- **Pagina 404:** verifica `Settings → Pages`, la branch `main`, `/ (root)` e la presenza di `index.html` nella root.
- **Foto mancanti:** verifica i percorsi `images/foto-01.webp` … `foto-11.webp`, con maiuscole e minuscole esatte.
- **Modifiche non visibili:** prova ricaricamento forzato del browser; controlla in **Actions** o **Settings → Pages** se la pubblicazione è completata.
- **Logo:** `assets/logo-originale.svg` è conservato come originale; per l'animazione vengono usati gli stessi tracciati già presenti in `index.html`.

## Continuità in altre chat

Conserva questo ZIP. Per chiedere modifiche in una nuova conversazione, allega il pacchetto e specifica che la base è **DAGOSTUDIO V14**, con V1/V2/V2+ e le 11 fotografie. Il CSS e il JS sono incorporati in `index.html`, non in file separati.
