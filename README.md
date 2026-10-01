<p align="center"><img src="assets/forgia.svg" width="96" alt="Logo Forgia"></p>

# Forgia 0.3.1 Preview

Assistente desktop per **Linux e Windows**: programma su una copia del progetto, rivedi le modifiche e applicale quando sei pronto. Puoi anche chattare senza progetto con i modelli locali.

## Scarica e avvia

| Sistema | Download consigliato | Alternativa |
| --- | --- | --- |
| **Windows x64** | [Scarica l’installer .exe](https://github.com/lorenzoneri-dev/Forgia-downloads/releases/download/v0.3.1/Forgia-0.3.1-Windows-x64-Setup.exe) | [ZIP da estrarre](https://github.com/lorenzoneri-dev/Forgia-downloads/releases/download/v0.3.1/Forgia-0.3.1-Windows-x64.zip) |
| **Linux x64** | [Scarica l’AppImage](https://github.com/lorenzoneri-dev/Forgia-downloads/releases/download/v0.3.1/Forgia-0.3.1-Linux-x64.AppImage) | [Archivio tar.gz](https://github.com/lorenzoneri-dev/Forgia-downloads/releases/download/v0.3.1/Forgia-0.3.1-Linux-x64.tar.gz) |

[Apri la release e tutti i file](https://github.com/lorenzoneri-dev/Forgia-downloads/releases/tag/v0.3.1) · [Impronte SHA-256](https://github.com/lorenzoneri-dev/Forgia-downloads/releases/download/v0.3.1/SHA256SUMS)

**Windows:** apri l’installer, scegli la cartella di installazione e avvia **Forgia** dal menu Start. In alternativa estrai **tutto** lo ZIP e apri **Forgia.exe** nella cartella estratta.

**Linux:** nelle proprietà dell’AppImage abilita **Consenti l’esecuzione del file come programma**, poi aprila con doppio clic. Se la distribuzione non supporta AppImage/FUSE, estrai tutto l’archivio `tar.gz` e apri **forgia-desktop** nella cartella estratta, mantenendo accanto tutte le risorse. Su alcuni desktop scegli **Esegui** quando richiesto.

Non servono Node.js, pnpm o compilazione. Questa versione supporta computer **Intel/AMD a 64 bit (x64)**; non offre pacchetti ARM o macOS.

## Collega un assistente

Forgia non include un modello di chat. Configura almeno uno degli assistenti in **Connessioni e impostazioni**:

- **Ollama:** installa Ollama, scarica un modello e avvia il suo servizio locale. Indirizzo predefinito: `http://127.0.0.1:11434/v1`.
- **LM Studio:** scarica un modello e avvia il server locale. Indirizzo predefinito: `http://127.0.0.1:1234/v1`.
- **ChatGPT/Codex:** installa il programma ufficiale **Codex CLI**, seleziona il suo eseguibile se necessario e completa **Accedi** in Forgia con un account abilitato.
- **Claude:** installa il programma ufficiale **Claude Code**, seleziona il suo eseguibile se necessario e completa il login con un account abilitato.

La chat senza progetto è disponibile per Ollama e LM Studio. Non servono chiavi API cloud; i programmi ufficiali gestiscono login e accesso ai rispettivi servizi. Forgia è un progetto indipendente, non un prodotto ufficiale OpenAI o Anthropic.

Prima di lavorare automaticamente sui file con un modello locale, premi **Verifica modello**. Testo, immagini e strumenti hanno risultati separati: un modello testuale non può ricevere immagini.

## Novità 0.3.1

- Loghi autentici di ChatGPT/OpenAI, Claude, Ollama e LM Studio nelle connessioni e nei selettori.
- Menu uniformi con navigazione da tastiera e ricerca dei modelli; Codex usa il catalogo disponibile per il tuo account.
- Barra di scrittura centrale nelle conversazioni vuote, in basso dopo il primo messaggio.
- Conversazione, bozza, allegati e assistente ripristinati separatamente tra Programmazione e Chat locale.
- **Aggiungi file** nella libreria registra più percorsi senza copie e senza allegarli alla chat.
- Sidebar ridimensionabili, richiudibili e riapribili.
- Eliminazione persistente delle conversazioni; per i progetti vengono conservati i backup e le modifiche già applicate.

## Cosa offre la Preview

- Tema antracite, editor con schede e confronto Prima/Dopo.
- Copie di lavoro, test configurati, applicazione esplicita e ripristino con controllo dei conflitti.
- Chat locale, immagini, testo/codice e PDF con testo estraibile.
- Libreria che conserva i percorsi degli originali senza duplicarli.
- **Dettatura locale:** in impostazioni o dal microfono premi **Scarica modello vocale** (circa 153 MB). Dopo il download la trascrizione italiana funziona offline. Primo clic registra, secondo clic trascrive e aggiunge il testo alla bozza; controllalo prima di inviarlo. Il modello non è incluso nei pacchetti.

Gli allegati e i messaggi inviati a Codex o Claude vengono elaborati dai rispettivi servizi secondo le loro condizioni. Le copie di lavoro separano i file del progetto, ma non sono container del sistema operativo.

## Stato e verifiche

Questa è una **pre-release non firmata**. Windows può mostrare un avviso di editore sconosciuto/SmartScreen; Linux può richiedere il permesso di esecuzione. Scarica soltanto da questa pagina e confronta le impronte, se vuoi verificare i file. Non è necessario disattivare le protezioni del sistema.

Sono stati collaudati automaticamente sorgenti e pacchetti su Linux e Windows, allegati con provider simulati e il ciclo di copie/revisione/applicazione/ripristino. Le prove reali hanno verificato MiniCPM con testo e strumenti, e Whisper offline anche su una registrazione di due minuti. La trascrizione può contenere errori.

Restano da collaudare login e attività reali con account Codex/Claude, un modello visivo reale, LM Studio e microfoni fisici. I test simulati non attestano questi casi.

Per segnalare problemi usa [Issues](https://github.com/lorenzoneri-dev/Forgia-downloads/issues), indicando sistema operativo, versione, assistente e messaggio di errore. Evita credenziali, conversazioni private e file personali nelle segnalazioni.

## Licenze e aggiornamenti

[Licenza Forgia](LICENSE) · [Avvisi delle dipendenze](https://github.com/lorenzoneri-dev/Forgia-downloads/releases/download/v0.3.1/THIRD_PARTY_NOTICES.txt). Le licenze Electron e Chromium sono incluse anche nei pacchetti. Il modello vocale conserva la licenza della propria distribuzione.

Questo repository contiene documentazione, logo e download; i sorgenti dell’app sono mantenuti nel repository privato. Gli archivi automatici **Source code** di GitHub contengono soltanto questo repository di documentazione: per avviare Forgia scegli il pacchetto per il tuo sistema.

Le release sono pubblicate manualmente. L’app non si aggiorna automaticamente: scarica il nuovo installer o pacchetto dalla pagina Releases. Prima di aggiornare conserva un backup delle attività nella directory dati (`~/.config/Forgia` su Linux, `%APPDATA%/Forgia` su Windows).
