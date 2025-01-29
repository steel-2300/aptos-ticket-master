# aptos-nft-ticket
A simple module which would mint an NFT to the user whenever they purchase a ticket.

In this module a person can do the following things
- Host a venue specifying the name and the description ( this is when an empty collection would be created )
- Create tickets for the venue by specifying name, description, uri, maximum tickets available and also the price. ( this is when token data would be created ).
- Users can purchase tickets by specifying the ticket name and the quantity. If the ticket purchase is successful, a NFT would be minted.

Whenever a venue is created, a resource account is created which would hold the venue data as well the ticket information. The resource account would be used to be mint the token to the person buying the ticket. So the venue owner doesnt have to sign everytime for minting the NFT. Whenever the purchase is successful, the NFT is minted.
