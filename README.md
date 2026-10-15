<p align="center"><img src="assets/glass-bosa-logo.svg" alt="GLASS Bosa" width="300"></p>

<p align="center"><a href="#glass-bosa">Italiano</a> · <a href="#glass-bosa-1">English</a></p>

# GLASS Bosa

*Trasformare le bottiglie vuote di una città in qualcosa di fatto a Bosa*

## Di cosa si tratta

Bosa è una piccola città sulla costa occidentale della Sardegna. Per un secolo è stata la capitale italiana della concia. Oggi non produce quasi niente, e l'unica cosa che ogni giorno esce dalla valle, a camion pieni, sono i suoi rifiuti.

Il vetro è una parte importante di quei rifiuti. Nel 2024 Bosa ne ha raccolto **596 tonnellate**, circa **81 kg per ogni residente**, ben più di un milione di bottiglie. Viene soprattutto da bar, ristoranti e case vacanza. Tutto viene portato via in camion, e mandarlo via è un costo che la città paga: circa **0,21 € per ogni chilo**, intorno ai **17 € l'anno** per la quota di ogni residente.

GLASS Bosa parte da un'idea semplice: quelle bottiglie non sono rifiuti, sono una materia prima, consegnata gratis, ogni giorno, alla porta della città.

## Cosa produciamo

Le bottiglie vengono ritirate direttamente dai bar prima che siano buttate, lavate, frantumate e fuse in un piccolo forno alimentato dal sole. Diventano due oggetti:

- **La B** (Bosana): una mezza oliva di vetro verde, da 10 grammi. Prende il nome dall'oliva più diffusa in Sardegna e ha un piccolo foro, così si può indossare.
- **Il BAR**: un lingotto di vetro marrone da 1 chilo esatto, a forma di lingotto d'oro.

Cento B pesano quanto un BAR.

Ogni pezzo viene pesato, numerato e iscritto in un registro pubblico. Chiunque può fondere una bottiglia; solo i pezzi registrati sono *Made in Bosa*.

## Come si vendono

I primi dieci BAR e le prime cento B, l'*Edizione 0*, saranno venduti all'asta in una galleria ospitata in uno dei vecchi edifici delle concerie di Sas Conzas, il luogo dove Bosa ha prodotto qualcosa per l'ultima volta. Dopo, i pezzi si producono solo quando qualcuno li ha ordinati, e chi li possiede può scambiarli con altri sul **Glass Exchange**, un mercato ospitato nei bar e nei caffè della città.

Nessuno sa ancora quanto valgono una B o un BAR, quindi il prezzo non si indovina: si scopre. I pezzi non si vendono mai sotto quello che costa farli, e si vendono come oggetti da collezione, non come investimenti. Non sono una moneta e non promettono niente. Ognuno è semplicemente un pezzo certificato del vetro di Bosa, di cui si conoscono l'origine, il peso, l'energia e il lavoro.

## Tutto alla luce del sole

Un [dashboard pubblico](https://blankworker1.github.io/GLASS/dashboard/) mostra i numeri del progetto, senza giudizi: quanto costa il vetro alla città, quanto vetro produce Bosa, quanto può produrre un forno, cosa è stato prodotto e venduto, a quali prezzi, e quanta energia è venuta dal sole.

La maggior parte di questi numeri è piccola. Un forno può trasformare al massimo circa lo 0,1% del vetro di Bosa in B e BAR. GLASS Bosa non pretende di risolvere i rifiuti della città. Rende visibile il problema, e dimostra che la città può tornare a produrre qualcosa da ciò che oggi butta via.

## Da dove nasce

GLASS Bosa è il primo esempio concreto di un'idea più ampia per la città: una produzione piccola, pulita e di proprietà locale, gestita come cooperativa, fatta solo su ordini reali, senza contributi pubblici, e misurata da quanto resiste alle difficoltà più che da quanto cresce. I testi di questo archivio spiegano quell'idea passo per passo.

## I testi

Da leggere in ordine: ognuno si basa su quello precedente.

| # | Testo | Di cosa parla |
| --- | --- | --- |
| 1 | [Una città non può vivere di rifiuti](docs/it/01-una-citta-non-puo-vivere-di-rifiuti.md) | L'appello: perché Bosa deve tornare a produrre |
| 2 | [Un modello di produzione per Bosa](docs/it/02-un-modello-di-produzione-per-bosa.md) | Come deve funzionare la produzione: una cooperativa, prima la domanda, misurata dalla resilienza, e le sei prove che ogni prodotto deve superare |
| 3 | [Made in Bosa • Un'officina diffusa](docs/it/03-made-in-bosa-officina-diffusa.md) | Dove: piccoli laboratori sparsi per la città riuniti in un'unica impresa, il punto centrale, il marchio collettivo *Made in Bosa* e un censimento di ciò che Bosa ha già |
| 4 | [GLASS Bosa](docs/it/04-glass-bosa.md) | L'esempio concreto: il materiale, il prodotto, il processo, l'Edizione 0, le fasi di produzione e il Glass Exchange |
| 5 | [Il dashboard](docs/en/05-dashboard.md) | Cosa mostra il cruscotto pubblico, da dove viene ogni numero e come si calcola (per ora solo in inglese) |

## Il cruscotto

**[blankworker1.github.io/GLASS/dashboard](https://blankworker1.github.io/GLASS/dashboard/)**

Si apre in italiano; il pulsante IT / EN in alto a destra passa all'inglese. La pagina è [`dashboard/index.html`](dashboard/index.html), pubblicata con GitHub Pages. Legge i file CSV in `data/` ogni volta che si apre: per aggiornarla basta modificare un CSV. Una nuova riga in `bosa-register.csv`, `bosa-firings.csv` o `bosa-prices.csv` compare subito sulla pagina.

## I dati

Il cruscotto legge solo i file in [`data/`](data/). Nella pagina non si scrive nessun numero a mano.

| File | Contenuto |
| --- | --- |
| `bosa-glass-ispra.csv` | Vetro raccolto a Bosa ogni anno, con la popolazione, 2015–2024 (ISPRA) |
| `bosa-costs-ispra.csv` | Costi dei rifiuti di Bosa per voce, 2019–2024 (ISPRA) |
| `bosa-kiln.csv` | Capacità e impianto solare del primo forno (dati di progetto) |
| `bosa-units.csv` | La B e il BAR: peso, rapporto e prezzo minimo |
| `bosa-register.csv` | Una riga per pezzo prodotto: numero di serie, unità, peso, provenienza del vetro, data di fusione, posizione della rondella, data di vendita |
| `bosa-firings.csv` | Una riga per cottura, con l'energia misurata dal sole e dalla rete |
| `bosa-prices.csv` | Una riga per vendita o scambio: prima l'Edizione 0, poi il Glass Exchange |
| `bosa-assumptions.csv` | Stime di progetto, da sostituire con i dati misurati |

I file del registro, delle cotture e dei prezzi restano vuoti finché l'Edizione 0 non è prodotta e venduta.

## A che punto siamo

Prima dell'Edizione 0. Il disegno della B e del BAR è definito, sono stati individuati due laboratori sardi del vetro per il primo lotto, e la sede dell'asta è scelta. Prossimi passi: una cottura di prova, i primi dieci BAR e le prime cento B, e l'asta.

Ancora da scrivere: posizionamento e campagne pubbliche, le misure di resilienza, i dati del Comune e il governo della cooperativa.

## Partecipare

Le correzioni ai numeri sono benvenute: citate la fonte. Le proposte su cosa Bosa potrebbe produrre dopo passano per le sei prove di *Un modello di produzione per Bosa*.

---

# GLASS Bosa

*Turning a town's empty bottles into something made in Bosa*

## What this is about

Bosa is a small town on the west coast of Sardinia. For a century it was the tanning capital of Italy. Today it makes almost nothing, and the one thing that leaves the valley every day, by the lorry load, is its rubbish.

Glass is a large part of that rubbish. In 2024 Bosa collected **596 tonnes** of it, about **81 kg for every resident**, or well over a million bottles. Most of it comes from bars, restaurants and holiday lets. All of it is trucked away, and sending it away is a cost the town pays: about **€0.21 for every kilo**, around **€17 a year** for each resident's share.

GLASS Bosa starts from a simple idea: those bottles are not rubbish, they are a raw material, delivered free, every day, to the town's own doorstep.

## What we make

Bottles are collected directly from bars before they are thrown away, washed, crushed and cast in a small kiln powered by the sun. They become two objects:

- **The B** (Bosana): a half olive in green glass, weighing 10 grams. It is named after Sardinia's most common olive, and it has a fine hole so it can be worn.
- **The BAR**: an ingot of brown glass weighing exactly 1 kilo, in the shape of a gold bar.

One hundred B weigh the same as one BAR.

Every piece is weighed, given a serial number and entered in a public register. Anyone can melt a bottle; only registered pieces are *Made in Bosa*.

## How they are sold

The first ten BAR and one hundred B, *Edition 0*, will be sold at auction in a gallery in one of the old tannery buildings of Sas Conzas, the place where Bosa last produced something. After that, pieces are made only when someone has ordered them, and holders can trade them with each other on the **Glass Exchange**, a market hosted in bars and cafés around town.

Nobody knows yet what a B or a BAR is worth, so the price is not guessed: it is discovered. Pieces are never sold below what they cost to make, and they are sold as collectibles, not investments. They are not a currency and they promise nothing. Each one is simply a certified piece of Bosa's glass, with a known origin, weight, energy and work.

## Everything in the open

A [public dashboard](https://blankworker1.github.io/GLASS/dashboard/?lang=en) shows the numbers behind the project, without judgement: what glass costs the town, how much glass Bosa produces, how much one kiln can make, what has been made and sold, at what prices, and how much of the energy came from the sun.

Most of these numbers are small. One kiln can turn at most about 0.1% of Bosa's glass into B and BAR. GLASS Bosa does not claim to solve the town's waste. It makes the problem visible, and shows that the town can make something again from what it currently throws away.

## Where it comes from

GLASS Bosa is the first worked example of a wider idea for the town: production that is small, clean and locally owned, run as a cooperative, made only against real orders, funded without grants, and measured by how well it withstands shocks rather than how fast it grows. The texts in this repository set out that idea step by step.

## The documents

Read them in order. Each one builds on the one before.

| # | Document | What it covers |
| --- | --- | --- |
| 1 | [A Town Cannot Live on Rubbish](docs/en/01-a-town-cannot-live-on-rubbish.md) | The call: why Bosa needs to produce again |
| 2 | [A Production Model for Bosa](docs/en/02-a-production-model-for-bosa.md) | How production should operate: a cooperative, demand first, measured by resilience, and the six tests every product must pass |
| 3 | [Made in Bosa • Un'officina diffusa](docs/en/03-made-in-bosa-officina-diffusa.md) | Where: small workshops across town joined into one enterprise, the hub, the *Made in Bosa* collective trademark, and a census of what Bosa already has |
| 4 | [GLASS Bosa](docs/en/04-glass-bosa.md) | The worked example: the material, the product, the process, Edition 0, the production stages and the Glass Exchange |
| 5 | [The dashboard](docs/en/05-dashboard.md) | What the public dashboard shows, where every number comes from and how it is worked out |

## The dashboard

**[blankworker1.github.io/GLASS/dashboard](https://blankworker1.github.io/GLASS/dashboard/?lang=en)**

It opens in Italian; the IT / EN switch at the top right changes to English, and the `?lang=en` link opens it in English directly. The page is [`dashboard/index.html`](dashboard/index.html), served by GitHub Pages. It reads the CSV files in `data/` each time it opens, so updating the dashboard means editing a CSV and committing it: a new row in `bosa-register.csv`, `bosa-firings.csv` or `bosa-prices.csv` appears on the page straight away.

## The data

The dashboard reads only from the files in [`data/`](data/). Nothing is typed into the page.

| File | Contents |
| --- | --- |
| `bosa-glass-ispra.csv` | Glass collected in Bosa per year, with population, 2015–2024 (ISPRA) |
| `bosa-costs-ispra.csv` | Bosa's waste costs by heading, 2019–2024 (ISPRA) |
| `bosa-kiln.csv` | Capacity and solar supply of the first kiln (planning figures) |
| `bosa-units.csv` | The B and the BAR: weight, relation and floor price |
| `bosa-register.csv` | One row per piece made: serial, unit, weight, glass source, date cast, rove position, date sold |
| `bosa-firings.csv` | One row per kiln firing, with metered energy from solar and from the grid |
| `bosa-prices.csv` | One row per sale or trade: Edition 0 first, then the Glass Exchange |
| `bosa-assumptions.csv` | Planning estimates still to be replaced by measured figures |

The register, firings and prices files are empty until Edition 0 is made and sold.

## Status

Pre-Edition 0. The design of the B and the BAR is settled, two Sardinian glass studios have been identified for the first batch, and the auction venue is chosen. Next: a test firing, the first ten BAR and one hundred B, and the auction.

Still to be written: positioning and public campaigns, the resilience measures, figures from the Comune, and governance of the cooperative.

## Contributing

Corrections to figures are welcome: please cite the source. Proposals for what Bosa could make next should go through the six tests in *A Production Model for Bosa*.
