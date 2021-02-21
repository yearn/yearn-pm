# Meeting notes: Doers standup call Feb 03 2021

## Attendance

- Nebula
- Facu
- x48
- Klim
- Doggie
- Trach
- Bull
- DarkGhosty
- Lehnberg
- Dudesahn
- Santiago
- Luciano
- Orb
- Doug

## 1. Weekly Updates

### 1.1 Done

- **Strategies / Vaults:**
  - 13 curve vaults/strategies shipped with new proxy to fortify the backscratcher system
  - Checklist for v1 and v2 deployment of vaults
  - sETH/ETH test vault 𓀀 from Boarding School
  - Mushrooms test vault 🍄 from Boarding School
  - ETH vault Launch
  - Reinstate 0.5% withdrawal fee in Curve vaults and WETH (with orb)
  - Define json and add metadata to vaults. Created Cloudflare + Pinata account
  - Improvements to yearn.rocks
  - IronBank lender strat review
  - Tag mapping to subgraph
  - Launched Idle v2 strat in experimental
- **Keep3r:**
  - sugarMommy v1.0 reviewed & tested
  - sugarMommy jobs (CRV, vaults, generic v2 strategy, escrow)
- **Web:**
  - onboard new team members to code
  - sync/prioritization effort of existing web ecosystem work
  - Website 2.1 sprint team kicked off
  - web goals clarified and focus aligned
  - v2 bug fixes
  - APY improvement discussions
  - QA process (PR CI pipeline)
  - Short term alchemy fix
  - Front end dev candidates
  - User feedback
- **Treasury:**
  - Paid reimbursements
  - Income statement through Dec
- **Audits:** Cover/Vaults wrapped up
- **Integrations:**
  - Talked to project about integration of their treasury
  - Several active integration discussions w CExes and DeFi projects
  - New vault + strat promo project
- **Design:**
  - New tokens for the new vaults (HUSD, USDK, USDN, UST, HBTC, PBTC, BBTC, OBTC, DUSD
  - Fixed SBTC, REN, sUSD and sEUR tokens
  - New design for yveCRV backscratcher token and logo
- **yearn-exporter:** use new curve registry for lookups instead of hardcoded overrides, added all the new vaults
- **Roastee Starter Pack** created and used for onboarding
- **New developers** negotiated to join
- **Docs:** Wiki.js test instance to evaluate whether migrating user docs to.

### 1.2 Doing

- **Strategies / Vaults:**
  - Incentives for yvecrv on sushi
  - curve vaults to be made modular to be used by v2 strategies
  - stablecoin strategies to be updated for boosties
  - Document the process to add metadata to a vault
  - Migration plan
  - Adding minime balances to Vaults
- **Keep3r:**
  - testing vaults/strategy jobs with the new sugarMommy structure
  - simple version of RNG generator contract
- **Web:**
  - backscratcher ui
  - 2.1 sprint (2 weeks, started monday)
- **WeChat comms** next post
- **BizDev:** List of projects and their treasuries
- **Financial report**
- **Compensation plan**
- **New Treasury**
- **tokenWrapper** for integrators
- **yearn-exporter** further optimizations and adding stateful features so it can pick up registry and strategy changes from the chain
- **yearn.science**, to host a historical dashboard there, like https://dashboard.balancer.community
- **Integrations**, negotiating with a defi project for TVL
- **Partnership program**, MVP
- **Decentralized org chart**, for yearn's growth and roles definition
- **Mint process** CoinTelegraph OpEd
- **SDK:**
  - Add new underlying curve APY calculations to SDK
  - Update SDK to filter out non-tagged experimental vaults
  - Define and mock SDK interfaces
  - @andy8052's PR a

### 1.3 Todo

- **Strategies / Vaults:**
  - port v2-feasible strategies to v2
  - dca, stealth-txs, custom-swaps
  - review swap
  - review Pickle Strats BAS-DAI and MithCash
  - review port strats for v2
  - lean strategy review process
  - Upgrade Brownie and Add code verification script to brownie strategy mix
- **Web:** Fix remaining issues in subgraph for use in yearn API and website
- **Devdocs** forever in queue rip
- **Legal opinion** re YFI in EU, UK, SP
- **chief-multisig-officer**, extract useful stuff and release it as a library, add docs
- **release curve voting scripts**, done, but in need of testing
- **print yfi**
- **establishing compensation group**
- **YFI Legal Opinions**
- **Dev docs**
- **Vyper storage slot lifter**
- **Firehose:** Integration with VulcanizeDB
- **yVault migration**, using token wrapper

### 1.4 Blocked

- gas price levels
- vision-finding interviews on hold due to workload

## 2. Call-out topics

### 2.1 Mint: What happens now?

- Minting on friday
- No quorum requirement issues, FUD, has been 20% of _staked_ YFI, not supply. All have passed on that metric since YIP-12, YIP-55 removed all quorum requirements.

#### Compensation working group

- Launching today
- Nine people
- Pending a couple of mu-sig approvals
- Feedback from doers and community
- Aim to do it quick
- Goal to establish comp tiers
- How we work & roles
- Decentralized mgmt
- Compensation packages
- New hiring

##### Group members

- Vance
- Eli
- Santiago
- @onlylarping (yfi-matching proposal)
- Hat tip
- Banteg
- Klim
- Trach
- Lehnberg

#### Treasury

- what to do with 4444?

### 2.2 Partnerships / co-ops / integrations

_Misc discussion about ongoing deals._

#### Wrapper Token

Use cases:

1. vault registry, we release lots of new vaults, need vault migrations between versions, token that wraps vault positions, automated migration based on some instruction
1. could offer easy way to see how much TVL each partner contributes to
1. ability to do airdrops through the wrapper

Timeline est: couple of weeks to see if it meets use case

### 2.3 Vaults & Strats

Strategists boarding school are not deploying because of gas fees. Do we want to have a budget for those deployments?

#### Testing

- Learn how to deploy: Testnet
- Ganache
- Mainnet
- Strategist test-suite for mainnet fork?

#### UX

- Simplify vaults to have only base tokens as entry points?
- could be handled for curve
- more difficult for uni / sushi

#### yUSD

New yPool for 3 x v2 vaults -> yUSD v2?

#### ETH launch evaluation

- Last time there was no lido, eth2, or AH
- Good first case for a single base token?

#### Launch / deployment process

- how to deploy
- when to make it to the web page
- making announcements

### 2.4 Web site

- v2.1 team assembled
- Two-week sprint
- Making announcement on forums later today
- New UX person joining
- Stopped v2 website work (putting out immediate fires re alchemy)
- Focus is to make super easy with B2B integrators for yearn
- Heavy focus on SDK
- v2.1 - new repo using SDK, demo + template
