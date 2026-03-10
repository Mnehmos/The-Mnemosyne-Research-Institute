# Security Baseline — The Mnemosyne Research Institute

## Authentication Policy

| Setting | Value |
|---------|-------|
| **2-Step Verification** | Enforced for all users |
| **Minimum Password Length** | 12 characters |
| **Password Complexity** | Letters + numbers + symbols |
| **Password Expiration** | 90 days recommended |
| **Session Duration** | 12 hours (web), 30 days (mobile) |
| **Login Challenges** | Enabled |

## Data Protection

- All Google Drive files default to **organization-only** sharing
- External sharing requires explicit permission
- No file download/copy for external viewers
- Google Vault enabled for data retention and eDiscovery

## Admin Access

- Minimum two super admins for redundancy
- Admin actions logged and reviewed monthly
- Delegated admin roles for non-critical tasks

## Email Security

- SPF, DKIM, DMARC all configured (see DNS records)
- Advanced phishing protection enabled
- Attachment scanning enabled
- Suspicious login alerts enabled

## Device Management

- Basic device management at minimum
- Screen lock required on mobile devices
- Remote wipe capability enabled
- Endpoint verification for sensitive data access
