---
type: markdown
---
# Report ricerca — Article Generator, 9 novembre 2026

## Query
Novità operative AI e strumenti per sviluppatori pubblicate dal 2 al 9 novembre 2026; esclusi Gemini API CLI (articolo della settimana precedente), marketing, e-commerce ed etica. Fonti primarie consultate: note di rilascio ufficiali VS Code, GitHub, Databricks e GitHub Agentic Workflows.

## Cinque risultati rilevanti
1. **VS Code 1.145 — harness diversi in nested agent sessions (4 novembre)**. La funzione Preview `chat.agentHost.multipleChatProviders.enabled` permette alle sessioni annidate di selezionare un harness differente dal parent; ogni chat mantiene modello, agente e permessi propri. Spostamento e fork conservano cronologia/configurazione secondo le note. Fonte primaria: [Visual Studio Code 1.145](https://code.visualstudio.com/updates/v1_145).
2. **GitHub Copilot in JetBrains Air (annuncio 3 novembre, nel riepilogo settimanale del 6 novembre)**. Copilot permette di seguire più sessioni agentiche e avviare attività localmente nell'IDE o nel cloud tramite Air Teams, con la subscription Copilot esistente. Fonte: [GitHub Changelog](https://github.blog/changelog/2026-11-06-github-copilot-weekly-releases-november-2/).
3. **GitHub Copilot in Xcode (4 novembre)**. Integrazione nel coding assistant nativo di Xcode, in public preview da Xcode 27.3 beta. Fonte: [GitHub Changelog](https://github.blog/changelog/2026-11-04-github-copilot-is-now-available-in-xcodes-coding-assistant/).
4. **GitHub Agentic Workflows v1.2.1 (6 novembre)**. Tra i cambiamenti: continuazione di workflow tramite artifact tra agenti, aggiornamenti più sicuri, supporto auth/engine e revisione di sicurezza fail-closed per casi irrisolti. Fonte: [Weekly Update ufficiale](https://github.github.com/gh-aw/blog/2026-11-09-weekly-update/).
5. **Databricks Unity Gateway — Kimi K3.1 Pro (4 novembre)**. Il modello è disponibile su endpoint pay-per-token in `us-east-1`, con visione e reasoning nativi, per coding, knowledge work e tool use agentico. Fonte: [Databricks November release notes](https://docs.databricks.com/aws/en/release-notes/product/2026/november).

## Argomento scelto
VS Code 1.145: le nested agent sessions possono usare harness diversi all'interno di una stessa sessione principale.

## Perché
È una funzione concreta e documentata direttamente nelle release notes Microsoft; riguarda il lavoro quotidiano con agenti di coding, non ripete il tema Gemini API CLI della settimana precedente e consente di spiegare con precisione il confine tra sessione parent e chat annidate. L'articolo deve mantenere espliciti lo stato Preview e il fatto che modello, agente e livelli di permesso restano propri di ciascuna chat; non attribuirà interoperabilità o condivisione di stato non dichiarate.
