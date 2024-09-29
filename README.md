# Thrifteazy - Web 3 Marketplace for Thrifted Goods

Thrifteazy is a decentralized Web 3 marketplace that leverages the power of blockchain technology to enable users to buy and sell secondhand items in a secure and transparent manner. Each thrifted item is represented as an NFT (Non-Fungible Token), carrying not only the item’s current ownership but also its historical journey, making each piece uniquely valuable based on its past. Through integrating with Andromeda's ADOs and Embeddables, Thrifteazy utilizes advanced Web 3 protocols for creating dynamic, story-driven NFTs.

## Key Features

NFT-Linked Thrift Items: Each item is represented by a unique ERC-721 token, with ownership history recorded immutably on the blockchain.

Andromeda ADO Integration: Leveraging Andromeda’s Asset Definition Objects (ADOs) for modular smart contract functionality, enabling customizable metadata and functionality for NFTs.

Embeddable Components: Utilizes Andromeda’s Embeddable NFTs to create layered ownership structures, allowing multiple embedded assets (stories, transactions) to be attached to a single NFT.

CosmWasm Smart Contracts: Thrifteazy is built using CosmWasm, a multi-chain smart contract platform that enables high performance, gas-efficient contract execution with rich on-chain logic.

Personalized Value Mechanism: The story of previous owners is embedded within the NFT metadata, impacting the item’s value as its journey unfolds through the marketplace.

Decentralized Storage with IPFS: NFT metadata, including history and ownership data, is stored using InterPlanetary File System (IPFS) to ensure decentralized, immutable records.


## Learning Journey

Throughout this project, I deepened my understanding of blockchain technologies, particularly in the areas of:

**CosmWasm:** A high-performance WebAssembly (Wasm) runtime for multi-chain smart contracts. By working with CosmWasm, I explored how to create, deploy, and manage smart contracts with customizable modules.
**Andromeda’s ADOs:** Through integrating with Andromeda’s ecosystem, I learned how to utilize Asset Definition Objects to enhance the functionality of smart contracts, enabling modular interactions for NFTs and embedding metadata.
**Smart Contract Development:** I gained hands-on experience with Rust and CosmWasm, focusing on efficient contract deployment and the importance of gas-optimized code in production environments.

## Architecture Overview
**1. Andromeda ADOs**
Andromeda ADOs were integrated to handle modular contract functionality. These ADOs define customizable attributes for each thrifted item and allow for future extensibility, making the NFT structure adaptable for additional features (such as embedded stories, dynamic pricing).

**2. Embeddables**
Using Andromeda’s embeddable features, each NFT can hold a layered asset structure. For example, the thrifted item's story is embedded directly into the token, and this layer evolves as the item changes hands. Each transfer updates the NFT's metadata, making the ownership journey part of the item’s history.

**3. CosmWasm Smart Contracts**
Smart contracts are the backbone of Thrifteazy. Contracts were written in Rust and deployed via CosmWasm for efficient execution across multiple chains. These contracts handle core logic, such as item listings, purchases, transfers, and metadata updates.

**4. IPFS Integration**
To maintain decentralized storage of NFT metadata, IPFS is used. Metadata (e.g., owner history, stories) is stored off-chain while the smart contracts maintain pointers to the data. This ensures scalability and redundancy while preserving the decentralized nature of the marketplace.
