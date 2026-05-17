# Product Backlog — User Stories
## PayFlow Open Banking Payments Feature

---

## Backlog Summary

| Story ID | Title | Epic | Story Points | Sprint | Priority |
|----------|-------|------|--------------|--------|----------|
| POB-01 | OAuth Bank Authentication | POB-E1 | 8 | Sprint 1 | Highest |
| POB-02 | Two-Factor Authentication on Payments | POB-E1 | 5 | Sprint 1 | Highest |
| POB-03 | Connect Bank Account | POB-E2 | 13 | Sprint 1 | Highest |
| POB-04 | View Bank Connection Status | POB-E2 | 3 | Sprint 2 | High |
| POB-05 | Initiate a Payment | POB-E3 | 13 | Sprint 2 | Highest |
| POB-06 | View Payment History | POB-E3 | 5 | Sprint 3 | High |
| POB-07 | Scheduled Recurring Payments | POB-E3 | 8 | Sprint 3 | Medium |
| POB-08 | FCA Audit Log | POB-E4 | 8 | Sprint 2 | Highest |
| POB-09 | SCA Compliance | POB-E4 | 8 | Sprint 2 | Highest |

**Total Story Points:** 71

---

# Epic 1: User Authentication & Security

---

## POB-01: OAuth Bank Authentication

**Story Points:** 8  
**Sprint:** Sprint 1  
**Priority:** Highest  
**Epic:** POB-E1 — User Authentication & Security  

### User Story

As a PayFlow client,  
I want to authenticate with my bank using secure OAuth 2.0,  
So that I can connect my account without sharing my banking credentials with PayFlow.

### Acceptance Criteria

```gherkin
Scenario: Client successfully authenticates via OAuth
  Given the client is on the Connect Bank screen in PayFlow
  When they select their bank and click Connect
  Then they are redirected to the bank's official login page
  And PayFlow never sees or stores the client's banking password
  And after successful authentication, they are redirected back to PayFlow
  And a Connected confirmation is displayed
  And an encrypted OAuth token is stored securely server-side

Scenario: Client's OAuth token expires
  Given a client has a connected bank account
  And their OAuth token has expired
  When they attempt to initiate a payment
  Then the system displays a reconnection message
  And they are guided through the reconnection flow
  And their payment history remains available
```

### Technical Notes

- TrueLayer OAuth 2.0 integration
- Token stored encrypted server-side
- No banking passwords stored by PayFlow

---

## POB-02: Two-Factor Authentication on Payments

**Story Points:** 5  
**Sprint:** Sprint 1  
**Priority:** Highest  
**Epic:** POB-E1 — User Authentication & Security  

### User Story

As a PayFlow client,  
I want two-factor authentication required every time I initiate a payment,  
So that my account is protected even if my login is compromised.

### Acceptance Criteria

```gherkin
Scenario: 2FA challenge triggered on payment initiation
  Given the client is logged into PayFlow
  And they have completed the payment initiation form
  When they click Confirm Payment
  Then a 2FA challenge is presented before payment processing
  And supported methods include SMS OTP and authenticator app
  And the payment is not processed until 2FA succeeds

Scenario: Client fails 2FA three times
  Given the client is on the 2FA challenge screen
  When they enter an incorrect OTP three times
  Then the payment attempt is cancelled
  And the account is locked for payment initiation for 30 minutes
  And an alert email is sent to the client
  And the failed attempts are recorded in the audit log
```

---

# Epic 2: Bank Account Connection

---

## POB-03: Connect Bank Account

**Story Points:** 13  
**Sprint:** Sprint 1  
**Priority:** Highest  
**Epic:** POB-E2 — Bank Account Connection  

### User Story

As a PayFlow client,  
I want to connect my UK business bank account to PayFlow,  
So that I can initiate payments directly without manual transfers.

### Acceptance Criteria

```gherkin
Scenario: Client connects their bank account successfully
  Given the client is on the Bank Connections screen
  When they select Barclays Business from the bank list
  And they complete OAuth authentication with their bank
  Then their account shows as Connected with the bank logo
  And the last 4 digits of the account number are displayed
  And the connection timestamp is recorded
  And the process completes in under 90 seconds

Scenario: Client attempts to connect an unsupported bank
  Given the client is on the Bank Connections screen
  When they search for a bank not in the supported list
  Then a message displays that the bank is not yet supported
  And a waitlist email capture form is shown
```

### Technical Notes

- Show supported bank list alphabetically
- Display bank logo from TrueLayer metadata
- Store bank name, account last 4 digits, connection timestamp, and encrypted token reference

---

## POB-04: View Bank Connection Status

**Story Points:** 3  
**Sprint:** Sprint 2  
**Priority:** High  
**Epic:** POB-E2 — Bank Account Connection  

### User Story

As a PayFlow client,  
I want to see the status of all my connected bank accounts,  
So that I know immediately if any connections need attention.

### Acceptance Criteria

```gherkin
Scenario: Client views connection dashboard
  Given the client has two connected bank accounts
  When they navigate to Bank Connections
  Then each bank shows name, account last 4, status, and last used date
  And status options are Active, Expired, and Error
  And expired connections show a Reconnect button
  And the page loads in under 2 seconds

Scenario: Connection shows Error status
  Given a client's bank connection has returned an API error
  When they view the Bank Connections screen
  Then the connection shows Error
  And an error code is displayed with a Get Help link
  And a Retry Connection button is visible
```

---

# Epic 3: Payment Initiation

---

## POB-05: Initiate a Payment

**Story Points:** 13  
**Sprint:** Sprint 2  
**Priority:** Highest  
**Epic:** POB-E3 — Payment Initiation  

### User Story

As a PayFlow client,  
I want to send money from my bank account to my PayFlow wallet,  
So that I can fund my wallet instantly without logging into online banking.

### Acceptance Criteria

```gherkin
Scenario: Client initiates a successful payment
  Given the client has an active bank connection
  And they are on the Make a Payment screen
  When they enter Amount: £5,000, select their bank account, add a reference, and click Continue
  Then a confirmation screen shows the amount, from account, destination, reference, and estimated arrival
  And after 2FA confirmation, the payment is submitted to TrueLayer
  And the payment appears in the PayFlow wallet within 60 seconds
  And a confirmation email is sent within 2 minutes

Scenario: Client enters an amount below minimum
  Given the client is on the Make a Payment screen
  When they enter an amount of £0.50
  Then an inline error displays Minimum payment is £1.00
  And the Continue button remains disabled

Scenario: Client enters an amount above maximum
  Given the client is on the Make a Payment screen
  When they enter an amount of £300,000
  Then an inline error displays Maximum single payment is £250,000
  And the Continue button remains disabled
```

### Technical Notes

- Amount validation: £1.00 to £250,000
- Payment status polling every 5 seconds for up to 2 minutes
- Timeout should show clear manual check instruction

---

## POB-06: View Payment History

**Story Points:** 5  
**Sprint:** Sprint 3  
**Priority:** High  
**Epic:** POB-E3 — Payment Initiation  

### User Story

As a PayFlow client,  
I want to see a history of all my Open Banking payments,  
So that I can reconcile my bank statement against PayFlow transactions.

### Acceptance Criteria

```gherkin
Scenario: Client views payment history
  Given the client has made payments in the last 90 days
  When they navigate to Payment History
  Then a table shows Date, Amount, From Bank, Status, and Reference
  And status options are Completed, Pending, and Failed
  And the list is paginated
  And a date range filter is available
  And an Export to CSV button is visible and functional

Scenario: Client filters payment history by date range
  Given the client is viewing payment history
  When they set the date range to Last 30 days and click Apply
  Then only payments within the last 30 days are shown
  And the total amount for the filtered period is displayed
```

---

## POB-07: Scheduled Recurring Payments

**Story Points:** 8  
**Sprint:** Sprint 3  
**Priority:** Medium  
**Epic:** POB-E3 — Payment Initiation  

### User Story

As a PayFlow client,  
I want to set up recurring payments from my bank account,  
So that my PayFlow wallet is funded automatically each month.

### Acceptance Criteria

```gherkin
Scenario: Client sets up a monthly recurring payment
  Given the client has an active bank connection
  When they create a monthly payment schedule
  Then the schedule is saved and shown in Scheduled Payments
  And a confirmation email is sent
  And a reminder email is sent 24 hours before each payment

Scenario: Client pauses a scheduled payment
  Given the client has an active payment schedule
  When they click Pause
  Then the schedule status changes to Paused
  And no further payments are taken until the client resumes
  And the client receives a confirmation email
```

---

# Epic 4: Compliance & Audit

---

## POB-08: FCA Audit Log

**Story Points:** 8  
**Sprint:** Sprint 2  
**Priority:** Highest  
**Epic:** POB-E4 — Compliance & Audit  

### User Story

As a PayFlow compliance officer,  
I want every payment event logged with full details,  
So that we can demonstrate FCA PSD2 compliance during regulatory audits.

### Acceptance Criteria

```gherkin
Scenario: Payment event is logged in audit trail
  Given a client has initiated a payment
  When the payment is processed successfully or unsuccessfully
  Then an audit log entry is created containing timestamp, event type, client ID, IP address, payment amount, bank used, and outcome
  And the log entry is immutable

Scenario: Compliance officer exports audit trail
  Given the compliance officer is on the Audit Log screen
  When they set a date range and click Export CSV
  Then a CSV file downloads containing all events in the selected range
  And the export completes within 30 seconds for up to 10,000 records
  And the export action is logged in the audit trail
```

---

## POB-09: SCA Compliance

**Story Points:** 8  
**Sprint:** Sprint 2  
**Priority:** Highest  
**Epic:** POB-E4 — Compliance & Audit  

### User Story

As PayFlow,  
We need all payments to meet Strong Customer Authentication requirements,  
So that we maintain regulatory compliance and reduce security risk.

### Acceptance Criteria

```gherkin
Scenario: SCA challenge presented on every payment
  Given any client is initiating any payment
  When they reach the payment confirmation step
  Then an SCA challenge is presented using at least two factors
  And the payment is not processed until both factors are verified

Scenario: Non-SCA-compliant payment attempt is blocked
  Given a client attempts to bypass the SCA step through a direct API call
  When the payment request reaches the server without an SCA token
  Then the payment is rejected with HTTP 403
  And the attempt is logged as a security event
  And an alert is sent to the PayFlow security team
```