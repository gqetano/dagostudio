# DAGOSTUDIO V62 — GitHub Pages

Tutte le scelte visive e interattive restano quelle della V61. In questa versione è stato corretto solo il caricamento di Ronzino Medium: dichiarazione @font-face con sorgente WOFF2 diretta e preload.

## FONT — UN PASSAGGIO PRIMA DI PUBBLICARE

Copia **il tuo file originale** `Ronzino-Medium.woff2` dentro `assets/` del sito. Il pacchetto contiene il percorso e il CSS necessari, non una copia del file del font. Non servono Regular, Bold o Oblique: questa versione usa solo Medium 500. Non rinominare il file.

Dopo l'upload apri `https://<tuo-sito>/verifica-font.html` e controlla che segnali il caricamento; in caso di cache Safari prova a ricaricare la pagina.

## GitHub Pages

Estrai lo ZIP, copia il font nella cartella `assets/`, poi carica **i contenuti estratti**, con `index.html` alla radice. In Settings → Pages seleziona branch main e cartella / (root).

Il colophon contiene due paragrafi, a due colonne su desktop e una su iPhone; l'About usa lettering rosso pieno, senza selettori o switch. I contatti sono ancora provvisori. Crediti immagini: `CREDITI-IMMAGINI.md`.
