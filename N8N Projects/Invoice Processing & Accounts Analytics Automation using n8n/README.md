# ⚙️ Invoice Processing & Accounts Analytics Automation using n8n

An automated **Invoice Processing & Accounts Analytics workflow** built using **n8n** to automate invoice validation, duplicate detection, payment monitoring, transaction analysis, reconciliation, exception detection, and financial reporting.

The project combines **Workflow Automation, Finance & Accounting, and Data Analytics** to transform raw invoice and transaction data into meaningful financial insights.

---

## 📊 Project Overview

Invoice processing involves multiple manual activities such as validating invoice details, checking duplicate invoices, monitoring payment status, tracking overdue payments, reconciling invoice amounts with transactions, and identifying financial exceptions.

This project demonstrates how **n8n can automate these Finance & Accounting processes** through a structured workflow.

The workflow processes invoice and transaction data from an Excel dataset, performs invoice validation, checks for duplicate invoices, analyzes payment and due-date status, processes transaction records, aggregates valid invoice-related payments, performs reconciliation, detects exceptions, and generates financial analytics for reporting.

The processed data is also prepared for visualization in **Microsoft Power BI**, providing an interactive dashboard for financial analysis and monitoring.

---

## 🎯 Objectives

- Automate invoice data processing
- Validate invoice information
- Identify duplicate invoices
- Analyze payment and due-date status
- Process invoice-related transaction data
- Aggregate valid payment transactions
- Reconcile invoice amounts with transaction payments
- Detect financial exceptions
- Generate financial analytics
- Prepare data for Power BI reporting
- Reduce manual finance and accounting processing effort

---

## 🛠️ Tools & Technologies

- **n8n** – Workflow Automation
- **Microsoft Excel** – Invoice & Transaction Dataset
- **Google Drive** – File Storage & Input
- **Power BI** – Data Visualization & Dashboard

---

## 📂 Dataset

The project uses an Excel workbook containing two main datasets:

### 🧾 Invoices

The invoice dataset contains information such as:

- Invoice ID
- Invoice Date
- Due Date
- Vendor ID
- Vendor Name
- Purchase Order Number
- Category
- Currency
- Subtotal
- Tax Rate
- Tax Amount
- Total Amount
- Payment Status
- Paid Amount
- Balance Due
- Payment Method
- Payment Terms
- Invoice Status
- Source

### 💳 Transactions

The transaction dataset contains information such as:

- Transaction ID
- Transaction Date
- Invoice ID
- Vendor ID
- Transaction Amount
- Transaction Type
- Payment Method
- Reference Number
- Currency
- Transaction Status
- Description

---

## 🔄 Workflow Process

```text
Start Invoice Processing
        ↓
Google Drive – Download File
        ↓
Extract Invoice Data
        ↓
Validate Invoice Data
        ↓
Duplicate Invoice Check
        ↓
Payment & Due Date Check
        │
        │
        └─────────────────────┐
                              ↓
Transaction Data → Transaction Analysis
                              ↓
                 Aggregate Transaction Analysis
                              ↓
                           Merge
                              ↓
                       Reconciliation
                              ↓
                     Exception Detection
                              ↓
                     Financial Analytics
                              ↓
                      Final Reporting
```
---

## 🔍 Workflow Features

### 🧾 Invoice Validation

The workflow validates important invoice fields such as:

- Invoice ID
- Invoice Date
- Due Date
- Total Amount
- Due-date consistency

Each invoice is classified as **Valid** or **Invalid**, with validation errors recorded when required.

### 🔁 Duplicate Invoice Detection

Invoice IDs are checked across the dataset to identify duplicate invoice records.

This helps reduce the risk of duplicate invoice processing and duplicate payments.

### 💳 Payment & Due-Date Monitoring

Invoice payment information and due dates are analyzed to identify:

- Paid invoices
- Due invoices
- Overdue invoices
- Outstanding balances

### 📊 Transaction Analysis

Transaction records are analyzed based on invoice ID, transaction type, transaction status, description, and transaction amount.

Valid invoice-related payment transactions are identified and aggregated for reconciliation.

### 🔄 Reconciliation

Invoice amounts are compared with valid transaction payment amounts.

The reconciliation process identifies:

- Fully Matched
- Underpaid
- Overpaid
- No Payment

### ⚠️ Exception Detection

The workflow identifies invoices requiring further review, including:

- Invalid Invoice
- Duplicate Invoice
- Overdue Payment
- Underpaid
- Overpaid
- No Payment

### 📈 Financial Analytics

The workflow generates key financial metrics including:

- Total Invoices
- Total Invoice Amount
- Total Paid Amount
- Total Balance Due
- Overdue Invoices
- Exception Invoices
- Duplicate Invoices
- Valid Invoices

---

## 📌 Key Results

| KPI | Result |
|---|---:|
| **Total Invoices Processed** | **819** |
| **Total Invoice Amount** | **₹68.12 Million** |
| **Total Paid Amount** | **₹21.65 Million** |
| **Total Balance Due** | **₹24.44 Million** |
| **Overdue Invoices** | **360** |
| **Exception Invoices** | **360** |
| **Duplicate Invoices** | **0** |
| **Valid Invoices** | **819** |

---

## 📈 Key Insights

### 💰 Financial Analysis

- The workflow processed **819 invoices** through the final analytics stage.
- The total invoice value processed was approximately **₹68.12 Million**.
- Valid transaction payments identified were approximately **₹21.65 Million**.
- The workflow provides visibility into invoice values, payments, and outstanding balances.

### ⏰ Payment Analysis

- **360 invoices** were identified as overdue.
- Overdue invoices can be prioritized for payment follow-up.
- Due-date monitoring provides better visibility into payment obligations.

### ⚠️ Exception Analysis

- **360 invoices** were identified with exceptions in the processed dataset.
- Exception detection helps identify invoices requiring further review.
- Exceptions can be related to overdue payments, reconciliation differences, validation issues, duplicate records, or missing payments.

### 🔄 Reconciliation Analysis

- Invoice amounts are compared against **valid transaction payments**.
- The reconciliation process helps identify **underpaid, overpaid, fully matched, and unpaid invoices**.
- Transaction-level analysis provides better visibility into actual payment activity.

---

## 📊 Power BI Dashboard

The processed invoice data is visualized using **Microsoft Power BI** for interactive financial analysis.

### Dashboard Components

- Total Invoices
- Total Invoice Amount
- Total Paid Amount
- Total Balance Due
- Invoice Due Status
- Exception Type Analysis
- Vendor-wise Invoice Amount
- Category-wise Invoice Amount
- Payment Method-wise Invoice Amount
- Payment Status Analysis

### Interactive Filters

- Vendor Name
- Category
- Due Status
- Payment Status

---

## 🎯 Business / Financial Value

This automation helps to:

- Reduce manual invoice processing
- Improve invoice data validation
- Identify duplicate invoices
- Monitor overdue payments
- Track outstanding balances
- Automate payment reconciliation
- Detect financial exceptions
- Improve financial reporting
- Support faster financial analysis and decision-making

---

## 🔄 End-to-End Project Flow

```text
Invoice & Transaction Data
            ↓
       Data Extraction
            ↓
     Invoice Validation
            ↓
   Duplicate Detection
            ↓
 Payment & Due-Date Check
            ↓
    Transaction Analysis
            ↓
 Transaction Aggregation
            ↓
          Merge
            ↓
      Reconciliation
            ↓
    Exception Detection
            ↓
    Financial Analytics
            ↓
     Final Reporting
            ↓
      Power BI Dashboard
```

---

## 📚 Skills Demonstrated

- n8n Workflow Automation
- Invoice Processing
- Data Validation
- Duplicate Detection
- Payment Monitoring
- Due-Date Analysis
- Transaction Analysis
- Financial Reconciliation
- Exception Detection
- Financial Analytics
- Power BI Dashboard Development
- Data Visualization
- Finance & Accounting Analysis
- Insight Generation
  
---

## 🚀 Project Outcome

The project demonstrates how **n8n can automate Finance & Accounting processes** while supporting Data Analytics and Power BI reporting.

It transforms raw invoice and transaction data into a structured workflow for:

**Invoice Validation → Payment Monitoring → Transaction Analysis → Reconciliation → Exception Detection → Financial Analytics → Reporting**

The final solution provides a practical approach to improving **invoice processing, payment monitoring, financial reconciliation, and reporting efficiency**.
