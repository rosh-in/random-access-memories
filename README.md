# Random Access Memories - dApp

> Demo - https://www.loom.com/share/e5aedafd5e6744a6b1e3a9372294b6bd

> Built for a web3 hackathon.

Random Access Memories is a decentralized image‑sharing dapp that lets users to post images to an anonymous network of contributors and scroll a shared feed of all photos.


## What it does

- Lets users **post images** to a common pool.
- Shows a **global feed** of all images from all contributors.
- Uses **wallet-based login** instead of usernames and passwords.
- Anchors image data and ownership using web3 tools.

## Why we built it

Most social media apps are centralized. They control:

- Who can publish and see content.
- How long content stays up.
- How feeds are ordered.

We wanted to explore how an image feed could work if it was:

- Backed by **wallet identities** instead of app accounts.
- Using **IPFS / decentralized storage** for media.
- Running on **Polygon** so it stays cheap to use.

## How it works (high level)

- Users connect their wallet.
- When they upload an image:
  - The image is stored off‑chain (on IPFS).
  - A Solidity contract on Polygon stores a reference (hash) plus the sender address.
- The feed simply reads all stored image entries from the contract and renders them.

## Tech stack

- **Frontend**: React
- **Smart contracts**: Solidity
- **Blockchain**: Polygon
- **Storage**: IPFS - Interplanetary File System
