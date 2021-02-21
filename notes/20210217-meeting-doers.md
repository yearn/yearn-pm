# Meeting notes: Doers standup call Feb 17 2021

## Attendance

- bull
- facu
- banteg
- doggielicious
- darkghosty
- doug
- klim
- dudesahn
- luciano
- lehnberg

## 1. Weekly updates

### 1.1 Done

- **Vaults/Protocol:**
  - Final plan for v1 -> v2 migration
  - ydai early withdrawals reimbursed
  - vesting escrow contracts
  - New general zap UI component for yearn.rocks makes it easy to add zaps for test vaults
  - New v2 board to track progress
  - yBacklog board to track features that are on long(ish) term
  - yToken & AffiliateWrapper masterclass
  - Bonny v2 vault released with several fixes
  - Registry release
- **Strategies:**
  - wethmkr strategy debt fixed
  - OPERATIONS.md refined further
  - Mushroom wBTC strategy reviewed
- **Keep3r:**
  - unbonded LPs from deprecated mommy job
  - Yearn Proxy Keep3r Job
  - randomization contract for keep3r network to use
  - YFI mechanics group for maintaining keep3rs
  - monitor created for earn/harvest
- **Web/API:**
  - fork-net for frontend development
  - Lots of meetings/workshops/decisions/progress
  - Streamlined communication and roles for website and web group
  - Rough timeline for website
  - Mainnet fork up and running for QA
  - APY calcs improved
  - Remaining tasks for website v2.1 organized
- **Governance:**
  - YIP-57 mostly done, comp plan finalized
  - Interviews and 1:1s
  - multisig participation rate surveyed
  - Treasury Yield plan
  - YIP proposal to extend multi-sig released
  - All financial debts processed: grants, payments and gas
  - Donated YFI returned 2xed
- **Partnerships:**
  - lots of silk glove partnerships comms
  - internal alignment on partnerships approach reached

### 1.2 Doing

- **Vaults/Protocol:**
  - Review wrappers
  - Simple UI for vesting escrow contracts
  - Housekeeping yearn-protocol and v2 vaults issues and PR
  - Add Permit and gasToken to support to migrator to subsidize gas for users on v2
- **Strategies:**
  - Move WBTC 🍄 to production
  - Track BSC tests
  - Step 1 on curve v2 experiment
  - Glitches in curve v1 better for future migration plan
  - Curve structure in v2
- **Keep3r:**
  - Finish refactoring jobs to work with Proxy job.
- **Web/API:**
  - Release v2.1, improved APY calcs and info, tweaked UI/UX
  - Continue work on v3, new UI/UX flow, first to be released as a standalone app
  - Finalize TVL endpoint
  - Finalize APY in UI
- **Governance:**
  - January financials
  - Submit aave proposals
  - yChad audit
- **Comms/Docs:**
  - Onboard Chinese community help
- **Partnerships:**
  - Add more to projects' treasury doc
  - Documentation for partners
  - Partnership form & comms

### 1.3 Todo

- **Vaults/Protocol:**
  - DepositWrapper for v2 migration
  - Define zap approach to go with in house zapper like approach or zap per vault contract or integrate with zapper directly
  - Add backscratcher to subgraph mappings
  - Fix hardhat to integrate with brownie and improve testing on all our repos
  - Graph offical yearn repo
  - Add system vaults status checks to grafana
- **Strategies:**
  - Doc & video with resources to onboard new boarding school members
  - Port many already-done strategies to v2
  - Beginrepaying dai debt
  - Boost backscratcher even more
- **Keep3r:**
  - Recover and bond escrow LPs from mommy to proxy job
  - Add more jobs (yearn relayer, and deployer)
  - Internal contracts draft, using keep3r.network as a safeguard, or for no-risk jobs.
  - Improve yearn-keep3r-jobs repo with proper CI and tests
  - Build infra around monitoring and automation
- **Web/API:**
  - Create process to add Metadata
  - Get updated TVL for DeFi Pulse
- **Governance:**
  - Review bug bounty top tier
  - Legal opinions
  - Draw clean in\out budget flow
  - Define Treasury yield farming approach
- **Comms/Docs:**
  - Dev docs
  - More copywriting help for website
- **Partnerships:**
  - term sheet for partner project

### 1.4 Blocked

- ychad for January

## 2. Call-out topics

### Use minted YFI in Treasury to farm & service yDAI debt

- 2800 YFI left
- sushi, bancor, yvaults all options
- Capture all DAI available in Maker
- Should we be agnostic to eth?
- Bull to prepare detailed farming proposal

### Vaults / Strategies

#### Zaps

- Build ourselves or work with Zapper
- zapper does single contract handling all zaps
- uses offchain component for routing
- simplest way is to do a simple contract, but requires 1:1 mapping
  - 1 week turnaround
  - expensive on gas
  - not upgradeable
  - redeployment of contracts when there's new tokens
- best engineering approach: 1inch style off chain routing a la zapper
- zapping in and out of vaults: a priority
- zaps between vaults: nice to have
- seems sensible to focus on core business for us, and work with zapper on zaps
- can always be revisited based on need

#### Curve voting

- vote based on TVL? least political thing to do, codified
- vote based on maximizing vecrv?
- limit vault deposits to % of gauge equal to % of our vecrv to maximize yield?
- do some maths to figure out optimized approach
- banteg to do plan / proposal and we take it from there

#### yLINK, yaLINK and yYFI

- aave based strategies with v2 aave tokens
- "you can get 20% on your link on v2, marine"
- Facu to drop in strategists as a idea for them to pursue via Sam

### New projects

- Do we plan to build out the Yearn Ecosystem / finish some of Andre's prototypes? Do we just need devs?
- there's a desire, pick the core one
- Subset:
  - ydelegate - uses aave v2 delegated credit, only creates positions doesn't balance positions. if you have credit available it shows up in the UI
  - leveragex - create flashloan to leverage the asset. pick long, short, collateral.
  - yTrade - leveraged fx trades. needs LPs.
  - options.crv.finance - not keen to push that, hegic base rewards mostly negative, underlying protocol not making money
  - defi starter - kickstarter for defi projects
