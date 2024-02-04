
# Solidity Vault with ERC20 Token Interaction

This repository contains a Solidity smart contract `Vault` which acts as a vault for managing ERC20 token deposits and withdrawals. It interacts with an ERC20 token contract to facilitate these operations.

## Contracts

### Vault.sol

The `Vault` contract manages the deposit and withdrawal of ERC20 tokens. It calculates shares for depositors and converts shares back to tokens for withdrawal. The contract also keeps track of total supply and individual balances of deposited tokens.

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.17;

interface IERC20 {
    // Interface definition for ERC20 token functions
    ...
}

contract Vault {
    // State variables
    ...

    // Constructor
    ...

    // Internal functions
    ...

    // External functions
    ...
}
```

### ERC20.sol

The `ERC20` contract represents a basic ERC20 token with functionalities like transfer, approval, allowance, minting, and burning.

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.17;

contract ERC20 {
    // State variables
    ...

    // Events
    ...

    // External functions
    ...
}
```

## Usage

To use the `Vault` contract:

1. Deploy the ERC20 token contract (`ERC20.sol`).
2. Deploy the `Vault` contract, passing the address of the deployed ERC20 token contract to its constructor.
3. Interact with the `Vault` contract to deposit and withdraw ERC20 tokens.

## License

This code is licensed under the MIT License. See the `LICENSE` file for details.

