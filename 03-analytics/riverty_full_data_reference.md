# Riverty Consumer Card Case: Data Reference

> Consolidated reference for the Product School case work. This document
> strictly separates source-provided case data, simulated research, and
> proposed targets. Simulated data must not be represented as real
> Riverty data.

## Data labels

-   **\[CASE DATA\]** Explicitly provided in the Riverty case study.
-   **\[CASE ASSUMPTION\]** Modelling assumption provided by the case,
    not observed performance.
-   **\[SIMULATED QUAL\]** Fictional qualitative research created for
    the training.
-   **\[SIMULATED QUANT\]** Fictional quantitative data created for the
    training.
-   **\[PROPOSED TARGET\]** Future KPI threshold or experiment criterion
    selected for the project.
-   **\[PROJECT SYNTHESIS\]** Interpretation or framing created during
    the case work.

# 1. Case study data

## Strategic context \[CASE DATA\]

Riverty is one of the larger BNPL providers across DACH, Benelux and the
Nordics. Its growth depends largely on merchant acquisition, while the
consumer relationship is built at and after online checkout.

Three strategic gaps are identified:

1.  **No physical presence.** Riverty is not available at in-store
    points of sale.
2.  **Underserved heavy users.** Loyal and frequent users can only use
    Riverty where partner merchants offer it and are described as the
    most under-monetised.
3.  **Weak brand pull.** Brand preference in e-commerce checkout is
    approximately **6%**.

The challenge is to use a consumer card to build a direct, everyday
consumer relationship, increasing usage and monetisation without
undermining Riverty's merchant-first strategy.

## Persona: Lena \[CASE DATA\]

-   Lena, 32, Cologne.
-   Salaried on a middling income.
-   No real financial cushion.
-   Shops almost entirely on her phone.
-   Uses BNPL on most non-trivial purchases.
-   Says BNPL is not primarily about affordability.
-   Prefers money to leave her account only after deciding to keep an
    item.
-   Has Klarna and PayPal installed.
-   Uses whichever payment option appears at checkout.
-   Knows Riverty but does not prefer it and rarely actively seeks it
    out.
-   What she would value from a Riverty Card is explicitly left open for
    discovery.

## Merchant needs \[CASE DATA\]

Merchants care about:

-   Conversion.
-   Checkout experience.
-   Cost of acceptance.
-   Whether a Riverty Card directs customers towards or away from them.

## Competitive and status-quo evidence \[CASE DATA\]

Relevant alternatives include Klarna Card, PayPal cards and Pay in 3 /
Pay in 30, instalment card banks such as Santander Zero, Advanzia and TF
Bank, Scalapay, FLOA and Alma.

The most common alternative is doing nothing differently: choosing
whatever BNPL option appears at checkout or using an existing debit or
credit card.

## Platform context \[CASE DATA\]

-   Riverty holds principal membership with Mastercard.
-   Paymentology is the issuer processor.
-   A small B2B Amazon Business pilot for Germany and France is the
    first committed programme.
-   Multiple propositions compete for shared engineering, risk, finance
    and operations capacity.
-   Each new proposition requires regulatory approval covering
    proposition, pricing, credit policy and terms.

# 2. Case business-case metrics

These figures are supplied by the case but explicitly described as
modelling assumptions, not observed performance.

  Metric                                     Value Classification
  ----------------------------------- ------------ ------------------------------------
  Existing users converting to card             5% \[CASE ASSUMPTION\]
  Approval rate                                85% \[CASE ASSUMPTION\]
  Activation rate                              70% \[CASE ASSUMPTION\]
  Annual churn                                  5% \[CASE ASSUMPTION\]
  Spend per active user, Year 1          EUR 4,000 \[CASE ASSUMPTION\]
  Spend per active user, Year 3          EUR 7,000 \[CASE ASSUMPTION\]
  Active cards, Year 1                      31,238 \[CASE ASSUMPTION / MODEL OUTPUT\]
  Card volume, Year 1                     EUR 125m \[CASE ASSUMPTION / MODEL OUTPUT\]
  Active cards, Year 5                     164,365 \[CASE ASSUMPTION / MODEL OUTPUT\]
  Card volume, Year 5                   EUR 1.02bn \[CASE ASSUMPTION / MODEL OUTPUT\]

# 3. Simulated qualitative interview dataset

> **\[SIMULATED QUAL\]** These interviews were created for the training
> exercise. They are not actual Riverty UXR.

## INT-01: Frequent BNPL user

**Profile:** Female, 31, Cologne.

-   Shops online 3-4 times/month, mostly fashion.
-   Klarna and PayPal installed.
-   Usually chooses whichever option is easiest at checkout.
-   Uses Pay Later especially when ordering multiple sizes.
-   Has debit and credit cards already.
-   Questions why she needs another card.
-   Did not recognise Riverty immediately, but did after invoice payment
    was mentioned.
-   Usually uses debit in physical stores.
-   Would consider a card if there were no fee.
-   Likes seeing purchases and due dates in one place.
-   Does not want another app generating reminders.

> "I don't want to pay EUR 300 when I know I'm sending half of it back."

## INT-02: Occasional BNPL user

**Profile:** Male, 35, Hamburg.

-   Uses PayPal most often and describes it as "automatic."
-   Does not actively compare providers.
-   Uses BNPL mainly for electronics and larger purchases.
-   Has a Visa credit card.
-   Does not initially see a reason for a Riverty Card.
-   Cashback creates mild interest.
-   Choosing repayment date creates more interest.
-   Asks about SCHUFA and late-payment consequences.
-   Strong concern about accidentally accumulating debt.

> "For EUR 30 I don't care. For EUR 500 I want some flexibility."

## INT-03: Heavy mobile shopper

**Profile:** Female, 28, Berlin.

-   Almost never shops on desktop.
-   Uses Apple Pay for physical purchases.
-   Uses Klarna for online fashion.
-   Manual card entry creates friction.
-   Has used Riverty but cannot clearly describe the brand.
-   Values BNPL because returns can take 1-2 weeks.
-   Has paid an invoice before a refund arrived.
-   Would not want another physical card.
-   Finds virtual card plus mobile wallet appealing.
-   Wants immediate purchase notifications.

> "If I have to enter card details manually, I usually choose something
> else."

> "If it worked everywhere through Apple Pay, maybe."

## INT-04: Frequent Riverty user

**Profile:** Male, 39, Munich.

-   Uses Riverty when available.
-   Likes invoice payments.
-   Frustrated by merchant-dependent availability.
-   Uses existing Mastercard when Riverty is unavailable.
-   Interested in physical-store usage.
-   Wants all Riverty purchases in one app/account.
-   Asks whether existing Riverty history could simplify signup.
-   Does not care much about cashback.
-   Strongly resistant to annual fees.
-   Would try the card if application took under five minutes.

> "Sometimes I want Riverty but the shop only has Klarna."

## INT-05: Moderate BNPL user

**Profile:** Female, 33, Duesseldorf.

-   Uses Klarna, PayPal and bank debit.
-   Has several outstanding BNPL purchases simultaneously.
-   Sometimes forgets which provider a payment belongs to.
-   Once missed a payment because a reminder went to spam.
-   Wants one overview of what is due.
-   Does not want revolving credit.
-   Accepts instalments when deliberately selected.
-   Likes ability to move a payment date.
-   Would value a clear monthly spending limit.
-   Rewards are nice but not important.

> "That's actually the annoying part. Everything is scattered."

> "Instalments are fine if I actively choose them. I don't want debt
> happening automatically."

# 4. Simulated support tickets and bug reports

> **\[SIMULATED QUAL\]** These are fictional training inputs.

## SUP-18421: Return not reflected

> "Returned order 8 days ago but invoice still shows full amount. Do I
> need to pay this now? I don't want a late fee while waiting for the
> merchant."

Signal: Return status and payment obligation are not aligned.

## SUP-18456: Riverty unavailable

Customer normally uses Riverty but cannot select it at a particular
merchant.

Signal: Merchant-dependent availability limits usefulness.

## SUP-18503: Payment overview confusion

Customer cannot easily see all open invoices across several shops or
determine what is due next.

Signal: Fragmented payment visibility creates cognitive load.

## SUP-18544: Payment reminder during return

Customer receives a payment reminder while part of the order has already
been returned.

Signal: Merchant return state and payment state are misaligned.

## BUG-921: Mobile authentication drop-off

-   User leaves merchant checkout to authenticate.
-   Returning reloads checkout and loses payment selection.
-   Device: iPhone.
-   Reproduced in 3/5 simulated attempts.

Signal: Authentication creates checkout abandonment risk.

## BUG-947: Due-date inconsistency

-   App shows 14 October.
-   Email reminder shows 13 October.
-   Customer contacts support to determine the correct date.

Signal: Cross-channel inconsistency undermines trust.

## SUP-18602: Physical-store request

Customer asks whether Riverty can be used in a physical store.

Signal: Potential demand for extending Riverty beyond online partner
checkouts.

## SUP-18671: Consolidated payment request

Customer asks whether all Riverty invoices can be paid together.

Signal: Potential demand for cross-merchant consolidation.

# 5. Synthesised qualitative findings \[SIMULATED QUAL SYNTHESIS\]

## Payment control and transparency

-   Fragmented payment overview.
-   Return/payment mismatch.
-   Due-date inconsistency.
-   Limited repayment control.
-   Cognitive load from multiple invoices and providers.

## Everyday utility and acceptance

-   Merchant-dependent availability.
-   Online-only perception.
-   Mobile-wallet expectation.
-   Cross-merchant fragmentation.

## Proposition and adoption

-   Weak reason to adopt another card.
-   Strong existing payment habits.
-   Weak Riverty brand salience.
-   Annual-fee sensitivity.
-   Generic rewards appear insufficient for switching.

## Credit trust and financial safety

-   Fear of unintended revolving debt.
-   Uncertainty around late-payment consequences.
-   SCHUFA questions.
-   Desire for spending limits and deliberate repayment choices.

## Checkout and technical reliability

-   Mobile authentication drop-off.
-   Cross-system payment-state inconsistency.
-   Return synchronisation delay.
-   Notification and reminder inconsistencies.

# 6. Persona and problem synthesis

## Role \[CASE DATA + PROJECT SYNTHESIS\]

Lena, 32, Cologne, is a salaried mobile-first shopper with limited
financial cushion who regularly uses BNPL for non-trivial purchases and
switches between Klarna, PayPal and Riverty depending on availability.

## Goals \[CASE DATA + SIMULATED QUAL\]

1.  Stay in control of when money leaves her account, particularly while
    deciding what to keep or return.
2.  Have one clear view of what she owes, when it is due, and what
    requires attention.

## Friction / Moment of Misery \[SIMULATED QUAL\]

When a return, refund or payment does not go as planned, Lena cannot
easily tell what she owes or when she needs to pay. With several
purchases outstanding, information is scattered across merchants and
payment providers.

## Current workaround \[INFERRED\]

Lena manually pieces together information across Klarna, PayPal,
Riverty, merchant return information, emails, reminders and app
notifications.

# 7. Problem Hook, strategy and Value Proposition \[PROJECT SYNTHESIS\]

## Problem Hook

> Riverty risks losing relevance beyond existing merchants' checkouts,
> while consumers like Lena lack one flexible payment relationship that
> keeps them in control, especially when things don't go as planned.

## Strategy

> Deliver a payment method combining broad reach across purchases with
> the flexibility, overview and control that Lena needs.

## Value Proposition

> The Riverty Card combines the reach of Mastercard with the flexibility
> of BNPL, giving Lena one place to see what she owes, control when she
> pays, and get support when things don't go as planned.

# 8. Simulated quantitative dataset

> **\[SIMULATED QUANT\]** The case contains no historical Product Health
> dataset. These values were created as illustrative training data.

  -------------------------------------------------------------------------
  Metric            Earlier simulated  Current simulated             Change
                                state              state 
  ---------------- ------------------ ------------------ ------------------
  Users with clear                61%                74%              +13pp
  overview of                                            
  upcoming                                               
  payments                                               

  Payments                       8.2%               5.9%             -2.3pp
  requiring                                              
  support contact                                        

  Return-related                 12.5                8.1             -35.2%
  payment                                                
  enquiries /                                            
  1,000                                                  
  transactions                                           

  Users missing                  4.8%               2.9%             -1.9pp
  payment after                                          
  return initiated                                       

  Payment                       3.6/5              4.1/5               +0.5
  experience CSAT                                        

  Users agreeing                  58%                72%              +14pp
  "I feel in                                             
  control of my                                          
  payments"                                              
  -------------------------------------------------------------------------

## Quantitative baseline used in the hypothesis \[SIMULATED QUANT\]

> **12.5 return-related payment enquiries per 1,000 transactions.**

The other simulated metrics are illustrative Product Health indicators
and were not all incorporated into the final hypothesis.

# 9. Proposed success metrics

> **\[PROPOSED TARGET\]** These are future experiment criteria, not
> observed data.

## Primary success metric: M6 Active Card Rate

> Percentage of activated cardholders completing **at least 2 Riverty
> Card transactions in Month 6**.

**Target: \>=50%.**

## Merchant-first guardrail

> Partner-merchant checkout conversion must not decline by more than **1
> percentage point** versus baseline/control.

The metric is grounded in the case's merchant-first strategy. The 1pp
tolerance is a proposed project threshold.

# 10. Decision window \[PROPOSED TARGET\]

-   **Duration:** 6 months.
-   **Minimum sample:** \>=1,000 activated cardholders.
-   **Interim checkpoints:** Month 1 and Month 3.
-   **Final decision:** Month 6.

### Scale

-   M6 Active Card Rate \>=50%.
-   Merchant checkout conversion decline \<=1pp.

### Pivot

-   Meaningful repeat usage but primary threshold missed.
-   Merchant guardrail remains intact.
-   Research indicates a correctable proposition or experience issue.

### No-go

-   Repeat usage materially below the agreed threshold.
-   And/or merchant checkout conversion deteriorates beyond the
    guardrail.

# 11. Evidence reconciliation

## Qualitative evidence \[SIMULATED QUAL\]

> "Returned order 8 days ago but invoice still shows full amount. Do I
> need to pay this now? I don't want a late fee while waiting for the
> merchant."

Supporting signal:

> "That's actually the annoying part. Everything is scattered."

## Quantitative evidence \[SIMULATED QUANT\]

> **12.5 return-related payment enquiries per 1,000 transactions.**

## Supporting strategic evidence \[CASE DATA\]

-   Approximately **6% Riverty brand preference at e-commerce
    checkout**.
-   Frequent Riverty users remain restricted to merchants where Riverty
    is offered.
-   The status quo is often another BNPL option or an existing
    debit/credit card.

## Strategic outcome \[PROJECT SYNTHESIS\]

Move Lena from opportunistically selecting whichever provider appears at
checkout towards repeatedly choosing Riverty.

Expected logic:

**Greater control and reach -\> repeat usage -\> stronger retention -\>
higher transaction frequency -\> greater card volume -\> higher revenue
potential.**

# 12. Final hypothesis

> **Based on recurring qualitative evidence of fragmented payment
> visibility and return-related uncertainty, supported by a simulated
> baseline of 12.5 return-related payment enquiries per 1,000
> transactions, I believe that giving Lena one broadly accepted payment
> relationship with flexible repayment and a unified payment overview
> will result in increased repeat Riverty usage, as measured by \>=50%
> of activated cardholders completing at least 2 Riverty Card
> transactions in Month 6. I will protect partner-merchant checkout
> conversion, allowing no more than a 1pp decline, and will make a
> go/no-go decision after 6 months with at least 1,000 activated
> cardholders.**

# 13. Provenance summary

  -----------------------------------------------------------------------
  Item                                Classification
  ----------------------------------- -----------------------------------
  Lena's basic persona and BNPL       \[CASE DATA\]
  behaviour                           

  \~6% checkout brand preference      \[CASE DATA\]

  Merchant concerns                   \[CASE DATA\]

  Mastercard / Paymentology platform  \[CASE DATA\]
  context                             

  5% card conversion                  \[CASE ASSUMPTION\]

  85% approval                        \[CASE ASSUMPTION\]

  70% activation                      \[CASE ASSUMPTION\]

  5% annual churn                     \[CASE ASSUMPTION\]

  EUR 4k -\> EUR 7k spend per active  \[CASE ASSUMPTION\]
  user                                

  Year 1 / Year 5 projections         \[CASE ASSUMPTION / MODEL OUTPUT\]

  INT-01 through INT-05               \[SIMULATED QUAL\]

  SUP / BUG dataset                   \[SIMULATED QUAL\]

  12.5 return enquiries / 1,000       \[SIMULATED QUANT\]

  Illustrative Product Health metrics \[SIMULATED QUANT\]

  M6 Active Card Rate \>=50%          \[PROPOSED TARGET\]

  \>=2 transactions in Month 6        \[PROPOSED TARGET\]

  Merchant conversion guardrail       \[PROPOSED TARGET\]
  \<=1pp decline                      

  6-month decision window             \[PROPOSED TARGET\]

  \>=1,000 activated cardholders      \[PROPOSED TARGET\]

  Problem Hook and Value Proposition  \[PROJECT SYNTHESIS\]

  Final hypothesis                    \[PROJECT SYNTHESIS + SIMULATED
                                      EVIDENCE + PROPOSED TARGETS\]
  -----------------------------------------------------------------------

## Source note

The **\[CASE DATA\]** and **\[CASE ASSUMPTION\]** sections are based on
the provided *Riverty Case Study: BU Pay & Credit - Riverty's First
Consumer Card*. All other material is explicitly labelled as simulated,
inferred, synthesised, or proposed for the Product School training
exercise.
