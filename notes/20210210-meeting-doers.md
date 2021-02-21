# Meeting notes: Doers standup call Feb 10 2021

## Attendance
- luciano
- x48
- facu
- banteg
- darkghosty
- orb
- doug
- bull
- klim
- dude
- doggie
- trach
- lehnberg

## 1. Weekly updates

### 1.1 Done

- **Decentralized org chart**, draft shared
- **ETHDenver talk**, on Yearn org
- **Brrr:**
   - **Compensation working group** launched
   - **YFI printed** successfully
- **Coordinape** contributor team 
- **Design:**
   - yveCRV token (backscratcher new logo)
   - yveCRV-ETH Sushi onsen visual (spirited away)
   - yveCRV-ETH SLP on Pickle visual (banteg floating in pickles)
   - cDAI, cUSDC, cUSDT, aDAI, aUSDC, aUSDT tokens + aLINK token rework
- **yveCRV:**
   - updates to crv.ape.tax
   - listed on coingecko
- **yDAI exploit:**
   - Disclosure published
   - cdp opened to rescue the vault
   - Reviewed improve strategy
- **Strategists:**
   - First weekly call
   - Published new version of OPERATIONS.md
   - Review SingleSidedAssetStrat
- **Vaults/Protocol:**
   - First triage of issues
   - build zap contract to migrate v1 to v2
   - Review USDT
   - Review gas token integration
- **Keep3r:**
   - New repo for Keep3r jobs 
- **Partnerships:** 
   - misc negotiations
   - Initial rev share table drafted
- **ARC** for no borrowing of YFI written
- **Docs call** arranged
- **Income statement and balance sheet** for Nov/Dec 
- **Treasury Management plan**
- **yearn-exporter**, dashboard and feedbacks for dockerized version

### 1.2 Doing
- **Comms:**
   - CoinTelegraph OpEd
   - Defi / crypto treasuries list
   - Chinese wechat newsletter
   - Coingecko listing of vaults
- **Design:**
   - BT finance, Dollar Protocol, Origin Dollar tokens for cover
- **Vault/Protocol:**
   - Make yDAI and yETH whole
- **Strategies:**
   - Improve normal migration and emergency procedures
- **Keep3r:**
   - call applyCredits on meta-job to get credits on SugarMommy
   - deploy new meta-jobs
   - work on yearn contract deployer meta-job
- **Governance:**
   - Org chart
   - Compensation plans
   - Aave proposals
   - Jan Financials
- **Partners:**
   - Documentation 

### 1.3 Todo
- **Docs/Comms:**
   - Check on Miya for Chinese PR
   - Kickstart Chinese contributors group
   - Touch base with translators
   - dev docs
   - get decision on yWiki
- **Web:**
   - Fix remaining Subgraph issues to integrate and use in yearn API and website
   - tg\twitter bots to show apy regularly 
   - fix apy calucation
- **Vault/Protocol:**
   - Pay off CDP for ydai
   - Tools to monitor the cdp and scripts to rebalance it
   - pay gas 
- **Strategies:**
   - Create a video to onboard strategists to v2
   - Deploy contracts to a testnet (Boarding School, maybe use BSC 👀?)
   - Write short steps for a lean process for reviewing v2 strategies that we can use as base
   - Ideas to avoid sandwich attacks
- **Governance:**
   - Multisig Transition (high priority)
   - Collect specs for the new treasury
   - pay grants 
   - add report for ychad 
   - create proper treasury management 
- **Partnerships:**
   - term sheet for partner project

### 1.4 Blocked
- Gas price is too damn high


## 2. Call-out topics

### Exploit status/aftermath
- Maker vault
    - 9.7m, 1m extra might be needed for eth vault
    - two snapshots required count diff
- Tether: Contact CTO, try to get funds back 
- Aave proposals: good to deepen partnership with them 
- Cream: Deepen co-opeartion further

#### How do we pay the DAI loan?
   - farming with treasury
   - diverting baby
   - depends a bit on priorities
   - need data/forecast for time to repay 

### Vaults & Strategies

#### Vaults v1 -> v2 plan
- Are we heading towards single token deposits to replace Curve? 
- Plan to migrate Curve v1 strats to v2?
- Wrap the v1 vault and treat it as a strategy for a v2 vault, offer single side deposit?
- Latest fix for Dai v1 has mitigation, public `earn()` cannot be enforced.
- Possible sandwich mitigations: 
   1. no deposit+withdrawal in the same block as harvest
   1. earnings maturation for 6 hrs 
   1. withdrawals using a lagging share price from 6 hrs ago 

#### BSC for boarding school / strategy testnet 
- Using BSC and Testnet for boarding school.
- BSC demand way more time from core devs/strats than a 100% school-managed testnet
- Yearn on BSC for Boarding School
- strategists in training
- low fees
- bring experience to ethereum
- help build relationship with binance
- don't distract the core team
- don't trust the system with huge amounts, keep it small ball
- Yearn's kusama?
- NO BRIDGE

#### Content/onboarding material for v2 strategies?
- Video to onboard new strategists? Maybe record a live dev AMA session (?) 

### Partnerships / Integrations
- Several in early discussions
- Rev share tiers evaluated

### Multisig transition proposal

YIP-41 expires this month. Preliminary draft of the multisig transition proposal Gabe and Trach wrote a while ago shared. Gives an idea of what was in mind but needs a lot of work still.