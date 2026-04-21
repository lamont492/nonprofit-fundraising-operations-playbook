# Donor Tracking Workflow

## Objective

Create a disciplined donor tracking process that supports relationship management, campaign attribution, stewardship, and reporting consistency.

## Lifecycle Overview

1. Prospect identified
2. Contact qualified
3. Relationship established
4. Solicitation planned
5. Ask made
6. Gift or pledge recorded
7. Acknowledgement completed
8. Stewardship scheduled
9. Donor retained, upgraded, or re-engaged

## Recommended Salesforce NPSP Concepts

### Account
Use Household Accounts for individual donors and Organization Accounts for corporate, foundation, and community partners.

### Contact
Track the individual relationship owner, donor profile, communication preferences, role, and engagement history.

### Opportunity
Use Opportunities to track gifts, grants, pledges, and sponsorship commitments.

### Campaign
Use Campaigns to represent the fundraising initiative, event, appeal, or sponsorship effort tied to donor engagement and revenue attribution.

## Suggested Status Stages

| Stage | Description | Exit Criteria |
|---|---|---|
| Identified | name added to pipeline | basic contact data captured |
| Qualified | prospect fits target segment | owner assigned and rationale documented |
| Cultivating | relationship building in progress | next step scheduled |
| Solicitation Planned | ask strategy agreed | ask amount, timing, and owner defined |
| Ask Made | donor has been solicited | date and outcome captured |
| Committed | donor verbally or formally committed | commitment amount and expected payment date recorded |
| Closed Won | donation or pledge booked | gift posted and campaign linked |
| Closed Lost | opportunity not advancing | disposition reason documented |
| Stewardship | post-gift engagement underway | follow-up plan assigned |

## Campaign Attribution Guidance

- associate each Opportunity to the primary Campaign
- use Campaign Members to track outreach and engagement status
- avoid attributing one gift to multiple primary campaigns unless there is a defined allocation rule
- define in advance how events, appeals, and sponsorships roll up to broader fundraising categories
