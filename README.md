# NFT Auction Platform Monorepo

This monorepo contains all components of the NFT Auction Platform: smart contracts, backend API, and frontend application.

## Project Structure

```
nft-auction-monorepo/
├── smart-contracts/     # Foundry Solidity project
├── backend/             # NestJS backend API
└── frontend/            # React frontend
```

## Components

### Smart Contracts (Foundry)

Solidity smart contracts for the NFT auction platform, including:
- ERC721 NFT contract with private and public sale phases
- English auction contract
- Tests using Foundry

### Backend (NestJS)

REST API providing auction data and admin functionality:
- Auction and NFT endpoints
- Admin routes for sale configuration
- PostgreSQL database integration

### Frontend (React)

User interface for interacting with the auction platform:
- Auction listings
- Admin panel for managing sales
- Web3 wallet integration

## Getting Started

### Prerequisites

- Node.js (v16+)
- Foundry (for smart contract development)
- PostgreSQL
- Git

### Installation

1. Clone this repository:
```
git clone https://github.com/iliyanB-lime/nft-auction-monorepo.git
cd nft-auction-monorepo
```

2. Install dependencies for each project:

```
# Smart Contracts
cd smart-contracts
forge install

# Backend
cd ../backend
npm install

# Frontend
cd ../frontend
npm install
```

### Running the Projects

#### Smart Contracts
```
cd smart-contracts
forge build
forge test
```

#### Backend
```
cd backend
npm run start:dev
```

#### Frontend
```
cd frontend
npm run dev
```

## Features

- NFT minting with private and public sale phases
- English auctions for NFTs
- ETH payment support
- Admin functionality for whitelist and price management
- Basic auction listings and management UI

## Testing

- Smart Contracts: Foundry tests
- Backend: Unit tests for API endpoints
- Frontend: Manual testing

## License

[MIT](LICENSE) 