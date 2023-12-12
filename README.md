# Magister Militum
## How Does the Logic Works
Magister Militum is different from conventional NFT collections in terms of operation. It does not have a specific number of tokens. It only has a certain number of nft content. There are 10 different commander metadata contents in this demo. Any of these contents are matched with the next minted token and are created with NFT metadata. Here is an example NFT collection that explains how this works:
Token Id: 0 ---> Metadata: Su Dingfang
Token Id: 1 ---> Metadata: Robert Guiscard
Token Id: 2 ---> Metadata: Danishmend Gazi
Token Id: 3 ---> Metadata: Robert Guiscard
Token Id: 4 ---> Metadata: Olga of Kiev
Token Id: 5 ---> Metadata: Olga of Kiev
Token Id: 6 ---> Metadata: Su Dingfang
Token Id: 7 ---> Metadata: Valens
Token Id: 8 ---> Metadata: Batu Khan
Token Id: 9 ---> Metadata: Su Dingfang
Token Id: 10 ---> Metadata: Cnut the Great
Token Id: 11 ---> Metadata: William the Conqueror
Token Id: 12 ---> Metadata: Valens
Token Id: 13 ---> Metadata: Valens
As can be seen, the content of the token is determined completely randomly. Even though the token contents are the same, they are essentially different tokens. The user can mint tokens by paying a certain amount of fee. The NFT metadata content also includes information about the commander's features. Example:
Attack: 88
Defense: 87
Administration: 91
Morale: 82
The user has the right to change the above features of his NFT for a certain fee creating an new URI using IPFS and submitting it to our app. In this way, it can increase the originality of NFT.
## What Does Chainlink Services Do
In our project, we use chainlink services to increase decentralization and verifiability, improve user experience and automate processes.
### Chainlink Data Feeds
We receive data from the ETH/USD price feed to pay the fee requested from the user for minting NFT and updating URI transactions in a certain dollar amount in the gas token of the network. This elevates the user experience by allowing the user to pay in fiat currency as value but in gas tokens as unit.
### Chainlink VRF
We use Chainlink VRF, which produces verifiable randomness, when creating the content of the NFT. The content selected with the random number generated by VRF constitutes the metadata of the newly minted NFT. In this way, true randomness is used to ensure that the application works as intended.
### Chainlink Functions
Users can only change the "attributes" data of the NFTs they own by creating a new URI for their own tokens. We use Chainlink Functions to check that only the attributes data of the newly created URI has been changed appropriately. The URI that successfully passes the validity check becomes the new metadata of the relevant NFT.
### Chainlink Automation
The income obtained from the user in native gas tokens through NFT minting and URI updating is automatically converted into LINK tokens when it reaches a certain amount and is automatically sent to subscriptions in Chainlink services that request LINK for use. We use Chainlink Automation for this entire process.
