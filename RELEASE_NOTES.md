## Download consigliati

- **Windows x64:** `Forgia-0.4.1-Windows-x64-Setup.exe`; alternativa ZIP da estrarre interamente.
- **Linux x64:** `Forgia-0.4.1-Linux-x64.AppImage`; alternativa archivio tar.gz.

Non servono Node.js o compilazione. Consulta il [README](https://github.com/lorenzoneri-dev/Forgia-downloads#scarica-e-avvia) per requisiti e collegamento degli assistenti.

## Novità 0.4.1

- **Servizio e modello in un solo menu:** pulsante compatto con logo, cataloghi raggruppati, ricerca e aggiornamento, errori separati e navigazione da tastiera.
- **Progetti di Chat locale:** organizza chat in cartelle logiche, cerca, rinomina e sposta le conversazioni. La rimozione del progetto conserva chat e libreria.
- **Fonti del progetto:** collega file della libreria o seleziona file dal computer; vengono inclusi automaticamente nei messaggi successivi. Anteprima e selezione di porzioni, con controllo dei file mancanti/modificati e limiti di 8 allegati e 40.000 caratteri.
- **Codice più leggibile:** evidenziazione sintattica, copia del testo originale e download tramite dialogo di salvataggio. I contenuti HTML non vengono eseguiti.
- **Ragionamento:** pannello espandibile con testo o riepiloghi forniti dal provider e selezione dei livelli compatibili. La disponibilità dipende dal modello e dal servizio.
- **Dettatura corretta:** raccolta dei campioni finali prima della chiusura, ricampionamento a 16 kHz ed errori distinti; limite di due minuti e trascrizione nella bozza senza invio automatico.
- Saluti più naturali nella Chat locale; cronologia conservata con backup preventivo nella migrazione allo schema 5.

## Verifiche e compatibilità

56 test unitari e sette suite desktop su sorgenti e pacchetti Linux/Windows x64, più le verifiche MCP e runtime vocale previste dalla pipeline. I quattro pacchetti provengono dallo stesso [workflow verificato](https://github.com/lorenzoneri-dev/Forgia/actions/runs/36924938526), commit sorgente `67a1c46b356c72a0eb8b122d0dd4de80b996df60`.

La migrazione dei dati 0.3.1 conserva conversazioni, libreria e attività, creando prima un backup. Le fonti sono riferimenti agli originali, non copie. Whisper è stato provato localmente anche con una registrazione di due minuti e un dispositivo simulato.

I provider e i cataloghi sono collaudati con simulazioni: restano da attestare login e inferenza cloud reali, modelli visivi reali, LM Studio, microfoni fisici e installazione su un Windows personale. Il pannello Ragionamento mostra esclusivamente quanto fornito dal provider.

**Preview x64 non firmata:** sono allegati checksum SHA-256, licenza e avvisi delle dipendenze. Modelli, credenziali, sorgenti privati e dati personali non sono inclusi. Nessun aggiornamento automatico. Le release precedenti restano disponibili.
