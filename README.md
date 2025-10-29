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
    }
}
