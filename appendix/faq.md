# FAQ

## Is the butterfly protocol limited to a single TLD?

No. Unlike other blockchain based naming systems the eventual goal of the butterfly protocol is to replace the legacy system. In a url the http:// part denotes what protocol is being used. We will be following that format in clients we build where possible. We do have gateways on the roadmap that will allow butterfly protocol domains to be accessed through existing dns systems. These gateways will live at existing domains such as bpro.to but will be open source allowing anyone to host it on any legacy domain.

## Why are you not scoping the butterfly protocol to a single TLD?

While we will provide ways to connect the old and the new we don’t want the new to be held back. The TLDs are important, if we rely on the old system the butterfly protocol would be crippled. An example is the .dev TLD. Until recently .dev wasn’t a valid domain so many developers used it to point to different projects on their local machine. When ICANN released it into the wild it broke. Any new naming system that relies on an existing TLD not existing on legacy DNS is dependent on that legacy system.

## How will TLDs be selected and made available on the butterfly protocol?

ICANN currently charges $185k to evaluate a new TLD. For the butterfly protocol we want the community to be able to decide what TLDs they want. To that end we will be releasing, via IEO, a utility token that is used to sponsor a new TLD.  It will initially cost 10k of the utility tokens to sponsor a domain with that cost going down every block until it reaches a minimum of 1 token after about 3 years. 

Once a domain is sponsored a batch of ERC20 tokens is created for use in buying subdomains for that specific TLD. These tokens are split between community with the sponsor getting 5%, holders of the butterfly protocol utility token getting 15% airdropped based on their ownership, and the final 80% made available through a public auction.

## How does the butterfly protocol compare to namecoin?

One of the biggest differences is that namecoin was it’s own blockchain while the butterfly protocol builds its ownership control on ethereum using standardized tokens. This means that any marketplace or wallet that supports the ERC721 standard \(popularized by crypto kitties\) will work with your domains. Another key differentiator is that once you own a domain on the butterfly protocol you don’t rent it you own it. Most other systems, including namecoin, make you pay every year just to keep something you already paid for. 

## How does the butterfly protocol compare to ENS?

ENS is a great project and has a couple things in common with the butterfly protocol. They are both built on ethereum and use similar name hashing. But just like namecoin ENS doesn’t let you plug into existing tools by using standard tokens to represent ownership of names, and you have to pay every year. There are a number of other differences such as how the butterfly protocol stores data and allows the community to creates TLDs.

## How does the butterfly protocol compare to IPFS/IPNS?

IPFS is pretty amazing and it is actually a main component of the butterfly protocol not a competitor. While IPFS has some tools for linking traditional domains to files stored on IPFS it doesn’t have a naming system of its own. Even IPNS just provides a consistent address that can link to different files. We make full advantage of different parts of IPFS including IPLD to allow us to store much more than ethereum by itself or legacy DNS.

## Does the butterfly protocol prevent domain squatters?

Not exactly, and we don’t want to. Although we do have a couple features that make squatting on a high value domain more difficult. The ability to buy a domain for a low price and selling it for more than you paid is a good thing. It creates an open market where the value of a name is determined by free trade. We also make it easy for domain owners to create and sell subdomains, create ERC20 tokens tied to a domain, and provide many other ways for a creative domain owner to turn a profit besides squatting.

One reason it is a problem on legacy DNS is that all legacy domains under a TLD cost a fairly consistent low price from the start. This is partly because it needs to be low since people pay the fee every year. But it allows someone to swoop in and buy up a bunch of names. With the butterfly protocol after the tokens used to create a domain for a specific TLD are distributed the cost in those tokens starts fairly high at 1k tokens and slowly goes down over time. This makes it costly for a squatter to just buy all domains under a TLD. 

## Does the butterfly protocol use BSV \(or some other chain I hate\)?

Drama aside our team really likes where BSV is going on a technical level and have used it for several projects. The butterfly protocol however lives primarily on the ethereum chain with data \(domain records, site data, etc\) stored on IPFS. One of the reasons we use IPFS though is the IPLD project which allows linking between different hash based data formats. That sounds complicated but what it means is that through IPLD we have the potential to store data on many different systems and access it all through IPFS. Data on IPFS isn’t guaranteed to stay around unless someone is hosting it. We think BSV has great potential to be one of the places that data is stored.

## How will funds raised from TLD auctions be used?

When a new TLD is sponsored 5% of the TLDs ERC20 tokens go to the sponsor, 15% are airdropped to butterfly protocol utility token holders, and 80% of the tokens are auctioned off to the public all through a smart contract. This process serves two purposes. One it provides a fair way for everyone to get a chunk of a new TLD while rewarding those more involved in the process. And two it provides funding for development of the base protocol and supporting software. Since there is no annual renewal fee for domains this provides a way for us to continue development through the bootstrap phase. One important aspect of this process is that the auctions, ownership, and functionality of the system is all handled in smart contracts and doesn’t depend on us to continue to work.



