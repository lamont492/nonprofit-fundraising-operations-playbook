# Architecture Notes

## Objective

Define a practical operating architecture for nonprofit fundraising using CRM, donations, accounting, event management, and communications platforms.

## Core System Roles

### CRM
System of relationship management.

Used for:
- contacts and households
- organization accounts
- donor history
- opportunities and pledges
- campaign attribution
- sponsorship tracking
- reporting inputs

### Donation Platform
System of gift capture.

Used for:
- online giving
- recurring donations
- peer to peer campaigns
- event payments
- donor receipts

### Accounting System
System of financial record.

Used for:
- bank reconciliation
- revenue recognition
- deposits
- audit support
- financial statements

### Event Management Tool
System of event participation and sponsor execution.

Used for:
- registrations
- table sales
- auction or paddle raise tracking
- sponsor visibility management

### Email Marketing Platform
System of outbound communications.

Used for:
- newsletters
- donor campaigns
- stewardship communication
- event reminders

## Source of Truth Guidance

| Data Type | Primary System |
|---|---|
| donor relationship history | CRM |
| online payment transaction | donation platform |
| official financial reporting | accounting system |
| event registration details | event tool |
| campaign email engagement | email platform |

Avoid entering the same transaction manually into multiple systems when integration or controlled reconciliation is available.

## Integration Considerations

### Recommended Principles

- one primary owner per process
- one system of record per data type
- controlled sync direction
- duplicate prevention before automation
- reconciliation before reporting

### Common Integration Paths

- donation platform to CRM
- donation platform to accounting system
- event platform to CRM
- CRM to email platform
- accounting summary back to reporting views

## Common Failure Points

- duplicate donor creation across platforms
- sponsor commitments tracked only in spreadsheets
- finance and fundraising totals do not match
- campaign naming inconsistency across systems
- reporting built before data ownership is defined

## Implementation Notes

- document field mapping before imports
- define campaign hierarchy before first major event
- keep custom fields limited to clear operational need
- test reconciliation with one pilot campaign first
- publish metric definitions before dashboard rollout
