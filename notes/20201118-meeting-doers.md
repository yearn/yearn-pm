# Meeting notes: Doers standup call Nov 18 2020

**Attendance:** Banteg, Doggie, Facu, Graham, Klim, Lehnberg, Luciano, Orb, Santiago, x48 (sent written update)

## 1. Updates from the standup

### 1.1 Done

- **[YIP-54](https://gov.yearn.finance/t/yip-54-formalize-operations-funding/): Formalize operations funding**, written and passed.
- **Vault logos:** first iteration final
- **Localization:** three more languages added to docs
- **Generalized keep3r bot**, that can be tailored to specific strategies
- **Web development:** First pass at vaults page for v2 yearn UI being tested with developers, new functionality include:
   * notify.js
   * support for "dev mode" contract watching
   * support for easily calling write methods
   * generic modal that allows any write method to be called
   * batching contract state update requests (one json-rpc call instead of 100+)
   * websocket server that caches vault transaction and state and broadcasts state/tx diffs when contracts are touched in a block, **front-end demo** live at http://yevents.finance

### 1.2 Doing

- **POAP:** In progress, should be finished next few days
- **yHegic Vault:** Further testing
- **Feeltheyearn API update** improving responsiveness and data structure
- **New keep3r strategies**, thoughts around mitigation of exploits of `harvest()` and `earn()` function calls
- **DCA trading of ERC20s**, continued work in progress.
- **Review of forum structure**, work in progress
- **Strategy visualization** testing, experimenting with generating from code
- **YIPs repo** housekeeping and keeping it up to date
- **Vaults v2 audits:** mixbytes in progress, chainsecurity lined up for Nov 26
- **Vaults 0.2.0** release inbound with changes to strategists API and how deb reporting is done
- **yGift** code review in progress
- **Vaults guest list functionality**, restricting deposits based on qualifying criteria such as whitelist or token holdings
- **Multi-sig scripts** to make maintenance easier
- **Subgraph re-write**, handed over to chris.eth
- **DeBank** now lists Yearn and shows [accurate TVL](https://debank.com/ranking/locked_value)
- **v1 stablecoin strategies fixed**, no longer vulnerable to attacks, possibly worth considering deploying some again on v1 still? (discussed further below)
- **Yearn web UI v2**:
   - Refactoring to use batched requests as above, possibly also adding support for configurable batch sizes.
   - Integrate websockets support (yevents)
   - Update pending that drastically increases the stability and decreases lag due to re-renders
   - Load limit testing (load 100 watched contracts, for example)

### 1.3 To do

- **Maker YFI strategy**, maker is increasing debt ceiling to \$20m YFI -> get YFIUSD oracle whitelisted on maker to create a strategy for this.
- **Vault2 flows**, and additional documentation.
- **Compound vault**
- **Test v2 sandwich attacks**
- **Yearn v2 UI:** Begin implementing other Yearn UI v2 pages, like stats and governance staking.

### 1.4 Blocked

- **yUSD2**, put on hold, more research needed to understand motivation.
- **CeFi Exchange Integration SDK**, discussion has progressed a bit with Gemini, still not clear when we can move on it, but talks about launching vaults v2 with the GUSD vault (more below).

### 1.5 No update since last meeting

- **Treasury mgmt process document**, currently being drafted.
- **Grants structure proposal** is in progress, led by Substreight.
- **Argent integration**, to be followed up on.
- **Yearn Grafana dashboard**, in closed testing to be rolled out wider soon.
- **Governance swaps POC**, to allow harvesters and keep3rs to get better trades for token pairs, working with uniswap already, possibly to add sushiswap and 0x for less slippage in certain pairs.

## 2. Other topics

### 2.1 Vault v2 migration plan

Summary:

- Phased rollout, starting with smaller strats first with low TVL
- Anything above \$10m we want to avoid migrating early
- **veCRV** vault to stay on v1 as there's no withdrawal
- **yUSD** given TVL and complexity may not ever move over, tbd
- **GUSD** to be the initial launch strategy for vault v2, given low TVL, low risk, and positive for Gemini relationship
- **TUSD** strategy to be upgraded by Orb and then re-opened on v1 still, no need to wait for it to v2