# EU Unified Instant Payments App  
**Product Requirements Document (PRD)**  
**Version:** v1.0  
**Author:** Ayush Jha  
**Date:** Feb 2026  
**Status:** Draft

---

# 1. Executive Summary

This PRD proposes a BHIM-like unified instant payments application for the European Union that enables **phone-number–based alias payments (VPA-like)** for both peer-to-peer (P2P) and peer-to-merchant (P2M) use cases.

The product operates on top of **SEPA Instant** and Open Banking APIs, focusing on solving the **product and UX fragmentation** that currently exists across EU banks.

The app does **not replace payment rails**; it standardizes identity, UX, and orchestration to enable fast, low-friction everyday payments.

---

# 2. Problem Statement

## 2.1 Current State

Despite the availability of instant payment infrastructure in the EU, users face:

- IBAN-heavy payment flows  
- Inconsistent UX across banks  
- Poor cross-bank experience  
- Weak failure transparency  
- Continued reliance on third-party apps (Wise, PayPal)

## 2.2 Key Insight

> SEPA Instant solves settlement speed but does not standardize identity abstraction or consumer experience.

## 2.3 Opportunity

Build a bank-agnostic product layer that:

- Removes IBAN friction  
- Introduces phone-number aliases (VPA-like)  
- Unifies UX across banks  
- Enables low-cost merchant acceptance  

---

# 3. Product Vision

> Enable EU users to send and receive money as easily as sending a message using a phone-number–based payment identity.

---

# 4. Goals & Success Metrics

## 4.1 North Star Metric

**Monthly Successful Instant Transactions per Active User**

---

## 4.2 Primary Success Metrics

### Consumer

- Bank linking completion rate  
- First payment activation rate (≤ 7 days)  
- Payment success rate  
- Average payment completion time  
- 30-day retention  

### Merchant

- Merchant onboarding completion  
- Time to first transaction  
- Daily active merchants  
- Merchant repeat transaction rate  

### System Health

- SEPA Instant success %  
- Alias resolution success %  
- Payment failure rate  
- Bank downtime impact  

---

# 5. Target Users

## 5.1 Primary Users (Consumers)

EU residents who:

- Send money to friends/family  
- Split bills  
- Pay small merchants  
- Prefer mobile-first payments  

### User Needs

- Simplicity  
- Speed  
- Trust  
- Predictability  

---

## 5.2 Secondary Users (Merchants)

Small businesses and freelancers who want:

- Low-cost acceptance  
- Instant settlement  
- No card hardware dependency  

---

# 6. Product Scope

---

## 6.1 Must Have (Launch)

### Consumer

- Bank account linking via Open Banking  
- **Phone-number–based alias (primary identity)**  
- P2P instant payments  
- Unified transaction history  
- Failure & retry UX  

### Merchant

- Business onboarding (light KYB)  
- QR-based payment acceptance  
- Business phone alias  
- Basic merchant dashboard  
- Instant settlement visibility  

---

## 6.2 Should Have (Post-launch)

- Payment requests  
- Bill splitting  
- Multi-language support  
- Merchant analytics (basic)  

---

## 6.3 Won’t Have (v1)

- Lending / credit  
- Card issuing or acquiring  
- Non-EU transfers  
- Crypto/CBDC support  
- Inventory or POS systems  

---

# 7. Key Product Flows

---

## 7.1 Consumer Onboarding

**Flow**

1. User downloads app  
2. Consents to Open Banking  
3. Links bank account  
4. Registers phone number  
5. Phone verified via OTP  
6. Alias mapped to IBAN  
7. User lands on home screen  

**Success Criteria:** Onboarding completed in < 2 minutes.

---

## 7.2 P2P Payment Flow

**Flow**

1. User taps "Send"  
2. Enters recipient phone number  
3. System resolves alias → IBAN  
4. User confirms amount  
5. Payment initiated via SEPA Instant  
6. Real-time success/failure displayed  

**Target latency:** < 10 seconds

---

## 7.3 Merchant Payment Flow (P2M)

**Flow**

1. Merchant generates QR code  
2. Consumer scans QR  
3. Merchant phone alias resolved  
4. Consumer confirms payment  
5. Instant settlement to merchant  

**Goal:** Compete with card UX for small-value payments.

---

# 8. Alias System (Phone-Based, VPA-Like)

---

## 8.1 Design Principle

The phone number acts as the **primary payment identifier**, similar to UPI VPA behavior.

Mapping model:

# EU Unified Instant Payments App  
**Product Requirements Document (PRD)**  
**Version:** v1.0  
**Author:** Ayush Jha  
**Date:** Feb 2026  
**Status:** Draft

---

# 1. Executive Summary

This PRD proposes a BHIM-like unified instant payments application for the European Union that enables **phone-number–based alias payments (VPA-like)** for both peer-to-peer (P2P) and peer-to-merchant (P2M) use cases.

The product operates on top of **SEPA Instant** and Open Banking APIs, focusing on solving the **product and UX fragmentation** that currently exists across EU banks.

The app does **not replace payment rails**; it standardizes identity, UX, and orchestration to enable fast, low-friction everyday payments.

---

# 2. Problem Statement

## 2.1 Current State

Despite the availability of instant payment infrastructure in the EU, users face:

- IBAN-heavy payment flows  
- Inconsistent UX across banks  
- Poor cross-bank experience  
- Weak failure transparency  
- Continued reliance on third-party apps (Wise, PayPal)

## 2.2 Key Insight

> SEPA Instant solves settlement speed but does not standardize identity abstraction or consumer experience.

## 2.3 Opportunity

Build a bank-agnostic product layer that:

- Removes IBAN friction  
- Introduces phone-number aliases (VPA-like)  
- Unifies UX across banks  
- Enables low-cost merchant acceptance  

---

# 3. Product Vision

> Enable EU users to send and receive money as easily as sending a message using a phone-number–based payment identity.

---

# 4. Goals & Success Metrics

## 4.1 North Star Metric

**Monthly Successful Instant Transactions per Active User**

---

## 4.2 Primary Success Metrics

### Consumer

- Bank linking completion rate  
- First payment activation rate (≤ 7 days)  
- Payment success rate  
- Average payment completion time  
- 30-day retention  

### Merchant

- Merchant onboarding completion  
- Time to first transaction  
- Daily active merchants  
- Merchant repeat transaction rate  

### System Health

- SEPA Instant success %  
- Alias resolution success %  
- Payment failure rate  
- Bank downtime impact  

---

# 5. Target Users

## 5.1 Primary Users (Consumers)

EU residents who:

- Send money to friends/family  
- Split bills  
- Pay small merchants  
- Prefer mobile-first payments  

### User Needs

- Simplicity  
- Speed  
- Trust  
- Predictability  

---

## 5.2 Secondary Users (Merchants)

Small businesses and freelancers who want:

- Low-cost acceptance  
- Instant settlement  
- No card hardware dependency  

---

# 6. Product Scope

---

## 6.1 Must Have (Launch)

### Consumer

- Bank account linking via Open Banking  
- **Phone-number–based alias (primary identity)**  
- P2P instant payments  
- Unified transaction history  
- Failure & retry UX  

### Merchant

- Business onboarding (light KYB)  
- QR-based payment acceptance  
- Business phone alias  
- Basic merchant dashboard  
- Instant settlement visibility  

---

## 6.2 Should Have (Post-launch)

- Payment requests  
- Bill splitting  
- Multi-language support  
- Merchant analytics (basic)  

---

## 6.3 Won’t Have (v1)

- Lending / credit  
- Card issuing or acquiring  
- Non-EU transfers  
- Crypto/CBDC support  
- Inventory or POS systems  

---

# 7. Key Product Flows

---

## 7.1 Consumer Onboarding

**Flow**

1. User downloads app  
2. Consents to Open Banking  
3. Links bank account  
4. Registers phone number  
5. Phone verified via OTP  
6. Alias mapped to IBAN  
7. User lands on home screen  

**Success Criteria:** Onboarding completed in < 2 minutes.

---

## 7.2 P2P Payment Flow

**Flow**

1. User taps "Send"  
2. Enters recipient phone number  
3. System resolves alias → IBAN  
4. User confirms amount  
5. Payment initiated via SEPA Instant  
6. Real-time success/failure displayed  

**Target latency:** < 10 seconds
