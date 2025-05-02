# WEB3 + Solidity (NFT Auction Platform)

### **Task: Core NFT Auction Platform Development (Simplified for Junior Developer)**

**Objective:**

Build a straightforward and functional NFT auction platform using Solidity, NestJS, PostgreSQL, and React/Next.js. This project focuses on core features like basic NFT sales, simple auction mechanics, and a clean user interface. Designed to be beginner-friendly, the task emphasizes hands-on learning while creating a practical platform that delivers a smooth NFT auction experience. Perfect for gaining foundational skills in blockchain development while working on a real-world project!

---

### **Requirements**

### **1. Smart Contract Development (Solidity)**

**1.1 ERC721 Contract**

- **Sales Phases**:
    - **Private Sale**:
        - Static whitelist (hardcoded or set during deployment).
        - Fixed pricing for private sale NFTs.
    - **Public Sale**:
        - Open to all users with a fixed price.
- **Payment Support**:
    - Accept **ETH** only.
- **Role Management**:
    - Basic ownership model for admin functions (e.g., whitelist and price updates).

---

**1.2 Auction Contract**

- **Auction Types**:
    - Basic **English Auctions** only.
- **Payments**:
    - ETH bids only.

---

**1.3 Testing Expectations for Smart Contracts**

- Foundry tests for:
    - Basic NFT minting and bidding functionality.
    - Admin functions for whitelist and price updates.

---

### **2. Backend Services (NestJS)**

**2.1 RESTful API Endpoints**

- **Public Routes**:
    - `/auctions` (GET): Fetch ongoing auctions.
    - `/nfts` (GET): Fetch available NFTs.
- **Admin Routes**:
    - `/admin/sales` (PATCH): Update sale configurations (price, whitelist).

---

**2.2 Polling Notifications**

- Focus on periodic polling to update auction status.

---

**2.3 Testing Expectations for Backend**

- Unit tests for RESTful API routes.

---

### **3. Frontend (React/Next.js)**

**3.1 Features**

- **Auction Listings**:
    - Display a static list of auctions with manual refresh for updates.
- **Admin Panel**:
    - Allow price updates and managing whitelist.

---

### **4. Database (PostgreSQL)**

- Tables for:
    - **Users**, **NFTs**, and **Auctions**.

---

### **5. Testing and CI/CD**

- Foundry-based tests for smart contracts.
- Unit tests for backend API endpoints.
- Manual deployment process to keep setup straightforward.

---

### **Features Deferred (attention to Ogi), Attention to Hris: <3**

1. Dutch auctions and bundled auction logic.
2. Multi-token payments and Chainlink Oracle integration.
3. Escrow mechanism and royalties.
4. WebSocket support for real-time updates.
5. Multi-tenant backend support.
6. User dashboards, leaderboards, and token flow analytics.
7. Automated CI/CD pipelines.

### **Final Deliverables**

### **1. Smart Contracts**

- Deployed and verified ERC721 and Auction contracts with:
    - Static whitelist for private sale.
    - English auctions with ETH payments only.

### **2. Backend**

- Simple NestJS API with:
    - Auction and NFT endpoints.
    - Basic admin functionality.

### **3. Frontend**

- React/Next.js app with:
    - Static auction listings and basic admin panel.

### **4. Database**

- Minimal PostgreSQL schema for Users, NFTs, and Auctions.

### **5. Testing**

- Foundry tests for basic contract functionality.
- Backend unit tests for API routes.