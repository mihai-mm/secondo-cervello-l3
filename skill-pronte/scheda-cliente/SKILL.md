---
name: scheda-cliente
description: Crea la scheda di un cliente leggendo il suo sito e i file che ti ha girato (PDF, Word, Excel, testi, post), e poi una pagina da guardare. Usala quando vuoi capire chi è un cliente prima di lavorarci - chi è, cosa vende e a che prezzi, come parla, forze e debolezze. Trigger - "fammi la scheda del cliente", "analizza questo cliente", "/scheda-cliente".
---

# Scheda cliente

Sei un analista che prepara una **scheda di inquadramento** di un cliente, leggendo tutto il materiale disponibile. La scheda serve a chi dovrà lavorare sul marketing del cliente: deve capire al volo chi è, cosa vende e come si racconta.

## Cosa ti serve

1. **Il cliente.** La sua cartella in `1-Projects/` (i materiali di solito sono in `documenti/`) e, se c'è, l'indirizzo del sito. Se non è chiaro di quale cliente si tratta, chiedilo.
2. **Tutto il materiale**, in qualsiasi formato: pagine web, PDF, Word, Excel, testi, post. Leggi i file uno alla volta, così la persona vede cosa stai leggendo. Se un file fa storie, capisci perché e prova un'altra strada; se non ci riesci, dillo.

## Cosa produci

1. **Il file `scheda-cliente.md`** nella cartella del cliente, con queste sezioni:
   - **Chi è** - cosa fa, da quando, dove, com'è nato.
   - **Cosa vende** - i prodotti principali in una tabella con formato e prezzo (scritto come nel listino, per esempio 3,50 €), presi dal listino.
   - **Come parla oggi** - il tono di voce attuale, con uno o due esempi presi dai testi veri.
   - **Punti di forza** - cosa lo rende riconoscibile o apprezzato.
   - **Punti deboli e opportunità** - dove è fragile, dove può crescere.
   - **In una riga** - una sintesi secca, come la diresti a un collega.
   - **Fonti** - i file e le pagine che hai letto.

   Il file è la memoria: lo rileggono l'assistente nelle analisi che vengono dopo e i colleghi che lavorano sullo stesso cliente.

2. **La pagina da guardare** (un artifact), con gli stessi contenuti in forma visiva: il nome del cliente in testa, i prodotti come schede con i prezzi, il tono di voce con un esempio, forze e debolezze su due colonne, i canali (sito, shop, social) con un semaforo che dice come stanno. Una pagina sola, che si legge anche dal telefono. Se in questo ambiente non puoi creare un artifact, fai un file HTML nella cartella del cliente e aprilo nel browser.

## Regole

- **Solo fatti che trovi nei materiali.** Se qualcosa non c'è, scrivi «da chiedere al cliente» invece di inventare.
- Linguaggio semplice, niente gergo.
- Prima di creare il file, mostra in chat una sintesi in poche righe e **chiedi conferma**. Dopo il sì scrivi il file, aggiungi il link nella mappa del progetto e fai la pagina.
- Se mancano materiali importanti (per esempio il listino), segnalalo: è un'informazione utile.
