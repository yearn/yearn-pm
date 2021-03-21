# Meeting notes: Doers standup call Mar 17 2021

## Attendance

- Facu
- Luciano
- Banteg
- x48
- trach
- milkyklim
- dudesahn
- darkghosty
- doug
- D Dog Ser
- bull
- orb
- lehnberg

## 1. Weekly updates

### 1.1 Done

**Vaults/Protocol:**

- Registry upgrade
- Wrapper improvements
- 0.3.3 Vault release
- Script to check vault governance and deposit limit using yearn-exporter
- Follow ETH v1 unwinding
- Migration Pulse
- Initial work on "lens" contract
  - Multi-registry asset aggregator
  - On-chain TVL calculations
  - Multi-asset user positions
- migration roadmap
- IB vault launched
- Signal request to increase maker debt ceiling for yfi
- Paid back old weth strategy cdp to wind it down
- yearn-exporter rewritten so it can support historical data.
- Historical tvls cracked

**Strategies:**

- PT strat
- IB curve strat
- yvBOOST
- HBTC security info
- yfi maker v2
- weth maker v2
- IBCurveVoterProxy strategy
- YearnVECRV strategy
- $105m rescued from BDP farm
- POC web dashboard for strategies settings review before preparing drill

**Keep3r:**

- re-adapted all keep3r jobs
- keep3r harvest/earn script

**Web/API:**

- Roles and workflow revised
- Net APY on website
- UX community shareout

**Governance/Operations:**

- Scheduled ecosystem ops call
- 1-month comms project kicked off
- 1-month engineering project kicked off
- 0.03% plan, meeting upcoming
- Growth lead interview
- Colony <> Yearn partnership plan draft
- Coordinape: beta test UX and plan
- yGift: new UX/UI designer for yGift v2
- Early draft of a long-term vision / strategy document for yearn
- NFT liquidity mining brainstorm

**Treasury:**

- LM proposal
- February income statement
- Reimbursements for Klim
- Repaid dai debt
- Vesting escrow deployed

**Partnerships:**

- 81 partner leads categorized as gh issues+board to track
- List now down to 68 open tickets, 32 P1s, 19 P2s, 17 P3s
- Reach outs, lots of DMs, 3 phone calls

### 1.2 Doing

**Vaults/Protocol:**

- Adding alerts to grafana
- Adding fees and telegram notifications to the brownie script

**Strategies:**

- yvBOOST nft deal
- Curve template
- Single side template
- Update Iron Bank Strategy to be more gas efficient

**Keep3r:**

- new keep3r auto-credit escrow job system (3rd time is the charm) [public use]
- onboarding steffel to keep3r jobs (create restricted Keep3rV1OracleJob) [might be a bit tricky]
- Support strategy descriptions
- allocate kpr/eth liquidity

**Web/API:**

- zaps in v2 ui
- Finish on-chain TVL stuff
- Finish touches with yearn-exporter before adding an api for aggregators like defipulse, defillama to consume
- Finalize zapper zaps, coordinate announcement
- v3 app designs finalized this week
- Coordinate v3 web implementation

**Governance/Operations:**

- Onboard dedicated cmo resource
- Vision doc
- Next full draft of org structure that's more actionable
- Next step in gov, clean up and share out phased plan internally
- Next steps for growth lead recruiting

**Treasury:**

- February balance sheet

**Partnerships:**

- Partners: 1 pager use cases and solutions to converge around
- More lead generation follow ups
- 2+ more partner calls scheduled this week
- Integration for YFI + legal work as required

### 1.3 Todo

**Vaults/Protocol:**

- figure out a better path forward on migrations
- dca + custom swaps
- research optimism and zkOr for bridging pattern to vaults
- phase 2 migration

**Strategies:**

- Launch new IB strat and increase deposit limit so we can move to main site

**Keep3r:**

- v2 keep3r tend bot

**Web/API:**

- Integrate lens contract into SDK/website

**Governance/Operations:**

- Coordinape medium article about theory, concept, future
- Coordinape funding plan
- Coordinape surveys, interviews, and beta test
- Coordinape payout from alpha
- yGift project lead and future
- Map out all hiring goals and establish better tracking system

**Treasury:**

- Quarterly report
- New budget
- Quantify treasury farming profits vs. debt expenses
- Insurance backstop module potential APY modeling

**Partnerships:**

- Retroactive payments

### 1.4 Blocked

- Time split between too many different goals: general ops, hiring, org structure, governance, coordinape
- Cvp to roll out lazy ape zap
- Uniquote escrows for keeper to be finished
- v2 basestrategy template

## 2. Call-out topics

### Engineering project

We've tasked researching how engineering works at yearn. Basically interviewing a bunch of people that touch development in one way or another and gather what they thought worked well, what could be improved, and what ideas or recommendations they might have. Task is to collect everybody's feedback and put it together for us, should be done over the next month or so.

### Coordinape & yGift

- Should Coordinape and yGift be independent or part of yearn? Who should do the work, oversee it, and how should the projects be funded?
- Can anyone start a project and it's yearn's responsibility? Where is the line drawn?
- Should Coordinape be developed by the dev team at yearn?
- Can yAcademy be a model? Incubator?
- Potential other projects that could use co-ordinape: Sushi, Badger
- Can it be run as a recruitment pool for dev talent?
- Nobody is running yGift right now
- How do the projects interface with Yearn? Same way as yAcademy?

### v3 site launch

- Planning for launch: coordinating with comms, docs, mods, etc.
- Rough deadline for first release April 9th
- Test period one week ahead, doers should co-ordinate to be awawre and make sure everything runs smooth
- All to focus w/o April 1 on website
- Weekly update in Doers
- Produce launch video material: Dudesahn tracking

### Vaults Migration Status

- ETH unwinding done
- Endorse stables this week, co-ordinate migrate balance on web site
- Phase 2: Registry ready. Next steps is to decide on vaults / architecture for migrations / alignment in call tomorrow.
- WBTC: a v2 needs to migrate to another v2

### Strategies

- Only ETH vaults on yearn.finance
- Testing potentially risky strats from "newer" protocols in prod with 1% debtRatio vrs going to ape tax first, thoughts on process?
  - Check numbers on new vault/strategy going live as part of the approval process - strategy pitches
  - we have a process of checking security around the code
  - We do not have a process of understanding ROI vs risk - due dilligence
  - 1% of funds at risk makes sense if it's from a well known / tested protocol, not otherwise
  - Testing is what ape.tax is for, for more unknown protocols
- Prioritization
  1.  Vaults with higher liquidity tokens (USDT, WBTC, LINK etc)
  2.  Vaults and strategies that target Curve/boost gauge
  3.  Strategies that boost APY from current deployed production vaults
  4.  Strategies that boost APY but use a "brand new" protocol that no one else has tested in a vault or strategy need experimental first and due dilligence from security perspective. Review the underlying protocol code to check for issues.
  5.  Vaults and strategies with low liquidity tokens

### Keep3r / Uniquote

- if you provide liquidity, you provide liq for all token pairs.
- ideally should only provide liq for tokens you use
- can we remove _some_ pairs?
- can we fund only ETH/Keep3r and let everything else be
