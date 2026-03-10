# DNS Records — themnemosyneresearchinstitute.com

## Required Records for Google Workspace

### MX Records (Email)

| Priority | Host | Value |
|----------|------|-------|
| 1 | @ | ASPMX.L.GOOGLE.COM |
| 5 | @ | ALT1.ASPMX.L.GOOGLE.COM |
| 5 | @ | ALT2.ASPMX.L.GOOGLE.COM |
| 10 | @ | ALT3.ASPMX.L.GOOGLE.COM |
| 10 | @ | ALT4.ASPMX.L.GOOGLE.COM |

### TXT Records (Security)

| Host | Type | Value | Purpose |
|------|------|-------|---------|
| @ | TXT | `v=spf1 include:_spf.google.com ~all` | SPF — Authorize Google to send email |
| google._domainkey | TXT | *(Generate from Admin Console)* | DKIM — Email signing |
| _dmarc | TXT | `v=DMARC1; p=quarantine; rua=mailto:admin@themnemosyneresearchinstitute.com` | DMARC — Email authentication policy |

### Domain Verification

| Host | Type | Value | Purpose |
|------|------|-------|---------|
| @ | TXT | *(From Google Admin Console)* | Domain ownership verification |

## Notes

- MX records must be set before email will work
- SPF + DKIM + DMARC are all required for reliable email delivery
- DKIM key is generated per-domain in Admin Console > Apps > Google Workspace > Gmail > Authenticate email
- Allow 24-48 hours for DNS propagation
