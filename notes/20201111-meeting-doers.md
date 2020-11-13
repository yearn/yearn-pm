# Meeting notes: Doers standup call Nov 11 2020

**Attendance:** Banteg, Bull, Doggie, Facu, Graham, Klim, Lehnberg, Luciano, Santiago, x48 (sent written update)

## 1. Updates from the standup

### 1.1 Done
- **[YIP-51](https://gov.yearn.finance/t/yip-51-set-vault-v2-fee-structure/7752): Set Vault v2 Fee Structure**, written and passed.
- **[YIP-52](https://gov.yearn.finance/t/yip-52-make-strategist-skin-in-game-partner-for-make-benefit-of-glorious-brain-of-yearn-voting-open-nov-9-nov-12/): Increase strategist rewards,** written and passed.
- **Vyper source code documentation generator**, poc created, and test [live](https://app.gitbook.com/@lehnberg/s/yearn-docs-test/untitled-1).
- **POAP for YFI NFT**, [live](https://poap.delivery/yfi-og/)
- **YFI on Maker**, onboarding complete.
- **keep3r live**, running jobs for ycrv 3pool yusd
- **Vault logos**, final version complete
- **YFI approved for Monolith**, with yUSD to follow
- **Mixbytes agreement** for audit
- **Aug-Oct Financials** done
- **YTD Financial performance** done
- **Backscratcher vault UI** [live](https://crv.ape.tax)
- **Web development:**
   - Drizzle integration working
   - First pass at vaults page, looking good
   - "Dev mode" playground added:
       - Add arbitrary contracts to local UI and view real-time updates
       - Add and interact with test vaults
       - Access to all write methods for a contract (deposit/withdraw/earn, etc)
       - Enable power user features for normal UI
   - Confirmed subdomains are safu

### 1.2 Doing

- **YIP-54: Formalize Operations Funding**, in progress 
- **Add more keep3r support**, comp and gusd for crv strats, dforce usdc maker dai
- **yGift core review**, one bug found further scrutiny pending
- **Pickle strategy**, migrations and further improvements
- **Refactoring web API**, lint restructure, make APY API utilize vault registry (was built before vault registry existed).
- **DCA trading of ERC20s**, continued work in progress.
 

### 1.3 To do
- **Better strategy visualization**, preferably writing and maintaining it in code.
- **Vault2 flows**, and additional documentation.
- **yUSD2**, proposal for the next iteration.
- **compound vault**
- **vault migration for v2**
- **Front-end:**
   - Finish first pass at vaults page.
   - Implement governance staking page.

### 1.4 Blocked

- **Subgraph re-write**, due to time constraints.
- **CeFi Exchange Integration SDK**, waiting for Gemini to get back to us.

### 1.5 No update since last meeting

- **Treasury mgmt process document**, currently being drafted.
- **Grants structure proposal** is in progress, led by Substreight.
- **Argent integration**, in progress and their team have confirmed it should be ready soon.
- **Yearn Grafana dashboard**, in closed testing to be rolled out wider soon.
- **Governance swaps POC**, to allow harvesters and keep3rs to get better trades for token pairs, working with uniswap already, possibly to add sushiswap and 0x for less slippage in certain pairs.


## 2. Other topics

- **Multi-sig signer wanted**, to replace Klim due to lack of time.

