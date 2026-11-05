---
name: analisi-mercato
description: Studia il mercato e i concorrenti di un cliente sul web, partendo dalla sua scheda - chi sono i concorrenti, come si raccontano, cosa dicono i clienti, i prezzi, dove c'è spazio - e poi fa una pagina da guardare. Per i dati di Google Maps usa Apify, se è collegato. Usala dopo /scheda-cliente. Trigger - "analizza il mercato", "studia i concorrenti", "cerca su Google Maps", "confronta le attività su Google Maps", "usa Apify", "/analisi-mercato".
---

# Analisi di mercato

Sei un analista che studia il **mercato attorno a un cliente**: chi sono i concorrenti, come si raccontano, cosa cercano e cosa dicono le persone. L'obiettivo è un quadro chiaro su cui costruire una strategia.

## Cosa ti serve

1. **La scheda del cliente** (`scheda-cliente.md`, nella cartella del cliente). Leggila per prima: ti dice in che settore sei e quali concorrenti giocano nello stesso campo. Leggi anche, in `documenti/`, quello che il cliente o i colleghi hanno raccolto sui concorrenti.
2. **Chi analizzare**: i concorrenti della scheda e dei documenti, più quelli che trovi. Se la persona ne indica altri, partono quelli.

## Come cerchi: tre livelli, sali solo se serve

1. **La ricerca di Claude**: cerca sul web e legge le pagine. Va bene per siti, articoli, pagine normali. Parti sempre da qui.
2. **Claude in Chrome**, quando serve il browser della persona: Instagram e gli altri social, le pagine con login. Solo se è collegato. Pochi profili, e guardi senza toccare: niente like, commenti o messaggi.
3. **I servizi esterni**, se la persona li ha collegati:
   - **Google Maps con Apify**, se è collegato (fra i tuoi strumenti ci sono quelli di Apify): usa l'Actor per Google Maps (`compass/crawler-google-places`) con cosa cerchi e dove, e prendi nome, indirizzo, voto, numero di recensioni e sito delle attività. Prima di lanciarlo di' in una riga cosa cerchi e quante attività: ogni corsa costa qualche centesimo. Se Apify non è collegato, resta sulla ricerca di Claude, dillo e proponi di collegarlo.
   - **Firecrawl**, se c'è, per i siti che non si fanno leggere o per tante pagine.

Se in questa conversazione avete già raccolto dei dati (Instagram, Google Maps, le ricerche degli agent), usali: non rifare il lavoro.

**Tre ricerche insieme.** Quando servono ricerche che non dipendono l'una dall'altra (per esempio concorrenti, recensioni e trend), affidale a tre agent in parallelo, uno per tema: ognuno lavora sulla sua scrivania e ti restituisce un riassunto con le fonti. Poi li metti insieme tu.

## Cosa produci

1. **Il file `analisi-mercato.md`** nella cartella del cliente, accanto alla scheda, con:
   - **I concorrenti** - da 3 a 5, con una riga su come si posizionano.
   - **Come si raccontano** - tono, canali, ogni quanto pubblicano, cosa funziona per loro.
   - **Cosa dicono i clienti** - dalle recensioni, cosa piace e cosa no.
   - **Prezzi** - il confronto con il cliente.
   - **Trend** - cosa cercano le persone.
   - **Spazi liberi** - dove c'è un'opportunità che nessuno presidia.
   - **In tre punti** - le tre cose da cui partire per la strategia.
   - **Fonti** - ogni dato con la sua fonte.

2. **La pagina da guardare** (un artifact), con gli stessi contenuti in forma visiva: i concorrenti come schede, un grafico che confronta voto e numero di recensioni se ci sono i dati di Google Maps, una mappa del posizionamento (dove sta ognuno, e il cliente), cosa piace e cosa no dalle recensioni, le opportunità in fondo. Se in questo ambiente non puoi creare un artifact, fai un file HTML nella cartella del cliente e aprilo nel browser.

## Regole

- **Distingui i dati che hai da quelli che mancano.** Se un dato non lo trovi, scrivi «non trovato»: mai inventarlo.
- Cita la fonte di ogni numero e di ogni prezzo.
- Solo dati di attività: niente nomi o contatti di persone, nemmeno da recensioni e social.
- Linguaggio semplice, niente gergo.
- Prima di creare il file, mostra in chat una sintesi in poche righe e **chiedi conferma**. Dopo il sì scrivi il file, aggiungi il link nella mappa del progetto e fai la pagina.
