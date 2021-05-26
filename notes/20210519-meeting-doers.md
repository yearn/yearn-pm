# Meeting notes: Doers standup May 19, 2021

## Updates from
- facu
- tracheopteryx
- steffel
- jmonteer
- poolpi tako
- bull
- luciano
- doug
- guillermo
- dark ghosty
- bob the buidler
- nymmrx
- banteg
- klim
- wavey
- xgambitox
- gotzen
- dudesahn
- vany365
- sebastian
- x48

## 1. Weekly updates

### 1.1 Done
**Vaults/Protocol:**
- Protocol developers' charter
- Audit support & facilitation 
- Auto release changelog
- New smart contract monitoring/debugging tools
- [SNX](https://yearn.finance/vaults/0xF29AE508698bDeF169B89834F76704C3B205aedf) & [sUSD](https://yearn.finance/vaults/0xa5cA62D95D24A4a350983D5B8ac4EB8638887396) yVaults to production
- WOOFY depolyed on Fantom, Binance Smart Chain, and Polygon: `0xd0660cd418a64a1d44e9214ad8e459324d8157f1`
- yOracle proof of concept
- ySwapper proof of concept    
- Subgraph updates: addStrategy and StrategyReportResult
- Incident analysis of [strategy proxy](https://github.com/yearn/yearn-security/blob/master/disclosures/2021-05-13.md)
- Incident analysis of [single-sided curve strategy: estimate assets](https://github.com/yearn/yearn-security/blob/master/disclosures/2021-05-14.md)
- SDK MVP & updates
- Updated gauge weight voter for metapool support
- Disabled yvBoost zap
- Zap updates
- Test issue tracking tool

**Strategies:**
- Review complifi
- Review Vesper
- Update generic Aave lender/borrower
- Update PoolTogether
- Review KeeperDAO
- Review IDLE
- Review Rook
- Review yvBoost updates

**Strategist:**
- Strategists' charter
- Update vault strategy reports
- Update [strategy mix](https://github.com/yearn/brownie-strategy-mix) 
- KeeperDAO strategies deposit before fee deadline

**Keep3r:**
- Make keep3r-multisig [repository](https://github.com/keep3r-network/keep3r-multisig)
- Setup ENS
- Setup project board

**Coordinape**
- Review contracts

**Web/API:**
- IPFS hosting & metadata updates
- Integrate SDK/Lens updates into web v3
- Update UI/UX
- Custom themes
- Website v3 updates
- SDK updates

**Governance/Ops:**
- Compensation plan for new contributors 
- Vesting escrows for new contributors deployed
- Review website v3 UX/UI

**Treasury:**
- Reimbursements
- Evaluate cash burn run-rate to EOM April
- Revenue projections
- Update income statement
- Update [buyback table](https://github.com/yearn/ychad-audit/blob/master/reports/buy-backs.csv)
- Update ychad-audit for [April](https://github.com/yearn/ychad-audit/blob/master/reports/financial/2021-04-budget-report.csv)
- Deposit USDT in crvUSDN yVault: [Transaction 1](https://etherscan.io/tx/0xe5055e0dda3ff5d9a19291949d9157bf59a5f87a811077332cf1031a21a69e2c) and [2](https://etherscan.io/tx/0x04b28311618d8aabe4c590aebf8f6d3c9b7ecbe1a7155aac7b48735e6a81e8be)

**Comms/User Docs:**
- [Vaults at Yearn](https://medium.com/yearn-state-of-the-vaults/the-vaults-at-yearn-9237905ffed3) Updated

---

### 1.2 Doing
**Vaults/Protocol:**
- WOOFY crosschain liquidity mining
- yOracle deployment
- Iterate on ySwapper
- Research layer 2
- Subgraph updates
- Iterate superbooster
- SDK updates
- IPFS metadata
- Review automated vault management 
- Generalize veToken products
- v1 to v2 yVault migrations

**Strategies:**
- Deploy generic Aave lender/borrower
- Deploy sUSD's sETH/sBTC shorting

**Strategist:**
- Update review board

**Keep3r:**
- New queue job
- Keep3r-grafana board specifications

**Coordinape**
- Launch plan

**Community Sites**
- Make forum access redundant
- Yearn vision: updates & alerts
- Yearn hub features
- YFIStats updates & UI/UX improvements 

**Web/API:**
- Update v3 UI/UX
- Custom theme updates
- Update web v3 SDK
- Onboarding to issue tracking tool

**Governance/Ops:**
- Yearn vision draft
- Implement yGov v2
- Improve on organizational structure and project management
 
**Treasury:**
- April income and balance sheet
- Draft cash management plan

**Technical Docs**
- Push SDK documentation to repo

**Partnerships:**
- Review pickle jar changes

---

### 1.3 To do
**Vaults/Protocol:**
- Updates to Zaps
- Update emergency toolbox
- ySwapper
- Review veToken template
- Subgraph updates
- Update missing logos
- New yvBoost zap
- RAI vault
- Rollout issue tracking tool
- yApeScanner updates

**Strategies:**
- Big borrower

**Keep3r:**
- Protocol upgrades
- Update keep3r jobs repository

**Community Sites**
- Yearn hub fixes
- Yearn vision updates: historical APY

**Web/API:**
- Web v3 updates
- UI updates

**Governance/Ops:**
- Finalize growth candidate onboarding & review plan
- Feedback on yTeam signers draft
- Test new coordination tool
- Yearn engineering assessment meeting    

**Treasury:**
- Yield farming analysis & optimization

**Technical Docs**
- Review guidelines/checklist
- Update SDK documentation

**Comms/User Docs:**
- Schedule AMA

---

### 1.4 Blocked
- Final v3 design