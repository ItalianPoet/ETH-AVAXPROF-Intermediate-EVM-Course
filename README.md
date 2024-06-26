# ETH + AVAX PROOF: Intermediate EVM Course Module 1 Assessment

This project demonstrates the usage of require(), assert(), and revert() statements in a Solidity smart contract. It allows an owner to deposit and withdraw Ether, check balances, and intentionally trigger a revert.

## Description

This Solidity smart contract is designed for reveiwing purpose to illustrate basic error handling and conditional checks in Solidity. The contract includes functions for depositing and withdrawing Ether, ensuring that certain conditions are met using require(), validating internal invariants using assert(), and demonstrating how to use revert() to explicitly trigger an error and roll back a transaction.

## Getting Started

### Installing

* Clone the repository to your local machine: https://github.com/ItalianPoet/Solidity-Module-1/edit/main
* Navigate to the project directory: Module 1 Assessment.

### Executing program

* Deploy the Contract:

Use Remix, Truffle, or Hardhat to deploy the contract to an Ethereum network.

* Interact with the Contract:

1. Use the deposit function to send Ether to the contract:
```
// In Remix or your chosen environment, call the deposit function and send some Ether
exampleContract.deposit({ value: web3.utils.toWei('1', 'ether') });

```
2.Use the withdraw function to withdraw Ether (only the owner can call this function):
```
// Ensure you are the owner and call the withdraw function
exampleContract.withdraw(web3.utils.toWei('0.5', 'ether'));


```
3.Use the checkBalance function to verify that the balance is non-negative:
```
// Call the checkBalance function
exampleContract.checkBalance();


```
4.Use the causeRevert function to intentionally trigger a revert:
```
// Call the causeRevert function
exampleContract.causeRevert();


```


## Help

If you encounter any issues:

Ensure that you have a valid Ethereum account with sufficient funds.

Make sure you are using a compatible Solidity version (^0.8.26).

Check the Remix console or your development environment's logs for detailed error messages.

## Authors

Raunak Raj 
raunakraj3002@gmail.com

## License

This project is licensed under MIT.
