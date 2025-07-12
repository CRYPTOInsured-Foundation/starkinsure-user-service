# StarkInsure User Service

The **StarkInsure User Service** is a Nest.js application handling user identity, authentication, and KYC processes for the StarkInsure DeFi insurance platform. It integrates with StarkNet for wallet-based identity verification and secure user management. This service runs on port `5000`.

---

## 🔗 API Documentation  
[View Swagger Docs](http://localhost:5000/docs) | [StarkNet Identity Spec](https://docs.starknet.io/identity/)

---

## ✨ User Features  
- **StarkNet Wallet Authentication**:  
  - ArgentX/Braavos wallet login  
  - SIWE (Sign-In With Ethereum) integration  
- **Compliance**:  
  - KYC/AML verification flows  
  - Identity attestation via Cairo contracts  
- **Security**:  
  - Multi-factor authentication  
  - Session management with zk-proofs  
- **Profile Management**:  
  - Insurance policy preferences  
  - Claim history tracking  

---

## 🛠️ Tech Stack  
| Component           | Technology                                                                 |
|---------------------|---------------------------------------------------------------------------|
| Framework           | [Nest.js](https://nestjs.com/)                                           |
| Authentication     | [SIWE](https://login.xyz/) + [StarkNet.js](https://www.starknetjs.com/)  |
| Database           | PostgreSQL + [Prisma](https://www.prisma.io/)                            |
| Compliance        | [Sumsub](https://sumsub.com/) API integration                           |
| Queue              | [BullMQ](https://docs.bullmq.io/) (for KYC processing)                  |

---

## 🚀 Quick Start  

### Prerequisites  
- Node.js v18+  
- PostgreSQL 14+  
- StarkNet devnet (for testing)  
- Sumsub API keys (for KYC)  

### Installation  
1. **Clone the repo**:  
   ```bash
   git clone https://github.com/CRYPTOInsured-Foundation/starkinsure-user-service.git
   cd starkinsure-user-service
   ```
2. **Install dependencies**:
   ```bash
   pnpm install
   ```
3. Setup environment:
   ```bash
   cp .env.example .env
   ```
## 🤝 Contributing

1. Fork the repository
2. Create your feature branch:
```bash
git checkout -b feat/your-feature
```
3. Commit changes following Conventional Commits
4. Push to the branch:
   ```bash
   ```
5. Open a Pull Request
