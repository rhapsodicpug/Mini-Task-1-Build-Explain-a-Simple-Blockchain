 Blockchain Simulation in React

This project demonstrates fundamental blockchain concepts using a React-based UI. It is designed to help beginners understand how blockchains function through visual and interactive examples.

---

 Objectives

1. Build a Basic Blockchain:**
   - Create 3 blocks linked using SHA-256 hashes.
   - Each block contains: index, timestamp, data, previousHash, nonce, and hash.
   - Show how changing one block breaks the chain.

2. **Proof-of-Work Simulation:**
   - Mine blocks using a `nonce` until the hash starts with a defined pattern (e.g., `0000`).
   - Track the number of attempts and time taken.
   - Visualize computational effort behind mining.

3. **Tamper Detection:**
   - Allow editing block data.
   - Show that changing a block invalidates all following blocks unless they’re re-mined.
   - Reinforce the idea of blockchain immutability.

---

Concepts Covered

 Blockchain Basics
A blockchain is a chain of blocks where each block contains data and the hash of the previous block. This makes the system tamper-evident — any modification in a block invalidates the whole chain.

Block Anatomy
Each block contains:
- `index`: its position in the chain
- `timestamp`: creation time
- `data`: the block’s content
- `previousHash`: hash of the prior block
- `nonce`: used for mining
- `hash`: the block’s unique identifier

 Proof-of-Work
To add a block, we must find a `nonce` that produces a hash starting with a specific number of zeros. This simulates the mining process and requires significant computational effort.

 Tampering Effect
If any data in a block is changed:
- Its hash changes
- All following blocks become invalid
- Re-mining is required to restore validity

---

 Real-Life Applications

1. **Supply Chain Tracking**: Ensures transparent product movement and authenticity.
2. **Digital Identity**: Users own and control their identity without central authority.

---

 Learning Outcomes

- Understand how blocks are structured and connected
- Experience how Proof-of-Work adds security
- Visualize the importance of hashes in maintaining trust
- See firsthand how tampering breaks a blockchain

---

## Tech Stack (UI)

- React.js for frontend interface
- crypto-js for SHA-256 hashing
- JavaScript logic for simulating block and chain behavior
