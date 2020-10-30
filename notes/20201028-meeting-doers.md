# Meeting notes: Doers standup call Oct 28 2020

**Attendance:** Banteg, Bull, DarkGhosty, Doggie, Facu, Graham, Klim, Lehnberg, Luciano, Santiago, x48

## 1. Overview of current workstreams

- **Governance**, group led by lex_node, second meeting this week.
- **Docs**, budget distribution complete, project board updated.
- **Protocol devs**, vault2 experiments, security audits, and more strategy testing.
- **CeFi Exchange Integration SDK**, group created, early discussions held with Gemini, opportunities may also exist with Coinbase and Huobi. Led by Santiago on BizDev side, Doggie on Dev side.
- **Naming strategies**, still not fully concluded but a proposal is more or less final at this point. Led by dudesahn with contributions from chris.eth among others.
- **Social media**, AMA just took place on discord and was well received.
- **Branding & Design**, front-end work led by x48, visual design & ux by Future.
- **Vault Strategies**, iterating on new strategy ideas, led by Banteg.
- **yGift**, design effort commissioned and in progress, effort led by Klim.

## 2. Updates, actions & ideas from the round-table standup

- **No blockers.** Everyone seems able to progress independently of each other.
- **yCover NFT Contest** is underway, and ends in 3 days.
- **ETH hackathon winners** are Hegic strategy writers and Tokenlog.
- **keep3r** is an Andre Cronje project that just launched. It is not directly under the Yearn umbrella, keep3r fees are **not** going to YFI holders. More info on the project [website](https://docs.keep3r.network). Yearn is however a potential customer of the protocol, which can be likened to a decentralized system for executing cronjobs on Ethereum. There are some explorations underway to test using keep3r jobs for Yearn `harvest()` calls.
- **Token logo designs** are being considered. There are some thoughts on taking a break and re-iterating on them, this is still pending discussion in the Brand group.
- **Subgraph is being re-written from scratch**, wasn't possible to maintain as is. Vaults v2 should be able to support subgraph with less work.
- **Argent integration is moving forward again** after a bounty was paid to fix a bug.
- **GUSD vault has launched**, more tests are needed, as is more liquidity. Santiago to ask Gemini to contribute. Thoughts to migrate to vaults v2.
- **vaults2:**
  - **0.1.2 was just released**, further refinements on the way, mainly around improvements to documentation and testing.
  - **several smaller experiments** are on mainnet, with capped deposit limits, and no front-end UI.
  - **audits are pending** and need a legal entity to contract with one of the security firms that are bidding. Santiago or Doggie may be able to provide a legal entity.
  - **in terms of release process**, the current approach is to gain slow and steady confidence through smaller contained tests, wait for audit results to come back, and in parallel begin work on front-end work required for an official roll out.
- **Vaults registry v2** is being explored.
- **yHegic vault + Strat** underway, possibly also a WBTC Hegic vault.
- **Leveraged DAI strategy** is live on mainnet as an alpha, next steps are more tests and migration to the new version of the vault.
- **Uniswap LP strats are being tested**, a WBTC/WETH pair is deployed farming and dumping pickle using Vault v2. Migration might be tested for this.
- **Treasury may require an iteration** as Vaults v2 are launching. There's an opportunity to rethink fee structures, allocations, how expenses are being calculated. Opportunity to use the vaults2 tests to gather data on different approaches. A separate group was created after the call for this, ask Banteg for access.
- **yearn.finance migration** has been completed successfully, now hosted on AWS under our control. CI has been set up for the github branches:
  - Staging environment, dev.yearn.finance -> push to `develop` branch.
  - Production, yearn.finance -> push to `main` branch.
- **Website redesign** is in progress. [Drizzle](https://www.trufflesuite.com/drizzle) integration is now working which should allow for more responsive data updates.

## 3. Doers: Org, Collab processes, tools

- Is the weekly stand up call efficient?
- Other ideas for updating each other?
