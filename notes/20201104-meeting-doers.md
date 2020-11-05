# Meeting notes: Doers standup call Nov 04 2020

**Attendance:** Banteg, Bull, Doggie, Facu, Klim, Lehnberg, Luciano, Orbxball, Santiago, x48

## 1. Updates from the standup

### 1.1 Done

- **New security vulnerability was handled and disclosed**, for details see [Vulnerability disclosure 2020-10-30](https://github.com/iearn-finance/yearn-security/blob/master/disclosures/2020-10-30.md).
- **New vaults2 version (0.1.3) released**, likely will be used for audits, where Mixbytes is first out.
- **Hegic vault + strategy launched** in test mode, using vaults v2.
- **Proposal presented to restructure fees and distribution,** currently [discussed on forum](https://gov.yearn.finance/t/restructure-fees-and-align-incentives/).
- **yCover Rari NFT Contest** has finished, with winners declared.
- **Naming convention rules** were finalized this week, for details see [the document](https://hackmd.io/PzIRsKmMQ-CLrMhkvblYKg).
- **Financials for aug/sep done**, some details available in the [yChad-audit](https://github.com/iearn-finance/ychad-audit) repo.

### 1.2 Doing

- **Treasury mgmt process document**, currently being drafted.
- **Grants structure proposal** is in progress, led by Substreight.
- **Website redesign**, is progressing, with general look & feel nailed and a team working on providing copy.
- **yTokens logos redesign**, is in progress, new cleaner versions are evolving.
- **keep3r testing**, curve strategy integration complete and being tested, with more keep3rs for strategies in the works.
- **yGift NFT rewards with yUSD**, the UI/UX flow is now ready and work is progressing.
- **Argent integration**, in progress and their team have confirmed it should be ready soon.
- **Yearn Strategy group shows promise**, lots of discussion, they've been shipping like crazy, including an ETH strategy for vault v2, and a y-wrapped Nexus Mutual proposal is being reviewed.
- **Yearn Grafana dashboard**, in closed testing to be rolled out wider soon.
- **Governance swaps POC**, to allow harvesters and keep3rs to get better trades for token pairs, working with uniswap already, possibly to add sushiswap and 0x for less slippage in certain pairs.
- **DCA trading of ERC20s**, calling harvest over timed intervals. You send 1000 CRV to this contract, asks for them to deliver a trade by the end of the week, and swaps happen slowly over time, using keep3rs.
- **Automated developer documentation for vaults2**, using the newly added NatSpec.

### 1.3 To do

- **Better strategy visualization**, preferably writing and maintaining it in code.
- **Vault2 flows**, and additional documentation.
- **yUSD2**, proposal for the next iteration.
- **Full backtesting of all vaults**, based on new fee proposals.
- **Pickle strategy upgrade** to use the new vaults version.

### 1.4 Blocked

- **Subgraph re-write**, due to time constraints.
- **CeFi Exchange Integration SDK**, as we're waiting for Gemini to get back to us, also Huobi is being contacted.
- **GUSD liquidity top up**, all stables should first migrate to Vaults2.

## 2. Doers processes

Testing a new two part meeting structure:

1.  (30min max) Tight standup format with a few minutes each to update on:

    - Done since last
    - Doing right now
    - Planning to work on
    - Blocked by anything

1.  (30 min max) Optional in-depth discussion on specific topics added to agenda or brought up in standup.
