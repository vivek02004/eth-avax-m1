# Moneymanagment Contract

## Overview
The `Moneymanagment` smart contract is designed to demonstrate the use of error handling in Solidity. It includes functions for depositing and withdrawing funds, adjusting the balance, and deactivating the contract, all with appropriate access controls and error checks.

## Features
- **Ownership Control**: Only the owner can adjust the balance and deactivate the contract.
- **Active Check**: Functions can only be called when the contract is active.
- **Deposit and Withdrawal**: Users can deposit funds and withdraw up to the available balance.

## Functions
- `constructor()`: Initializes the contract with the creator as the owner and an initial balance.
- `deposit()`: Allows users to deposit funds into the contract.
- `withdraw(uint _amount)`: Allows users to withdraw funds from the contract.
- `setBalance(uint _newBalance)`: Allows the owner to set a new balance.
- `deactivateContract()`: Allows the owner to deactivate the contract and withdraw the remaining balance.

## Modifiers
- `onlyOwner`: Restricts function access to the contract owner.
- `onlyWhenActive`: Ensures the contract is active before executing a function.


- Checks for ownership, contract activity, deposit amount, and sufficient balance are implemented using `require` statements for robust error handling.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
