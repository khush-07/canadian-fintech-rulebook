---
id: payments-transfers
title: "Payments & transfers"
summary: "What applies when your product holds money, sends it, or moves it across borders."
rules: [rpaa-registration, rpaa-safeguarding-funds, rpaa-operational-risk-incidents, fintrac-eft-reporting, sanctions-screening, fintrac-business-relationship]
coming_soon: [virtual-currency-transfers, payments-canada-real-time-rail-rules, interac-e-transfer-participant-rules, unauthorized-transaction-liability, fintrac-ministerial-directives]
last_verified: 2026-10-27
---

## In 30 seconds

1. **Holding balances or moving money as a business? You probably need Bank of Canada registration** under the RPAA, unless you're a bank or another excluded institution. [rpaa-registration]
2. **Keep customer money safe and separate:** a trust account or an insured or guaranteed dedicated account, plus a daily ledger. [rpaa-safeguarding-funds]
3. **Plan for outages:** a written risk framework, and notify users and the Bank without delay when an incident hits them. [rpaa-operational-risk-incidents]
4. **Cross-border transfers of $10,000+ get reported to FINTRAC**, and every transfer gets screened against sanctions lists. [fintrac-eft-reporting] [sanctions-screening]

## Which payment functions does your feature perform?

| Feature | RPAA payment function | Likely obligations |
|---|---|---|
| Wallet or stored balance | Maintaining an account, holding funds | RPAA registration, safeguarding, operational risk |
| "Send money" / P2P | Initiating a transfer | RPAA registration, operational risk; FINTRAC if you're an MSB |
| Bill pay from a balance | Holding funds, initiating a transfer | RPAA registration, safeguarding |
| Payment processing for merchants | Authorizing or transmitting instructions, clearing and settlement | RPAA registration, operational risk |
| International remittance | Initiating a transfer | RPAA, FINTRAC MSB duties, EFT reporting, sanctions |
| Card-linked budgeting, read-only | None (no funds held or moved) | Likely outside the RPAA. Check privacy and data rules |

*Payment functions are listed in RPAA s.2. Banks and other institutions listed in RPAA s.9 are excluded from the RPAA.*

## Pre-build checklist

**Registration and scope**
- [ ] Every feature mapped to the RPAA payment functions
- [ ] Written decision on whether you (or a partner) must register with the Bank of Canada
- [ ] Registration in place before the feature launches
- [ ] FINTRAC MSB status checked if you transfer funds or deal in virtual currency

**Customer funds**
- [ ] Funds held in trust, or in a dedicated account with insurance or a guarantee
- [ ] Daily per-user ledger reconciled to the safeguarding account
- [ ] Written safeguarding framework with a named senior officer, reviewed yearly

**Operations and incidents**
- [ ] Written operational risk and incident framework, including third-party vendors
- [ ] Incident notice templates (in-app, email, status page) with the required fields
- [ ] Process to notify the Bank of Canada without delay

**Transfers**
- [ ] Beneficiary name and address required for international transfers
- [ ] 24-hour aggregation and EFT reports filed within 5 business days
- [ ] Policy for incoming transfers with missing information
- [ ] Sanctions screening on payees and counterparties

## Common mistakes

- Assuming "we use a partner bank, so the RPAA doesn't apply". It depends on which functions you perform yourself.
- Mixing customer balances with operating funds.
- Saying customer wallets are "insured" or "protected" when they aren't covered by CDIC.
- Waiting for root-cause analysis before telling customers about an outage.
