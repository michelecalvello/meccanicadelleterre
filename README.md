# Meccanica delle terre · Cheat Sheet Geotecnico

Gioco didattico a indizi annidati sugli argomenti di meccanica delle terre, ispirato a *Cheat Sheet* di TED Games.

Pagina del gioco: https://michelecalvello.github.io/meccanicadelleterre/cheatsheet.html

## Contenuto del repository

| Percorso | Descrizione |
|---|---|
| `cheatsheet.html` | Il gioco: una sola pagina HTML, senza dipendenze da installare |
| `fogli/modello-sondaggio.xlsx` | Modello vuoto per scrivere un nuovo sondaggio |
| `fogli/sondaggio-L1-base-tensioni-efficaci.xlsx` | Sondaggio del livello 1 (Base) |
| `fogli/sondaggio-L2-intermedio-compressibilita.xlsx` | Sondaggio del livello 2 (Intermedio) |
| `fogli/sondaggio-L3-avanzato-liquefazione.xlsx` | Sondaggio del livello 3 (Avanzato) |

## Regole del gioco

- Si parte da 100 punti.
- La domanda principale ha 3 parole-indizio e 9 parole oscurate.
- Ogni indizio apre una domanda di strato 1, con 2 indizi che portano a domande di strato 2 (10 domande in tutto).
- Negli strati 1 e 2: risposta errata −2 punti; "Rivela" −5 punti e nessun bonus; risposta esatta +1 bonus.
- Un bonus svela una parola oscurata della domanda principale, al costo di 2 punti.
- Domanda principale: 3 tentativi; i primi due errori costano 5 punti ciascuno, il terzo chiude il sondaggio con 0 punti.

## Aggiungere un sondaggio

1. Compila una copia di `fogli/modello-sondaggio.xlsx` (un file = un sondaggio da 10 righe; istruzioni nel foglio "Istruzioni").
   Nella colonna `domanda` scrivi gli indizi come `{{parola}}` e, solo nella riga P, le 9 parole oscurate come `[[parola]]`.
2. Apri `cheatsheet.html` (la pagina pubblicata o il file in locale), apri **Aggiungi sondaggi** e carica il file: la pagina segnala eventuali errori riga per riga.
3. Premi **Aggiungi a questo file**, poi **Scarica pagina aggiornata**: ottieni un nuovo `cheatsheet.html` con tutti i sondaggi.
4. Sostituisci `cheatsheet.html` nel repository con il file scaricato (e, se vuoi, aggiungi il foglio in `fogli/`).

I sondaggi aggiunti senza ricaricare il file nel repository restano visibili solo nel browser in cui sono stati caricati.

## Pubblicazione su GitHub Pages

Settings → Pages → Build and deployment → Source: *Deploy from a branch* → Branch: `main`, cartella `/ (root)`.
