# MyBody — PWA, prototipo v1

Applicazione personale per alimentazione, peso, allenamenti, sonno e benessere, statistiche settimanali, esportazione CSV/JSON e ripristino JSON.

## Pubblicazione

GitHub Pages: Settings → Pages → Deploy from a branch → main → / (root). Aprire l'indirizzo HTTPS in Safari su iPhone e scegliere Condividi → Aggiungi alla schermata Home.

## Privacy e limiti

Il codice del repository è pubblico, ma i dati inseriti dall'utente non vengono inviati a GitHub e sono salvati in localStorage sul dispositivo/browser. Non usare il repository per caricare dati personali. I dati locali possono essere rimossi dal browser: esportare periodicamente un backup JSON e verificarne il ripristino. La ricerca di alimenti invia il solo codice EAN/UPC a Open Food Facts. La lettura tramite fotocamera richiede il supporto browser di BarcodeDetector e potrebbe non funzionare in Safari: inserimento manuale disponibile. L'app non è un dispositivo medico. Versione dimostrativa non ancora collaudata su iPhone reale.

## Struttura

index.html, app.js, manifest.webmanifest, sw.js, icon.svg.

## Note tecniche

Sito statico HTTPS, nessun backend; funzionalità offline tramite service worker dopo il primo caricamento; ricerca alimenti online. Il database del prototipo usa il campo workout (non workouts) e non va sostituito con backup creati da build differenti senza migrazione.
