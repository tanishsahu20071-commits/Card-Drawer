# Card Drawer

## Project Description
The Card Drawer contract provides a simple system for drawing and storing cards on the Stellar blockchain. It allows addresses to draw cards and retrieve their drawn card, creating an immutable record of card draws. This contract is useful for games, lotteries, or any application where random card selection needs to be recorded permanently. The blockchain ensures that card draws cannot be tampered with, providing fairness and transparency.

This contract is ideal for gaming applications, lottery systems, trading card games, or any scenario where card selection needs to be verifiable and tamper-proof. The immutable nature of blockchain records ensures that once a card is drawn, the result cannot be changed, providing complete fairness and transparency for all participants. This makes it perfect for applications where trust and verifiability are crucial.

**Key Benefits:**
- **Fairness Guaranteed**: Card draws are permanently recorded and cannot be altered
- **Transparency**: All draws are publicly verifiable on the blockchain
- **Tamper-Proof**: Once a card is drawn, the result is immutable
- **Trustless System**: No need to trust a central authority for fairness
- **Audit Trail**: Complete history of all card draws is maintained
- **Gaming Applications**: Perfect for online games, lotteries, and card games

![Contract Explorer](img/contract-explorer.png)

**Contract Address:** `CATQMW2YNPRWRT7GB6HOQIUJMBR2KXB73Z6NX52V3ETBWGE6SXWNAYDZ`

**View on Stellar Expert:** [https://stellar.expert/explorer/testnet/contract/CATQMW2YNPRWRT7GB6HOQIUJMBR2KXB73Z6NX52V3ETBWGE6SXWNAYDZ](https://stellar.expert/explorer/testnet/contract/CATQMW2YNPRWRT7GB6HOQIUJMBR2KXB73Z6NX52V3ETBWGE6SXWNAYDZ)

## Features
- Simple getter function to retrieve drawn cards
- Simple setter function to draw and store cards
- Basic storage model using address-to-card mapping
- Minimal, gas-efficient logic

## Functions
- `draw_card(address, card)` - Draws and stores a card for an address
- `get_card(address)` - Returns the card drawn by an address

## Building the Contract

To build use:
```bash
stellar contract build
```

## Deploy to Testnet
Run:

```bash
stellar contract deploy \
  --wasm target/wasm32v1-none/release/project-4.wasm \
  --source-account alice \
  --network testnet \
  --alias project-4
```


