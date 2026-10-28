# Gioco a indizi · Meccanica delle terre

Gioco didattico a indizi annidati sugli argomenti di meccanica delle terre, ispirato a *Cheat Sheet* di TED Games.

Pagina del gioco: https://michelecalvello.github.io/meccanicadelleterre/cheatsheet.html

## Contenuto del repository

| Percorso | Descrizione |
|---|---|
| `cheatsheet.html` | Il gioco: una sola pagina HTML, senza dipendenze da installare |
| `fogli/modello-sondaggio.xlsx` | Modello vuoto per scrivere un nuovo sondaggio |
| `fogli/sondaggio-per-iniziare-terreni-saturi.xlsx` | "Terreni saturi" (Per iniziare) |
| `fogli/sondaggio-per-iniziare-compressibilita.xlsx` | "Compressibilità" (Per iniziare) |
| `fogli/sondaggio-per-iniziare-azioni-sismiche.xlsx` | "Azioni sismiche" (Per iniziare) |
| `fogli/sondaggio-identificazione-e-classificazione-dimensione-dei-grani.xlsx` | "Dimensione dei grani" (Identificazione e classificazione) |
| `fogli/sondaggio-identificazione-e-classificazione-consistenza.xlsx` | "Consistenza" (Identificazione e classificazione) |
| `fogli/sondaggio-identificazione-e-classificazione-stato-delle-sabbie.xlsx` | "Stato delle sabbie" (Identificazione e classificazione) |
| `fogli/sondaggio-tensioni-e-deformazioni-stato-di-sforzo.xlsx` | "Stato di sforzo" (Tensioni e deformazioni) |
| `fogli/sondaggio-tensioni-e-deformazioni-acqua-nei-pori.xlsx` | "Acqua nei pori" (Tensioni e deformazioni) |
| `fogli/sondaggio-tensioni-e-deformazioni-spinte-orizzontali.xlsx` | "Spinte orizzontali" (Tensioni e deformazioni) |
| `fogli/sondaggio-filtrazione-e-consolidazione-moto-nei-pori.xlsx` | "Moto nei pori" (Filtrazione e consolidazione) |
| `fogli/sondaggio-filtrazione-e-consolidazione-scavi-sotto-falda.xlsx` | "Scavi sotto falda" (Filtrazione e consolidazione) |
| `fogli/sondaggio-filtrazione-e-consolidazione-argilla-sotto-carico.xlsx` | "Argilla sotto carico" (Filtrazione e consolidazione) |
| `fogli/sondaggio-comportamento-meccanico-tensioni-orizzontali.xlsx` | "Tensioni orizzontali" (Comportamento meccanico) |
| `fogli/sondaggio-comportamento-meccanico-grandi-spostamenti.xlsx` | "Grandi spostamenti" (Comportamento meccanico) |
| `fogli/sondaggio-comportamento-meccanico-post-picco.xlsx` | "Post-picco" (Comportamento meccanico) |
| `fogli/sondaggio-prove-di-laboratorio-storia-tensionale.xlsx` | "Storia tensionale" (Prove di laboratorio) |
| `fogli/sondaggio-prove-di-laboratorio-picco-e-residuo.xlsx` | "Picco e residuo" (Prove di laboratorio) |
| `fogli/sondaggio-prove-di-laboratorio-breve-termine.xlsx` | "Breve termine" (Prove di laboratorio) |

## Contenitori

I sondaggi sono raccolti in sei contenitori, scelti con la colonna `contenitore` del foglio:

1. Per iniziare
2. Identificazione e classificazione
3. Tensioni e deformazioni
4. Filtrazione e consolidazione
5. Comportamento meccanico
6. Prove di laboratorio

I contenitori ancora senza sondaggi compaiono nella pagina come "in preparazione".
Le partite dei contenitori 2–6 si basano soprattutto su Berardi R., *Fondamenti di geotecnica*, Città Studi Edizioni (cap. 1–2; cap. 3; cap. 4 e § 5.1–5.2; § 6.1–6.3; § 9.1–9.5), con alcune domande di cultura ingegneristica tratte da altre fonti, citate in ogni domanda.
I fogli preparati con il vecchio modello (colonna `livello` con 1 - Base, 2 - Intermedio, 3 - Avanzato) sono ancora accettati e finiscono in "Per iniziare".

## Regole del gioco

- Si parte da 100 punti.
- La domanda principale ha 3 parole-indizio e 9 parole oscurate.
- Ogni indizio apre una domanda di strato 1, con 2 indizi che portano a domande di strato 2 (10 domande in tutto).
- Negli strati 1 e 2: risposta errata −2 punti; "Rivela" −5 punti e nessun bonus; risposta esatta +1 bonus.
- Un bonus svela una parola oscurata della domanda principale, al costo di 1 punto.
- A fine partita si possono rivedere tutte le 10 domande con le risposte, le note e le fonti.
- Domanda principale: 3 tentativi; i primi due errori costano 5 punti ciascuno, il terzo chiude il sondaggio con 0 punti.

## Scaricare o aggiungere un sondaggio

Nella pagina del gioco, il pannello **Scarica o aggiungi sondaggi** permette di:

- scaricare il modello vuoto e il foglio di calcolo (.xlsx) di ogni sondaggio presente, per correggerlo o usarlo come esempio;
- caricare un foglio compilato: la pagina controlla le regole, segnala eventuali errori riga per riga e, se il foglio è valido, aggiunge il sondaggio **solo nel browser** in cui è stato caricato.

Per rendere un sondaggio visibile a tutti va aggiunto a `cheatsheet.html` nel repository, insieme al foglio in `fogli/`.

### Come compilare il foglio

Compila una copia di `fogli/modello-sondaggio.xlsx` (un file = un sondaggio da 10 righe; istruzioni nel foglio "Istruzioni"), scegliendo il contenitore dal menu a tendina.
Nella colonna `domanda` scrivi gli indizi come `{{parola}}` e, solo nella riga P, le 9 parole oscurate come `[[parola]]`.

## Pubblicazione su GitHub Pages

Settings → Pages → Build and deployment → Source: *Deploy from a branch* → Branch: `main`, cartella `/ (root)`.
