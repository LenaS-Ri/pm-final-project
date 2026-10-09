# Unified Card + BNPL Overview in Riverty App, Simplified PRD (Your Riverty case)

**Author:** Me · **Status:** Draft · **Target:** High-Fidelity Prototype · **Persona:** Lena, 32, Cologne A salaried, mobile-first shopper with a middling income and limited financial cushion. She uses BNPL regularly for non-trivial purchases, particularly because she wants to decide what she keeps before money leaves her account. Behaviour: She already has Klarna and PayPal and typically uses whichever payment option is available and easiest at checkout. She knows Riverty but doesn't actively prefer or seek it out.  Goals:   1. Stay in control of when her money leaves her account, especially around returns. 2. Have one clear view of what she owes, when it's due, and what needs her attention. Moment of Misery: When a return or payment doesn't go as planned, payment information becomes fragmented. She may be unsure whether a return has been reflected, what she still owes, or whether she risks missing a due date. Current workaround: She pieces together information across Riverty, Klarna, PayPal, merchant return information, emails and reminders. What she needs from the Riverty Card: Not simply another credit card. She needs broader payment reach while retaining the visibility, flexibility and control she values from BNPL. Core JTBD:   “Help me stay in control of what I owe and when I pay, wherever I shop.”

## 1. The Big Picture
- **Vision:** Give Lena one trustworthy Riverty overview where she can immediately understand purchases made with Riverty and her Riverty Card, without manually reconciling payment information.
- **Press release:** Riverty brings card and checkout purchases together in one clear payment overview. Lena no longer needs to piece together what she bought, how she paid, whether a transaction is complete, or whether a refund has been reflected across disconnected experiences.
The new overview integrates Riverty Card purchases directly alongside existing Riverty purchases, clearly distinguishing “Paid with Riverty” from “Paid with Riverty Card.” Transaction status, merchant, amount and refund information help Lena understand what happened and what requires her attention, especially when something does not go as planned.
- **Success metric:** M6 Active Card Rate: ≥50% of activated cardholders complete at least 2 Riverty Card transactions in Month 6. The overview contributes by making card activity understandable and trustworthy enough to support repeated use.
- **Guardrail:** Partner-Merchant Checkout Conversion: Existing partner-merchant checkout conversion must not decline by more than 1 percentage point versus baseline/control. The card experience must extend Riverty’s consumer relationship without weakening its merchant-first business.

## 2. The Details
### User stories
- Story 1. Understand everything in one place
- As a mobile-first Riverty user managing multiple purchases, I want card and existing Riverty purchases in one overview, so that I can understand my activity without reconstructing it across different places.
- Acceptance criteria
- •	Existing Riverty and Riverty Card purchases appear in the same overview.
- •	Each transaction displays merchant, amount, date and status.
- •	Transactions use a consistent chronological structure.
- •	Card transactions do not require navigating to a separate card area.
- Story 2. Understand how I paid
- As a user who does not think in terms such as “BNPL” or “card rails,” I want each purchase to clearly show how I paid, so that I understand why transactions may behave differently.
- Acceptance criteria
- •	Existing checkout transactions display “Paid with Riverty.”
- •	Card transactions display “Paid with Riverty Card.”
- •	Purchase source is visually distinguishable without dominating merchant and amount.
- •	Repayment method is represented separately from purchase source.
- Story 3. Understand when something changes
- As a user waiting for a refund or transaction to settle, I want its current status to be obvious, so that I know whether I need to act rather than worrying about paying incorrectly.
- Acceptance criteria
- •	Card transactions support Pending, Completed, Refunded and Reversed states.
- •	Status changes are reflected consistently in overview and detail screens.
- •	Refunded/reversed transactions retain the original purchase context.
- •	The UI never claims that a merchant return has completed unless the prototype state explicitly contains that information.
### Screens to build
- Screen 1. Entry Point: Riverty Overview
- Purpose: Show Lena that her existing Riverty and new card activity now live together.
- •	Existing Riverty app header/navigation.
- •	“Purchases” / overview heading.
- •	Upcoming or attention-needed summary.
- •	Unified chronological transaction list.
- •	Merchant name, amount and transaction date.
- •	“Paid with Riverty” / “Paid with Riverty Card” label.
- •	Status indicator: Pending / Completed / Refunded / Reversed.
- •	Visual distinction for items requiring attention.
- •	Tap target into transaction detail.
- Screen 2. Feature Core: Card Transaction Detail
- Purpose: Answer Lena’s basic questions: What happened? How did I pay? What’s its status?
- •	Merchant name, amount and transaction date.
- •	“Paid with Riverty Card” label.
- •	Current transaction status.
- •	Merchant/location information where available.
- •	Transaction timeline/status history.
- •	Refund/reversal information when applicable.
- •	Clear back navigation to unified overview.
- •	Contextual explanatory text for Pending, Refunded and Reversed states.
- •	No new repayment configuration is introduced here.
- Screen 3. Success / Confirmation: Refund Updated
- Purpose: Demonstrate resolution of the Moment of Misery without pretending Riverty controls the merchant’s return process.
- •	Merchant and original transaction.
- •	Original amount.
- •	“Paid with Riverty Card” label.
- •	Clear Refunded status and refund amount.
- •	Status confirmation and updated transaction timeline.
- •	Updated overview/balance representation.
- •	CTA: Back to overview.
- •	Only communicate information present in the transaction state; do not claim a physical return was received or approved unless that information exists.
### Functional requirements
- 1.	Unified rendering: 100% of supplied Riverty and Riverty Card prototype transactions must render within one chronological overview.
- 2.	Purchase-source identification: 100% of transactions must display either “Paid with Riverty” or “Paid with Riverty Card.”
- 3.	Core information: Every card transaction must display merchant, amount, transaction date and current status.
- 4.	Status support: Card transactions must support exactly four prototype states: Pending, Completed, Refunded and Reversed.
- 5.	Status consistency: The same transaction must display the same status on overview, detail and confirmation screens.
- 6.	Refund traceability: A refunded transaction must remain associated with its original merchant, purchase amount and transaction details.
- 7.	Detail access: Every card transaction in the overview must open its corresponding transaction-detail state in one interaction.
- 8.	Chronological integrity: Card and existing Riverty purchases must be ordered using the same transaction-date logic.
### Smart behaviors (Situation → Outcome)
- | Situation | Outcome |
- |---|---|
- | **If** transaction source = existing Riverty checkout | **Then** display **“Paid with Riverty.”** |
- | **If** transaction source = Riverty Card | **Then** display **“Paid with Riverty Card.”** |
- | **If** card transaction = Pending | **Then** show Pending and explain that the final amount/status may still change. |
- | **If** card transaction = Completed | **Then** show Completed without additional warning treatment. |
- | **If** full refund is recorded | **Then** show Refunded and retain original transaction context. |
- | **If** transaction is reversed | **Then** show Reversed rather than presenting it as a completed purchase. |
- | **If** transaction data is incomplete | **Then** show only verified fields. Never generate missing merchant/payment information. |
- | **If** user opens a transaction | **Then** preserve the exact amount, source and status shown in the overview. |
### Technical constraints
- This prototype validates comprehension and interaction, not production architecture.
- - No external APIs.
- - No Mastercard/Paymentology integration.
- - No production Riverty backend integration.
- - No authentication or login flow.
- - Use predefined local mock transaction data.
- - Use React useState only for interactive state.
- - No Redux, Zustand, database or persistent state.
- - No real payments, refunds, credit decisions or card actions.
- - Do not build new identity verification or credit-agreement flows.
- - Do not simulate unsupported backend intelligence.
- - Prototype only the three defined screens.

## 3. The Logistics
### Features out
- Explicitly excluded from this prototype:
- - Flexible Card Repayment configuration.
- - Apple Pay / Google Pay provisioning.
- - Physical card management.
- - Rewards and cashback.
- - Premium card benefits.
- - Card dispute submission.
- - Chargeback case management.
- - Advanced budgeting.
- - Spending insights.
- - New credit decisioning.
- - New identity verification.
- - Redesign of the broader Riverty app.
- - Full transaction-enrichment platform.
- - Automatic merchant-return reconciliation.
- Scope rule: this prototype shows transaction state. It does not create or control that state.
### Edge cases & safety guard
- Pending transaction changes amount
- A Pending transaction may later settle at a different amount.
- Expected: Show the current supplied amount and Pending state. Do not imply that it is final.
- Refund after completed transaction
- A Completed transaction later becomes Refunded.
- Expected: Preserve original transaction context and update the status/refund information consistently across screens.
- Reversed transaction
- A card authorisation disappears or is reversed rather than completing.
- Expected: Display Reversed. Do not classify it as Refunded.
- Unknown merchant
- Card data contains an incomplete or unclear merchant descriptor.
- Expected: Display the available descriptor rather than inventing a consumer-friendly merchant name.
- Missing optional data
- Location or enriched merchant information is unavailable.
- Expected: Omit the field gracefully. Core transaction information remains visible.
- Conflicting prototype state
- Overview says Pending while detail data says Refunded.
- Expected: Treat this as an invalid state and surface a prototype/data error rather than silently selecting one.
- Safety / hallucination guard
- The UI must never infer that a return, refund, payment or merchant action has occurred from contextual clues alone.
- If the data does not confirm the state:
- Status unavailable
- is preferable to a plausible but fabricated explanation.
### Decision log
- Decision 1. One overview, two understandable purchase sources
- Decision: Use “Paid with Riverty” and “Paid with Riverty Card”, not “BNPL” vs “Card.”
- Reason: BNPL describes financing mechanics rather than a purchasing behavior Lena can reliably recognise. It also breaks once card purchases receive flexible repayment.
- Decision 2. Visibility before functionality
- Decision: The prototype shows refunds, reversals and transaction status but does not build repayment, return or dispute workflows.
- Reason: The selected feature solves fragmented understanding. Expanding into transaction management would turn one 3-week feature into several major projects and obscure whether the unified overview itself solves Lena's friction.
### Evals
- 1. Purchase-source comprehension
- Target: ≥95% accuracy
- In prototype testing, users correctly identify whether a transaction was Paid with Riverty or Paid with Riverty Card in ≥95% of tested transactions.
- 2. Moment-of-Misery task
- Target: ≥90% completion within 30 seconds
- Given a scenario involving a card purchase followed by a refund, ≥90% of users can determine:
- - what they originally spent,
- - how they paid,
- - whether the transaction was refunded,
- - whether they currently need to take action,
- within 30 seconds and without assistance.
- 3. Safety / state accuracy
- Target: 100%
- Across all prototype states:
- - no fabricated merchant information,
- - no incorrect refund/return claims,
- - no contradictory transaction statuses across screens.
- Any false financial-status confirmation is a failed evaluation, regardless of overall usability score.

## MoSCoW scope
- **Must:** Unified transaction feed: Card purchases appear alongside existing Riverty purchases.; Clear purchase-source labels: “Paid with Riverty” vs. “Paid with Riverty Card.”; Core transaction details: Merchant, amount, transaction date and current status.; Correct status handling: Card transactions clearly show Pending, Completed, Refunded or Reversed.; Refund/reversal visibility: Changes remain linked to the original card transaction.; Consistent chronological ordering: Card and existing Riverty purchases follow one timeline.; Transaction detail view: Users can open a card transaction and understand its key information.
- **Should:** Transaction filters: Filter by Card/Riverty and transaction status.; Merchant search: Find a specific purchase quickly.; Attention-needed indicators: Highlight transactions requiring user action.; Card balance summary: Show card obligations alongside existing Riverty payments.; Merchant-name enrichment: Replace cryptic card descriptors with understandable merchant names.; Contextual explanations: Explain unfamiliar card statuses such as Pending or Reversed.
- **Could:** Spending categories and monthly summaries.; Merchant logos.; Advanced search and filtering.; Custom transaction tags.; Transaction-history export.; Personalised spending insights.; Merchant location/map information.
- **Won't (now):** Flexible Card Repayment configuration.; Apple Pay / Google Pay setup.; Physical card management.; Rewards or cashback.; Premium card benefits.; Card dispute and chargeback workflows.; Advanced budgeting tools.; New credit decisioning or identity verification.; Major redesign of the existing Riverty app.; Full transaction-enrichment platform rebuild.; Automatic merchant-return reconciliation.

---
**Builder hook:** Build a working prototype based on this PRD. Use the User Story as the core flow, Functional Requirements as build constraints, and prioritize speed and clarity over visual complexity.
