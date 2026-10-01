## Download consigliati

- **Windows x64:** `Forgia-0.3.1-Windows-x64-Setup.exe` — installa e apri dal menu Start.
- **Linux x64:** `Forgia-0.3.1-Linux-x64.AppImage` — consenti l’esecuzione nelle proprietà del file e apri con doppio clic.
- Alternative: ZIP Windows e archivio Linux tar.gz. Estrai l’intero archivio e mantieni insieme le risorse.

Non servono Node.js o compilazione. Consulta il [README](https://github.com/lorenzoneri-dev/Forgia-downloads#scarica-e-avvia) per requisiti e collegamento degli assistenti.

## Novità 0.3.1

- Loghi autentici dei quattro provider e menu uniformi accessibili da tastiera.
- Ricerca dei modelli con nomi visualizzati e identificatori corretti. Codex legge il catalogo del tuo account; i modelli locali mostrano il logo di Ollama o LM Studio.
- Schermata iniziale pulita: barra centrale finché non viene inviato il primo messaggio, anche nelle chat locali.
- Ripristino separato di conversazione, bozza, allegati, assistente e modello nel passaggio Programmazione ↔ Chat locale.
- **Aggiungi file** nella libreria con selezione multipla, senza duplicare gli originali o allegarli automaticamente.
- Sidebar ridimensionabili e richiudibili, con comandi compatti per riaprirle.
- Eliminazione effettiva e persistente delle conversazioni, con conferma interna. Nei progetti conserva backup, metadati delle transazioni e modifiche già applicate.
- Cambio assistente e modello nella stessa attività; ogni turno Codex riceve esplicitamente il modello scelto.

## Verifiche e limiti

45 test automatici e sei suite desktop su sorgenti e pacchetti Linux/Windows x64, inclusi selettori, ricerca, tastiera, server non disponibili, cambio modalità, bozza, libreria, sidebar, eliminazione e conservazione dei backup. I pacchetti provengono dallo stesso workflow verificato.

I provider ufficiali e i cataloghi sono collaudati con simulazioni. Restano da attestare login e attività reali con account Codex/Claude, modelli visivi reali, LM Studio, microfoni fisici e installazione su un Windows personale.

**Preview non firmata:** possono comparire avvisi di editore sconosciuto. Non richiede di disattivare le protezioni del sistema. Sono allegati checksum SHA-256, licenza e avvisi delle dipendenze. I modelli, le credenziali e i dati personali non sono inclusi. Nessun aggiornamento automatico.
