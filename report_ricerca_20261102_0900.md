---
type: markdown
---
# Report ricerca — Article Generator, 2 novembre 2026

## Query
Ricerca di novità operative per sviluppatori AI annunciate dal 26 ottobre al 2 novembre 2026: Gemini API/AI Studio CLI, agenti di coding, API e nuovi modelli. Verifica su fonti ufficiali Google AI Studio/Gemini API e release GitHub recenti. Tema della settimana precedente (server MCP gestiti Snowflake) escluso.

## Cinque risultati rilevanti
1. **Gemini API CLI (`gemini-api`) beta — 27 ottobre**. Client CLI stateless e senza dipendenze di progetto, pensato per coding agents, script e pipeline CI. Opera sull'Interactions API per generare testo/media, analizzare file e avviare Gemini managed agents. La guida documenta schema/usage lookup, dry-run, output strutturato, file scritti su disco, stato beta e pin della release nei job automatici. Fonti: [changelog Google AI Studio](https://aistudio.google.com/docs/changelog), [guida Gemini API CLI](https://aistudio.google.com/docs/cli).
2. **Computer Use GA — 30 ottobre**. Il tool è GA per Interactions e GenerateContent APIs. Annuncio breve; il client resta responsabile di ambiente, screenshot ed esecuzione delle azioni. Fonte: [Gemini API changelog](https://ai.google.dev/gemini-api/docs/changelog).
3. **Storage Generate Content API `store=true` di default per nuovi progetti a pagamento — 26 ottobre**. Vale per nuovi progetti; quelli esistenti mantengono la configurazione. È possibile impostare `store=false` per richiesta o disattivare il logging dal dashboard Logs and Datasets. Fonte: [AI Studio changelog](https://aistudio.google.com/docs/changelog).
4. **Snowflake — Tools for Cortex AI Gateway (Preview), 19 ottobre**. Catalogo MCP gestito, policy sui tool e activity review; tema già pubblicato la settimana precedente come articolo sul `CODING_AGENT` MCP tool, quindi escluso dalla scelta.
5. **GitHub Copilot CLI 1.0.103-0**. La release recente consultata aggiunge riuso di snapshot MCP fra worktree e correzioni a sessioni remote/sandbox; aggiornamento incrementale e non un annuncio di nuova funzione paragonabile all'interfaccia Gemini CLI. [Release](https://github.com/github/copilot-cli/releases/tag/v1.0.103-0).

## Argomento scelto
Gemini API CLI in beta: un client da terminale per coding agent, script e CI che espone operazioni Gemini tramite Interactions API.

## Perché
È il lancio ufficiale più specificamente orientato allo sviluppo di questa finestra. Permette di chiarire il confine utile per il lettore: `gemini-api` è un client API invocabile da shell, non un coding agent interattivo; zero dipendenze di progetto non significa zero setup, poiché servono il binario e una chiave. I dettagli su output strutturato, file su disco, dry-run e pinning sono ancorati alla guida ufficiale. Computer Use GA e il cambiamento di storage sono tenuti separati e solo come contesto; nessun prezzo, SLA o benchmark non documentato viene attribuito alla CLI.
