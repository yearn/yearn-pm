# Meeting notes: Doers standup Apr 07 2021

## Updates from

- lehnberg
- tracheopteryx
- dark ghosty
- bull
- dudesahn
- doggie
- facu
- doug
- poolpi
- luciano
- klim
- x48
- banteg

## 1. Weekly updates

### 1.1 Done

**Vaults/Protocol:**

- More Uni approaches
- 0.3.5 release
- 1.0.0-audit.0 release (Baseline for audit)
- Update OPERATIONS.md
- Create DEPLOYMENT.md
- Emergency drill scheduled
- review and merge subgraph PR with tests
- iearn problem affecting curve, fixed by aave disabling stable rate v1 borrowing
- multicall context manager for brownie
- hardhat support for brownie

**Strategies:**

- yfiMaker strategy fix/disclosure
- Review of Pool Together DAI/USDC 0.3.0
- Help added to manage sms tx and debt ratios
- yvboost audit
- cvp call on lazy ape and extending it to v2 vaults

**Keep3r:**

- yearn/keep3r-jobs repo
- oracle issues patches and manual labor
- keep3r-liquidity-manager site
- auto-bonding

**Web/API:**

- Web demo site
- Condense down requirements for MVP
- Lots of minor web fixes/PRs
- Fixing WBTC APY
- v3 call on final process
- lens contract/adapters iteration
- general purpose helper utility contracts
- dynamic length array concatenation utility for solidity
- Add extensive unit tests for lens contracts
- Improve TVL oracle contract (fix edge case issue and add additional logic to mirror banteg's logic)
- Isolate common lens logic into one contract
- Set up SDK with eth_call overrides to test contracts
- Discuss new TVL plan with DeFi Pulse
- yearn.science released, integrated in theblock and defilama

**Governance/Ops:**

- Airdrop YIP proposal
- Cream LP prop
- More org / team mgmt discussion
- Hiring proposals
- Payroll and HR information organized
- Governance 2.0 mechanics for YIP
- Governance 2.0 YIP draft for review
- Compensation packages and guidelines
- Coordinape HR and payouts

**Treasury:**

- claim ellipsis airdrop
- set up monitoring for eps farming
- vote for curve gauge weights with overrides

**Comms/Docs:**

- Chinese newsletters translations
- Newsletters writing and editing
- Interview face of Yearn

**Partnerships:**

- Reach outs
- HBTC deposit, launch plan preparations
- High level brief for Partners dashboard
- Request to makerdao to add yearn to oasis save

### 1.2 Doing

**Vaults/Protocol:**

- yvBOOST launch
- audit preparations
- code alert bot
- revamp DEPLOYMENT(.md) procedure
- review path to production and due dilligence docs
- post mortem and plan of action on yvYFI incident
- fixes to brownie

**Strategies:**

- Get SNX strat ready

**Keep3r:**

- plan next yMechanics roadmap
- keep3r-liquidity-manager web review and test
- improve docs and unit tests on yearn/keep3r-jobs
- fix oracle issue ☠️

**Web/API:**

- Update Yearn Exporter dashboards
- Update lens adapters to support delegatecall logic
- Prepare for mainnet lens/adapter deployment

**Governance/Ops:**

- Offers & HR processes
- governance 2.0 YIP
- launch coordinape circles for strategists, 0.03%, and Sushiswap

**Treasury:**

- March Financials
- Quarterly Report
- Cash burn analysis
- Buy back some yfi

**Comms/Docs:**

- Video on yVaults

**Partnerships:**

- measure partners

### 1.3 Todo

**Vaults/Protocol:**

- devdocs
- uni v3 mvp
- figure out what to do with yToken
- emergency drill
- wrapper masterclass
- make a list of emergency actions
- researching Optimism and SNX
- fixes to yearn-hub

**Strategies:**

- Strategy descriptions
- collect maintenance specs for strategies
- review USDP strat
- review SNX strat
- research index token to avoid taxable events

**Keep3r:**

- keep3r-liquidity-manager web deploy
- monitoring and alerts
- finalize keep3r copy
- finalize keep3r tracking specs

**Web/API:**

- Web dev planning session
- DeFi Pulse adapter
- add delegated assets and earnings data to yearn.science
- figure out web v3 review process
- use alerts on yearn.vision

**Governance/Ops:**

- publish Gov 2.0 YIP
- finalize pending offers
- decide on new hires

**Treasury:**

- roll out march financials
- upload reports

**Partnerships:**

- Payout reporting
- Set up partnerships group
- review integration code
- distribute partner rewards

### 1.4 Blocked

- Lack of dev resources to support integrators
- Retroactive payment calculations
- ychad for March
