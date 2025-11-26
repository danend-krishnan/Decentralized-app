# Decentralized-app
Decentralized Staking App
This is a project I built to explore how decentralized finance (DeFi) works and to create a simple, secure, and user-friendly platform for staking tokens. With this app, users can stake their tokens, earn rewards, and withdraw anytime—all with minimal effort.

What Does It Do?
Stake Your Tokens: Put your tokens to work with just a few clicks.
Earn Rewards: Watch your rewards grow in real time as the app calculates them automatically.
Withdraw Anytime: You can withdraw your tokens and rewards whenever you want. No lock-ins, no hassles.
Secure and Decentralized: Built on blockchain technology, your assets are safe, and every transaction is fully transparent.
1. Tether.sol

A mock USDT ERC-20 token used as the staking currency.

Key Features:

Standard ERC-20 implementation

Mintable token supply

Users use this token to stake in the system

2. RWD.sol

Reward token issued to users for staking.

Key Features:

ERC-20 token

Minted only by the DecentralBank contract

Acts as the reward for stakers

3. DecentralBank.sol

This is the main contract that handles staking logic.

Responsibilities:

Accepting Tether deposits

Tracking staking balances

Issuing RWD tokens as rewards

Allowing users to withdraw their staked tokens

Important Functions:

depositTokens(uint _amount) – Stake Tether

unstakeTokens() – Withdraw staked Tether

issueTokens() – Issue RWD rewards (only owner can call)

Only the contract owner may issue rewards, ensuring access control.
