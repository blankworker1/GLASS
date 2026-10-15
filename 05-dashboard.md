# GLASS Bosa: the dashboard

*The transparent part: what the public dashboard shows, where each number comes from, and how it is worked out*

---

The dashboard publishes the numbers behind GLASS Bosa without judgement. Most of them are small as a percentage of Bosa's glass, and that is the point of showing them: nothing is claimed that the figures do not support.

It has six sections, in this order.

## 1. What glass costs Bosa

Residents pay for waste through TARI. This section shows what that costs, and what each kilo cast in Bosa saves.

| Figure | How it is worked out |
| --- | --- |
| Diversion value per kg | Collection cost per kg of separated waste (CRD) + treatment cost per kg of separated waste (CTR), latest year |
| Each resident's glass, per year | Glass per resident per year × diversion value |
| All waste, per resident | Total waste cost per resident per year (CTOT) |
| Saved at full kiln capacity | Maximum BAR per year × 1 kg × diversion value |
| Saved so far | Glass cast × diversion value |
| Diversion value by year | The same figure for each year from 2019 (2022 is not published) |

In 2024 the diversion value was about **€0.21 per kg** (€0.14 collection + €0.07 treatment). Each resident's 81 kg of glass cost about **€17**; all waste cost **€263** per resident.

**Limits.** ISPRA's costs cover all separated waste together, not glass alone, and they are before any payment from the recycling consortia, which would lower them. CTR per kg is derived from the per-resident figures: CRD per kg × (CTR per resident ÷ CRD per resident), since both are spread over the same separated tonnage. Years before 2019 are left out because the figures jump between reporting methods.

## 2. The glass stream

| Figure | How it is worked out |
| --- | --- |
| Glass collected, latest year | ISPRA, separate collection |
| Per resident, every month | Year's glass ÷ residents ÷ 12 (about 6.8 kg in 2024) |
| Per resident, per year | Year's glass ÷ residents (about 81 kg in 2024) |
| Charts | Tonnes per year, and kg per resident per month, 2015–2024 |

The per-resident figure includes the glass visitors leave behind.

## 3. One local production kiln

| Figure | How it is worked out |
| --- | --- |
| Per firing | 15 BAR, or about 12 BAR + 40 B |
| Maximum per year | BAR per firing × firings per year (52, firing weekly) = about 780 BAR |
| Share of the stream at full capacity | Maximum kg per year ÷ latest year's glass (about 0.13%) |

These are planning figures for the Stage 1 kiln, to be replaced by Edition 0's measured numbers.

## 4. Made and sold

| Figure | How it is worked out |
| --- | --- |
| BAR made / sold | Count of BAR in the register; those with a date sold |
| B made / sold | Count of B in the register; those with a date sold |
| Glass cast | Sum of finished weights in the register |
| Glass stream diverted | Glass cast ÷ latest year's glass |

The register table lists every piece: serial, unit, weight, glass source, date cast, rove position (X, Y, optional) and date sold.

## 5. Prices

| Figure | How it is worked out |
| --- | --- |
| BAR / B, last price | Most recent trade of that unit |
| Range | Lowest and highest trade of that unit |
| Floor | €10 per BAR, €0.50 per B |
| Trades | Number of auction sales and Glass Exchange trades |
| Chart | Every trade by date, BAR and B on separate rows |

Prices are not part of the register. The first prices are Edition 0's hammer prices. When the Glass Exchange goes live, its trades feed this section directly.

## 6. Energy

| Figure | How it is worked out |
| --- | --- |
| Power supply | About 4–5 kWp of solar, 10–15 kWh battery, grid backup |
| Electricity from solar | Solar kWh ÷ total kWh, all firings |
| Firings fully on solar | Firings whose grid meter reads zero: the only ones called carbon free |
| Energy used | Total metered kWh, and kWh per kg of glass loaded |
| CO₂ avoided | Solar kWh × grid emission factor (0.25 kg CO₂ per kWh, to confirm against ISPRA) |
| Firings table | Each firing: date, kiln, glass loaded, total, solar and grid kWh |

"Carbon free" covers the electricity used, not the manufacture of the panels. Edition 0 is cast at an outside studio, so its electricity counts as grid unless that studio runs on solar.

## Data

Every figure comes from a file in `data/`. Nothing is typed into the page.

| File | Contents | Source |
| --- | --- | --- |
| `bosa-glass-ispra.csv` | Glass collected per year, and population, 2015–2024 | ISPRA Catasto Rifiuti |
| `bosa-costs-ispra.csv` | Waste costs per resident by heading, and CRD and total per kg, 2019–2024 | ISPRA Catasto Rifiuti |
| `bosa-kiln.csv` | BAR per firing, mixed load, firings per year, solar supply | Planning figures, this project |
| `bosa-units.csv` | B and BAR: weight, relation, floor price | This project |
| `bosa-register.csv` | One row per piece made | The cooperative |
| `bosa-firings.csv` | One row per firing, with metered kWh | The cooperative |
| `bosa-prices.csv` | One row per sale or trade | Auction, then the Glass Exchange |
| `bosa-assumptions.csv` | Planning estimates, including the grid CO₂ factor | This project |

## Still to come

- Bosa's own glass-only collection cost and consortium payment, to replace the all-separated-waste average.
- A live feed from the Glass Exchange for prices.
- The resilience measures of the production model.
