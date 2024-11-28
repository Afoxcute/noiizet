# n01zet-staking-vesting-smartcontract
N01zet Dashboard Staking Vesting and Smart contract of the Tokenomics
Project N01zet

Description 
DAO Dashboard

Prerequisites
Before you begin the deployment process, ensure you have the following tools installed and set up:

Solana CLI: Installation Guide
Anchor CLI: Included in your project dependencies, but you can check the Anchor documentation for more details.
A Solana wallet with sufficient SOL to cover deployment fees.
Deployment Process

1. Set Solana Cluster
Select the Solana cluster you wish to deploy to (devnet, testnet, or mainnet):

solana config set --url https://api.devnet.solana.com # For devnet




2. Build Your Program
Compile your Solana program:

anchor build


Note the program ID output by this command, as you will need it for deployment.

3. Fund Your Wallet
Ensure your wallet has enough SOL for the deployment. If deploying to devnet or testnet, you can airdrop SOL:

solana airdrop 1


4. Update Anchor.toml
Update the Anchor.toml file to include your program's ID under the appropriate cluster section:

Toml

[programs.devnet]
your_program_name = "YourProgramID"

5. Deploy the Program
Deploy your program to the specified Solana cluster:

anchor deploy



6. Verify Deployment
Check that your program has been deployed successfully:

solana account YourProgramID


Post-Deployment
After deployment, you can interact with your program using client-side scripts or the command line, based on the functionalities you've implemented.

tokenomics program link: https://explorer.testnet.soo.network/address/EBdu7ax329bQdrSqzfUhzPbZm74vQbL3RGiYHqoQ4pku

token vesting program link: https://explorer.testnet.soo.network/address/FPMWFeVjrYcZJXRDU8W2XrMVNHmHGa6qXrJ16rW92fRp

token staking program link: https://explorer.testnet.soo.network/address/A8euEuZ3kkhtwnhf7tHqXyst7AigA8pneC12mNPjRNry

link to the Dapp: https://noiizet.vercel.app/



Monitoring and Updating
Monitor your program's performance and usage. For updates or modifications, repeat the build and deployment process with necessary changes.

Support
For additional help or information, please refer to the Anchor documentation or reach out to the community forums.


THINGS TO NOTE

1. All the SOON programs needed is developed and deployed
2. Frontend for the Dapp is completed
3. What is left is final integration with the SOON programs
4. To activate the admin features, you need to hardcode your wallet address in the source code deployment
5. 

