# learn-base-smart-contract
A simple Solidity contract deployed on Base network. Part of Base Learn course.
# 🚀 Learn Base – My First Smart Contract on Base

This project is part of the [Base Learn](https://docs.base.org/learn) course.  
It includes simple Solidity contracts I deployed on the Base testnet (Base Sepolia).

---

## 📘 Contract: AddressBook.sol

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract AddressBook {
    mapping(address => string) private names;

    function setName(string memory _name) public {
        names[msg.sender] = _name;
    }

    function getName(address _address) public view returns (string memory) {
        return names[_address];
    }

    function removeName() public {
        delete names[msg.sender];

🌐 Deployed on Base Testnet

Network: Base Sepolia

Verified via: Base Learn Consul Exercise

Wallet: MetaMask

🧩 My Learning Notes

Learned how to use mapping in Solidity

Practiced error handling and gas optimization

Connected MetaMask with Base network

Deployed and verified contracts using Remix

💫 Next Steps

Build a frontend with Gradio or Next.js

Deploy to Base Mainnet using forge or hardhat

Contribute to open-source projects on Base 🌉

---

6️⃣ Kliknij **Commit changes**



## 🧩 KROK 4 — (Opcjonalnie) Dodaj plik kontraktu

1️⃣ Kliknij **Add file → Upload files**  
2️⃣ Wgraj plik `AddressBook.sol` z Twojego komputera  
3️⃣ Kliknij **Commit changes**

---
# Update: My first commit to GitHub 🚀

## ✅ GOTOWE!

