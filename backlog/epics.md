# Product Epics
## PayFlow Open Banking Payments Feature

---

## Epic 1: User Authentication & Security

**Epic ID:** POB-E1  
**Goal:** Secure OAuth 2.0 bank authentication and payment security.

### Business Value

This epic ensures that PayFlow clients can securely authenticate with their banks without sharing banking credentials directly with PayFlow. It supports trust, security, and compliance for the Open Banking payment journey.

### Scope

- OAuth 2.0 bank authentication
- Secure token handling
- Two-factor authentication for payment initiation
- Session expiry and reconnection handling
- No storage of client banking passwords

### Acceptance Criteria

- Clients can authenticate through their bank using OAuth 2.0.
- PayFlow does not store banking passwords.
- OAuth tokens are encrypted and stored securely server-side.
- 2FA is enforced before payment initiation.
- Expired sessions guide users through reconnection clearly.

---

## Epic 2: Bank Account Connection

**Epic ID:** POB-E2  
**Goal:** Connect UK client bank accounts through a regulated Open Banking API.

### Business Value

This epic allows PayFlow clients to connect their business bank accounts directly to the PayFlow platform, reducing manual bank transfer effort and preparing the system for instant wallet funding.

### Scope

- Bank selection screen
- Open Banking API connection
- Supported UK bank list
- Connected account status display
- Re-authentication flow for expired connections

### Acceptance Criteria

- Clients can connect supported UK bank accounts.
- Supported banks are displayed clearly in the PayFlow dashboard.
- Connected accounts show bank name, account last 4 digits, connection status, and last used date.
- Expired or failed connections show a clear reconnect or retry action.
- Account connection completes in under 90 seconds.

---

## Epic 3: Payment Initiation

**Epic ID:** POB-E3  
**Goal:** Allow clients to send payments from their bank account to their PayFlow wallet.

### Business Value

This epic delivers the core commercial value of the project: replacing slow manual wallet funding with fast Open Banking payments. It directly addresses the 2–3 day settlement delay and improves customer satisfaction.

### Scope

- Payment initiation form
- Payment amount validation
- Payment confirmation screen
- Payment submission through TrueLayer
- Payment status polling
- Payment history view
- Scheduled payments, subject to sprint capacity

### Acceptance Criteria

- Clients can initiate payments from £1 to £250,000.
- Payments complete in under 60 seconds.
- Payment status is shown clearly.
- Confirmation email is sent within 2 minutes.
- Payment history is available for reconciliation.
- Invalid payment amounts are blocked before submission.

---

## Epic 4: Compliance & Audit

**Epic ID:** POB-E4  
**Goal:** Meet FCA PSD2, Strong Customer Authentication, and audit logging requirements.

### Business Value

This epic protects PayFlow from regulatory, security, and operational risk. It ensures payment activity is traceable, compliant, and auditable before go-live.

### Scope

- Strong Customer Authentication controls
- Immutable audit logs
- Security event logging
- Audit export for compliance review
- Compliance documentation support

### Acceptance Criteria

- Every payment event is logged with timestamp, user ID, IP address, payment amount, bank used, and outcome.
- Audit logs cannot be edited or deleted by users.
- Compliance officers can export audit logs as CSV.
- SCA is required for all payment initiation attempts.
- Non-compliant payment attempts are blocked and logged.