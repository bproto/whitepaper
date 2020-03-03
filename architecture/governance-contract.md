# Governance Contract

The Governance contract owns the root domain and all TLDs and is therefore responsible for creating TLDs and managing the sponsorship of each TLD. This contracts kick off the auction process and handle the distribution of the associated ERC-20 compatible tokens. Note that the Governance contract will allow BitBoss to create and own 5 TLDs for promotional purposes. For example, BitBoss will own the .human TLD to use within its mobile app to give away .human subdomains. A BUTTERFLY TOKEN holder must burn 10,000 tokens to sponsor a new TLD name. This amount goes down by 10 tokens daily, which is a mechanism intended to incentivize continued sponsorships of new TLDs. The Governance contract manages the current cost to sponsor a TLD, and it burns the tokens that are spent by a BUTTERFLY TOKEN holder for sponsorship.

Checkpoints are used to determine how many BUTTERFLY TOKENS each account owns prior to the start of a new TLD auction. This allows the Governance contract to precisely distribute ERC-20 compatible tokens for the TLD at the end of the auction across all BUTTERFLY TOKENS holders.

**Governance Contract Functions**

The following functions are used by the auction website and clients to operate and participate in auctions, as well as facilitating creation/sponsorship of a new TLD. 

auctions: Returns information about each auction, including:

* State \(available or sponsored\)
* Label \(TLD name\)
* Index
* Start date 
* Address of associated Token contract
* Sponsor
* Checkpoint used
* Total amount raised

totalAuctions: returns the total number of auctions 

auctionsByIndex: retrieves an auction 

sponsorshipCost: returns cost to sponsor a TLD 

sponsor: sponsors a TLD

currentTranche: a view that returns what tranche an auction is currently on. A tranche is a period of time, for example, a typical auction will have 10 tranches, each one last 24 hours. 

bid: payable function to bid on an auction 

raised: a view that returns the amount raised for the auction 

raisedByTranche: a view that returned the amount raised for a specific tranche of an auction 

bidFor: returns the total sum of bids that an account has made for an auction 

payoutByTrancheFor: total payout for an account for a specific tranche 

payoutFor: total payout for an account 

airdropRewardFor: uses a checkpoint to calculate how much of the total airdrop goes to a specific account

claim: mints ERC-20 compatible tokens for:

* sponsor reward \(if the specified account was the sponsor\)
* airdrop reward \(if the specified account holds BUTTERFLY TOKENS\)
* auction payout, based on the total ETH contributed by the specified account

claimed: returns a boolean as to if the tokens have already been claimed for an account

