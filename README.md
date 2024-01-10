# ERC20 Token Contract

## Solidity Token (SOL)

This is a simple ERC-20 compliant token contract implemented in Solidity. The token is named "Solidity" with the symbol "SOL". Below are some key features and information about the contract:

### Contract Details:

- **Name:** Solidity Token
- **Symbol:** SOL
- **Decimals:** 18
- **Total Supply:** Dynamic (can be minted)
- **Events:** 
  - `Transfer`: Triggered when tokens are transferred.
  - `Approval`: Triggered when an allowance is approved.

### Functions:

1. **transfer**
   - Allows users to transfer tokens to another address.
   - Emits a `Transfer` event.

2. **approve**
   - Allows users to approve another address to spend a specific amount of tokens on their behalf.
   - Emits an `Approval` event.

3. **transferFrom**
   - Allows an approved spender to transfer tokens from one address to another.
   - Emits a `Transfer` event.

4. **mint**
   - Allows the contract owner to mint new tokens.
   - Emits a `Transfer` event.

5. **burn**
   - Allows users to burn their own tokens.
   - Emits a `Transfer` event.

### Usage:

1. Deploy the contract to the Ethereum blockchain.
2. Use the provided functions to interact with the token (transfer, approve, mint, burn).
3. Monitor the emitted events for transaction details.

## Vault Contract

# Token Vault

This Solidity contract represents a simple vault for managing ERC-20 tokens. The vault allows users to deposit and withdraw tokens while maintaining a record of their shares in the vault. The primary token interaction is done through the ERC-20 interface.

### Contract Details:

- **Vault Token Interface:** ERC-20
- **Events:**
  - `Transfer`: Triggered when tokens are transferred.
  - `Approval`: Triggered when an allowance is approved.

### State Variables:

- `token`: Immutable variable storing the ERC-20 token address.
- `totalSupply`: Total shares of the vault.
- `balanceOf`: Mapping of addresses to their corresponding share balances.

### Functions:

1. **deposit**
   - Allows users to deposit ERC-20 tokens into the vault.
   - Calculates and mints new shares based on the deposited amount.

2. **withdraw**
   - Allows users to withdraw ERC-20 tokens from the vault.
   - Burns the specified shares and transfers the corresponding amount of tokens.

## Author

mahesh

maheshzabade24@gmail.com
