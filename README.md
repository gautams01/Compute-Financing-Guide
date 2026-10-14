# Compute Financing Guide

- [Financing tree](#financing-tree): sources of capital and credit enhancements for data centers and GPUs
- [Compute procurement](#compute-procurement): renting, colo, modular or building your own
- [Interactive models](#interactive-models): one model per procurement structure, plus a side-by-side comparison

---

# Financing tree

Click any item to expand it.

## Sources of capital
*Where the money comes from*

### Equity

<details><summary><b>Venture capital &amp; strategic equity</b></summary>

Equity from VCs, growth funds and strategic investors such as chip vendors and hyperscalers. The most expensive and dilutive capital, but it provides the equity cushion lenders require: venture debt and asset-backed loans are sized against it.

*Risk addressed: funding need*

</details>

<details><summary><b>Internal cash flow</b></summary>

Fund capex from operating cash flow. Hyperscalers fund most of their buildout this way. For a startup, margin from existing clusters funds the next one: no dilution or leverage, but slower growth.

*Risk addressed: funding need*

</details>

### GPU Debt

<details><summary><b>Vendor financing</b></summary>

Deferred payment terms (60–180 days) or 3–5yr loans and leases from OEM finance arms. Easiest debt to get: vendors lend on their sale margin and can recover and resell the gear. Limits: down payment or guarantee, cost may be buried in a smaller discount, first lien on the gear (needs venture-debt carve-out), vendor lock-in.

*Risk addressed: residual value*

</details>

<details><summary><b>Equipment leasing</b></summary>

- **Equipment lease:** A lessor owns the GPUs and leases them to you; operating lease or finance lease with a purchase option. Sale-leasebacks work the same way for GPUs you already own. Lessor retains residual risk.
- **Ring-fenced lease (SPV):** At scale, a special purpose vehicle raises equity and debt, buys the GPUs and leases them to the user (e.g. 5yr). Lenders’ claim is limited to the chips and lease payments, separate from the user’s other creditors. Outside investors, including chip vendors, can invest in the SPV equity.

*Risk addressed: residual value, user credit*

</details>

<details><summary><b>Venture debt</b></summary>

Term loans from venture lenders and bank tech desks, underwritten on equity backing rather than assets. Usually comes with warrants. Revenue-based financing is a variant for companies with recurring revenue.

- **Terms:** Sized at ~20–35% of the last equity round; 3–4yr, interest-only then amortizing; fees plus warrants; blanket lien and minimum-cash covenant.
- **Repaid from equity, not GPUs:** A cluster's cash flow typically covers only part of the debt service; the rest comes from the equity raise. A bridge until offtake contracts support GPU-backed debt.
- **Negotiate a carve-out:** The blanket lien blocks later GPU loans and leases unless future equipment financing is excluded.

*Risk addressed: funding need*

</details>

<details><summary><b>GPU-backed term loans</b></summary>

Secured by GPUs plus assigned offtake contract. Delayed draw tied to chip delivery; amortizes over the contract term.

- **Contract is the real collateral:** Offtaker consent to assignment, no early termination for convenience or SLA misses, tenor at least matching the loan.
- **Outpace depreciation:** Front-loaded amortization, LTV tests with cash sweep, small or insured balloon.
- **Enforcement:** Colo access agreement, backup operator, fire-sale risk if many lenders sell the same GPU model.
- **Pricing:** Offtaker credit spread plus operator execution premium; commitment fees on undrawn amounts.

*Risk addressed: offtaker credit, residual value*

</details>

<details><summary><b>Mezzanine &amp; preferred equity</b></summary>

Subordinated capital that fills the gap between senior debt (70–80% LTV) and sponsor equity. Can sit at the project, SPV or parent level; often PIK. Preferred equity ranks below all debt. Unlike corporate debt, available against a single project.

*Risk addressed: funding need*

</details>

<details><summary><b>Corporate debt</b></summary>

Senior debt at the parent, repaid from total company cash flow rather than one asset; can be unsecured or secured by all assets. Generally needs scale and operating history.

- **Forms:** IG bonds (hyperscalers), HY bonds, leveraged loans, converts (popular with volatile public stocks), revolvers.
- **Structural subordination:** Parent bondholders are paid only after asset-level SPV lenders, so they price wider even when both are “senior.”
- **Covenants:** HY baskets cap how much secured and SPV debt can be layered ahead of the bonds.

</details>

### Data Center Debt

<details><summary><b>Venture debt</b></summary>

Term loans from venture lenders and bank tech desks, underwritten on equity backing rather than assets. Usually comes with warrants. Revenue-based financing is a variant for companies with recurring revenue.

- **Terms:** Sized at ~20–35% of the last equity round; 3–4yr, interest-only then amortizing; fees plus warrants; blanket lien and minimum-cash covenant.
- **Repaid from equity, not GPUs:** A cluster's cash flow typically covers only part of the debt service; the rest comes from the equity raise. A bridge until offtake contracts support GPU-backed debt.
- **Negotiate a carve-out:** The blanket lien blocks later GPU loans and leases unless future equipment financing is excluded.

*Risk addressed: funding need*

</details>

<details><summary><b>Mezzanine &amp; preferred equity</b></summary>

Subordinated capital that fills the gap between senior debt (70–80% LTV) and sponsor equity. Can sit at the project, SPV or parent level; often PIK. Preferred equity ranks below all debt. Unlike corporate debt, available against a single project.

*Risk addressed: funding need*

</details>

<details><summary><b>Warehouse to ABS</b></summary>

Fill a revolving warehouse line (65–75% advance, floating, 2–3yr) with eligible contracts. Once the pool is large and seasoned, issue tranched ABS and use the proceeds to repay the warehouse, then refill it.

- **Why term out:** Lower blended cost from AAA–A senior notes; higher advance rate, so less equity per dollar of assets; fixed-rate, longer-dated debt that amortizes with the contracts; warehouse capacity recycled for new deals; access to insurers and ABS funds.
- **Why not GPUs yet:** Short chip life caps term and advance rate; little resale data to support residual value; pools concentrated in a few offtakers cap ratings. Could work as GPU contracts lengthen, price indices develop and offtakers diversify.

*Risk addressed: concentration, refinancing*

</details>

<details><summary><b>SPV project bonds</b></summary>

A sponsor puts one campus in a ring-fenced SPV, signs a long lease with a single tenant, and the SPV issues bonds to fund construction. Bondholders are repaid from the lease, secured by the land, building and assigned lease. Sponsor equity is the only credit support.

- **Investment grade:** IG hyperscaler tenant, 15–20yr triple-net lease. Fully amortizing, ~90–97% debt financed. Rating and spread track the tenant’s.
- **High yield:** Lower-rated or backstopped tenant. 5NC2, partial amortization, refi at year 5; typically ~80% debt financed.
- **Construction protections:** Fixed-price construction contract, completion guarantee from the sponsor, capitalized interest reserve until rent starts, delay damages from the contractor.
- **What to underwrite:** Tenant credit and concentration; lease termination rights, especially for late delivery; whether rent starts on delivery regardless of tenant fit-out; refi risk on HY bullets.
- **Who can use it:** Developers with a signed lease from a highly rated tenant. A startup is usually the tenant, not the issuer.

*Risk addressed: construction, tenant credit*

</details>

<details><summary><b>Corporate debt</b></summary>

Senior debt at the parent, repaid from total company cash flow rather than one asset; can be unsecured or secured by all assets. Generally needs scale and operating history.

- **Forms:** IG bonds (hyperscalers), HY bonds, leveraged loans, converts (popular with volatile public stocks), revolvers.
- **Structural subordination:** Parent bondholders are paid only after asset-level SPV lenders, so they price wider even when both are “senior.”
- **Covenants:** HY baskets cap how much secured and SPV debt can be layered ahead of the bonds.

</details>

<details><summary><b>ABS &amp; CMBS</b></summary>

Securitizations of stabilized, leased facilities; tranched by subordination.

- **ABS:** Master trust of multiple facilities, ~5yr ARD; new series added off the same pool. GPU-contract ABS is possible in future but not established.
- **CMBS:** Mortgage loan on a single asset or portfolio. Mostly floating with extension options; balloon at maturity.

*Risk addressed: concentration, re-leasing*

</details>

<details><summary><b>Building sale-leaseback</b></summary>

Sell the stabilized facility to a REIT or infra fund and lease it back; recycles capital into the next build.

</details>

### Tax & public incentives

<details><summary><b>Federal tax</b></summary>

Depreciation, R&D credit, loss rules, interest deductibility, energy credits.

</details>

<details><summary><b>State &amp; local</b></summary>

Sales tax exemptions on equipment and power; property tax abatements.

</details>

<details><summary><b>Investment &amp; public financing</b></summary>

Opportunity zones, export credit agencies, federal energy loans and sites.

</details>

See [Tax & public incentives detail](#tax--public-incentives-detail) below.

## Credit enhancements
*How a borrower becomes bankable*

### Debt structure

<details><summary><b>Sizing &amp; pricing</b></summary>

GPU loans at 70–80% LTV. Sized to at least 1.3x DSCR, tested assuming any backstop is triggered. Priced at offtaker credit spread plus an execution premium.

</details>

<details><summary><b>Debt terms</b></summary>

- **Interest:** Fixed or floating; floating usually requires swaps on most of the balance. PIK toggle during ramp; margin step-downs at utilization milestones.
- **Amortization:** Sculpted to contracted cash flow, minimal balloon. Cash sweep below a utilization threshold.
- **Maturity:** Inside the lease or offtake term. For GPUs, also inside the chip's useful life; sub-1yr rental books are hard to finance.
- **Prepayment:** Non-call periods, make-wholes and prepayment fees set how cheaply you can refinance later.

*Risk addressed: residual value, re-leasing*

</details>

<details><summary><b>Recourse</b></summary>

Non-recourse (SPV assets only), limited (parent guarantees completion or overruns) or full (parent guarantee). Startups with thin contracts often have to give some.

*Risk addressed: offtaker credit, construction*

</details>

<details><summary><b>Collateral &amp; covenants</b></summary>

Bankruptcy-remote SPV per asset or contract with step-in rights; lockbox and DSCR covenant.

- **Reserves:** Debt service reserve (~6 months), maintenance reserve for failed GPUs, interest reserve during construction.
- **Cash traps:** Below a DSCR lock-up level, equity distributions stop; lower still, a cash sweep pays down debt.

*Risk addressed: offtaker credit*

</details>

<details><summary><b>Borrowing base</b></summary>

Availability recalculated periodically from eligible contracts and appraised GPU values; shrinks automatically as contracts roll off or chips lose value.

*Risk addressed: residual value*

</details>

<details><summary><b>Intercreditor terms</b></summary>

Sets payment priority and enforcement rights when venture debt, mezzanine, GPU loans and vendor liens coexist; where equipment carve-outs live.

</details>

<details><summary><b>Equity kicker</b></summary>

Warrants to the lender in exchange for lower coupon or higher advance rate.

</details>

### Cash flow enhancement

<details><summary><b>Customer prepayments</b></summary>

Up to 100% of contract value upfront on 1yr compute deals. Reduces the amount borrowed and the equity required.

*Risk addressed: offtaker credit, funding need*

</details>

<details><summary><b>Customer-funded hardware</b></summary>

Customer buys the GPUs and the operator hosts them, or the tenant funds the fit-out. Shrinks what the operator has to finance.

*Risk addressed: funding need, residual value*

</details>

<details><summary><b>Revenue share</b></summary>

Lender receives a share of GPU-hour revenue in exchange for a lower base coupon.

*Risk addressed: utilization, price*

</details>

<details><summary><b>Multiple offtakers</b></summary>

Single GPU contract supported by two offtakers with complementary workloads (daytime inference, nighttime training). Higher utilization, diversified payment risk.

*Risk addressed: offtaker credit, utilization*

</details>

<details><summary><b>Contract terms</b></summary>

Take-or-pay or minimum commitments, tenor matching the debt, no termination for convenience, price escalators, power cost pass-through. A reserved base plus on-demand upside works too; lenders size off the base.

*Risk addressed: offtaker credit, utilization, power price*

</details>

<details><summary><b>Resale rights</b></summary>

Contract rights to resell a customer’s unused reserved capacity, which also makes customers more willing to sign longer take-or-pay commitments. Uncontracted GPUs go to spot marketplaces or brokers.

*Risk addressed: utilization*

</details>

### Credit support

<details><summary><b>3rd party credit backstop</b></summary>

NVIDIA, AMD or Google guarantee of lease payments, or take-or-pay floor on GPU capacity (typically ~6yr, declining price curve). The lender underwrites the backstopper's credit. Covers the full contract term, so it substitutes for the customer's credit.

- **Backstopper compensation:** Share of revenue above the floor, warrants or equity stake, or a fee.
- **Related-party exposure:** Lenders haircut credit when the backstopper is also the supplier and an equity investor.

*Risk addressed: offtaker credit, utilization*

</details>

<details><summary><b>Customer credit support</b></summary>

Letter of credit from the customer’s bank, security deposit or parent guarantee from weaker customers such as startup labs. LCs and deposits usually cover only a few months of payments: a cushion while the GPUs are re-leased, not a replacement for the customer’s credit.

*Risk addressed: offtaker credit*

</details>

### Risk transfer

<details><summary><b>Insurance</b></summary>

- **Offtaker interruption:** Covers offtaker or tenant default and early termination.
- **Residual value:** Guaranteed minimum resale value of the chips at maturity.
- **SLA / uptime:** Pays on missed SLAs from power, cooling or network failures, before downtime trips a DSCR covenant. Backstops cover demand, not uptime.

*Risk addressed: offtaker credit, residual value, operational*

</details>

<details><summary><b>Futures &amp; options</b></summary>

Hedge GPU-hour pricing on uncontracted capacity; rate and power hedges alongside. No liquid GPU derivatives market or widely used price index yet.

*Risk addressed: price, residual value*

</details>

<details><summary><b>Power purchase agreements</b></summary>

10–20yr contract to buy power at a set price. Fixes the largest operating cost, stabilizing DSCR.

- **Types:** Physical (power delivered), virtual (financial hedge settled against a hub price), sleeved (utility delivers and passes the price through).
- **Risks:** Take-or-pay even if GPUs sit idle; 15yr term vs 3–5yr GPU contracts; seller needs a creditworthy buyer or collateral; virtual PPAs carry basis risk.
- **For startups:** Rarely signed; colo passes power through. Relevant once you own the site. Power pass-through in customer contracts gives similar protection.

*Risk addressed: power price*

</details>

## Reference

### Capital providers

| Provider | Role |
|---|---|
| Banks | Construction loans, revolvers, warehouse lines; arrange bonds and ABS. |
| Private credit funds | GPU-backed loans, HoldCo and mezzanine debt, bespoke structures. |
| Infrastructure funds | Debt and equity for data centers and power; buyers in sale-leasebacks. |
| Insurers & bond investors | Long-dated project bonds; ABS and CMBS tranches. |
| Venture lenders | Venture debt for early-stage companies. |
| Strategics | Chip vendors and hyperscalers: backstops, equity, vendor financing. |

### Refinancing path

- **GPUs:** Vendor financing or venture debt → GPU-backed term loan → Warehouse facility → ABS (not yet established for GPUs)
- **Data centers:** Construction loan → Term loan or project bond → ABS, CMBS or sale-leaseback

## Tax & public incentives detail

*Federal, state and public financing levers that lower the cost of GPUs, facilities and power. Status as of October 2026; state programs are changing quickly.*

### Federal tax

| Scheme | How it helps | Watch for |
|---|---|---|
| **100% bonus depreciation (§168(k))** | Immediately expense GPUs, servers, electrical and cooling. With no taxable income, get the value through a lessor or tax-equity partner. | Property placed in service after Jan 19, 2025; now permanent. CA, MA and NY don’t conform. |
| **§179 expensing** | Alternative immediate expensing for smaller purchases. | Capped at $2.5M, phasing out above $5M of purchases; immaterial at cluster scale. |
| **R&D credit (§41)** | Payments to use someone else’s computers for qualified research count toward the credit, so cloud GPU spend on research can qualify. Startups can apply up to $500K/yr against payroll tax. | Hardware must be owned and run by others, off-site, and not primarily used by you; allocate mixed use; keep usage records. Payroll offset needs under $5M of receipts and no receipts more than 5 years back. |
| **R&D expensing (§174)** | Domestic R&D deductible immediately again from 2025. | Foreign R&D still amortized over 15 years. |
| **Losses (NOLs & §382)** | Losses from depreciation carry forward to offset future profits. | Can offset only 80% of taxable income per year. A >50% ownership shift over 3 years, common after big VC rounds, caps annual use. |
| **Interest deduction (§163(j))** | Cap is 30% of adjusted taxable income, now measured before depreciation; leveraged builds deduct more interest. | Tax years after 2024; some states decouple. |
| **Energy credits (§48E / §45Y)** | Credits on on-site storage, fuel cells and generation. | Storage, fuel cells, geothermal: full credit for construction starting through 2033, 75% in 2034, 50% in 2035. Solar and wind: construction by July 4, 2026, else in service by end-2027. Foreign-entity sourcing limits. |
| **Credit transfer (§6418)** | Sell credits for cash, typically at a discount; lenders bridge against expected sales. | No transfers to specified foreign entities. |

### State & local

| Scheme | How it helps | Watch for |
|---|---|---|
| **Equipment sales tax exemptions** | Exempts servers and equipment from sales tax, often the largest state tax on a GPU build. Colo tenants may qualify through the operator. | Investment and job thresholds (Illinois: $250M over 5yrs, 20 jobs). 2026: Ohio and Illinois paused new approvals, Washington narrowed its program, Virginia’s is under budget review. |
| **Power tax exemptions & utility rates** | Some states exempt data center electricity from sales tax; utilities offer economic development rates for large new loads. | Varies by state and utility; new large-load tariffs often add minimum bills. |
| **Property tax abatements** | Local PILOT agreements, often through industrial revenue bonds: the city holds title and leases the property back, so it’s tax-exempt. | Investment deadlines and claw-backs; political risk (Independence, MO granted Nebius a 90% abatement in March 2026; a supporting councilman was recalled in September). |

### Investment & public financing

| Scheme | How it helps | Watch for |
|---|---|---|
| **Opportunity zones** | Investors defer and reduce capital gains tax by investing in projects in designated zones; helps raise equity for a site there. | Made permanent; new rolling 10-year zone designations start in 2027. |
| **Export credit agencies** | Government-backed loans for US equipment used at non-US sites; longer tenor, lower cost. | US content requirements. |
| **Federal energy loans** | Loans and guarantees for new generation, storage and grid projects. | Long process; large project minimums. |
| **Federal sites** | DOE picked Idaho National Lab, Oak Ridge, Paducah and Savannah River (July 2025) for private AI data center and energy projects. | Site-by-site solicitations; suited to large developers. |

---

# Compute procurement

| | **Rent from cloud**<br><sub>Neocloud or hyperscaler capacity</sub> | **Colo + own GPUs**<br><sub>Lease space and power; buy and install GPUs</sub> | **Modular data center**<br><sub>Prefab containerized units, e.g. Armada, Giga, Rune Energy</sub> | **Own powered shell**<br><sub>Build or buy the building and power; buy GPUs</sub> |
|---|---|---|---|---|
| **What you own** | Nothing. Contract for GPU-hours or reserved capacity. | GPUs, servers, networking. Space, power and cooling leased from the colo provider. | Modules (power, cooling, racks) plus GPUs. Site leased or owned; power sourced separately. | Land, building, power and cooling infrastructure, GPUs. |
| **Upfront capital** | Low. Prepayments on reserved capacity. | GPU and networking capex; colo deposits. | Modules plus GPUs, site prep and power connection. | Full facility capex plus GPUs. |
| **Time to compute** | Days to weeks, subject to availability. | Months. Gated by GPU lead times and available colo power. | Months once a powered site is secured. Factory-built, faster than construction. | Typically 1–3 years. Power interconnection is the longest lead item. |
| **Control** | Limited choice of hardware, location and network design. | Own the hardware stack; facility terms set by the colo provider. | Own the stack and choose the site, including stranded or behind-the-meter power. | Full control over design, density, cooling and expansion. |
| **Cost at high utilization** | Highest per GPU-hour; pays the provider's margin. | Lower; pays colo rent in place of compute margin. | Lower; depends on power cost at the site. | Lowest at scale, once the facility is full. |
| **Key risks** | • Capacity availability and price resets at renewal<br>• Take-or-pay commitments if usage falls<br>• Provider counterparty risk | • GPU residual value<br>• Utilization of owned GPUs<br>• Colo lease term shorter than the debt | • Site power reliability and uptime<br>• Limited track record of module operators<br>• Density and cooling limits for newest GPUs | • Construction and delivery delays<br>• Power interconnection<br>• Underused capacity if demand slows |
| **Financing routes** | • Opex funded by VC equity or internal cash<br>• Venture debt extends runway; repaid from equity, not compute<br>• Reserved capacity often needs prepayment | • Start with vendor financing, then equipment leases (lessor carries residual risk)<br>• Venture debt as a bridge; carve out future GPU liens<br>• GPU-backed term loans once an offtake contract is signed; backstops or customer LCs strengthen weak contracts | • Equipment financing on modules and GPUs; modules are relocatable collateral<br>• GPU debt as in colo<br>• Lender needs site access rights | • Construction loan, then SPV project bonds once a strong tenant signs; startups are usually the tenant, not the issuer<br>• Mezzanine or preferred equity fills the gap above senior debt<br>• Once stabilized: ABS, CMBS or sale-leaseback to recycle capital<br>• PPAs; GPU debt alongside |
| **Best fit** | Early stage, uncertain demand, burst training runs. | Steady, predictable workloads at a few thousand GPUs. | Access to cheap or stranded power; speed matters more than density. | Large, long-term contracted demand and balance sheet to match. |
| **Who to contact** | **Hyperscalers:** AWS, Microsoft Azure, Google Cloud, Oracle Cloud<br>**Neoclouds:** CoreWeave, Nebius, Lambda, Crusoe, Together AI, Vultr, Fluidstack, Voltage Park<br>**Marketplaces & spot:** SF Compute, Vast.ai, RunPod | **Colocation:** Equinix, Digital Realty, CoreSite, Switch, Flexential, DataBank<br>**High-density AI colo:** Colovore<br>**AI hosting (former bitcoin miners):** Core Scientific, Hut 8, IREN, TeraWulf, Cipher. Mostly large wholesale deployments. | **AI-focused modular:** Armada, Giga Energy, Rune (solar-sited), Crusoe<br>**Prefab power & cooling modules:** Vertiv, Schneider Electric | **Powered land:** Lancium, Tract<br>**Existing powered sites:** Former bitcoin miners: Core Scientific, Hut 8, IREN, TeraWulf, Cipher<br>**Design-build:** DPR Construction, Holder, Turner, Mortenson<br>**Power & cooling equipment:** Vertiv, Schneider Electric, Eaton |

### For any option where you own the GPUs

- **GPU servers & OEMs:** Dell, Supermicro, HPE, Lenovo
- **Vendor financing:** Dell Financial Services, HPE Financial Services
- **Private credit active in GPU and DC lending:** Blackstone, Apollo, Magnetar, Blue Owl

*Time and cost comparisons are directional and vary with GPU generation, site and market conditions. Company lists are a starting point as of October 2026, not exhaustive.*

---

# Interactive models

Five tabs run live in `compute-financing-guide.html` (open it via GitHub Pages or in a browser). Every input can be changed and all outputs and sensitivity grids recompute.

### Compare
The four procurement models side by side, per GPU, reading each tab's live inputs: deal shape, upfront capital and equity, project and equity IRR, NPV and equivalent annual NPV, payback, breakeven blended price and cushion, debt/EBITDA and min DSCR. Shared assumptions (sales mix, contract terms, market price path, GPU capex and GPU debt) start from the same defaults on every tab.

### One model per procurement structure
Each column of the procurement table has its own per-GPU model, on the same basis so results compare across tabs. Defaults are illustrative.

| Structure | What it models | Base case |
|---|---|---|
| **Rent from cloud** | Monthly model of take-or-pay reserved capacity resold through fixed-price contracts and on-demand sales, with a rise-then-fall market price path, utilization ramp, billing timing, deposit, delivery delay and SLA credits; compared with buying on-demand | 59% IRR on upfront cash (5-yr commitment at $2.75); breaks even at 49% steady on-demand utilization |
| **Colo + own GPUs** | Returns on one GPU in third-party colo: $65k capex, 75% debt at 7%, contract and on-demand sales on a rise-then-fall market price path, customer prepayment, colo deposit | 29.2% project IRR, 110% equity IRR, $3.33 breakeven blended price |
| **Modular data center** | Own modules + GPUs on cheap or stranded power; 6 months to revenue; same sales and market price inputs; modules partly recovered at exit | 23.1% project IRR, 82.7% equity IRR |
| **Turnkey data center** | Build the powered shell over 24 months with capex drawn through construction, then run four 5-year GPU generations in it; construction debt with capitalized interest; offtaker toggle (IG or HY) sets the debt terms | 23.6% project IRR; 110% equity IRR with an IG offtaker (90/10, 15-yr amortizing), 46.5% with HY (80/20, 5-yr HY refinanced into IG) |

Each tab shows headline returns, breakeven rent or utilization, the annual cash flow schedule, a one-way sensitivity table (pick any input and edit the test values) and a two-way heat map (pick the row and column inputs and the output to watch).
