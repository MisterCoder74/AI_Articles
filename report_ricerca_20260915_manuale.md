# Report Generazione Articolo — 15 Settembre 2026 (esecuzione manuale)

## Richiesta
Esecuzione manuale (non attesa la ricorrenza cron del lunedì) richiesta direttamente dal proprietario: creare un articolo per la categoria/tag "strumenti" che pubblicizza il prodotto **CertainThing**, basato sulla pagina:
https://www.vivacitydesign.net/vd_ai_division/vd-ai-certainthing/certainthing_project_report.html

## Nota sul vincolo anti-marketing della routine
La routine automatica settimanale vieta contenuti di marketing nella selezione autonoma dei topic. Questa esecuzione è un override esplicito e manuale del proprietario per promuovere un proprio prodotto (CertainThing) — non la routine che sceglie da sé un topic di marketing. Procedura eseguita come da istruzione diretta.

## Fonte
Pagina "CertainThing — Report di Progetto" (Vivacity Design AI Division): origine e tappe di sviluppo, stack tecnico (PHP/JS vanilla, JSON piatti, Stripe), architettura BYOK, processo di sviluppo agentico su SureThing AI (1 agente, 327 run, 11.276,6 crediti, stima $56–$113), tre assi di differenziazione (BYOK, Agentic Workspace, reasoning trasparente) e tabella di posizionamento competitivo (Cursor/Windsurf, Replit Agent, Bolt.new/Lovable, v0, GitHub Copilot Workspace).

## Articolo pubblicato
**Titolo**: "CertainThing: il Vibe Coder che Mette la Trasparenza dei Costi al Centro"
**Tag/categoria**: Strumenti AI → filtro "strumenti"
**Slug**: certainthing_vibe_coder_byok_vivacity
**Lunghezza**: 1.078 parole, 6 sezioni H2 in numeri romani, 2 highlight-box, 1 quote box

## Nota tecnica: mojibake reintrodotto sull'indice live
Al fetch dell'indice live fresco da GitHub in questo run sono stati trovati 48 marcatori di corruzione di encoding (caratteri accentati italiani mostrati come "PerchÃ©" ecc.), reintrodotti da due commit diretti dell'utente sull'editor web di GitHub avvenuti dopo l'ultimo push di questa cella (commit "Add Open Graph image meta tag" e "Update JSON-LD schema for blog page URL", entrambi del 15 settembre alle ~04:3x UTC, entrambi firmati GPG da GitHub web-flow). La corruzione è stata quindi reintrodotta da un'edit diretta lato utente sull'interfaccia web di GitHub, non dal meccanismo di pubblicazione di questa cella. È stata riparata (ftfy.fix_text, verificata a zero marcatori residui) prima di applicare l'aggiornamento dell'indice per il nuovo articolo.

## Aggiornamento indice
- Sezione "Last Article" → nuovo articolo CertainThing
- Articolo precedentemente in "Last Article" ("Agents API di OpenAI...") spostato in cima a "Previous Articles"
- JSON-LD `Blog.blogPost[]`: nuova voce prepended, cap mantenuto a 15 elementi
- Card HTML totali nella griglia: 53 (storico completo, nessun taglio)
