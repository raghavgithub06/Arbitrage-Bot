# Arbitrage-Bot

The FlashLoaner smart contract allows users to execute flash loans on the PancakeSwap decentralized exchange (DEX) using the UniswapV2Router02. The contract allows borrowers to borrow a specified amount of a token from a UniswapV2Pair and execute custom logic during the flash loan process.

## Contract Details

- **Solidity Version Compatibility**: ^0.8.0

## State Variables

- `factory` (address): The address of the UniswapV2Factory contract.

- `deadline` (uint): A constant variable representing the deadline (10 days) for executing the flash loan.

- `bakeryRouter` (address): The address of the UniswapV2Router02 contract.

## Functions

1. `constructor(address _factory, address _bakeryRouter)`: The constructor function to initialize the contract with the UniswapV2Factory and UniswapV2Router02 contract addresses.

2. `pancakeCall(address _sender, uint _amount0, uint _amount1, bytes calldata _data) external`: The function is called by the PancakeSwap pair contract during the flash loan. It performs the flash loan logic, swaps tokens, and transfers them back to the pair contract.

## Note

This documentation provides an overview of the FlashLoaner smart contract and its functionalities. The contract demonstrates how to execute flash loans on the PancakeSwap DEX using the UniswapV2Router02. Before deploying or interacting with any smart contract, it is crucial to conduct a thorough code review, audit the contract's security, and understand the implications of each function. The contract allows borrowers to perform flash loans and execute custom logic during the flash loan process.
