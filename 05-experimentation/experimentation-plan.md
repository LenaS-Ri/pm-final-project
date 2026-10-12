# A/B Experiment Brief, Riverty business-unit case

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | Unified Card + BNPL Overview in Riverty App (testing 2 variants of this feature) |
| Persona | Lena, 32, mobile-first BNPL user who wants control over purchases, returns and payment obligations. |
| Expected outcome | Users can find and understand purchases more easily in one chronological overview, reducing the need to contact customer service. |
| Primary success metric | Longterm: M6 Active Card Rate: ≥50% of activated cardholders complete ≥2 Riverty Card transactions in Month 6. But for this test: Overview-related CS contacts per 1,000 invoice-equivalent transaction records, covering checkout invoices and card purchases. |
| Baseline rate | 120 contacts per 1,000 invoices (simulated, grouped overview) |
| Guardrail metric | Partner-merchant checkout conversion rate. |
| Guardrail boundary | No decline greater than 1 percentage point versus baseline/control. |
| Second guardrail | No increase in unresolved payment complaints or incorrect financial-status information. |
| Minimum Detectable Effect | −20 contacts per 1,000 invoices (−16.7%). |
| Sample size per arm | 4500 invoices |
| Traffic split | 50/50 |
| Test duration | 30 days, or until required sample size is reached. |
| Significance threshold | 95% confidence (two-sided, p < 0.05). |

## Control vs. Variant
- **Control (A):** Riverty Card and existing checkout purchases appear in the same app overview, grouped into two sections: “Paid with Riverty” and “Paid with Riverty Card.”
Each transaction displays merchant, amount, date and status. Users navigate within the relevant group to find and understand their purchases.
- **Variant (B):** Riverty Card and existing checkout purchases appear together in one chronological feed, regardless of payment method.
Each transaction displays merchant, amount, date, status and the label “Paid with Riverty” or “Paid with Riverty Card.”
Users can locate purchases without first identifying how they paid.
- **Held constant (isolation check):** Both variants contain identical transaction data, amounts, dates, statuses, payment-source labels, transaction details and refund information.
Card functionality, repayment options, notifications, navigation and customer support access remain unchanged.
Both designs use consistent transaction row styling, information density and date ordering within their respective layouts.
The only experimental difference is transaction organisation: grouped by payment method versus one chronological feed.

## Hypothesis
> I believe that Unified Card + BNPL Overview in Riverty App (testing 2 variants of this feature) for Lena, 32, mobile-first BNPL user who wants control over purchases, returns and payment obligations. will result in Users can find and understand purchases more easily in one chronological overview, reducing the need to contact customer service., as measured by a −20 contacts per 1,000 invoices (−16.7%). change in Longterm: M6 Active Card Rate: ≥50% of activated cardholders complete ≥2 Riverty Card transactions in Month 6. But for this test: Overview-related CS contacts per 1,000 invoice-equivalent transaction records, covering checkout invoices and card purchases. within 30 days, or until required sample size is reached.. We will protect Partner-merchant checkout conversion rate. throughout the test.

## Shipping criteria
> We will **ship** if Longterm: M6 Active Card Rate: ≥50% of activated cardholders complete ≥2 Riverty Card transactions in Month 6. But for this test: Overview-related CS contacts per 1,000 invoice-equivalent transaction records, covering checkout invoices and card purchases. improves by ≥ −20 contacts per 1,000 invoices (−16.7%). at 95% confidence (two-sided, p < 0.05). and Partner-merchant checkout conversion rate. does not reach No decline greater than 1 percentage point versus baseline/control. after 30 days, or until required sample size is reached..
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 30 days, or until required sample size is reached., no results reviewed before this date.
