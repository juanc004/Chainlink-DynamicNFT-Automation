# Dynamic NFT with Chainlink Automation

Create a Dynamic NFT that evolves over time using Chainlink Automation. This project utilizes smart contracts to change the NFT's metadata based on time intervals, simulating the growth stages of a flower.

## Getting Started

### Deploying the Contract

1. **Deploy on Remix**: Use the provided `Flower` contract code. Set the `UPDATEINTERVAL` constructor argument to your desired time interval (in seconds).
2. **Verify Inputs**: After deployment, call `interval`, `name`, and `symbol` functions to confirm your inputs.

### Minting Your NFT

1. **SafeMint Function**: Call `safeMint` with your wallet address to mint your NFT.
2. **Contract Address**: Copy the deployed contract address.
3. **View on OpenSea**: Go to [testnets.opensea.io](https://testnets.opensea.io/) and paste your contract address in the search bar to view your NFT. Ensure the Token ID is 0.

### Setting Up Automation

1. **Chainlink Automation**: Visit [automation.chain.link](https://automation.chain.link/) and select "register new upkeep."
2. **Custom Logic**: Choose "custom logic" and input your contract address.
3. **Upkeep Name**: Enter a name for your automation job.
4. **Starting Balance**: Allocate 3 LINK tokens for the starting balance.
5. **Register**: Leave other fields as default and register your upkeep.

### Growing Your Flower

1. **Interact with Contract**: Return to Remix and call the `growFlower` function with your Token ID (0).
2. **Wait and Refresh**: After the set interval, refresh your NFT on OpenSea. You should see the updated metadata.

## Contract Functions

- **`safeMint`**: Mint your NFT with an initial stage.
- **`growFlower`**: Triggers the next growth stage of your NFT.
- **`flowerStage`**: Returns the current stage of the flower.

## Chainlink Automation

This project utilizes Chainlink Automation to periodically call the `growFlower` function, simulating the growth process of the flower. It ensures that your NFT dynamically updates without manual intervention.

## Exploring Your NFT

Your NFT will evolve through predefined stages, with each stage represented by unique metadata stored on IPFS. Starting as a seed, your flower can sprout and eventually bloom, visualizing the lifecycle of a plant.

## Conclusion

This guide provides the steps to deploy and interact with a dynamic NFT using Chainlink Automation. By following this guide, you can create an NFT that grows over time, offering a unique digital collectible experience.

## Watch the Tutorial

For a detailed walkthrough of this project, watch our [YouTube tutorial](https://www.youtube.com/watch?v=AEvN7UN1T5Y).
