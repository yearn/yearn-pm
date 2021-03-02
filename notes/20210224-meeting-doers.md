# Meeting notes: Doers standup call Feb 24 2021

## Attendance

- klim
- x48
- facu
- banteg
- bull
- trach
- darkghosty
- doug
- luciano
- dude
- doggie
- lehnberg

## 1. Weekly updates

### 1.1 Done

- **Vaults/Protocol:**
  - Migration board to follow migration progress
  - Vaults added to yearn.rocks
  - Token wrapper review
  - zapper co-ordination
- **Strategies:**
  - LINK v2 explorations
  - New Issue Template for strategy review
  - New DAI v1 strategy reviewed
  - BTC mushroom strat reviewed
  - yveCRV to pickle jar zap reviewed
  - new strategyProxy reviewed
  - backscratcher improvements
- **Keep3r:**
  - proxy + jobs upgraded (utils machinery & mechanics contracts)
  - scripts for v1, v2 and stealth txs
- **Web/API:**
  - v2.1 of website launched
  - Gross and net APY calcs added for all vault types, including bonus rewards for Curve pools
  - Cross-chain support added to yearn.rocks
- **Governance:**
  - Hiring calls
  - Dev onboarding negotiations wrapped up
- **Partnerships:**
  - Miscommunication clearing with ecosystem partners
  - Aave ARC published
  - Cream co-operation ideas

### 1.2 Doing

- **Vaults/Protocol:**
  - DAI and USDC v2 migration
  - v2 vaults presentation for yAcademy Kernel
  - vault migrator integration on web
  - backscratcher fix and disclosure
- **Strategies:**
  - crvrenBTC single sided vault deployment
  - New Boarding School members onboarded
  - quick review 1Inch strat for experimental vault
  - iron bank curve pool strategy review for new vault
- **Keep3r:**
  - KP3R credits spendage calculations (way harder than expected)
  - waiting to release LP tokens from deprecated jobs
  - scripts for deploying new keep3r job and mechanics related contracts
  - more upgrades on jobs (yDice)
- **Governance:**
  - Work with contributors left out of retention packages
  - January financials
  - More new hire negotiations
  - catchups
- **Partnerships:**
  - aave ARC iteration
  - partnerships onboarding process

### 1.3 Todo

- **Vaults/Protocol:**
  - Pickle veCRV zap UI
  - make plan for  emergency drill for v2 and schedule it
- **Strategies:**
  - Define how to support metadata for vaults and strategies
  - Review pool together uni/comp strats
  - Review single sided curve strats for v2
  - Final tests for IB strategy
- **Keep3r:**
  - improve yMechanics devops, automate all the things.
  - stealth-txs, custom-swaps, dca. (nice to have, but not a priority right now)
- **Web/API:**
  - Splash page changes (for alchemy)
  - Vault migration UI
  - expose tvl endpoint to integrators
- **Governance:**
  - more calls scheduled this week with fulltime candidates: Wot, bob
  - coordinape progress
  - post to kick off new governance discussion / multisig transition

### 1.4 Blocked

- yChad reports (anticipated soon)
- v1 -> v2 stable vaults: Vault Swap web implementation
- waiting on Zapper docs for integration

## 2. Call-out topics

### Backscratcher fix

#### What happened

- person front-ran backscratcher claim
- all 3crv tokens went to the wrong pool
- harvest call front-ran fix so all 3crv tokens went into y3crv strategy
- ~190k 3crv from treasury used to make yveCRV whole

#### How to fix

- New strategyproxy by Andre
- Doug reviewed
- Preferably deployed before next yveCRV distro (thursday)

### Gas / Congested ethereum strategy

- Yearn: "socializing the gas costs"
- more economical for smaller users
- greater opportunity cost to leave vaults
- cost efficiency, cost/benefit analysis
- fees.wtf style website we can always point to
- will consumer facing servives on L1 really be viable?
- Batching deposits/withdrawals using Keeper?
- Zaps as a way of batching?

### Treasury mgmt

- New CDP opened, went into USDN
- Farming with yUSD, CREAM v1 has 72% interest

#### Next actions

- sushi decision (91% APY in sushi rewards)
- bancor 135 YFI space
- YFI farmers tg group
- yYFI vault

### Vaults/Strategies

- TVL for DeFi Pulse
- yveCRV farming (200% APY)
- Affiliate wrapper / Partnerships

### Misc

- Team investment management via yYFI
- Marketing & comms needs
