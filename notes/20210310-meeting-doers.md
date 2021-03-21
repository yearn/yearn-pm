# Meeting notes: Doers standup call Mar 10 2021

## Attendance

- x48
- banteg
- doug
- klim
- facu
- trach
- luciano
- doggie
- dark ghosty
- dudesahn
- bull
- orb
- lehnberg

## 1. Weekly updates

### 1.1 Done

**Vaults/Protocol:**

- Wrapper merged
- Registry code updated
- yearn-exporter: event and registry support with live updates
- ape-safe: clean up chief-multisig-officer codebase, document it and release as ape safe
- Final PWC audit report
- Alchemix integration review
- Migration and unwinding of ETH, USDC, DAI, USDT v1 vaults
- PR fix based on fuzz testing
- yvBOOST facilitation and heads up to pickle & sushi
- Prepare yearn security talk for yAcademy
- yearn.rocks deprecated in favor of ape.tax with docs
- Unit tests for yearn-vaults repo
- Scripts for monitoring vaults/strategies
- weth v1 migration plan

**Strategies:**

- Curve-dao gauge weights voting strategy codified - tl;dr exclude max boost vaults, then vote proportional to tvl
- Iron Bank Curve changes
- Single sided ETH strat for WETH v2 vault
- crvRen BTC
- YFI vault + strat
- 1inch strat in ape.tax
- Idle strategies fixes
- Holyheld smart contracts
- setup lazy ape sushi rewards

**Keep3r:**

- proxy-job + jobs improvements
- updated new curve keep3r job

**Web/API:**

- pickle zap
- website fixes
- launch several new vaults on UI
- yvecrv added to UI
- Debug state issues on pickle implementation - DMARC fix

**Governance:**

- Jan income statement and balance sheet
- Governance Open Thread forum post
- Coordinape launch
- Multisig risk evaluation and legal advice
- Reviewed multisig alternatives
- Colony v2 discussions with Jack du Rose, launched collab
- filled ychad audit for jan
- paid subscriptions with mixbytes

**Comms/Docs:**

- Spokesperson strategizing

**Partnerships:**

- Lead generation survey
- Announcement
- Reach outs, 3 new groups, 1 phone call

### 1.2 Doing

**Vaults/Protocol:**

- integration testing migrations with DAI and USDC Vault users
- Adding historical data to yearn-exporter
- gnosis-safe safe snap for executable proposals
- Insurance backstop ideas
- Αlerts for vault conditions via Telegram

**Strategies:**

- strategy descriptions
  -building quick web dashboard for strategies settings review before preparing drill
  - strategies reviews
- Finalizing IB vault
- ETH v1 unwinding & migration
- DAI and USDC v1 migration
- Curve v2 template

**Web/API:**

- v3 facilitation
- Getting YLA, zapper zaps, and YFI/ETH migrations live on site
- Web devs planning best practices/framework for v3 web codebase
- More work on "lens" contract
- Integrate lens into SDK
- Host coordinape

**Governance:**

- Org & comms structure
- Hiring plan
- 0.03% facilitation
- Governance research
- Coordinape alpha
- Finish ychad audit for feb

**Partnerships:**

- retroactive partner payments
- lead generation follow ups
- integration + legal work as required

### 1.3 Todo

**Vaults/Protocol:**

- Registry migration plan
- Redefine how to support metadata for vaults and strategies
- Deploy updated Registry
- Deploy yDAI and yUSDC (yTokens)
- Create Curve LP wrappers + guest list combo for Curve migrations
- Dev docs
- Emergency drill for v2 vaults
- Launch IB vault, coordinate with CREAM for marketing
- Reimburse double dips

**Keep3r:**

- Allocate funding for keepr jobs
- Improve yKeep3r & yMechanics

**Web/API:**

- Gas savings stats

**Governance:**

- Add new yvyfi vault to snapshot
- Feb financials

**Partnerships:**

- Verify partnership data
- Pay retroactive partner fees

### 1.4 Blocked

- ETH vault unwinding
- Need another reviewer
- Improve process for strats roll-outs & migrations

## 2. Call-out topics

### Vaults & Strats

#### ETH migration

- Code + Web must be ready in order for migration to happen
- Stick to the process
- Don't run in front of the train, or Klim will eat you alive
- Have full process ready before announcing

#### Phase 1 migration status

- delayed, issues discovered with stables
- everyone need to migrate from eth v1->v2 first, and then stables can migrate
- Can we unwind the v1 vault?
  - As long as the v1 vault goes down to 1k ETH it should be fine
  - 15k current deposit size means it's unlikely it will migrate
- v1 yYFI vault shows we can't expect anyone will move those funds
- Facu, dude, bull to sync and organize migration plan

#### Phase 2 migration status

- registry required (in process)

### TVL

- Needs to get finalized including proper subtractions for double-counting
- Defi Pulse need on-chain contracts, in process

### Other

#### Fund coordinape with farming

- to fund grants
- a lot of details to be fleshed out
  - how much YFI?
  - Timelocked?
  - What strategies?
  - Floor and Ceilings for how much of returns are used?
  - what's the spec?

#### Treasury: To diversify for stables or not

- farming / dogfooding with our funds
- fees earned is automatically diversifying our treasury
- thought to put into diversifying the YFI holdings
- could use vaults to farm gov tokens of other protocols as a way of diversifying
- better to invest in our own protocol and make it ready for the bear market
- making sure yearn is set for the medium and long term for sustainability

#### Advertising/displaying Net APY vs Gross APY?

- Tide has changed, many other projects show APY after fees
- Bull to spearhead honest farmer alliance (coalition for displaying standardized set of APYs between projects)

#### Boosting earnings by x1.5 to handle rising overheads

- Focus on the main vaults, our bread and butter
- Should we really put smaller tokens on prod before USDT?
- Partners

#### Incentivizing yveCRV locks

- Treasury YFI farming for boost
- yveBOOST
- Changing 10% lock amount into higher
