# Module-21-Challenge

[![Screen-Shot-2022-05-29-at-4-50-21-PM.png](https://i.postimg.cc/65ctJrmc/Screen-Shot-2022-05-29-at-4-50-21-PM.png)](https://postimg.cc/WhdQ0kjq)

# Background

After waiting for years and passing several tests, I was selected by the Martian Aerospace Agency to be part of the first human colony on Mars. As a prominent fintech professional, I was chosen to lead a project to develop a monetary system for the new Mars colony. I've decided to base this new monetary system on blockchain technology, and to define a new cryptocurrency called KaseiCoin. (“Kasei” means “Mars” in Japanese.)

KaseiCoin will be a fungible token that is ERC-20 compliant. I'll launch a crowdsale that will allow people who are moving to Mars to convert their earthling money to KaseiCoin.

---

## Technologies

* [Solidity](https://docs.soliditylang.org/en/v0.8.14/)  - Solidity is an object-oriented, high-level language for implementing smart contracts. Smart contracts are programs which govern the behaviour of accounts within the Ethereum state. Solidity is a curly-bracket language designed to target the Ethereum Virtual Machine (EVM). It is influenced by C++, Python and JavaScript.

* [Remix IDE](http://remix.ethereum.org/) - allows developing, deploying and administering smart contracts for Ethereum like blockchains. It can also be used as a learning platform.

---
## Installation Guide

In this challenge I used [Remix IDE](http://remix.ethereum.org/) to compile to deploy our contracts.

---
## Usage
* Created a constructor for the KaseiCoin contract.

```java
// Create a constructor for the KaseiCoin contract and have the contract inherit the libraries that you imported from OpenZeppelin.

contract KaseiCoin is ERC20, ERC20Detailed, ERC20Mintable{

    address public owner;

    constructor (string memory name, string memory symbol, uint initial_supply) 
        ERC20Detailed(name, symbol, 18) public {
            owner = msg.sender;
            mint(owner, initial_supply);
    }

}
```
---

## Evaluation Evidence

* Contract Deployment

[![Screen-Shot-2022-05-29-at-3-52-07-PM.png](https://i.postimg.cc/gc52tq1Z/Screen-Shot-2022-05-29-at-3-52-07-PM.png)](https://postimg.cc/Yj67hgrr)

[![Screen-Shot-2022-05-29-at-3-55-24-PM.png](https://i.postimg.cc/xCp12KCB/Screen-Shot-2022-05-29-at-3-55-24-PM.png)](https://postimg.cc/k68mNRWy)

[![Screen-Shot-2022-05-29-at-3-58-01-PM.png](https://i.postimg.cc/Xv8v2M0j/Screen-Shot-2022-05-29-at-3-58-01-PM.png)](https://postimg.cc/kV294p4z)

  **Remix IDE**

[![Screen-Shot-2022-05-29-at-4-33-27-PM.png](https://i.postimg.cc/Y0V011BQ/Screen-Shot-2022-05-29-at-4-33-27-PM.png)](https://postimg.cc/xNv9QNCd)

**METAMASK**

[![Screen-Shot-2022-05-29-at-3-50-38-PM.png](https://i.postimg.cc/4dPhh731/Screen-Shot-2022-05-29-at-3-50-38-PM.png)](https://postimg.cc/FdfKMK3f)

**GANACHE**

[![Screen-Shot-2022-05-29-at-4-30-15-PM.png](https://i.postimg.cc/WzfFXBgF/Screen-Shot-2022-05-29-at-4-30-15-PM.png)](https://postimg.cc/Fk3HKnPN)

[![Screen-Shot-2022-05-29-at-4-29-43-PM.png](https://i.postimg.cc/KjY37Gkh/Screen-Shot-2022-05-29-at-4-29-43-PM.png)](https://postimg.cc/sQt2sR4T)

---

## Contributors

Brought to you by Elgin Braggs Jr.

---
## License

MIT