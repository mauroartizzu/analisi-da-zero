# Analisi da zero

Un corso interattivo di Analisi Matematica 1 che non dà nulla per scontato: 19 capitoli: fondamenti (insiemi e relazioni, numeri complessi, equazioni e disequazioni, funzioni, induzione, vettori e matrici, rette e piani) e analisi (successioni, serie, limiti, continuità, derivate, teoremi e De l'Hôpital, Taylor, integrali, aree/volumi/impropri, studio di funzione), più una sezione di allenamento (generatore infinito di esercizi, flashcard a ripetizione spaziata, tracciamento dei progressi con esporta/importa senza account), formulario e simulazione d'esame con test a punteggio.

Ogni capitolo ha spiegazione in parole povere, definizioni, esempi svolti, grafici interattivi e un quiz.

## Come si usa

Apri `index.html` in un browser, oppure visita la versione pubblicata su GitHub Pages:

`https://<tuo-username>.github.io/<nome-repository>/`

Il sito è un singolo file HTML senza dipendenze da installare. I progressi (capitoli, quiz, palestra, flashcard) si salvano automaticamente nel browser e si possono esportare/importare come file JSON dalla sezione "I miei progressi". Le formule matematiche vengono renderizzate da KaTeX, caricato da CDN (serve una connessione internet per vederle).

## Pubblicare su GitHub Pages

1. Crea un repository pubblico su GitHub.
2. Carica tutti i file di questa cartella (compreso `.nojekyll`).
3. Vai in **Settings → Pages**, alla voce *Source* scegli **Deploy from a branch**, branch `main`, cartella `/ (root)`, e salva.
4. Dopo un minuto circa il sito è online all'indirizzo indicato nella stessa pagina.

## Struttura

```
index.html   il corso completo (HTML, CSS e JavaScript in un unico file)
.nojekyll    dice a GitHub Pages di pubblicare i file così come sono
README.md    questo file
LICENSE      licenza MIT
```

## Modificare il corso

Tutto è in `index.html`. I capitoli sono blocchi `<section class="cap" id="...">`; i grafici interattivi sono nello `<script>` in fondo, uno per capitolo, tutti costruiti sulla stessa piccola classe `Plot`.
