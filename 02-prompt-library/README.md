# 02 — AI Prompt Library

## Flavors of Ceylon

**Business Field:** Food Manufacturing and Hospitality

**Current Development Stage:** Initial Prompt Development

## Section Purpose

This section contains 10 AI prompts designed to support
workflow automation at Flavors of Ceylon, an Australian
food production business specialising in authentic
Sri Lankan cuisine.

The library is organised into four interconnected
business workflows.

---

## Workflow 01 — Planning and Manufacturing

**Business Function:** Operations and Supply Chain

**Trigger:** Weekly sales and production planning cycle.

| ID | Prompt | Version | Status |
|---|---|---|---|
| P01 | [Product Demand Forecasting](P01-product-demand-forecasting.md) | v1.2 | Final Testing in Progress |
| P02 | [Ingredient Inventory and Replenishment](P02-inventory-and-replenishment.md) | v1.0 | Initial Draft |
| P03 | [Supplier Purchase Order Preparation](P03-supplier-purchase-order.md) | v1.0 | Initial Draft |
| P04 | [Food Production and Batch Planning](P04-production-and-batch-planning.md) | v1.0 | Initial Draft |

### Workflow Sequence

    Weekly Sales Information
            |
            v
    P01 — Demand Forecasting
            |
        Human Review
            |
            v
    P02 — Inventory Assessment
            |
        Human Review
            |
            v
    P03 — Supplier Purchase Order
            |
    Approval and Confirmed Supply
            |
            v
    P04 — Production Planning
            |
    Production Manager Approval

---

## Workflow 02 — Food Safety and Product Quality

**Business Function:** Quality Assurance

**Trigger:** Food safety incident or product label review.

| ID | Prompt | Version | Status |
|---|---|---|---|
| P05 | [Food Safety and Quality Incident Reporting](P05-food-safety-incident-reporting.md) | v1.0 | Initial Draft |
| P06 | [Product Label and Allergen Information Review](P06-product-label-and-allergen-review.md) | v1.0 | Initial Draft |

These prompts support documentation and information
verification. All safety-critical decisions require
qualified human review.

---

## Workflow 03 — Customer Experience and Marketing

**Business Function:** Customer Service and Marketing

**Trigger:** Customer enquiry, feedback or promotional activity.

| ID | Prompt | Version | Status |
|---|---|---|---|
| P07 | [Customer Enquiry Response](P07-customer-enquiry-response.md) | v1.0 | Initial Draft |
| P08 | [Customer Complaint and Feedback Analysis](P08-customer-complaint-analysis.md) | v1.0 | Initial Draft |
| P09 | [Digital Marketing Content Generation](P09-digital-marketing-content.md) | v1.0 | Initial Draft |

These prompts support customer communication,
complaint categorisation and marketing content
preparation.

---

## Workflow 04 — Management Reporting

**Business Function:** Business Management

**Trigger:** Weekly business performance review.

| ID | Prompt | Version | Status |
|---|---|---|---|
| P10 | [Weekly Business Performance Reporting](P10-weekly-business-reporting.md) | v1.0 | Initial Draft |

This prompt consolidates verified operational
information to support management decision-making.

---

## Prompting Strategies

The initial prompt library introduces:

- Role-based prompting
- Contextual prompting
- Task-oriented prompting
- Structured-output prompting
- Task decomposition
- Constraint-based prompting
- Classification prompting
- Audience-focused prompting

These strategies will be evaluated and refined
during practical testing.

## Prompt Documentation

Every prompt contains the five compulsory
assessment requirements:

1. Prompt text
2. Intended workflow or task
3. Problem being solved
4. Automation potential
5. Risks and limitations

## Version Development

| Version | Purpose | Status |
|---|---|---|
| v1.0 | Initial prompt development | Created |
| v1.1 | Revision based on testing | Pending |
| v1.2 | Further refinement and evaluation | Pending |

Additional versions may be created when required.

## Development Progress

- [x] Select 10 business prompt topics
- [x] Organise business workflows
- [x] Create initial prompt versions
- [ ] Conduct initial testing
- [ ] Evaluate actual AI outputs
- [ ] Refine prompts
- [ ] Complete final evaluation

## Related Portfolio Sections

- [Business Context](../01-business-context/README.md)
- [Testing Evidence](../03-testing-evidence/README.md)
- [Iteration Logs](../04-iteration-logs/README.md)
- [Evaluation](../05-evaluation/README.md)
- [References](../06-references/README.md)
- [Return to Main Portfolio](../README.md)

---

All prompts are currently initial drafts.
Testing and evaluation results are pending.

The proposed AI workflows require human oversight
and have not been deployed commercially.
