# Registry ERC-721 Contract

The primary values that get stored for each domain are:

* **Label**: the domain name \(ex: "fantasy"\)
* **Parent**: the parent domain \(ex: "sports"\)
* **Token Contract**: a pointer to the ERC-20 compatible contract specific to this domain
* **Owner**: the Ethereum public key representing the owner of this token/domain
* **Record**: a type and pointer used to lookup the data for the domain
* **Price**: the cost in Ether for each domain
* **Tokens** **to create new**: the number of ERC-20 compatible tokens that must be burned to create a subdomain

## Registry Contract Functions

{% tabs %}
{% tab title="register" %}
Creates an ERC-721 token and sets the domain fields to configure it. The Register function in the smart contract will be called from the Registrar website when a user registers a new domain. The Registry contract checks that the owner has enough of the ERC-20 compatible token and then burns it as part of the registration process.
{% endtab %}

{% tab title="resolve" %}
Uses the FQN to find the data store and to retrieve information about how to connect the client to the domain resource. This could be an IP address pointing at a centralized website, or it could be a pointer into an IPFS folder that contains an index.html and all dependent resources to launch a decentralized website.
{% endtab %}
{% endtabs %}

