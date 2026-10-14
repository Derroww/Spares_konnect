# Product Requirements Document (PRD): Spares Konnect

## 1. Overview & Vision
Spares Konnect is a specialized digital platform designed to bridge local garage owners and independent mechanics with efficient spare parts and stock management. It eliminates inventory leakage and tracking discrepancies by tying every parts movement directly to workshop job cards.

## 2. Target User Personas
- **Garage Owners / Shop Managers:** Need visibility into parts expenditure, inventory valuation, technician efficiency, and low-stock replenishment.
- **Floor Mechanics:** Need fast, mobile-friendly ways to request, reserve, log, and return parts against active vehicle job cards.
- **Spare Parts Vendors:** Local suppliers linked to the platform to fulfill purchase requests and streamline B2B parts delivery.

## 3. Core Functional Requirements
- **Job-Linked Inventory Ledger:** Track parts across 5 distinct states: *Received*, *Reserved*, *Used*, *Returned*, and *Sold*, linked directly to an individual repair job card[cite: 2].
- **Real-Time Stock Management:** Live inventory level tracking with automated triggers/alerts when fast-moving service items drop below threshold[cite: 2].
- **Audit & Returns Trail:** Complete transaction history tracking core charges, supplier returns, and warranty replacements to minimize monthly discrepancies[cite: 2].

## 4. Non-Functional Requirements
- **Mobile Responsiveness:** The mechanic interface must be fully optimized for smartphones and tablets used directly on the workshop floor.
- **Data Integrity & Security:** Secure JWT-based authentication[cite: 2] and strict relational constraints preventing negative inventory counts.