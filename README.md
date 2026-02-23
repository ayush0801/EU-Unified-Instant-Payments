# EuroSwift - Unified Instant Payments for Europe

A BHIM-inspired unified payments application for the European Union enabling **phone-number–based P2P transfers** and **QR-based merchant payments** on top of **SEPA Instant** and **Open Banking**.

---

## 🚀 Overview

EuroSwift is designed as a **Payment Initiation Service Provider (PISP)** that simplifies bank-to-bank payments across Europe by introducing a **phone alias abstraction layer**, similar to UPI in India.

The platform does **not hold user funds**. Instead, it orchestrates payments directly between bank accounts using SEPA Instant rails.

**Goal:**  
Make sending money in Europe as simple as sending a message.

---

## 🎯 Problem Statement

Despite SEPA Instant availability, EU payments still suffer from:

- IBAN-heavy user experience  
- Fragmented bank interfaces  
- Poor cross-bank UX consistency  
- Limited low-cost merchant acceptance for small businesses  
- Lack of a unified consumer payments layer  

---

## 💡 Solution

EuroSwift introduces:

- 📱 Phone-number-based payment identity (alias)  
- ⚡ Real-time P2P transfers via SEPA Instant  
- 🧾 QR-based merchant payments  
- 🏦 Bank-agnostic experience via Open Banking  
- 🔔 Real-time payment status and notifications  

---

## 🧩 Key Features

### Consumer

- Bank linking via Open Banking  
- Phone alias registration  
- Instant P2P payments  
- QR scan & pay  
- Real-time payment status  
- Failure handling & retry UX  

### Merchant

- Business alias mapping  
- Static QR acceptance  
- Instant settlement visibility  
- Low-cost acceptance model  

---

## 🏗️ System Architecture

The platform operates as a **PISP orchestration layer** between users and banks.

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/0b3a69f3-c052-4c8b-8c0e-fd225e790822" />


---

## 🔄 How Money Flows

### 1️⃣ Bank Linking

1. User selects bank in the mobile app  
2. App redirects to bank via Open Banking  
3. User completes **Strong Customer Authentication (SCA)**  
4. Bank grants consent token  
5. User account is linked (no funds stored)

---

### 2️⃣ P2P Payment (Phone Alias)

1. User enters recipient phone number  
2. Alias Directory resolves **Phone → IBAN**  
3. Risk & limits checks executed  
4. Payment initiated via Open Banking  
5. Sender bank performs SCA  
6. SEPA Instant transfers funds  
7. Recipient bank credits account  
8. User receives real-time confirmation  

**Target settlement:** < 10 seconds

---

### 3️⃣ Merchant QR Payment

1. Merchant displays static QR  
2. User scans QR via mobile app  
3. Merchant alias resolved  
4. Payment initiated via PISP flow  
5. SEPA Instant settles funds  
6. Merchant receives confirmation webhook  

---

## 🧱 Tech & Product Stack

**Product & Design**

- Figma - UX flows & prototype  
- Notion - PRD & planning  
- Stitch AI - UI generation  

**Architecture**

- Mermaid / Eraser - system design  
- GitHub - documentation  

**Analysis**

- Excel - merchant economics  
- KPI framework defined  

---

## 📊 Success Metrics

### Consumer

- Bank linking success rate  
- First payment activation  
- Payment success rate  
- Time to complete payment  
- 30-day retention  

### Merchant

- Merchant activation rate  
- Time to first transaction  
- Repeat transaction rate  
- Cost vs card MDR savings  

### System Health

- SEPA Instant success %  
- Alias resolution latency  
- Payment failure rate  

---

## 🔐 Compliance Positioning

EuroSwift is designed to operate under EU regulations:

- Acts as **PISP under PSD2/PSD3**  
- Banks perform KYC/KYB  
- SCA handled by issuing bank  
- No custody of customer funds  
- Uses SEPA Instant (SCT Inst) rail  

---

## 🚧 Future Roadmap

- Request-to-Pay (R2P)  
- Cross-border extensions  
- Merchant analytics  
- Smart rail routing  
- Value-added merchant services  

---

## 👤 Author

**Ayush Jha**  
Product Manager 

- Strong focus on instant payments, Open Banking, and risk-aware product design  
- Background in backend systems and financial workflows  

---

## ⭐ Why This Project Matters

This project demonstrates:

- End-to-end fintech product thinking  
- EU payments ecosystem understanding  
- PISP architecture knowledge  
- UX + systems + business alignment  
- Production-realistic design decisions  

---

**Status:** Portfolio Project - Ready for review & feedback
