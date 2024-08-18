# 100xDevs-Blockchain
 This project implements a simplified version of a Bitcoin-like cryptocurrency system, featuring a central server for miners to communicate, miner servers for blockchain management, and a frontend for user interaction. The tech stack includes Node.js, React, Tailwind CSS, Express, and WebSocket (ws).

## Table of Contents

- [100xDevs-Blockchain](#100xdevs-blockchain)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Architecture](#architecture)
    - [1. Central Server](#1-central-server)
    - [2. Miner Server](#2-miner-server)
    - [3. Frontend](#3-frontend)
  - [Tech Stack](#tech-stack)
  - [Features](#features)
    - [Central Server](#central-server)
    - [Miner Server](#miner-server)
    - [Frontend](#frontend)
  - [Setup Instructions](#setup-instructions)
    - [Prerequisites](#prerequisites)
    - [Installation](#installation)

## Overview

This project aims to simulate the core components of a Bitcoin-like cryptocurrency network. It includes a central WebSocket server that facilitates communication between miners, individual miner servers responsible for creating and verifying blocks, and a frontend interface for users to create wallets, sign transactions, and interact with the network.

## Architecture

### 1. Central Server
- **Purpose:** Acts as a communication hub for all connected miner servers.
- **Technology:** WebSocket server using Node.js and `ws`.

### 2. Miner Server
- **Purpose:** 
  - Performs proof of work (PoW) to create blocks.
  - Verifies transaction signatures and balances.
  - Manages its local copy of the blockchain.
  - Rejects smaller or erroneous blockchains.
  - Syncs with the latest blockchain on startup.
- **Technology:** Node.js, Express, and `ws`.

### 3. Frontend
- **Purpose:** 
  - Allows users to create a BTC wallet.
  - Enables users to sign and send transactions to miner servers.
  - Displays transaction history and blockchain sync status.
- **Technology:** React, Tailwind CSS.

## Tech Stack

- **Node.js:** Backend server for both the central server and miner servers.
- **Express:** API framework for the miner servers.
- **WebSocket (ws):** Real-time communication between servers.
- **React:** Frontend framework for user interaction.
- **Tailwind CSS:** Utility-first CSS framework for responsive design.

## Features

### Central Server
- Broadcasts messages between connected miners.
- Manages the network of miner servers.

### Miner Server
- Performs proof of work and block creation.
- Verifies signatures and transaction validity.
- Rejects invalid blocks and ensures blockchain integrity.
- Syncs with the latest blockchain on startup.

### Frontend
- Wallet creation with a unique address.
- Transaction signing and submission to miner servers.
- Real-time display of transaction history and blockchain status.

## Setup Instructions

### Prerequisites
- Node.js (v14+)
- npm (v6+)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/mohitchaudhary2207/100xDevs-Blockchain.git
   cd bitcoin-like-server
