# How it works

Trugate Invoice acts as a middleware layer between business systems and the fiscal clearance process.

## Standard workflow

1. A user or ERP submits invoice data.
2. Trugate validates the invoice fields and tax logic.
3. Trugate transforms the invoice into the required electronic format.
4. Trugate sends the invoice to the clearance process.
5. Trugate receives the response.
6. If cleared, Trugate generates a trusted invoice record and PDF with verification data.
7. Trugate returns the result through the dashboard or webhook/API.

## Business value

This workflow allows businesses to stay focused on invoicing while Trugate handles compliance orchestration.

## Example flow

```mermaid
graph TD
A[Business or ERP submits invoice] --> B[Trugate validation]
B --> C[Format generation]
C --> D[Fiscal clearance]
D --> E[Cleared invoice record]
E --> F[PDF and QR generation]
E --> G[Webhook / API status update]