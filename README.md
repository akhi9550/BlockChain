# 🛠️ Simple Blockchain Implementation in Go

This is a **basic blockchain implementation** in Go (Golang).  
It helps you understand how blockchain works by linking blocks through hashes.

---

## How It Works

- **Block Structure**
  - `Data`: The data stored in the block.
  - `PrevHash`: The hash of the previous block.
  - `Hash`: The current block's hash (generated from `Data` + `PrevHash`).

- **Blockchain**
  - A slice of blocks (`[]*Block`).
  - Each block securely links to the previous one via its hash.

- **Hashing**
  - Uses `SHA-256` to generate a unique hash from the `Data` and `PrevHash`.

---

## 🔑 Key Functions

| Function       | Purpose                                      |
|----------------|----------------------------------------------|
| `DeriveHash()` | Generates the SHA-256 hash of a block         |
| `CreateBlock()`| Creates a new block with given data and hash  |
| `AddBlock()`   | Appends a new block to the blockchain         |
| `InitBlockChain()` | Initializes the blockchain with the genesis block |


---

## What You Will Learn
- How Blockchain stores blocks with previous hashes
- How immutability is ensured via cryptographic hashes
- How Go handles byte slices and hashing
- Fundamentals of chaining data in-memory
