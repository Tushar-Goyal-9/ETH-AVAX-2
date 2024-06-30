# NightToken ERC20 Contract

This Solidity program implements the NightToken ERC20 token contract, showcasing basic functionalities such as minting, burning, transferring tokens, and custom logging. It serves as an example of implementing an ERC20 token with additional features on the Ethereum blockchain.

## Description

NightToken is a smart contract written in Solidity for Ethereum. It includes the following functionalities:

- **Token Information:**
  - Name: NightToken
  - Symbol: NGT
  - Decimals: 18 (default for ERC20)
  - Maximum Supply: 100,000 tokens

- **Functions:**
  - **Constructor:** Upon deployment, mints 10,000 tokens to the contract creator.
  - **Minting:** Allows the owner to mint additional tokens, restricted by a maximum supply cap.
  - **Burning:** Enables token holders to burn (destroy) their own tokens.
  - **Transferring:** Standard ERC20 transfer function overridden to log transfers using Hardhat's `console.log`.

## Executing the Program

### Deployment and Interaction:

To deploy and interact with the NightToken contract:

1. **Using Remix IDE:**
   - Go to [Remix Ethereum IDE](https://remix.ethereum.org/).
   - Create a new file named `NightToken.sol` and paste the contract code.
   - Compile the contract in the "Solidity Compiler" tab.

2. **Deployment:**
   - Deploy the contract in the "Deploy & Run Transactions" tab.
   - Select `NightToken` from the contract dropdown and click "Deploy".

3. **Token Operations:**
   - Upon deployment, the deployer receives 10,000 NightTokens.
   - Use the `mint` function (accessible to the owner) to mint additional tokens up to the maximum supply.
   - Transfer tokens between addresses using the `transfer` function.
   - Burn tokens using the `burn` function.

4. **Logging:**
   - Transfer events are logged to the Hardhat console for each successful token transfer.

## Authors

- Metacrafter Chris
- [@metacraftersio](https://twitter.com/metacraftersio)

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
