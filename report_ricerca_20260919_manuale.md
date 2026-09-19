# Report Generazione Articolo — 19 Settembre 2026 (esecuzione manuale on-demand)

## Richiesta
Esecuzione manuale, non legata alla ricorrenza cron del lunedì, richiesta direttamente dal proprietario: creare un articolo seguendo una traccia dettagliata in 7 punti fornita in chat, sul tema dell'AEO (Answer Engine Optimization) come possibile hype di marketing digitale.

## Fonte
Traccia originale dettata dall'utente in chat (7 punti): nascita del marketing AEO/GEO/LLMO, usi reali di ChatGPT (prevalentemente informativi/creativi, non di ricerca commerciale), il problema dei denominatori nei dati statistici citati dal marketing AEO, la concorrenza e la volatilità delle risposte AI, il vero parametro del ROI economico (volume ricerche, geografia, frequenza citazioni, concorrenza, traffico, conversioni, valore cliente), una conclusione bilanciata (monitorare senza farsi vendere una rivoluzione prematura), e la chiusura con le tre domande chiave da porre a un consulente AEO.

## Articolo pubblicato
**Titolo**: "AEO: la Nuova Frontiera del Web o l'Ennesimo Hype del Marketing Digitale?"
**Tag/categoria**: Critica AI → filtro "fenomeni"
**Slug**: aeo_hype_marketing_o_nuova_frontiera
**Lunghezza**: 1.006 parole, 7 sezioni H2 in numeri romani (una per punto della traccia), 1 highlight-box, 1 quote box, 1 lista di controllo ROI

## Nota tecnica: mojibake sull'indice live
Anche in questo run l'indice live fresco da GitHub conteneva 48 marcatori di corruzione di encoding (stesso pattern osservato il 15 settembre), riparati con lo script dedicato prima di applicare l'aggiornamento per il nuovo articolo — verificati a zero marcatori residui sia sul file locale che, dopo il push, sul file remoto.

## Aggiornamento indice
- Sezione "Last Article" → nuovo articolo AEO
- Articolo precedentemente in "Last Article" ("CertainThing: il Vibe Coder...") spostato in cima a "Previous Articles"
- JSON-LD `Blog.blogPost[]`: nuova voce prepended, cap mantenuto a 15 elementi
- Card HTML totali nella griglia: 54 (storico completo, nessun taglio)
