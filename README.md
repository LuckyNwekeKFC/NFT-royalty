## Note that this code is for educational purposes and I will liable for any losses. You can contact a professional developer like me for a wholesome contract for business application.

This contract is a marketplace for NFTs that allows creators to set royalties on their NFTs. It inherits from the ReentrancyGuard contract, which prevents the contract from being called recursively. It also inherits from the ERC2981 contract, which allows the contract to calculate and distribute royalties on the sale of an NFT.

The contract has two functions: sellNFT() and buyNft(). The sellNFT() function allows the owner of an NFT to list the NFT for sale. The buyNft() function allows a user to buy an NFT that is listed for sale.

When a user buys an NFT, the contract first checks to make sure that the offer is valid and that the user is paying the reserve price. If the offer is valid and the user is paying the reserve price, the contract then transfers the NFT to the user and pays the royalties to the creators.

The contract uses the royaltyEngineMainnet contract to calculate and distribute royalties. The royaltyEngineMainnet contract is a decentralized royalties registry that is maintained by Manifold XYZ.

Here is a more detailed explanation of the contract:
* sellNFT() function:
    * This function requires the owner of the NFT to approve the contract to sell the NFT on their behalf.
    * The function then creates a new offer and stores it in the offers mapping.
    * The function emits an OnSale event to notify the marketplace that the NFT is now for sale.
* buyNft() function:
    * This function requires the user to pay the reserve price for the NFT.
    * The function then transfers the NFT to the user and pays the royalties to the creators.
    * The function emits a Bought event to notify the marketplace that the NFT has been sold.
