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

A [public dashboard](https://blankworker1.github.io/GLASS/dashboard/) shows the numbers behind the project, without judgement: what glass costs the town, how much glass Bosa produces, how much one kiln can make, what has been made and sold, at what prices, and how much of the energy came from the sun.

Most of these numbers are small. One kiln can turn at most about 0.1% of Bosa's glass into B and BAR. GLASS Bosa does not claim to solve the town's waste. It makes the problem visible, and shows that the town can make something again from what it currently throws away.

## Where it comes from

GLASS Bosa is the first worked example of a wider idea for the town: production that is small, clean and locally owned, run as a cooperative, made only against real orders, funded without grants, and measured by how well it withstands shocks rather than how fast it grows. The texts in this repository set out that idea step by step.

---

## The documents

Read them in order. Each one builds on the one before.

| # | Document | What it covers |
| --- | --- | --- |
| 1 | [A Town Cannot Live on Rubbish](docs/en/01-a-town-cannot-live-on-rubbish.md) | The call: why Bosa needs to produce again |
| 2 | [A Production Model for Bosa](docs/en/02-a-production-model-for-bosa.md) | How production should operate: a cooperative, demand first, measured by resilience, and the six tests every product must pass |
| 3 | [Made in Bosa • Un'officina diffusa](docs/en/03-made-in-bosa-officina-diffusa.md) | Where: small workshops across town joined into one enterprise, the hub, the *Made in Bosa* collective trademark, and a census of what Bosa already has |
| 4 | [GLASS Bosa](docs/en/04-glass-bosa.md) | The worked example: the material, the product, the process, Edition 0, the production stages and the Glass Exchange |
| 5 | [The dashboard](docs/en/05-dashboard.md) | What the public dashboard shows, where every number comes from and how it is worked out |

Italian versions of the first four texts are in [`docs/it/`](docs/it/). The dashboard description is in English only for now.

## The dashboard

**[blankworker1.github.io/GLASS/dashboard](https://blankworker1.github.io/GLASS/dashboard/)**

The page is [`dashboard/index.html`](dashboard/index.html), served by GitHub Pages. It reads the CSV files in `data/` each time it opens, so updating the dashboard means editing a CSV and committing it: a new row in `bosa-register.csv`, `bosa-firings.csv` or `bosa-prices.csv` appears on the page straight away. [`docs/05-dashboard.md`](docs/en/05-dashboard.md) explains how every figure is worked out.

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
