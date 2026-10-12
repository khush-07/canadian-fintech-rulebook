---
id: onboarding-kyc
title: "Onboarding & KYC"
summary: "What you must check, ask and record when a new customer signs up, from ID verification to sanctions screening."
rules: [fintrac-identity-verification, fintrac-pep-hio, fintrac-third-party-determination, fintrac-business-relationship, sanctions-screening, crs-tax-self-certification, biometric-id-privacy, bank-basic-banking-access, casl-consent]
coming_soon: [beneficial-ownership-for-business-accounts, fintrac-suspicious-transaction-reports, pipeda-consent-and-retention, quebec-law-25, fintrac-ministerial-directives]
last_verified: 2026-10-12
---

## In 30 seconds

1. **Verify identity before the account is usable.** Use a FINTRAC-approved method, and allow only the initial deposit until it passes. [fintrac-identity-verification]
2. **Ask the right questions and record the answers:** PEP status, whether anyone else will use the account, what it's for, and tax residency. [fintrac-pep-hio] [fintrac-third-party-determination] [fintrac-business-relationship] [crs-tax-self-certification]
3. **Screen against sanctions and terrorist lists** at sign-up and every time the lists change. [sanctions-screening]
4. **Treat selfies as sensitive data:** express consent, an alternative path, and short retention. [biometric-id-privacy]

## Which rules apply to your business?

| Rule | Bank | Credit union | MSB (payments, remittance, crypto) | Securities dealer |
|---|---|---|---|---|
| FINTRAC ID verification, PEP, third party, monitoring | Yes | Yes | Yes | Yes |
| Sanctions: don't deal, disclose to RCMP/CSIS | Yes | Yes | Yes | Yes |
| Sanctions: continuous check of property you hold | Yes | Yes | Yes, if you open accounts for clients (sanctions regulations, e.g. SEMA Russia s.6(i)) | Yes |
| CRS/FATCA self-certification | Yes | Yes | Usually no. Check if you hold accounts for customers | Yes |
| Bank Act basic banking access | Yes | Federal credit unions only | No | No |
| Biometric privacy | If you use selfies or biometrics | Same | Same | Same |

*Based on PCMLTFA s.5, Criminal Code s.83.11, SEMA Russia Regulations s.6 and Bank Act s.627.17. Open each rule for the exact citations.*

## The onboarding flow, step by step

1. **Before you start:** consent screens for biometrics (if used) and a separate, unticked marketing opt-in. [biometric-id-privacy] [casl-consent]
2. **About you:** name, address, date of birth, occupation, and tax residency (plus SIN if the account earns interest). [crs-tax-self-certification]
3. **Verify identity:** ID scan + live selfie, with credit-file, dual-process or assisted options as fallbacks. [fintrac-identity-verification] [bank-basic-banking-access]
4. **A few questions:** PEP declaration, "Will anyone else use this account?", and "What will you use it for?" [fintrac-pep-hio] [fintrac-third-party-determination] [fintrac-business-relationship]
5. **Screening, behind the scenes:** sanctions and PEP database checks, with potential matches sent to a review queue. [sanctions-screening]
6. **Account opens:** the initial deposit is allowed. Everything else unlocks once verification passes.
7. **Afterwards:** risk-based monitoring, periodic re-screening, and in-app "update your info" refreshes. [fintrac-business-relationship]

## Pre-build checklist

**Identity verification**
- [ ] The ID flow uses a FINTRAC-approved method (photo ID, credit file, dual-process or reliance)
- [ ] Remote photo ID authenticates the document and matches a live selfie to it
- [ ] Only the initial deposit is allowed before verification passes
- [ ] There's a fallback when the first method fails (e.g. newcomers with no credit history)
- [ ] The verification record stores the method, date, document type and number, jurisdiction and expiry
- [ ] Retention is set to 5+ years after the account closes

**Questions and records**
- [ ] PEP / HIO self-declaration plus database screening
- [ ] Foreign PEP case flow: source of funds and wealth, senior approval, 30-day timer
- [ ] "Will anyone else use this account?" with a third-party details form
- [ ] Account purpose and expected activity are captured
- [ ] Tax residency self-certification, with foreign TIN when needed
- [ ] SIN collected only when needed for tax slips, and not used as an ID

**Screening**
- [ ] Sanctions and terrorist list screening before the account is usable
- [ ] Re-screening of all customers when lists update
- [ ] A match review queue that shows the customer a neutral message

**Privacy and access**
- [ ] Biometric consent screen naming the vendor and the retention period
- [ ] A "Verify another way" option
- [ ] Banks: no minimum deposit, accepted-ID list shown, assisted path for people who fail digital checks

## Common mistakes

- Letting customers send money before ID verification completes.
- Hard-rejecting anyone who fails the selfie check, especially newcomers and people with older ID photos.
- Treating a PEP "yes" as an automatic decline.
- Telling a customer they matched a sanctions list.
- Keeping ID images and face templates indefinitely "just in case".
- Using the SIN as a customer number.
