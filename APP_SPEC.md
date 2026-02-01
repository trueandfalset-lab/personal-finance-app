# APP SPECIFICATION

## Overview
This app is a personal finance manager for a single user.
It works offline and is manual-first.
No bank login, no OTP, no automatic money movement.

## Core Modules
- Dashboard
- Bank Accounts
- Loans & EMI
- Assets
- Business / Farm
- Investments
- Credit Score (Internal)

## Dashboard
- Total Net Worth
- Total Bank Balance
- Total Loan Remaining
- Credit Score
- Last Updated Date

Net Worth =
(All Assets + Cash + Investments + Business Value) - (Loans Remaining)

## Bank Accounts
Fields:
- Bank Name
- Account Type
- Balance
- Last Updated
- Notes

## Loans & EMI
Fields:
- Loan Name
- Lender
- Loan Type
- Total Amount
- Paid Amount
- Remaining Amount
- EMI Amount
- Due Date
- Status

## Assets
### Cash
- Amount
- Location

### Jewellery
- Metal Type
- Weight
- Purity
- Estimated Value

### Property / Vehicle
- Type
- Location
- Purchase Price
- Current Value
- Year

## Business / Farm (Generic)
Fields:
- Name
- Category
- Initial Investment
- Monthly Income
- Monthly Expense
- Current Value
- Notes

Category:
- Farming
- Livestock
- Shop
- Online
- Rental
- Manufacturing
- Service
- Custom

## Credit Score (Internal Logic)
- Start Score: 500
+5 = EMI Paid On Time
-30 = EMI Missed
-50 = High Credit Usage

Range: 300 - 900

## Security
- App Lock (PIN)
- Local Encrypted Storage
- No cloud by default

## Future
- Backup / Export
- API Integration
- Multi-user support
