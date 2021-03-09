# Meeting notes: Doers standup call Mar 03 2021

## Attendance

- Facu
- Tach
- Banteg
- DarkGhosty
- MilkyKlim
- Dudesahn
- Luciano
- Doug
- Bull
- Santi
- Lehnberg
- Orb

## 1. Weekly updates

### 1.1 Done

**Vaults/Protocol:**

- OPERATIONS.md
- Presentation and exercise on v2 vaults for yAcademy Kernel
- Session on remaining work for the graph
- v2 Deposit Wrapper Review
- yveCrv disclosure
- v2 vault version issue
- v2 vault deployment script

**Strategies:**

- Reviews: IDleStrats patch, New strategyProxy, crvRen BTC v2, IB curve pool, single sided eth v2
- Issue fixed on all stablecoins single sided strategies (dai, usdc, usdt, tusd)

**Keep3r:**

- Vaults & strategists monitored in yMechanics
- Proxy Keep3r intro call
- Keep3rProxyJob finished, deployed, unbonded, bonded, and credits applied
- CrvStrategyKeep3rJob deployed and tested
- Manual keep3r work for v1 + v2 strats
- Keep3r scripts to monitor and stealth work v1 and v2 strats
- Keep3r earn/harvest script

**Web/API:**

- helped web integrate vault migrator
- yvecrv UI design
- display fees UI
- UX Community share-out for v3
- Pickle zap

**Governance/Ops:**

- Work out v1 fee docs issue
- Interviews & negotiations for hiring fulltime candidates
- /yearn github migration
- Buy & lose @yearn twitter (rip)
- Treasury yield farming plans/strategies
- Potential LM program ideas
- Governance revamp work
- Coordinape plan (alpha test will run March 8–12)
- Aave ARC effort aborted

### 1.2 Doing

**Vaults/Protocol:**

- DAI and USDC v2 migration
- HBTC single sided vault deployment
- crvRenWBTC single sided vault deployment
- Vaults v2 intro
- At-a-glance yVault report
- Part 2 of security at yearn talk
- Yearn-Exporter Dashboard updates
- Curve v2 integration with deposit wrapper
- Merge deposit wrapper

**Strategies:**

- yveyveCRV championing
- v1 > v2 migration roadmap (stage 2)
- double/triple dip issue

**Keep3r:**

- Testing of sugarMommy
- Deploy new meta-jobs
- Add 1 week minHarvestTime to CrvStrategyKeep3rJob (for slow strats)
- Redeploy CrvStrategyKeep3rJob
- Proxy-keep3r repo cleanup + docs, then merge to yearn repo

**Web/API:**

- Coordinate Pickle zap implementation

**Governance/Ops:**

- More new hire discussions/negotiations
- Try to recover @yearn via Twitter support
- Monitoring and strategizing more treasury yield farming
- Forum post on evolving our governance
- Org structure
- Coordinape future plans
- Roll out YLA
- Prolong MixBytes subscription
- **Partnerships:**
- Partnerships onboarding process
- Partnership co-ordination
- Review partner contract integrations

### 1.3 Todo

**Vaults/Protocol:**

- v1 -> v2 migration phase 2: Curve LP vaults
- Redefine how to support metadata for vaults and strategies
- Script to check vault fees and governance using yearn-exporter
- make plan for  emergency drilled for v2 and schedule it
- Curve LP wrapper design

**Strategies:**

- Single sided curve strats reviews
- Experimental vault reviews
- Uni/comp strats
- Add backscratcher to TVL
- Deployment of IB strat whenever wrapper ready
- Generic curve v2 template
- Port maker & single side strats from v1 to v2

**Web/API:**

- Add Lazy Ape button in UI
- Start implementing UI/UX updates to yearn.fi

**Governance/Ops:**

- Feb financials
- Coordinape overview doc
- Finalize draft org structure
- Gov forum post
- Telegram optimization
- Return money to double dipped people
- Make “important not urgent” public board where people can pick up tasks

**Partnerships:**

- Legal opinion for partner

### 1.4 Blocked

N/A

## 2. Call-out topics

### Yearn's Brand and the remit of responsibility

#### Experimental vaults

- Make separation between yearn & experimental vaults more explicit and clear
- Change URL to ape.tax
- Change how vaults are communicated
- Core devs are not involved, vaults have matured, not as useful
- Apes are going to find vaults no matter what
- Possibly setting guard rails: max deposit amounts (even if set high), whitelist addresses, `/guest-list/`
- Tems checkboxes to agree
- Governance on experimental vaults are handed to Strategist multi-sig

#### Partnerships program

- Regardless of what may happen, some will always see it as yearn's fault / responsibility
- We should take measures to protect ourselves
  - Risk team, setting criteria for acceptable risks
  - Some actions taken based on certain TVLs
  - Spending time, reviewing & auditing code
- Communications strategy, making sure we are not hit by somebody else's failure
- Can't ignore the fact it will be bad for us if partners fail.
- Who's responsible?
  - Partners are building on us. They are responsible for their codebase
  - If something happens with their codebase, that's on them
- Yearn team members should not promote third party projects they have not thorughly vetted

#### Yearn communication policy

- Communicate affiliate / partnerships clearly, what is in and out of Yearn's remit
- Do we need a YFI Spokesperson?
  - Hiring: Growth lead?
  - Hiring: Comms lead?
- Need a internal comms policy

### Contributors

- Hiring: engineering coordinator role
- Coordinape funding & future

### Multi-chain approach

- Yearn remains L1, 100% focused on ETH
- Boarding School currently plans to use other chains as testnets, with no marketing, no liabilities, and no yearn affiliations. Purpose to get experience deploying, to do light testing of strategies with little capital, but not to operate on ongoing basis.

### Vaults & Strategies

#### USDC / DAI v1 migration

- Discussion on workaround for migration and handling fees from v1 vaults (double/triple dip). - Proposed scenario
  1.  pull all funds from strats
  2.  setmin(0)
  3.  user manually migrates
- Comms message: We're migrating the vault

#### Other points

- General migration update
  - Remaining stables ready
  - Phase 2: Deposit wrapper being reviewed
