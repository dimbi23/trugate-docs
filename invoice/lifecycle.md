# Invoice lifecycle

An invoice in TruGate e-Invoice moves through a clear state model.

## Statuses

### Draft
The invoice exists in the system but has not yet been submitted for clearance.

### Processing
The invoice has been submitted and is undergoing validation or clearance.

### Cleared
The invoice has passed clearance and has an official trusted status.

### Rejected
The invoice was rejected due to validation or clearance errors.

### Failed
The invoice could not complete processing because of technical issues or interrupted workflows.

## Why status clarity matters

Businesses and integrators need to understand whether an invoice is:
- still editable,
- legally valid,
- blocked by a business rule,
- or affected by a technical issue.

## Recommended lifecycle diagram

```mermaid
graph TD
A[Draft] --> B[Processing]
B --> C[Cleared]
B --> D[Rejected]
B --> E[Failed]