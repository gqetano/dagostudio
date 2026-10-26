# STUDIO DAGO — Interactive logo

Un'esperienza interattiva per esplorare il logo STUDIO DAGO in prospettiva, cambiare colori e composizione, attivare il flip a 180° o il movimento Spin ed esportare SVG/MP4.

## Struttura

- `index.html` — pagina completa, con grafica, stili e script incorporati: **non richiede build, framework o installazioni**.
- `assets/studio-dago.svg` — file SVG originale, conservato come sorgente per eventuali modifiche future. La pagina usa già una copia incorporata di questo SVG.
- `.nojekyll` — evita l'elaborazione Jekyll quando il sito è servito da GitHub Pages.

## Pubblicare su GitHub Pages

1. Crea un nuovo repository GitHub, ad esempio `studio-dago`.
2. Estrai lo ZIP e carica **il contenuto di questa cartella** nella radice del repository (`index.html` deve essere nella radice, non all'interno di una sottocartella).
3. Apri **Settings → Pages**, scegli **Deploy from a branch**, branch **main** e cartella **/(root)**, poi salva.
4. Apri il link pubblico che GitHub Pages mostra nella sezione Pages. In genere è `https://<tuo-username>.github.io/<nome-repository>/`.

## Uso

- **Clic sul canvas:** flip di 180°.
- **Trascina:** ruota liberamente in orizzontale, con una leggera inclinazione verticale limitata per preservare la leggibilità; **rotella:** zoom senza deformazioni.
- **Spin:** animazione con numero di giri, durata e direzione selezionabili.
- **Barra delle impostazioni:** elementi, distanza, colore del logo e dello sfondo.
- **Save SVG / Esporta MP4:** scarica i risultati.

> Nota: l'esportazione MP4 dipende dal supporto del browser per la codifica video H.264/MP4. È consigliato un browser moderno. Il sito è statico e non necessita di server applicativo.

## Asset e diritti

Il marchio SVG appartiene al rispettivo titolare. Nessuna licenza d'uso del logo è concessa tramite questa cartella.
