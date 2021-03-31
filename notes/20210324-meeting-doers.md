# Meeting notes: Doers standup Mar 24 2021

## 1. Weekly updates

### 1.1 Done

**Vaults/Protocol:**

- Data aggregation improvements
- TVL Oracle contract improvements
- Design review/technical implementation writeup
- Documentation for new contracts
- yearn-exporter improvements
- multiple audits finalized
- new path for migrations figured out
- management fee double charging fix
- yvBOOST launch planning
- New diagram for the v2 migration plan
- New diagram to help clarify performance fees

**Strategies:**

- First POC of yearn-hub with graphs https://github.com/dougstorm/yearn-hub
- Iron Bank Curve Vault & Strat deployed and moved to prod
- Weth strategy double fees reimbursed
- Double fees scripts for usdc, usdt, dai vaults (charged in 3crv) and for tusd vault (charged in yusd)
- BDP recovery complete, funds sold and returned to yfi vault
- HBTC deposits
- Reviews of synthethix generic strat for YFI (Bank Protocol)
- Curve v2 LPs template completed

**Keep3r:**

- Full keep3r design overhaul
- Partial Uni Oracle pair updater job (PartialKeep3rV1OracleJob)
- keep3r-liquidity-manager (aka soccer-mommy)

**Web/API:**

- Zaps live on the website
- test repo for v3 web codebase nearly finalized
- SDK working with @x48114's oracle contracts
- Lazy ape added to UI and opened one-sided liquidity

**Governance:**

- Phased plan shared for using SafeSnap, eventually migrating governance onto Colony v2
- Prototyping yearn project managment system in https://clickup.com/
- 2-week marketing project kicked off
- 0.03% discussion concluded positively
- Ecosystem call
- Coordinape alpha payouts & beta design flows finalized
- yGift: new UX/UI designer & Miguel onboarded as lead; team is independent now and moving forward
- Guest list modified to support more protocols, to be used for snapshot voting

**Treasury:**

- Feb Income statement and Balance Sheet
- Treasury farming profit/exp through 3/15

**Comms/Docs:**

- Twitter
- Newsletters writing and editing
- Backscratcher tweet draft

**Partnerships:**

- New delegated deposit tracking model, very well received by partners

### 1.2 Doing

**Vaults/Protocol:**

- More data aggregation work
- Finish on-chain TVL stuff
- CREAM IB discussions
- Integrate yearn-exporter tvl endpoint to defipulse etc. already in touch with nansen and theblock.
- Generate yearn tokenlist, add to tokenlists
- Research uni v3
- Release v0.3.4
- Co-ordinate migrations
- Optimism research
- List of good first issues to help newcomers
- Add alerting to grafana

**Strategies:**

- Facilitate claim of ellipsis airdrop
- Continue to add more strategy data to yearn hub

**Keep3r:**

- Move liquidity
- keep3r/eth LP quantification
- finish tests for soccer-mommy (complex contracts)
- guide to deploy, setup and use PartialKeep3rV1OracleJob

**Web/API:**

- interactive demo with SDK on v3 codebase
- MVP meeting with devs+designers
- All designs to complete a replicate of site on desktop+mobile done by tomorrow

**Governance:**

- Gather feedback on Colony plan
- Vision doc
- Next full draft of org structure
- Set up new snapshot space
- Staffing questions
- Yearn personality interviews

**Treasury:**

- Weekly at a glance vault report
- YFI buyback vs. using cash to farm in treasury modeling

**Comms/Docs:**

- Strategy descriptions

### 1.3 Todo

**Vaults/Protocol:**

- deploy yTokens
- plan emergency drill for v2 vaults to validate ops process doc

**Keep3r:**

- deploy soccer-mommy + her job
- deploy standalone jobs (v1-crv, v1-vault, v2-harvest)

**Web/API:**

- Dig deeper into yearn-lens
- Further review yToken contract to determine if front-end shuld use it
- Stakeholder web design review, solidify timelines/goals/task after
- finish subgraph MVP
- Port ape.tax to react

**Treasury:**

- mint 1 usdp to lower stability fee on unit
- Quarterly report
- New ops budget based on latest run-rate
- New treasury farming recommendations based on cash holdings

**Comms/Docs:**

- dev docs

**Partnerships:**

- Retroactive payments

### 1.4 Blocked

- Final yvBOOST code, all test to pass
- 80% done state of website
