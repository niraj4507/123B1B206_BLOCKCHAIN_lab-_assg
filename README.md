# 🧠 Blockchain Lab Assignments

## 👤 Student Details
- **Name:** Prathmesh Marathe  
- **Roll Number:** 123B1B186
- **Course Name:** Blockchain Lab  

---

## 📌 Overview
This repository contains a complete set of blockchain lab assignments demonstrating core concepts of Web3 development, including smart contracts, decentralized applications, IPFS storage, and DAO governance.

---

## 📁 Assignment Descriptions

### 🔹 Assignment 1: Smart Contract Development
Implemented a **MessageStore smart contract** using Solidity that allows storing and updating a message on the blockchain. It demonstrates the use of state variables, constructors, and functions.

---

### 🔹 Assignment 2: Polygon Deployment
Deployed the smart contract on the **Polygon Amoy Testnet**, showcasing improved scalability and reduced transaction costs compared to Ethereum.

---

### 🔹 Assignment 3: Web Interface + MetaMask
Developed a **frontend decentralized application (DApp)** using HTML, CSS, and JavaScript that interacts with the smart contract using **ethers.js** and MetaMask.

---

### 🔹 Assignment 4: IPFS Integration
Implemented decentralized file storage using **IPFS via Pinata**, allowing users to upload files and retrieve them using a unique CID (Content Identifier).

---

### 🔹 Assignment 5: DAO Smart Contract
Created a basic **Decentralized Autonomous Organization (DAO)** where users can create proposals, vote on them, and execute decisions based on voting results.

---

## 🛠️ Tech Stack Used
- Solidity  
- Remix IDE  
- MetaMask  
- Ethers.js  
- HTML, CSS, JavaScript  
- Sepolia Testnet  
- Polygon Amoy Testnet  
- IPFS (Pinata)  

---

## 🚀 How to Run Each Assignment

### ▶️ Assignment 1 & 2 (Smart Contracts)
1. Open Remix IDE: https://remix.ethereum.org  
2. Open the `.sol` file  
3. Compile the contract  
4. Go to **Deploy & Run Transactions**  
5. Select **Browser Provider (MetaMask)**  
6. Connect MetaMask wallet  
7. Choose network:
   - Sepolia (Assignment 1)
   - Polygon Amoy (Assignment 2)
8. Click **Deploy** and confirm  

---

### ▶️ Assignment 3 (Web DApp)
1. Open terminal in `assignment-3` folder  
2. Run:
   ```bash
   python -m http.server 3000
3. Open browser: http://127.0.0.1:3000
4. Connect MetaMask
5. Send and retrieve data

---

### ▶️ Assignment 4 (IPFS File Storage)
1. Open index.html (or use Live Server)
2. Upload a file
3. Copy generated CID
4. Paste CID to retrieve file

---

### ▶️ Assignment 4 (DAO Smart Contract)
1. Open Remix IDE
2. Compile dao.sol
3. Deploy using MetaMask
4. Interact with:
- createProposal
- vote    
- executeProposal
5. View results using getProposals()