# Report Generazione Articolo — 28 Settembre 2026, 09:00 (routine settimanale)

## Query di ricerca
1. "trending operational AI news this week: new model releases, developer tools, coding agents, agentic frameworks launches — week of September 21-28 2026"
2. "new AI model release week September 22 2026"
3. "AI coding agent announcement September 24 2026"
4. "Anthropic Claude Opus 5.5 announcement official"
5. "OpenAI GPT-6 Sol Luna announcement official"

## 5 risultati più rilevanti raccolti
1. **Introducing GPT-6 Sol and Luna** (openai.com, 22 settembre 2026) — annuncio ufficiale OpenAI: due nuovi modelli della famiglia GPT-6, prezzi API dimezzati rispetto alla tariffa promozionale di GPT-5.6, benchmark su AutomationBench/Agents' Last Exam/FrontierCode/DeepSWE/OSWorld 2.0, miglioramenti al prompt caching (dashboard, diagnostica, breakpoint espliciti). Fonte primaria ufficiale, freschissima. **Scelto come topic principale.**
2. **Introducing Claude Opus 5.5** (anthropic.com, 22 settembre 2026) — Anthropic rilascia Opus 5.5, primo modello della famiglia 5.5, con miglioramenti di sicurezza/allineamento e costo ridotto del 40% rispetto a Opus 5. Fonte primaria ufficiale, stesso giorno di GPT-6 Sol/Luna. Runner-up solido, deprioritizzato per evitare di scegliere fra due lanci-modello dello stesso giorno: l'annuncio OpenAI offriva più materiale operativo verificabile (prezzi, benchmark comparativi dettagliati, meccaniche di caching per sviluppatori) da coprire in un articolo tecnico-operativo.
3. **Introducing Muse: The World's First Personal AI Agent Built for Everyone** (about.fb.com, Meta) — nuovo agente personale Meta basato su Muse Spark, con VM sicura dedicata e pagamenti via Stripe Link. Scartato: la data esatta di questo run non è confermata entro la finestra 21-28 settembre dai risultati fetchati, e il contenuto è più orientato al consumer/agente personale che a strumenti/modelli per sviluppatori.
4. **Amazon CloudWatch Omni: AI-first observability for agents and applications** (aws.amazon.com) — nuovo strumento di osservabilità AI per agenti (LangGraph, CrewAI, OpenAI Agents SDK, Vercel AI SDK, Strands). Scartato come topic principale: più vicino a infrastruttura/osservabilità che a model/feature news, categoria a priorità più bassa per preferenza standing dell'utente.
5. **Best AI Coding Agents (September 2026)** (morphllm.com, aggiornato 22 settembre 2026) — classifica aggiornata dei coding agent (Codex + GPT-6 Astra in testa su Terminal-Bench 4.0). Fonte secondaria/aggregatrice, usata solo come conferma di contesto sul posizionamento dei modelli GPT-6, non come topic autonomo.

## Topic scelto
**GPT-6 Sol e Luna: il lancio OpenAI del 22 settembre 2026 che dimezza i prezzi API della famiglia GPT-6 e potenzia il caching per gli agenti.**

## Motivazione della scelta
- Fonte primaria ufficiale (openai.com), pubblicata appena 6 giorni prima di questo run.
- Notizia di modello/prodotto con forte componente operativa per sviluppatori (prezzi API, benchmark, meccaniche di caching per agenti e Codex) — priorità dichiarata dall'utente su model/feature/tool news rispetto a infra/protocollo (per questo scartata l'osservabilità AWS CloudWatch Omni).
- Prodotto sottostante distinto dal topic della settimana precedente (21 settembre: i livelli Efficienza/Equilibrio/Intelligenza di GitHub Copilot per instradare tra modelli già esistenti). Questo articolo riguarda l'altro lato del problema: l'arrivo di due modelli nuovi con propria politica di prezzo/caching, non l'interfaccia di scelta tra modelli di un prodotto terzo.
- Claude Opus 5.5 (Anthropic, stesso giorno) è stato valutato come runner-up equivalente in freschezza ma con meno materiale operativo/benchmark diffuso nella fonte fetchata rispetto all'annuncio OpenAI; citato nell'articolo solo come contesto concorrente nella sezione dei limiti, non trattato come topic principale, per evitare un confronto testa a testa non ancora verificabile in modo indipendente.

## Nota tecnica: mojibake sull'indice live (di nuovo) + correzione di un errore di sequenza in questo run
Il fetch fresco dell'indice live da GitHub ha mostrato 54 marcatori di corruzione di encoding (stesso pattern ricorrente osservato nei run precedenti). In questo run lo script di riparazione (`fix_mojibake_and_finalize.py`) opera sul file di output finale (`output/pillole_di_ai.html`), non sul file grezzo appena scaricato: un comando intermedio aveva sovrascritto la copia già riparata con il file grezzo non ancora corretto, e lo script di generazione articolo aveva poi letto ancora il file grezzo. L'anomalia è stata rilevata da un controllo diretto sul file di output finale (54 marcatori residui) prima del push, e corretta rieseguendo `fix_mojibake_and_finalize.py` sull'output finale — verificato a zero marcatori residui prima di procedere con il push.

## Aggiornamento indice
- Sezione "Last Article" → nuovo articolo GPT-6 Sol e Luna
- Articolo precedentemente in "Last Article" ("GitHub Copilot Sceglie il Modello per Te...") spostato in cima a "Previous Articles"
- JSON-LD `Blog.blogPost[]`: nuova voce prepended, cap mantenuto a 15 elementi
- Card HTML totali nella griglia: 56 (storico completo, nessun taglio)
