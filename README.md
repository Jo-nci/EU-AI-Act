---
workflow: smb-customer-tiering-analysis
risk_tier: minimal, because internal commercial analytics for B2B customer support classification do not constitute high-risk AI applications (such as employment or essential service access) or prohibited practices under the EU AI Act
owner: Sales Manager (Pinterest SMB)
last_audit: 2026-11-18
---

# SMB Customer Tiering & Propensity Analysis

## Risk classification
This workflow falls into the minimal risk tier. It uses internal AI analytics to evaluate corporate product adoption metrics and assign accounts to managed versus unmanaged service tiers. It does not perform prohibited manipulative scoring, nor does it fit high-risk categories under Annex III (such as credit scoring, recruitment, or access to essential private/public services). While it indirectly influences client support levels, B2B sales segmentation does not impair natural persons' fundamental rights under the Act. Consequently, no fundamental rights impact assessment or conformity assessment is legally mandated.

## Five-point hygiene check
bias:         PASS - evaluation targets business performance metrics (catalog integration, API installation, ad format choice) rather than protected individual attributes
privacy:      PASS - sensitive spend metrics and underlying raw datasets remain outside the AI prompt window
consent:      PASS - standard corporate processing of business-to-business customer telemetry for service optimization is covered under valid terms of service
attribution:  PASS - internal analytical models do not output third-party copyrighted material or claim unverified external sourcing
transparency: FAIL - SMB accounts shifted between managed and unmanaged support tiers have no visibility into how automated scoring influenced their service classification

## Remediation (do these in order)
1. Establish a human-in-the-loop validation process where sales managers review and approve AI-generated tiering recommendations before altering customer account designations.
2. Document the prompt templates, data inputs, and scoring parameters used in Gemini within an internal registry to ensure auditable, repeatable classification logic.

## Note
This is general education on the EU AI Act, not legal advice.
