# DATABASE SCHEMA

## Tables

### 1. Users
- user_id (PK)
- pin (Encrypted)
- last_login

### 2. Banks
- bank_id (PK)
- user_id (FK → Users.user_id)
- bank_name
- account_type
- balance
- notes
- last_updated

### 3. Loans
- loan_id (PK)
- user_id (FK → Users.user_id)
- loan_name
- lender
- total_amount
- paid_amount
- remaining_amount
- emi_amount
- due_date
- status

### 4. Assets
- asset_id (PK)
- user_id (FK → Users.user_id)
- asset_type (Cash / Jewellery / Property / Vehicle)
- name
- value
- location
- details (JSON or Notes)

### 5. Businesses
- business_id (PK)
- user_id (FK → Users.user_id)
- name
- category
- initial_investment
- monthly_income
- monthly_expense
- current_value
- notes

### 6. Investments
- investment_id (PK)
- user_id (FK → Users.user_id)
- type (FD / RD / MF / Stocks / Digital Gold / Other)
- amount
- current_value
- notes

### 7. CreditScore
- score_id (PK)
- user_id (FK → Users.user_id)
- current_score
- on_time_emi
- missed_emi
- active_loans
- last_updated

## Notes
- All date fields stored in ISO format (YYYY-MM-DD)
- All monetary values stored as decimal
- User_id links all personal data
