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

## Font

Ronzino Medium (peso 500) è incorporato in base64 dentro `index.html`: non dipende da nessun file esterno, quindi non può andare in 404 su GitHub Pages. Per aggiornarlo va sostituito il blocco `@font-face` nell'HTML.

## Verifiche

Confermati in test locale da server HTTP: Home e 11 foto, navigazione, apertura di About e font Medium senza file mancanti. Il sito usa immagini reali remote per alcuni hover quando raggiungibili e, in caso contrario, immagini di riserva locali. La versione Safari va verificata anche sul dispositivo di destinazione.

## Da completare prima della pubblicazione definitiva

Nell'About è ancora presente il testo segnaposto per email e social: sostituirlo quando disponibili.
