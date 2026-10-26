---
type: markdown
---
# Report ricerca — Article Generator, 26 ottobre 2026

## Query
Novità AI operative annunciate dal 19 al 26 ottobre 2026: modelli, coding agents, strumenti per sviluppatori e piattaforme agentiche. Esclusi marketing, e-commerce ed etica; evitato Gemini 4 Argon, tema dell'articolo della settimana precedente. Query di ricerca: rilasci ufficiali Snowflake MCP coding agent, GitHub Copilot/CLI e Visual Studio, Chrome DevTools MCP, OpenAI Cloud partnership e AI Gateway.

## Cinque risultati rilevanti
1. **Snowflake — “October 23, 2026: Coding agent MCP tool”** (23 ottobre, release note ufficiale): i server MCP gestiti possono dichiarare un tool `CODING_AGENT` senza un oggetto agent registrato; Snowflake aggiunge `code_toolset_all`, il sandbox è associato al thread e la documentazione descrive la continuazione con `thread_id`. https://docs.snowflake.com/en/release-notes/2026/other/2026-10-23-mcp-coding-agent
2. **Snowflake — “Oct 19, 2026: Tools for Cortex AI Gateway (Preview)”** (19 ottobre, release note): anteprima per amministrare server/tool MCP, catalogo curato, policy sui tool, server personalizzati e ispezione attività. Non è il tema scelto perché riguarda soprattutto governance e provisioning del gateway, non il nuovo coding tool. https://docs.snowflake.com/en/release-notes/2026/other/2026-10-19-cortex-ai-gateway-tools
3. **ChromeDevTools — chrome-devtools-mcp v1.12.0** (22 ottobre, release GitHub ufficiale): navigazioni parallele, analisi heap senza browser collegato e ricarica live della configurazione tra i cambiamenti. Alternativa forte, ma meno focalizzata su una singola nuova capacità agentica. https://github.com/ChromeDevTools/chrome-devtools-mcp/releases
4. **GitHub Copilot CLI — 1.0.103-0** (22 ottobre, release GitHub ufficiale): cache MCP locale riusata tra worktree, opzioni remote più chiare, impostazioni sandbox ACP rispettate al resume e altre correzioni. Non scelto per taglio più incrementale e vasto. https://github.com/github/copilot-cli/releases/tag/v1.0.103-0
5. **OpenAI — “OpenAI models are coming to Google Cloud”** (annuncio del 21 ottobre secondo gli annunci/news risultati; pagina ufficiale): partnership per rendere disponibili modelli OpenAI e workflow Codex in Google Cloud Model Garden; GA prevista nelle settimane successive, quindi non ancora dichiarata GA nella fonte. https://openai.com/index/openai-models-google-cloud/

## Argomento scelto
Il nuovo tool `CODING_AGENT` nei server MCP gestiti Snowflake: configurazione, chiamate MCP, thread e sandbox, differenze rispetto agli altri tipi di tool e limiti operativi/documentali.

## Perché
È la novità più circoscritta e direttamente rivolta all'uso di agenti di sviluppo: una nuova modalità di esporre coding agent in un'integrazione MCP, annunciata nella finestra corrente e descritta da fonti ufficiali Snowflake. Consente di spiegare un percorso pratico dalla definizione YAML all'invocazione e alla continuazione delle sessioni, senza ripetere l'articolo precedente sui modelli. Sono riportati i limiti della documentazione (50 tool per server, continuazione controllata da flag, annotazioni non equivalenti a controlli di sicurezza); non si attribuiscono al rilascio prezzi, benchmark, modello predefinito o garanzie non trovate nelle fonti.
