# Meeting notes: Doers standup call Jan 27 2021

## Attendance

- Doggie
- Santiago
- Facu
- Klim
- Trach
- Bull
- x48
- Dudesahn
- Luciano
- Orb
- Doug
- Lehnberg

## 1. Weekly Updates

### 1.1 Done

- **Strategies/Vaults:**
  - fix unwinding issue on weth v1 vault
  - reactivate weth v1 vault
  - review strategy proxy contract
  - fix interface on strategies
  - full test on curve lp vaults/strategies with the new proxy changes
  - set audits for pending strats
- **keep3r:**
  - metaKeep3r v1.0 structure
  - liquidity
  - KeeperEscrow
- **Chief Roastees:** dudesahn (web) & Facu (strats / protocol)
- **yearn.rocks** refactored tags added
- **yyBoarding School** created for new strategists
- **Minting proposal** proposal iterations and feedback repsponse
- **Minting keys** discussion split out to a separate thread
- **Web:**
  - tentative near, mid, and longterm plan
  - potential contributors and advisors collected for help
  - pending web ecosystem work organized into a HackMd
  - catalog web ops processes currently missing
  - Improve APY calculations
  - Organize and test new API work
  - Set up CI for develop version of v1 yearn.finance
- **SDK:** Requirements work
- **Yearn web help** group created
- **Telegram purge** various groups culled

### 1.2 Doing

- **Strategies / Vaults:**
  - vault all gauges to incentivize backscratcher vault
  - draft procedure for v2 strategies testing
  - Investigate deployment process
  - 3rd vault audit paid and confirmed
    -define ops checklists for vaults and strategies operations
- **Keep3r:**
  - update keep3r job interface
  - designing keep3r job for v2 strategies
- **Web:**
  - Akro frontend
  - Interview firms and candidates
  - Create RFP for a new frontend
- **Integrations:** various ongoing discussions
- **Multi-sig audit** for January
- **Strategy** ongoing discussions
- **stealth txs**, how not to rekt keepers or watchers on uncle blocks
- **custom swaps** dex-aggregator wrapper and tests
- **dca**, incentives and review work on internal-swaps
- **Nov/Dec Financials**, waiting on updated data
- **Docs repo:** Working through PR backlog, fixing broken github actions and trying to improve workflow in general
- **More devs** Conclude negotiations to onboard more
- **Roastees:** Prepare chief roastee starter pack

### 1.3 Todo

- **Strategies/Vaults**
  - Deploy FreedomSwap
  - Create some health controls
  - Refactor strategists onboarding
  - Create ops checklists
  - Define short steps for a lean process for reviewing v2 strategies
  - Upgrade Brownie and Add code verification script to brownie strategy mix
- **Mint YIP:** submit for vote
- **Compensation working group** kick off
- **Firehose** Finish refactor
- **Keep3r**
  - Test & Deploy Keep3rSugarMommy
  - Deploy stealth txs to be used on keep3r jobs
  - keeper-escrow-job for auto-refill-utopia
- **Devdocs** forever in queue rip
- **Legal opinion** re YFI in EU, UK, SP

### 1.4 Blocked

- Speed of gov msig
- Solid sdk
- solid mobile version
- Financial report
- Verifying vault revenue numbers

## 2. Call-out topics

### 2.1 SDK

- Read methods for APY, vaults, strategies
- Write methods wip
- Good start
- Documentation on interfaces
- Transport agnostic: read/write using different options
- Possible ability to migrate user from older vault to newer

### 2.2 Affiliates & Strategy

- Yearn is better at infrastructure
- Others are better on customer facing solutions i.e. zapper debank zerion
- Difference between custodial & non-custodial partners

### 2.3 Web plans

- Should still have the app, available for end users
- More about SDK more about vaults
- Still requires a solid front-end and have it maintained

### 2.4 Vault strategies

#### Migration

- V1 withdrawal fee creates problem with composability
- A holistic v1 strategy required in the context of v2
  - Which strategies/vaults do we keep as v1?
  - What are their fees moving forward?
  - Which strategies/vaults do we migrate to v2?
- A v2 vault that wraps the v1 vault?
- Keep legacy strat but take out fees?

#### yETH relaunch

- contract is live
- v1 site is now updated
- v2 site needs work

### 2.5 Current website work

- Akro Trade
  - 2-3 months, lots of work for them to do a UI for us, trade where we help them with protocol work and they do front-end work for us
- Head of design? Product? How does yearn do this?
- We need to hire help
  - The more pro react devs the better (4)
  - Someone for UX (1)
  - Need mobile design (1)
  - Need 1 (preferably 2) full-time react developers long-term

### 2.6 Planning tools

- JIRA
- Github issues/projects
- Notion, [example](https://pasteboard.co/JLARWu4.png)
- Criteria
  - export to md
  - internal wiki
  - kanban board
  - uses
    - meeting notes
    - project briefs
    - team resources
