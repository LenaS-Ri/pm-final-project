# GTM Launch Plan, Riverty business-unit case

| Field | Value |
|---|---|
| Feature | Unified Card + BNPL Overview in Riverty App. Integrates Riverty Card purchases alongside existing Riverty checkout purchases in one chronological overview. |
| Goal | Engagement |
| Launch tier | M, Targeted |

## Goal & Audience
- **Goal:** Engagement, The feature is designed for existing Riverty users adopting the new consumer card. The priority is to make the unified overview discoverable and establish it as their trusted place for checking purchases, payment statuses and refunds. Engagement is the leading behavior that can contribute to repeat card usage and reduced support dependency.
- **Target audience:** Primary: Existing Riverty app users in Germany who have activated the new Riverty Card and also have experience with Riverty checkout purchases. Focus on mobile-first, frequent BNPL users like Lena, who manage multiple purchases and value payment visibility and control.
Secondary: Newly activated Riverty Card customers in Germany who need to understand their card activity within the existing Riverty app.

## Launch Tier
- **M, Targeted**, This is a feature launch for an identifiable group of existing Riverty Card customers, not a new product launch requiring mass-market awareness. The unified overview supports card retention, repeat usage and lower servicing costs but does not directly generate revenue. Without targeted communication, eligible users may overlook the new capability and continue relying on fragmented payment information or customer service. An M-tier launch using existing Riverty channels provides sufficient reach without disproportionate marketing spend.

## Channels
1. **Owned: In-app announcement: Show a contextual announcement to eligible cardholders on their first app visit after card transactions become available. Include a direct CTA to the unified overview and a short first-use explanation. Display once per user, with the option to revisit the guidance.**
2. **Owned: Send an informational feature-update email to eligible existing cardholders through approved CRM channels, subject to applicable communication permissions. Highlight the new overview and provide a direct deep link into the app.**
3. **Owned: Publish an updated Help Centre article and app release notes explaining how card and checkout purchases appear together, what transaction statuses mean and where users can find refund information.**

## Enablement & Assets
Customer-facing: In-app announcement, short walkthrough, targeted email, Help Centre article, updated FAQs, release notes and approved screenshots of the unified overview.
Internal: Customer Service briefing, updated knowledge-base articles, support contact categorisation, analytics tracking specification, feature-flag rollout plan and rollback instructions.
Dependencies: German localisation, final UX copy, Legal/Compliance approval, CRM communication permissions, tested deep links and validated transaction-data accuracy.

## Ownership, Budget & Timeline
- **Ownership & budget:** The Consumer Card PM owns the overall launch, KPI monitoring and go/no-go decision. The Product Designer owns the in-app announcement and walkthrough, while the Engineering Lead is responsible for feature rollout, deep links and analytics tracking. The CRM Lead manages lifecycle emails, and the Content/Communications Lead owns Help Centre updates and release notes. The CS Operations Lead ensures support readiness through training and updated FAQs. Compliance provides mandatory regulatory and privacy approval. Budget: No paid media or external agency spend is planned. All activities use existing Riverty channels and internal resources. The Consumer Card PM must confirm reserved capacity with Engineering, Design, CRM, Content and CS Operations before launch. Any additional localisation, tooling or creative costs require explicit approval.
- **Timeline:** T−2 weeks: Confirm A/B result, select design, assign owners, approve assets and complete compliance review.



T−1 week: Validate transaction data, analytics, deep links, support readiness and rollback procedure.



T0: Enable the selected design for 10% of eligible cardholders. Validate release gates.



T+1 week: Expand to all eligible cardholders after technical and compliance approval. Activate in-app and approved CRM communications.



T+2 weeks: Evaluate 14-day feature discovery for the first fully exposed cohort.



T+5 weeks: Evaluate completed 30-day engagement and support outcomes. Decide whether to optimise or expand.

## Success Metrics
- **Metrics:** 1. Feature Discovery Rate: At least 80% of eligible cardholders open the unified overview within 14 days of launch, measured through app analytics.
2. 30-Day Repeat Overview Usage: At least 50% of eligible cardholders open the overview on two or more distinct days within 30 days, demonstrating recurring engagement.
3. Overview-Related CS Contact Rate: Maximum 100 contacts per 1,000 invoice-equivalent transaction records, indicating that customers can understand purchases and payment information more independently.
- **Bad signal to watch for:** Early warning. Day 7: If fewer than 40% of eligible cardholders have opened the overview within seven days, investigate whether in-app messaging is displayed correctly, deep links work and the audience is correctly targeted. Engagement warning. Day 30:  If discovery reaches 80% but repeat usage remains below 35%, investigate product relevance and usability before increasing communication frequency.   Safety warning. Immediate:  Any confirmed incorrect payment amount, misleading refund status or incorrect due date triggers immediate incident assessment and potential rollout suspension.
- **Likely post-launch decision:** Expand if feature discovery reaches ≥80%, repeat usage reaches ≥50%, CS contacts meet the validated target and partner-merchant checkout conversion remains within the 1pp guardrail. Iterate if discovery is strong but repeat usage falls below 50%, focusing on contextual guidance and overview clarity. Pause if transaction information is inaccurate, unresolved payment complaints materially increase or the merchant-first guardrail is breached.
