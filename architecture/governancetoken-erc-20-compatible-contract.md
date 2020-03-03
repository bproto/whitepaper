# GovernanceToken ERC-20 Compatible Contract

This is the contract that tracks the number of BUTTERFLY TOKENS that each account has. It is used by the Governance Contract to create checkpoints and distribute a TLD’s ERC-20 compatible tokens at the end of an auction.

GovernanceToken Contract Functions: 

balanceAt: retrieves the balance of BUTTERFLY TOKENS for an account, for a checkpoint 

currentCheckpoint: gets the current checkpoint information 

createCheckpoint: creates a new checkpoint

