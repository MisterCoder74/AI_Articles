# Report ricerca — Article Generator, 2026-11-16

## Query

- "Claude Code Code Mode v2.1.323 release notes November 2026"
- "Claude Code Code Mode documentation requirements limitations permissions"
- "November 2026 AI developer tools release notes Copilot CLI Codex OpenCode"

## Cinque risultati principali

1. [Anthropic Claude Code v2.1.323](https://github.com/anthropics/claude-code/releases/tag/v2.1.323), 12 novembre, stabile: aggiunge Code Mode sperimentale e opt-in.
2. [Documentazione ufficiale Code Mode](https://code.claude.com/docs/en/code-mode): esecuzione JavaScript per tool call, requisiti, permessi, limiti e opzioni di attivazione.
3. [GitHub Copilot CLI v1.0.112](https://github.com/github/copilot-cli/releases/tag/v1.0.112), 13 novembre, stabile: miglioramenti a subagent/sessioni e uso dei workflow.
4. [OpenAI Codex CLI v0.169.0](https://github.com/openai/codex/releases/tag/rust-v0.169.0), 13 novembre, stabile: side-chat nel terminale e provider personalizzati.
5. [OpenCode v2.3.0](https://github.com/anomalyco/opencode/releases/tag/v2.3.0), 13 novembre, stabile: subagent background predefiniti e ricerca dei prompt precedenti.

## Tema scelto e motivazione

**Claude Code Code Mode.** È un cambiamento operativo verificabile, circoscritto e con requisiti/limiti chiari; tratta l'esecuzione combinata dei tool, non l'annuncio di un nuovo modello. Evita sia il tema routine del 9 novembre (Gemini API CLI / VS Code 1.145) sia i recenti articoli su Fable 5.2 e Gemini Hydrogen. Fonti primarie, nessun benchmark.

## Limiti verificati

Funzione sperimentale opt-in. Non supporta gateway, Bedrock, altri hosting elencati nella documentazione, API headless, SDK, VS Code panel, Desktop e cloud sessions. In auto mode il classifier controlla il blocco di codice, non ogni singola tool call; le permission rules e gli hook continuano a operare.
