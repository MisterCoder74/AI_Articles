# Report Article Generator — 14 Settembre 2026

## Query di ricerca
- "latest AI model, developer tool, or agentic coding tool releases and news this week September 2026 operational AI announcements"
- "OpenAI Agents API public beta launch date features pricing developers"

## 5 risultati più rilevanti
1. **OpenAI, "Introducing the Agents API"** (openai.com/index, 10 settembre 2026) — annuncio ufficiale della Agents API in beta pubblica: harness gestito lato server, sandbox a scelta, compattazione automatica del contesto, tool search, multi-agente nativo. Fonte primaria, scelta come argomento principale.
2. **OpenAI, "New tools for building agents"** (11 marzo 2025) — precedente lancio di Responses API, Agents SDK e strumenti nativi; usato come contesto storico per mostrare l'evoluzione verso l'Agents API.
3. **Anthropic, Claude Platform release notes** (docs.anthropic.com, 10 settembre 2026) — permission policy `auto` per Claude Managed Agents e CLI `ant beta:sessions connect`; considerato ma scartato come argomento principale (troppo incrementale/di configurazione rispetto al lancio di una nuova API).
4. **Anthropic, Claude Fable 5.1 / Mythos 5.1** (1 settembre 2026) — nuovi modelli con contesto 1M e adaptive thinking; scartato perché il lancio risale a due settimane fa, meno "caldo" rispetto all'Agents API di 4 giorni prima.
5. **OpenAI, github.com/openai/codex** — repository open source dell'harness Codex, citato come fondamenta tecniche dell'Agents API.

## Argomento scelto
**Agents API di OpenAI: l'Infrastruttura di Codex Diventa un'API per Tutti** (beta pubblica, 10 settembre 2026).

## Motivazione della scelta
- Notizia più recente della settimana (4 giorni prima della generazione) con fonte primaria diretta (blog ufficiale OpenAI).
- Rilascio di tool/feature per sviluppatori, in linea con la preferenza per notizie di modello/funzionalità rispetto a deep-dive infrastrutturali.
- Argomento distinto dal tema della settimana scorsa (Xcode 26.3 + Claude Agent SDK/Codex nell'IDE Apple): qui il soggetto è il prodotto API di OpenAI stesso, non un'integrazione IDE di terze parti — nessuna ripetizione dello stesso prodotto sotto un'altra angolazione.
- Scartati come alternative: gli aggiornamenti di configurazione Claude Platform del 10 settembre (troppo granulari per reggere un intero articolo), Claude Fable 5.1/Mythos 5.1 (lancio di due settimane prima, meno "caldo").

## Nota tecnica rilevante di questo run
Durante l'aggiornamento dell'indice è stata scoperta una corruzione di encoding diffusa su gran parte delle card storiche (caratteri accentati italiani trasformati in sequenze tipo "PerchÃ©"), causata da un bug nel meccanismo di push usato finora (il transport che passa i contenuti a GitHub tramite riga di comando interpretava il testo con un locale non-UTF-8). La causa è stata isolata e risolta forzando un locale UTF-8 prima di ogni push; l'indice è stato riparato e ripubblicato pulito, verificato riscaricandolo da GitHub.
