# Sopralluoghi RSPP (PWA)

App installabile per il primo sopralluogo (D.Lgs. 81/2008): screening di applicabilità, 309 voci, priorità, foto e note vocali per ogni voce, funzionamento offline, backup ZIP e report con foto.

## Pubblicare su GitHub Pages

1. Su github.com crea un repository (per esempio `sopralluogo`). Con il piano gratuito deve essere **pubblico**: contiene solo la checklist, mai i dati dei sopralluoghi, che restano sul telefono.
2. Carica **tutto il contenuto di questa cartella** nella radice del repository (Add file → Upload files; trascina anche le cartelle `icons` e `lib` e il file `.nojekyll`).
3. Settings → Pages → Source: *Deploy from a branch* → Branch: `main`, cartella `/ (root)` → Save.
4. Dopo uno o due minuti l'indirizzo è `https://<tuo-utente>.github.io/<repository>/`.

## Installare sul telefono (Android, Chrome)

1. Apri l'indirizzo. Fai una prima apertura con la rete attiva: l'app si scarica per l'uso offline.
2. Menu ⋮ → *Installa app* (o il pulsante «Installa l'app» nella pagina iniziale).
3. Alla prima richiesta consenti fotocamera e microfono.

## Uso

- **Elenco**: ogni sopralluogo ha la sua scheda (Apri, Report, Backup ZIP, Elimina).
- **Foto** apre la fotocamera, **Registra** avvia la nota vocale, **Audio** allega un file già registrato.
- **Backup ZIP** contiene `sopralluogo.json`, `report.html`, `checklist.xlsx` e la cartella `allegati/` con foto e audio come file normali. «Condividi» usa il menu del telefono (email, OneDrive, WhatsApp). Per ripristinare: «Importa backup» nell'elenco.
- **Report con foto**: a schermo, con «Stampa / Salva PDF» e «Scarica report HTML con foto».
- I dati stanno nel browser del telefono. Se cancelli i dati del sito o disinstalli Chrome si perdono: il backup ZIP è l'unica copia.

## Aggiornare l'app

Sostituisci i file nel repository e cambia `VERSION` in `sw.js` (per esempio da `s81-v1` a `s81-v2`). Chi ha l'app aperta vede il pulsante «Ricarica».
