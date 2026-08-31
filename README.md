# AccessiWeb Widget for Google Tag Manager

Template ufficiale per integrare il Widget di accessibilità AccessiWeb in un sito web tramite Google Tag Manager.

Il widget offre:

- 8 profili di navigazione dedicati a specifiche esigenze di disabilità;
- 10 regolazioni sui contenuti;
- 12 impostazioni di accessibilità percettiva, visiva e uditiva;
- 15 regolazioni cromatiche.

## Requisiti

Per utilizzare il template è necessaria una License Key AccessiWeb valida, associata al dominio sul quale viene pubblicato il contenitore GTM. La chiave si ottiene registrandosi su [AccessiWeb](https://www.accessiweb.it).

## Installazione

1. In Google Tag Manager apri **Modelli**.
2. Cerca **AccessiWeb Widget** nella Community Template Gallery e aggiungilo al workspace.
3. Crea un nuovo tag utilizzando il modello AccessiWeb.
4. Inserisci la License Key e configura l'aspetto del widget.
5. Associa il trigger **Initialization - All Pages** o **All Pages**.
6. Usa la modalità Anteprima di GTM per verificare il caricamento.
7. Pubblica il contenitore.

Il tag inizializza il widget una sola volta per pagina, anche quando il trigger viene eseguito più volte.

## Configurazione

Il template supporta tutti i parametri correnti di `acsw.init()`:

- License Key;
- colore principale;
- posizione, offset e unità di misura;
- dimensione, forma e raggio dell'icona;
- link alla Dichiarazione di accessibilità;
- trigger CSS e scorciatoia da tastiera;
- possibilità di nascondere il bottone standard;
- personalizzazioni White Label disponibili con il piano Widget Large.

La validità della licenza, il dominio autorizzato e le funzionalità disponibili per il piano vengono verificati dal Widget AccessiWeb.

## Sicurezza e privacy

Il template richiede esclusivamente i permessi GTM necessari per:

- caricare `https://www.accessiweb.it/widget/acsw.js`;
- eseguire `acsw.init` con la configurazione inserita;
- impedire inizializzazioni duplicate nella stessa pagina;
- scrivere messaggi diagnostici solamente in modalità debug/anteprima.

La License Key viene passata direttamente a `acsw.init()` e non viene inserita nell'URL dello script.

## Link utili

- [AccessiWeb](https://www.accessiweb.it)
- [Configurazione e installazione del Widget](https://www.accessiweb.it/app/impostazioni-widget)
- [Guida Google Tag Manager](https://www.accessiweb.it/tagmanager)

## Licenza

Apache License 2.0.
