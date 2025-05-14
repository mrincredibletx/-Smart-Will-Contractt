## 📝 SmartWill - A Simple Ethereum Smart Contract for Digital Wills

### 📖 Overview

**SmartWill** is a decentralized Ethereum smart contract that allows users to create and store a digital "will" securely on the blockchain. Only the owner (creator) of the will can execute it, ensuring transparency, immutability, and authenticity.

---

### 🔧 Features

* ✅ Immutable storage of a textual will
* 🔐 Only the owner can execute the will
* 📡 Emits events on creation and execution
* 📖 Anyone can view the will content

---

### 🧾 Contract Details

```solidity
pragma solidity ^0.8.9;
```

* **Owner:** The person who deploys the contract.
* **Will Content:** A string message that represents the owner's last will.
* **Execution Status:** A boolean that prevents multiple executions.

---

### 📦 Functions

| Function                              | Access      | Description                               |
| ------------------------------------- | ----------- | ----------------------------------------- |
| `constructor(string memory _content)` | Public      | Sets the will content and owner           |
| `executeWill()`                       | Owner only  | Executes the will (can only be done once) |
| `getWillContent()`                    | Public view | Returns the stored will content           |

---

### ⚙️ How to Use

1. **Deploy the contract** using Remix, Hardhat, or any other Ethereum environment.
2. **Pass the will content** as a constructor parameter (string) during deployment.
3. Use the `executeWill()` function to finalize the will execution.
4. Anyone can call `getWillContent()` to view the will text.

---

### 📢 Events

* `WillCreated(address indexed creator, string content)`
* `WillExecuted(address indexed executor)`

---

### 🛡 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

---

### 🙋‍♂️ Author

Crafted with ❤️ for decentralized inheritance systems.
