# Auctioning a Domain \(ERC-721 ownership\)

A “reverse clock” auction contract and website will be created to facilitate a domain owner selling their domain. Note that this is separate from the auction process that we will use to initially sell TLDs. 

The ERC-721 domain is sold using a reverse clock auction that is defined and controlled via an Ethereum smart contract. We give credit to Crypto Kitties for bringing to light the benefits of non-fungible ERC-721 contracts, their usefulness, as well as the reverse clock auction. A maximum start price, minimum end price, and auction time are set, and then the sale of the TLD begins. The price \(in Ether\) of the TLD starts at the maximum price and ticks down to the minimum price over the time range allocated for the auction. The first person to purchase the TLD gains full ownership of the ERC-721 token. That person can then choose to sell or auction off some or all of the associated ERC-20 compatible tokens linked to that domain. The ERC-721 owner can trade, sell, or auction the token at any time transferring ownership of that domain.

