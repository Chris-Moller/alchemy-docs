---
description: >-
  Fetch NFTs, metadata, prices, owners, collections, and more with speed and
  accuracy across Ethereum, Polygon, Flow, testnets, and more.
---

# NFT API

Want to get started with code but not sure how to? Take a look at the [Quickstart Guide](https://docs.alchemy.com/alchemy/guides/nft-api-quickstart-guide).

{% content-ref url="nft-api-quickstart-guide.md" %}
[nft-api-quickstart-guide.md](nft-api-quickstart-guide.md)
{% endcontent-ref %}

## Introduction&#x20;

Welcome! If you're here, that means you're looking for a great API to work with to build your next NFT project. Well, you're in the right place! Alchemy powers all major NFT platforms as well a majority of DeFi applications, so you can rest assured -- you're in good company.

![](<../../.gitbook/assets/Screen Shot 2022-01-25 at 2.11.39 PM.png>)

{% embed url="https://www.bloomberg.com/news/articles/2021-03-21/nfts-mushroom-into-billion-dollar-market-with-help-from-alchemy" %}

Before you go any further, please visit the [Getting Started](https://docs.alchemy.com/alchemy/introduction/getting-started) guide to set up your Alchemy account. You will need an API key later!

### What is the NFT API?

Alchemy's NFT API allows you to quickly get all the information you need to know about NFTs from the blockchain (i.e. Ethereum, Polygon, Flow). Rather than searching, indexing, and storing data yourself - you can now make one request to fetch specific NFT information for both ERC-721 and ERC-1155 tokens, like:

* All NFTs owned by an address&#x20;
* Metadata and attributes for a specific NFT token

### What can I make?

Using the Alchemy NFT API allows you to both fetch and display NFTs for your users, making it easy to build all kinds of NFT projects. To take some inspiration from existing products, here are some examples you can explore:

#### Build an NFT Marketplace

![OpenSea](<../../.gitbook/assets/Screen Shot 2022-01-25 at 11.46.21 AM.png>)

#### NFT Analytics Platforms

![](<../../.gitbook/assets/Screen Shot 2022-06-30 at 12.09.59 PM.png>)

#### Build On-chain NFT Games

![CryptoRaiders](<../../.gitbook/assets/Screen Shot 2022-01-25 at 11.50.43 AM.png>)

#### Verify Ownership of Digital Assets

![Twitter NFT Profile Pictures](<../../.gitbook/assets/Screen Shot 2022-01-25 at 11.53.44 AM.png>)

#### ... and lots more!

Tell us on [Twitter](https://twitter.com/AlchemyPlatform) what you're trying to build!

### What do requests look like?

We've compiled some super easy to use, copy-and-paste code snippets :innocent:

You can check out the rest of our docs for more in-depth documentation about our endpoints, but for a quick walkthrough with some sample code ready to run, start with this GitHub repository!

{% embed url="https://github.com/alchemyplatform/nft-api-javascript-scripts" %}

## What Chains and Networks are Supported?

### Currently Supported Chains

#### Ethereum&#x20;

\-> Mainnet, Goerli, Rinkeby&#x20;

#### Polygon (Matic)

\-> Mainnet, Mumbai

#### Flow - view docs [here](https://docs.alchemy.com/flow/documentation/flow-nft-apis)

\-> Mainnet

## What NFTs are supported?

All NFTs made with the ERC721 and ERC1155 standards are supported by the NFT API. At the moment, we supports a select number of ERC20 NFTs that pre-date the existance of standaridized NFT contracts.

Alchemy is actively working on adding support for as many blockchains / NFT standards as we can. To influence our roadmap and let your voice be heard, please upvote or add requests here:&#x20;

{% embed url="https://roadmap.alchemy.com/b/feature-requests" %}

Or join our discord! [https://www.alchemy.com/discord](https://www.alchemy.com/discord)

## Quickstart Guides

Check out the guide below to get a quick setup using:

* [The Alchemy SDK,](nft-api-quickstart-guide.md#alchemy-sdk-recommended)
* [the `node-fetch` module,](nft-api-quickstart-guide.md#javascript-fetch)
* [or the `axios`  module.](nft-api-quickstart-guide.md#javascript-axios)

{% content-ref url="nft-api-quickstart-guide.md" %}
[nft-api-quickstart-guide.md](nft-api-quickstart-guide.md)
{% endcontent-ref %}

## API Endpoints Overview

### Ownership Endpoints

*   **``**[**`getNFTs`**](getnfts.md)**``**

    \- Given a user address, returns all of its ERC721 and ERC1155 tokens
*   **``**[**`getNFTsForCollection`**](getnftsforcollection.md)**``**

    \- Given an NFT contract address, returns all NFTs for a given NFT contract.
*   **``**[**`getOwnersForCollection`**](getownersforcollection.md)**``**

    \- Given an NFT contract address, returns all owner addresses.
*   **``**[**`getOwnersForToken`**](getOwnersForToken.md)**``**

    \- Given an NFT contract address and token ID, returns all owner addresses.

### Metadata Endpoints

*   **``**[**`getNFTMetadata`**](getnftmetadata.md)&#x20;

    \- Given an NFT contract address/token ID, returns the metadata, including traits, image URIs, and Alchemy cached NFT media for easy display.
*   **``**[**`getContractMetadata`**](getcontractmetadata.md)**``**

    \- Given an NFT contract address, returns high-level collection/contract level information.
*   **``**[**`reingestContract`**](reingestcontract.md)**``**

    \- Given an NFT collection's address, triggers a refresh of a collection's metadata after a reveal

### Spam Endpoints

*   **``**[**`getSpamContracts`**](getspamcontracts.md)**``**

    \- Returns a list of contracts earmarked as spam by Alchemy.
*   **``**[**`isSpamContract`**](isspamcontract.md)**``**

    \- Given an NFT contract address, checks whether it is on Alchemy's spam list or not.

### Price Endpoints

*   **``**[**`getFloorPrice`**](getfloorprice.md)**``**

    \- Given an NFT collection's address, returns its floor prices by marketplace
