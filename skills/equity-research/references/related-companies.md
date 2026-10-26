# Related companies: mapping, evidence and read-across

Contents:
1. Relation types
2. How to find related companies
3. Evidence standards
4. Read-across: what to check in each related company
5. Second-order effect playbook
6. Theme discovery procedure
7. Pitfalls

---

## 1. Relation types

Always label each related company with one (or more) of these types and
direction. Never present a list of "related stocks" without the type.

| Type | Meaning | Example evidence |
|---|---|---|
| `competitor` | Sells similar products to similar customers | Company's own competitor list, market share reports, overlapping segment |
| `customer` | Buys from the target | Disclosed major customers (有報「主要な販売先」, 10-K customer concentration), supplier lists, press releases |
| `supplier` | Sells to the target | Customer's supplier lists, components teardown, contracts, press releases |
| `parent` / `subsidiary` / `affiliate` | Ownership link | Filings (関係会社の状況, Exhibit 21), large-holder reports |
| `partner` / `JV` | Joint development, licensing, distribution | Press releases, contracts (8-K 1.01) |
| `substitute` | Different technology solving the same need | Industry analysis |
| `complement` | Demand moves together (e.g. GPUs and HBM) | Industry structure |
| `same-theme (unverified)` | Mentioned with the same theme in media/lists, exposure not yet verified | Media lists — must be verified before treating as exposure |
| `price-correlated` | Prices move together statistically | Price data only — not evidence of a business link |

Record direction (A supplies B), the evidence (document, section, date), and
whether the link is current (customer lists change).

## 2. How to find related companies

- **Company's own disclosures:** competitors named in the 10-K "Competition"
  section or 有報「事業の内容」; major customers (有報 主要な販売先 — customers
  ≥10% of sales; US 10-K customer concentration); subsidiaries and affiliates
  (関係会社, Exhibit 21).
- **The other side's disclosures:** a big customer's supplier list or
  sustainability/procurement report; a supplier's mention of key customers.
- **Earnings calls and presentations:** management often names customers,
  competitors and demand drivers in Q&A.
- **Industry structure:** map the value chain upstream (materials,
  components, equipment) and downstream (integrators, distributors, end
  users).
- **Index and ETF constituents** in the sector — useful for peers, not proof
  of exposure.
- **Cross-border peers:** the true competitors of many Japanese companies are
  in the US, Europe, Korea, Taiwan or China, and vice versa.

## 3. Evidence standards

- **Verified:** stated in a filing, official release, contract, or by the
  counterparty. Cite it with date.
- **Reported:** credible media/industry report; name the source and date.
- **Inferred:** logical but unconfirmed (same industry, plausible supplier).
  Label as a hypothesis and put verification into "Next investigations".
- Do not fill undisclosed customer names from memory or rumor. Record "major
  customer undisclosed (≈X% of sales)" as a concentration risk instead.
- Revenue exposure matters: a supplier for which the customer is 40% of sales
  is affected very differently from one at 2%.

## 4. Read-across: what to check in each related company

For each important related company, check the latest:

- Results and guidance (direction of demand, pricing, inventory)
- Capex plans (for suppliers of equipment/materials)
- Inventory levels and commentary (destocking/restocking)
- Order intake / backlog / book-to-bill
- Pricing and margin commentary
- Management comments about the target or its segment
- Price reaction to their results (what the market concluded)

Then state the implication for the target: supports / contradicts / neutral,
with the reason.

## 5. Second-order effect playbook

| Event at A | Check |
|---|---|
| A raises capex | Equipment and materials suppliers; A's competitors' response |
| A cuts capex or orders | Suppliers with high exposure to A; their order backlog and other customers |
| A loses share | Who gains (competitors); who supplies the winners |
| A raises prices | Competitors' pricing power; customers' margins |
| A is acquired / TOB | Peers that could be next (sector consolidation), A's suppliers/customers, the acquirer's financing and listed affiliates |
| A has a supply disruption (fire, sanctions, export controls) | Alternative suppliers, customers that lose output |
| A's regulator acts (antitrust, drug approval, tariff) | Peers under the same regulation |
| Commodity / FX / rate move | Companies with the largest disclosed sensitivity, both winners and losers |
| Parent sells a stake in listed subsidiary | The subsidiary's supply/demand overhang; other listed subsidiaries of the same parent |

## 6. Theme discovery procedure

1. Define the theme precisely (e.g. "data-center power" = power equipment,
   transformers, switchgear, UPS, generation, cooling, cables, grid).
2. Map the value chain into layers and list candidate companies per layer in
   both Japan and the US (and key overseas players for context).
3. For each candidate, look for **evidence of exposure**: segment revenue,
   orders, capacity expansions, named customers, management statements with
   numbers.
4. Classify: core (material, verified exposure) / meaningful / marginal /
   unverified-association.
5. Check what's priced in: valuation and price performance vs exposure. Theme
   stocks often move together regardless of exposure.
6. Identify potential **losers** of the theme (substitutes, cost-squeezed
   customers).
7. Note the theme's key risks and the data that would confirm or refute it
   (industry statistics, hyperscaler capex, orders).

## 7. Pitfalls

- Treating media "関連銘柄" lists as evidence of exposure.
- Treating price correlation as a business relationship.
- Ignoring exposure size (a link that is 1% of revenue rarely matters).
- Using stale customer lists.
- Stopping at first-order peers and missing the upstream/downstream layer
  where the real bottleneck or surprise is.
- Not checking whether the related company's latest results already told the
  market what the target will report.
