# Sonastream Protocol Takehome

     ___  _____  _  _    __      ___  ____  ____  ____    __    __  __ 
    / __)(  _  )( \( )  /__\    / __)(_  _)(  _ \( ___)  /__\  (  \/  )
    \__ \ )(_)(  )  (  /(__)\   \__ \  )(   )   / )__)  /(__)\  )    ( 
    (___/(_____)(_)\_)(__)(__)  (___/ (__) (_)\_)(____)(__)(__)(_/\/\_)

## Description
The goal of this takehome exercise is to create an upgradeable, NFT minting contract. We prefer submissions to use Solidity and Foundry, but are open to any implementation language and testing framework of your choosing (e.g. vyper/huff + ape/hardhat)

## Requirements
- Create an ERC721 NFT Minting contract that allows a caller to pass multiple IPFS CIDs at a time to mint their NFTs
  - The contract should include:
    - The ability to retrieve uri from a token id + contract address
    - The ability for only authorized users to update the underlying CID of an NFT
    - The ability for freeze an NFTs CID to prevent future CID updates
    - The ability to burn a track
- Make the ERC721 NFT Minting contract `upgradeable` using any implementation of your choosing. Please explain your reasoning and why you chose a certain implementation over others
- Write a deploy script that allows the takehome evaluator to deploy the minting contract to a local node and call the contract methods
- Add test coverage, comments and any simple gas optimizations and their reasonings for how they might save gas at runtime or deploy time

## Deliverables
- Implement your solution, including test cases for the smart contract code (fuzzing is a plus)
- Include a `README.md` that describes how to set up, run and test your smart contracts 
- Include any notes for our engineering team that describes your approaches and assumptions
- Email your point of contact that sent you this exercise with a link to a public Github or Gitlab repository.
    - If you are uncomfortable adding this project to your public Github profile, please make a separate account for this submission

## Notes
- Please show us strengths of your engineering abilities, technical design and attention to detail. While small/simple, this takehome is the main way we will assess your technical abilities. 