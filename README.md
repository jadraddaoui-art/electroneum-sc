#  Smart Chain

 Smart Chain implementation based on go-ethereum.

 Smart Chain is EVM-compatible, supports all the existing Ethereum tooling, provides nearly instant transaction verification and 1-block finality with a modified version of the Istanbul Byzantine Fault Torerance (IBFT) consensus protocol.

## Key Features

### IBFT Consensus Protocol

 Smart Chain implements a modified version of the standard IBFT proof of authority consensus protocol, making it the perfect consensus algorithm for public blockchains with a consortium of publicly-known validators participating in the block creation. Existing validators propose and vote to add or remove validators through our on-chain voting system.

This state-of-the-art consensus protocol features:

- **Immediate Finality:** blocks are final, meaning there are no forks or concurrent alt-chains, and valid blocks must be in the main chain
- **Nearly Instant Confirmations:** blocks are created every 5 seconds
- **Dynamic Validator Set:** validators can be added or removed from the network by an on-chain voting mechanism
- **Optimal Byzantine Resilience:** the protocol can withstand up to `(n-1)/3` Byzantine validators, where
`n` is the number of validators

### EVM-Compatible

 Smart Chain supports all the existing Ethereum tooling, smart contracts, decentralized applications and regular applications based on the Ethereum JSON RPC, such as MetaMask.

### Cross-chain Bridge

 Smart Chain supports cross-chain transfers between our legacy  Blockchain and the Smart Chain. All users, exchanges and other services providers can seemlessly transfer their funds over to the  Smart Chain, free of charge.

