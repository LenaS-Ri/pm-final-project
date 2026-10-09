# PRD & Prototype Sprint (Module 4)

## Pick & scope with MoSCoW
- **The “Now” feature I’m scoping (name + one-line core description):** I am deliberately picking a "next" feature, as "now" only consists of baseline features that don't answer core moments of misery, so will not be that suitable for this exercise:

Unified Card + BNPL Overview in Riverty App: Integrates card purchases into Riverty's existing purchase overview in the app alongside BNPL transactions.
- **My finalized Must-Haves (after overriding the AI):** Unified transaction feed
Show Riverty Card purchases alongside existing BNPL purchases in the current overview.

Clear payment-type identification
Each item must clearly indicate whether it is a Card or direct checkout transaction. 

Core transaction details
Show merchant, amount, transaction date and current status for every card purchase.

Pending vs. completed status
Make it obvious whether a card transaction is still pending or has been finalised.

Refund / reversal visibility
Show when a card transaction has been refunded or reversed, so Lena does not assume she still owes the original amount.

Chronological consistency
Card and direct checkout purchases must appear in one predictable timeline rather than separate disconnected sections.

Card transaction detail view
Tapping a card purchase must expose enough detail to understand what happened without leaving the Riverty app.
- **What I demoted from Must → Should/Won’t, and why:** Everything that did not fulful the scope principle: Can Lena understand her Card and BNPL purchase activity from one Riverty overview without checking another provider, email, or payment system?

## Generate your Simplified PRD
- **One thing my PRD makes explicit that a vague brief would have missed:** clear vision + metric + persona context. Clear screens to build

## Prompt-to-prototype sprint
- **Where did the prototype reveal a gap in my PRD logic? (what I had to update):** Two status words weren't defined in the document. Riverty purchases (not card) use "Open" and "Paid", since Pending, Completed, Refunded and Reversed only cover card purchases. Let me know if Riverty purchases should use different words.
- **My prototype, as a link or a screenshot (publish or share from your tool; in Lovable that is Share → Share Preview, in Bolt Publish → Web. No share URL? Screenshot the working flow):** Lovable: https://lovable.dev/preview/bNJ2IpIXzwcpTU1PDEl1N0Ssn1LNIyD7

Alternative: from chat GPT: https://github.com/LenaS-Ri/pm-final-project/blob/main/04-roadmap/riverty_unified_overview_prototype_v2.html
