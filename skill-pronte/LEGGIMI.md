# Skill pronte

Qui trovi le due skill dell'Analista che hai visto con Paola. Funzionano così come sono, ma **la strada consigliata è installarle con la guida «Il tuo Analista al lavoro»**, quando una delle tue opportunità le chiede: Claude te le spiega, ti fa una o due domande e le adatta al tuo modo di lavorare prima di installarle.

Prima di installarle, nel `CLAUDE.md` del vault va aggiunta la sezione «Le pagine da guardare» (Passo 1 della guida): le skill finiscono con una pagina da guardare, e la sezione dice al tuo Claude come farla.

## Cosa c'è

- **`scheda-cliente/`**: chi è un cliente, dai suoi file e dal suo sito. Legge il materiale uno alla volta, ti mostra una sintesi, e con il tuo sì scrive `scheda-cliente.md` nella cartella del cliente e fa la pagina da guardare.
- **`analisi-mercato/`**: il mercato attorno a un cliente. Parte dalla sua scheda, quindi si usa **dopo** `/scheda-cliente`. Cerca concorrenti, recensioni e prezzi sul web; usa Claude in Chrome e Apify solo se li hai collegati. Con il tuo sì scrive `analisi-mercato.md` e fa la pagina.

## Come si installa

1. Apri il tuo vault e vai nella cartella `.claude/skills/`. Se non la vedi, è normale: le cartelle che iniziano con un punto sono nascoste. Nel Finder premi Cmd+Maiusc+punto per mostrarle.
2. Copia dentro la cartella della skill (tutta, con il file `SKILL.md` dentro). Il risultato deve essere, per esempio, `.claude/skills/scheda-cliente/SKILL.md`.
3. Apri una conversazione nuova nella cartella del vault e scrivi `/`: nel menu deve comparire la skill. Se non compare, scrivi `/reload-skills`.

Se preferisci, chiedilo a Claude: «installa la skill scheda-cliente da skill-pronte in .claude/skills/: spiegamela prima». Claude ti dice cosa scrive e dove, e aspetta il tuo sì. L'app può mostrarti una richiesta di permesso, perché `.claude/` è una cartella speciale: va consentita.

Nessuna skill manda messaggi a nessuno. Tutte ti chiedono prima di scrivere un file.
