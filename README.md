# Kyber Smart Contracts Examples for Remix

This respository is inspired by [Kyber Workshop repo](https://github.com/KyberNetwork/workshop)

Use this example code if you don't want to use Truffle and Ganache and simply want to see how smart contracts can interface with Kyber's smart-contracts for [Trade](https://github.com/hammadtq/Kyber-Smart-Contracts-Examples-for-Remix/blob/master/contracts/Trade.sol), [Ether to Token swap](https://github.com/hammadtq/Kyber-Smart-Contracts-Examples-for-Remix/blob/master/contracts/SwapEtherToToken.sol), [Token to Token swap](https://github.com/hammadtq/Kyber-Smart-Contracts-Examples-for-Remix/blob/master/contracts/SwapTokenToToken.sol) and [Token to Ether swap](https://github.com/hammadtq/Kyber-Smart-Contracts-Examples-for-Remix/blob/master/contracts/SwapTokenToEther.sol).

## Steps to run an example
- Load all of the files located in contracts/ folder to your [Remix IDE](https://remix.ethereum.org).
- Now switch to one of the examples such as [SwapEtherToToken.sol](https://github.com/hammadtq/Kyber-Smart-Contracts-Examples-for-Remix/blob/master/contracts/SwapEtherToToken.sol) contract inside the remix.
- Select 4.0.18 as your compiler in the Remix IDE.
- Switch to Injected Web3 in the Remix and subsequently select Ropsten as network in your MetaMask plugin.
- Make sure you have some test ETH in your MetaMask, otherwise get some from the [Ropsten Faucet](https://faucet.ropsten.be/).
- Deploy the contract using KyberProxyNetwork.sol address `0x818E6FECD516Ecc3849DAf6845e3EC868087B755`. A complete list of Kyber's Ropsten adresses can be found [here](https://developer.kyber.network/docs/Environments-Ropsten/).
- Interact with a contract by running execSwap method of the contract after the deployment. You will need to provide a token contract address such as AST on Ropsten has `0xeF06F410C26a0fF87b3a43927459Cce99268a2eF` comma-separated by your own (or another ethereum address) where you want to send the converted tokens.
- Moment of truth, you will be able to see transaction on the etherscan.com

If you sent converted tokens to your own MetaMask address, you will need to add AST in the MetaMask to see the tokens. Just go to Add Token in the MetaMask, click on "Custom Token" tab and paste the above AST address in the window. All other supported tokens are again available on the [Kyber's Ropsten Environment page](https://developer.kyber.network/docs/Environments-Ropsten/).
