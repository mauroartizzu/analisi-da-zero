# Analisi da zero

Un corso interattivo di Analisi Matematica 1 che non dà nulla per scontato: insiemi, funzioni, successioni, limiti, continuità, derivate, teoremi (Fermat, Rolle, Lagrange, De l'Hôpital), Taylor, integrali e studio di funzione completo.

Ogni capitolo ha spiegazione in parole povere, definizioni, esempi svolti, grafici interattivi e un quiz.

## Come si usa

Apri `index.html` in un browser, oppure visita la versione pubblicata su GitHub Pages:

`https://<tuo-username>.github.io/<nome-repository>/`

Il sito è un singolo file HTML senza dipendenze da installare. Le formule matematiche vengono renderizzate da KaTeX, caricato da CDN (serve una connessione internet per vederle).

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
