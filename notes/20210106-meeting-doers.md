# Meeting notes: Doers standup call Jan 06 2021

**Attendance:** Banteg, Bull, Doug, Doggie, Dudesahn, Facu, Gabe, Graham, Klim, Lehnberg, Luciano, Orb, Trach, WrongNebula, x48

## 1. Updates from the standup

### 1.1 Done

- **Test UI for v2 vaults**, registry at https://yearn.rocks
- **Vault v2, audit #3 secured**, evaluated security firms, signed agreement with one provider, ETA April
- **Alchemy plan**, agreement negotiated and agreed
- **UI design work**, new icons, infocards, components, notifications, cream integration
- **Vault registry**, relatively stable now
- **Telegram bot** announcing big vault movements
- **2020 hoodies**, together with loldefi
- **Holiday cards distribution**

### 1.2 Doing

- **GUSD vault issue**, due to old strategy not revoked properly, compensation due to the few affected
- **Strategy audits**, unsustainable and inefficient to do security audits, peer reviews preferred, github project set up and reviews are underway.
- **New YIPs in progress:**
  - **Governance**, proposal to come in jan
  - **Aragon**, proposal eta tbd
  - **YFI buyback**, proposal expected within the next week
- **Strategy process document**, draft ready for review
- **yAcademy**, kernel kicking off, alignment call with yAcademy team
- **Integrations**, discussion with several partners underway at various stages
- **Mixbytes auduit**, results are back, addressing changes to vault code and base strategy code
- **Vault v0.3.0**, release imminent
- **Ecosystem bootstrap**, recent operations call did not have a lot of attendance
- **Emergency crisis process document**, wip
- **Keepers avoiding front running**, iterated on to create a smart contract to force keepers to use Taichi network.
- **Website v2 UI**, first design nearly complete:
  - v1/v2 support using registries
  - dev mode
  - cover support
  - historic charts
  - cream integration in progress
- **Lite mode v2 website**, nearly complete:
  - First iteration UX mimics current Yearn UX
  - Tabular approach, zapper like experience
  - Allowing rapid iteration with reusable UI components
- **Firehose**, new real-time back-end infrastructure:
  - Utilizes redis pub-sub over websockets
  - Subscribe to a protocol with appropriate args (account, for instance) and receive a cached/current state for the protocol
  - Any new state updates will be pushed to subscribers over websocket
- **Skeleton UI**, ultra-lightweight UI:
  - First site to integrate with Firehose
  - Provide a bare-bones real-time Yearn UI implementation
  - No more manually adding vaults/cover/cream assets, all updated automatically based on on-chain changes

### 1.3 To do

- **Vault v2 launch project**, kick off pending other priorities
- **Gitcoin yearn collection**, to make it easier to sponsor yearn projects
- **Automated Dev documentation**, pending other tasks

### 1.4 Blocked

- **Treasury**, blocked by pending YIPs

## 2. Other topics

### 2.1 Meeting format iteration

- Starting next meeting, written updates to be submitted ahead of time
- First part of meeting used to call out key topics to discuss that's relevant for all
- Use telegram and pinned chats to keep track of progress

### 2.2 Keeper credits

- Need to manage better, impressive the system is working so well that it's almost forgotten
- Potentially use a keeper job to replenish keeper credits
- Dashboards? Could use firehose

### 2.3 Transaction batching

- Technical discussion related to how to send transactions more efficiently from vaults
