# Prompt Management — Directive

## Goal
Gestire il prompt di sistema dell'IA in modo esternalizzato per garantire modifiche sicure, istantanee e una gestione efficiente dei token.

## Inputs
- `prompt.json`: File JSON contenente la stringa del prompt di sistema.

## Tools (Scripts)
- Al momento la gestione è manuale o tramite l'agente.

## Steps
1. **Modifica**: Aprire il file `prompt.json`.
2. **Aggiornamento**: Inserire le nuove istruzioni IA nel valore della chiave `systemPrompt`.
3. **Validazione**: Salvare il file e ricaricare l'applicazione `index.html`.
4. **Verifica**: Inviare un testo al correttore per testare il nuovo comportamento.

## Expected Output
Un file `prompt.json` correttamente formattato che viene caricato dinamicamente dall'applicazione.

## Known Edge Cases
- **File Mancante**: Se `prompt.json` non viene trovato, l'applicazione deve gestire l'errore o usare un prompt di fallback locale.
- **Formato JSON Errato**: Un errore di sintassi in `prompt.json` impedirà il caricamento; validare sempre il JSON dopo la modifica.
