# GrainUp — Laboratorio di cucina digitale

Sito interattivo di ricette personalizzabili: scegli una ricetta, tocca gli ingredienti sul tavolo, sostituiscili con alternative e ottieni la tua versione, con quantità, avvisi e valori nutrizionali stimati.

## Contenuto
- `index.html`: l'intera applicazione (HTML, CSS e JavaScript in un solo file, senza dipendenze esterne)
- `.nojekyll`: dice a GitHub Pages di servire il file così com'è

## Pubblicazione su GitHub Pages
1. Crea un repository su GitHub e carica questi file nella radice.
2. Vai su **Settings → Pages**.
3. In "Build and deployment" scegli **Deploy from a branch**, branch `main`, cartella `/ (root)`.
4. Dopo circa un minuto il sito è online su `https://TUONOME.github.io/NOME-REPO/`.

## Come estendere il catalogo
Dati e regole sono all'inizio dello script in `index.html`:
- `I`: catalogo ingredienti (nome, emoji, gruppo, valori nutrizionali per 100 g, descrizione, URL immagine opzionale come sesto elemento)
- `R`: regole di sostituzione (categorie di ricetta, da, a, fattore, affidabilità, avviso, nota nel procedimento)
- `RC`: ricette (ingredienti, quantità, passaggi)

Per usare foto reali, aggiungi l'URL come sesto elemento della riga dell'ingrediente in `I`.

## Limiti attuali
- 3 ricette dimostrative (pancake, torta al cioccolato, biscotti)
- Salvataggio solo nel browser (localStorage): niente account, preferiti o cronologia
- Valori nutrizionali: stime con dati medi
- Nessuna immagine viene generata: la foto del risultato è sempre quella della ricetta originale
