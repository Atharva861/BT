## Steps to Deploy and Test Smart Contract on Sepolia Testnet

1. **Create MetaMask Wallet**  
   - Install the MetaMask browser extension.  
   - Create a new wallet or import an existing one.  
   - Securely store your recovery phrase.

2. **Add Sepolia Test Network**  
   - Open MetaMask → Settings → Networks → Add Network.  
   - Add the following details:  
     ```
     Network Name: Sepolia Test Network
     RPC URL: https://sepolia.infura.io/v3/
     Chain ID: 11155111
     Currency Symbol: ETH
     Block Explorer URL: https://sepolia.etherscan.io
     ```
   - Save and switch to the Sepolia Test Network.

3. **Get Test ETH from Faucet**  
   - Search on Google: `ETH Sepolia Faucet`  
   - Example: https://sepoliafaucet.com/  
   - Paste your MetaMask wallet address and request tokens.  
   - Wait for the transaction to complete.

4. **Open Remix IDE**  
   - Go to https://remix.ethereum.org/  
   - Create a new file (e.g. `BankAccount.sol`).  
   - Paste your Solidity code into the editor.

5. **Compile the Contract**  
   - Open the Solidity Compiler tab.  
   - Select compiler version `0.8.19`.  
   - Enable “Auto Compile” or click “Compile BankAccount.sol”.

6. **Deploy the Contract**  
   - Go to the “Deploy & Run Transactions” tab.  
   - In the environment dropdown, select `Injected Provider - MetaMask`.  
   - Make sure MetaMask is connected to the Sepolia Test Network.  
   - Click “Deploy” and confirm the transaction in MetaMask.

7. **Test Contract Functions**  
   - After deployment, expand the deployed contract in Remix.  
   - Test the following functions:
     - `createAccount()` – Create a new account.  
     - `deposit()` – Deposit ETH into your account.  
     - `withdraw(uint amount)` – Withdraw specified ETH amount.  
     - `getBalance()` – Check your current account balance.

