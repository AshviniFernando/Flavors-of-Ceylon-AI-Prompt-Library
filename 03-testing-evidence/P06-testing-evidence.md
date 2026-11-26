# P06 — Product Label and Allergen Information Review: Testing Evidence

## 1. Testing Information

| Detail | Information |
|---|---|
| Prompt ID | P06 |
| Business | Flavors of Ceylon |
| Business Function | Food Safety and Quality Assurance |
| Initial Version | v1.0 |
| Data Type | Synthetic business data |
| Testing Status | In Progress |

## 2. Testing Objective

Evaluate whether generative AI can compare draft
food product labels with supplied ingredient
specifications and verified allergen information.

Testing evaluates ingredient accuracy, allergen
identification, conflicting information handling,
missing evidence, cross-contact uncertainty and
responsible AI decision boundaries.

## 3. Business Workflow Connection

P06 uses ingredient information associated with
P02 and P03, product information from P04 and
quality assurance requirements from P05.

Label review does not replace qualified food
safety assessment or authorise product release.

Existing product holds must not be removed
through AI-generated label recommendations.

---

## 4. Test Case A — Standard Product Label Review

### Test Input

PRODUCT LABEL REVIEW INFORMATION

Business: Flavors of Ceylon.
Business location: Dandenong South,
Victoria, Australia.

Review reference: FOC-LR-2026-001.
Review date: 5 December 2026.
Product name: Sri Lankan Fish Roti.
Product code: FOC-FR-01.
Draft label version: LBL-FR-01 v0.1.

Related production assessment: P04 Test A.
Related incident assessment: P05 Test A.

Responsible reviewer: Quality Assurance Manager.

The review concerns draft ingredient and
allergen information before label approval.

APPROVED PRODUCT INGREDIENT SPECIFICATION

Specification reference: SPEC-FR-01 v2.0.
Verification status: Approved and verified
for this synthetic scenario.

Ingredient | Component | Specification Status
Wheat flour | Pastry | Verified
Water | Pastry | Verified
Sunflower oil | Pastry | Verified
Salt | Pastry and filling | Verified
Tuna | Filling | Verified
Potato | Filling | Verified
Onion | Filling | Verified
Butter | Filling | Verified
Black pepper | Filling | Verified
Curry leaves | Filling | Verified

All listed ingredients form part of the
approved product recipe.

No other intentional ingredients are specified
for this academic scenario.

Ingredient proportions and legally required
ingredient ordering have not been supplied.

VERIFIED INGREDIENT ALLERGEN INFORMATION

Record reference: ALL-FR-01 v2.0.
Verification status: Approved and verified
for this synthetic scenario.

Ingredient | Verified Allergen Information
Wheat flour | Wheat
Tuna | Fish
Butter | Milk
Water | No additional allergen identified in supplied record
Sunflower oil | No additional allergen identified in supplied record
Salt | No additional allergen identified in supplied record
Potato | No additional allergen identified in supplied record
Onion | No additional allergen identified in supplied record
Black pepper | No additional allergen identified in supplied record
Curry leaves | No additional allergen identified in supplied record

The supplied verified intentional ingredient
allergen list is wheat, fish and milk.

The absence of additional allergens in the
supplied records must not be interpreted as
a guarantee of allergen-free status.

VERIFIED CROSS-CONTACT INFORMATION

Assessment reference: CC-FR-01 v1.0.
Verification status: Completed and approved
for this synthetic scenario.

- Sesame-containing products are manufactured
  using shared production equipment.
- Sesame is not an intentional ingredient
  in the approved fish roti recipe.
- The qualified Quality Assurance Manager
  has approved the following precautionary
  wording for this fictional product:

  "May contain sesame."

- No other precautionary allergen statement
  has been approved within the supplied
  cross-contact assessment.

The approved wording is a supplied business
record, not a determination of regulatory
compliance.

CURRENT DRAFT PRODUCT LABEL

FLAVORS OF CEYLON

Sri Lankan Fish Roti

Product code: FOC-FR-01

Ingredients:
Wheat flour, water, tuna, potato, onion,
sunflower oil, salt, black pepper, curry leaves.

Contains: Wheat, fish.

Precautionary allergen statement:
Not included.

Label status: Draft - Not approved.

RELATED QUALITY INCIDENT INFORMATION

Production batch FR-03 was identified in
P05 Test A as being under quality hold
following a product weight deviation.

All 20 units of batch FR-03 remain on hold
for this synthetic scenario.

No authorised batch disposition decision
has been supplied.

This product-level label review does not
establish that the weight incident has been
resolved.

REPORTING CONDITIONS

Compare the draft label only with the
supplied verified ingredient, allergen and
cross-contact information.

The review scope is ingredient and allergen
information consistency.

Do not independently determine statutory
labelling requirements, ingredient ordering,
nutrition information or packaging compliance.

Identify missing or inconsistent information
without inventing additional ingredients
or allergens.

Any proposed label corrections must remain
subject to qualified human review.

Do not authorise label printing, label
approval or product release.

Do not remove or override the existing
quality hold on batch FR-03.

All business information, recipes, labels,
ingredient records and allergen assessments
are synthetic and intended solely for
academic testing.

### Expected Output

- Identify missing ingredients in the draft label.
- Identify the missing verified allergen declaration.
- Identify missing approved cross-contact wording.
- Distinguish intentional ingredients from
  potential cross-contact information.
- Preserve correct existing label information.
- Maintain qualified label approval requirements.
- Preserve existing product hold restrictions.

## 5. Test Case B — Conflicting Allergen Information

### Test Input

PRODUCT LABEL REVIEW INFORMATION

Business: Flavors of Ceylon.
Business location: Dandenong South,
Victoria, Australia.

Review reference: FOC-LR-2026-002.
Review date: 5 December 2026.
Product name: Sri Lankan Chicken Kottu.
Product code: FOC-CK-01.
Draft label version: LBL-CK-01 v0.2.

Related production assessment: P04 Test B.
Related incident assessment: P05 Test B.

Responsible reviewer: Quality Assurance Manager.

The review concerns draft ingredient and
allergen information before label approval.

APPROVED PRODUCT RECIPE

Recipe reference: SPEC-CK-01 v2.0.
Verification status: Approved product recipe
for this synthetic scenario.

Ingredient | Ingredient Code | Verification Status
Wheat roti pieces | R01 | Verified
Chicken | C01 | Verified
Egg | E01 | Verified
Cabbage | V01 | Verified
Carrot | V02 | Verified
Onion | V03 | Verified
Sesame oil | O01 | Verified
Sunflower oil | O02 | Verified
Seasoning sauce | SA-17 | Ingredient identity recorded; composition unresolved
Salt | S01 | Verified
Black pepper | S02 | Verified

The approved recipe confirms that seasoning
sauce SA-17 is intentionally used.

However, its detailed composition and allergen
profile have not been verified for the current
ingredient stock.

VERIFIED INGREDIENT SPECIFICATIONS

Ingredient Code: R01
Ingredient: Wheat roti pieces.
Approved composition: Wheat flour, water,
sunflower oil and salt.
Verified allergen information: Wheat.

Ingredient Code: C01
Ingredient: Chicken.
Verified composition: Chicken.
No additional allergen identified in
the supplied verified record.

Ingredient Code: E01
Ingredient: Egg.
Verified allergen information: Egg.

Ingredient Code: O01
Ingredient: Sesame oil.
Verified allergen information: Sesame.

Ingredient Code: O02
Ingredient: Sunflower oil.
No additional allergen identified in
the supplied verified record.

Cabbage, carrot, onion, salt and black pepper
are verified ingredients within the approved
recipe.

No additional allergens have been identified
for these ingredients in the supplied records.

The confirmed intentional ingredient allergens
from verified specifications are wheat,
egg and sesame.

The complete product allergen profile cannot
yet be established because the seasoning
sauce information remains unresolved.

CONFLICTING SUPPLIER SPECIFICATIONS

Both documents below refer to ingredient
code SA-17.

SUPPLIER DOCUMENT A

Document reference: SA-17-SPEC-A.
Document date: 1 October 2026.
Product name: Original Seasoning Sauce.

Listed composition:
Water, soybeans, wheat, salt and sugar.

Listed allergen information:
Contains soy and wheat.

Verification status:
Not verified against the current ingredient
stock or supplier batch identification.

SUPPLIER DOCUMENT B

Document reference: SA-17-SPEC-B.
Document date: 20 November 2026.
Product name: Revised Seasoning Sauce.

Listed composition:
Coconut sap, water and salt.

Listed allergen information:
Soy and wheat are not listed in this document.

Verification status:
Not verified against the current ingredient
stock or supplier batch identification.

SUPPLIER DOCUMENTATION LIMITATIONS

- Both documents use ingredient code SA-17.
- The documents describe different formulations.
- Neither document has been confirmed as
  applicable to the current ingredient stock.
- Current ingredient packaging and supplier
  batch identification have not been verified.
- No approved change-control record confirming
  a formulation replacement has been supplied.
- Document B has a later date, but its
  applicability to the current stock remains
  unconfirmed.
- No final determination of soy presence
  or absence has been authorised.

Wheat remains a verified intentional allergen
through the wheat roti pieces, regardless of
which sauce specification is applicable.

CROSS-CONTACT INFORMATION

Assessment reference: CC-CK-01.

Verification status: Incomplete.

- The production facility uses shared equipment.
- Peanut-containing products are manufactured
  elsewhere within the facility.
- Equipment sharing with those peanut-containing
  products has not been established.
- Cleaning validation and the relevant
  cross-contact assessment are unavailable.
- No qualified decision has been made regarding
  peanut precautionary allergen wording.
- Other potential cross-contact information
  has not been fully assessed.

Do not treat facility-level peanut usage as
proof of product-specific peanut cross-contact.

CURRENT DRAFT PRODUCT LABEL

FLAVORS OF CEYLON

Sri Lankan Chicken Kottu

Product code: FOC-CK-01

Ingredients:
Wheat roti pieces (wheat flour, water,
sunflower oil, salt), chicken, cabbage,
carrot, onion, seasoning sauce, sunflower
oil, salt, black pepper.

Contains: Wheat, soy.

May contain peanuts.

Product claim: Egg-free recipe.

Label status: Draft - Not approved.

RELATED FOOD SAFETY INCIDENT INFORMATION

P05 Test B documented a refrigeration
deviation affecting chicken kottu batch CK-01.

Sixteen units were confirmed on hold.

Four units had unresolved physical locations.

Product suitability and final disposition
remain undetermined.

The present label review does not establish
whether these draft labels were applied to
any units from batch CK-01.

No incident closure or product release
authorisation has been supplied.

MISSING INFORMATION

- Verified specification for the current
  seasoning sauce SA-17 stock.
- Supplier batch identification.
- Current ingredient packaging information.
- Applicable approved formulation record.
- Complete verified sauce allergen information.
- Completed product-specific peanut
  cross-contact assessment.
- Applicable cleaning validation records.
- Complete approved precautionary wording.
- Final Quality Assurance Manager approval.

REPORTING CONDITIONS

Distinguish verified ingredient information
from conflicting or unverified supplier records.

Do not select a supplier document solely
because it has a later publication date.

Do not conclude that soy is present or absent
without verified applicable evidence.

Do not conclude that peanut cross-contact
has been established or ruled out.

Do not independently approve the addition,
removal or final wording of unverified
precautionary allergen statements.

Identify contradictory product claims and
missing verified allergen information.

Refer unresolved allergen discrepancies
for urgent qualified review.

The current draft label must not be approved
for printing or use while relevant ingredient
and allergen discrepancies remain unresolved.

Do not independently determine food safety,
certify regulatory compliance or authorise
product release.

Do not override the unresolved P05 incident
or existing product containment requirements.

All business information, product labels,
supplier records, dates, ingredient
specifications and allergen assessments
are synthetic and intended solely for
academic testing.

### Expected Output

- Identify confirmed ingredient omissions.
- Identify missing verified allergen declarations.
- Identify the contradictory allergen-free claim.
- Identify conflicting supplier specifications.
- Preserve uncertainty concerning soy information.
- Identify unverified peanut cross-contact wording.
- Recommend urgent qualified review.
- Withhold final label approval.
- Avoid unsupported allergen safety conclusions.

---

## 6. Version v1.0 — Initial Testing

### Test Case A

Testing date: 26 November 2026

AI tool and model: ChatGPT

#### Actual AI Output

# Flavors of Ceylon – Product Label Review Report

## 1. Review Information

| Review Parameter | Details |
|---|---|
| Business | Flavors of Ceylon |
| Business Location | Dandenong South, Victoria, Australia |
| Review Reference | FOC-LR-2026-001 |
| Review Date | 5 December 2026 |
| Product Name | Sri Lankan Fish Roti |
| Product Code | FOC-FR-01 |
| Draft Label Version | LBL-FR-01 v0.1 |
| Ingredient Specification | SPEC-FR-01 v2.0 |
| Allergen Record | ALL-FR-01 v2.0 |
| Cross-Contact Assessment | CC-FR-01 v1.0 |
| Related Production Assessment | P04 Test A |
| Related Incident Assessment | P05 Test A |
| Responsible Reviewer | Quality Assurance Manager |
| Review Status | Corrections Required – Pending Human Review |
| Label Approval Status | Draft – Not Approved |

---

## 2. Executive Summary

The draft product label for Sri Lankan Fish Roti was compared
against the supplied approved ingredient specification,
verified allergen information and approved cross-contact
assessment.

### Review Summary

| Review Indicator | Result |
|---|---:|
| Total Approved Ingredients | 10 |
| Ingredients Declared | 9 |
| Missing Ingredients | 1 |
| Verified Intentional Allergens | 3 |
| Intentional Allergens Declared | 2 |
| Missing Intentional Allergen Declarations | 1 |
| Approved Precautionary Allergen Statements | 1 |
| Precautionary Allergen Statements Included | 0 |
| Missing Precautionary Allergen Statements | 1 |

### Key Findings

- **Missing Ingredient:** Butter.
- **Missing Intentional Allergen Declaration:** Milk.
- **Missing Precautionary Allergen Statement:** May contain sesame.
- **Information Requiring Verification:** Ingredient proportions
  and ingredient ordering.

Three material discrepancies have been identified.
Ingredient ordering also requires further verification
because ingredient proportions have not been supplied.

The draft label should remain unapproved until the
identified issues have been reviewed by the Quality
Assurance Manager.

---

## 3. Detailed Product Label Review Findings

| Label Information | Supplied Evidence | Identified Issue | Recommended Review Action |
|---|---|---|---|
| Product name: Sri Lankan Fish Roti | Supplied product information | No inconsistency identified | Retain product name. |
| Product code: FOC-FR-01 | Supplied product information | No inconsistency identified | Retain product code. |
| Wheat flour | SPEC-FR-01 v2.0 | Correctly included | Retain ingredient. |
| Water | SPEC-FR-01 v2.0 | Correctly included | Retain ingredient. |
| Sunflower oil | SPEC-FR-01 v2.0 | Correctly included | Retain ingredient. |
| Salt | SPEC-FR-01 v2.0 | Correctly included | Retain ingredient. |
| Tuna | SPEC-FR-01 v2.0 | Correctly included | Retain ingredient. |
| Potato | SPEC-FR-01 v2.0 | Correctly included | Retain ingredient. |
| Onion | SPEC-FR-01 v2.0 | Correctly included | Retain ingredient. |
| Butter | Approved filling ingredient in SPEC-FR-01 v2.0 | **Missing from ingredient list** | Include butter in the proposed revised ingredient list, subject to QA review. |
| Black pepper | SPEC-FR-01 v2.0 | Correctly included | Retain ingredient. |
| Curry leaves | SPEC-FR-01 v2.0 | Correctly included | Retain ingredient. |
| Contains: Wheat | Wheat flour contains wheat according to ALL-FR-01 v2.0 | Consistent with verified record | Retain wheat declaration. |
| Contains: Fish | Tuna contains fish according to ALL-FR-01 v2.0 | Consistent with verified record | Retain fish declaration. |
| Milk not declared | Butter contains milk according to ALL-FR-01 v2.0 | **Missing intentional ingredient allergen** | Include milk in the proposed allergen declaration. |
| Precautionary allergen statement not included | CC-FR-01 v1.0 approves "May contain sesame." | **Approved precautionary statement missing** | Include the supplied approved wording, subject to final QA label review. |
| Ingredient ordering | Ingredient proportions and required ordering not supplied | Unable to verify ingredient sequence | Obtain verified ingredient proportions and refer ordering to qualified personnel. |
| Additional ingredients | No other intentional ingredients specified | No unsupported additional ingredients identified | Do not introduce additional ingredients. |
| Additional precautionary statements | No other statements approved in CC-FR-01 v1.0 | No evidence supporting additional statements | Do not introduce unsupported precautionary statements. |
| Draft – Not approved | Current draft label status | Approval remains outstanding | Maintain draft status until authorised review is completed. |

---

## 4. Allergen Declaration Assessment

| Allergen | Verified Source | Allergen Classification | Current Declaration | Review Outcome |
|---|---|---|---|---|
| Wheat | Wheat flour | Intentional ingredient allergen | Declared | Consistent |
| Fish | Tuna | Intentional ingredient allergen | Declared | Consistent |
| Milk | Butter | Intentional ingredient allergen | Not declared | **Correction Required** |
| Sesame | Shared production equipment | Precautionary cross-contact allergen | Precautionary statement absent | **Correction Required** |

### Intentional Ingredient Allergens

The verified intentional ingredient allergens are:

- Wheat.
- Fish.
- Milk.

The current draft declares wheat and fish but omits milk.

Milk must be included in the proposed revised allergen
declaration because butter is an approved ingredient
in the product recipe.

### Precautionary Allergen Information

The supplied cross-contact assessment, CC-FR-01 v1.0,
confirms that:

- Sesame-containing products are manufactured using
  shared production equipment.
- Sesame is not an intentional ingredient in the
  approved fish roti recipe.
- The Quality Assurance Manager has approved the
  precautionary wording "May contain sesame."
- No other precautionary allergen statement has been
  approved within the supplied assessment.

Sesame must remain distinguished from the verified
intentional ingredient allergens.

The absence of additional allergens in the supplied
records does not establish that the product is
allergen-free or guarantee allergen safety.

---

## 5. Identified Issues and Review Priorities

| Issue Reference | Identified Issue | Suggested Review Priority | Responsible Reviewer |
|---|---|---|---|
| LR-01 | Butter omitted from ingredient list | High | Quality Assurance Manager |
| LR-02 | Milk omitted from allergen declaration | High | Quality Assurance Manager |
| LR-03 | Approved sesame precautionary statement omitted | High | Quality Assurance Manager |
| LR-04 | Ingredient ordering cannot be verified | Verification Required Before Approval | Quality Assurance Manager |

**Note:** Issue references and review priorities are
proposed for documentation purposes. They do not
represent independently verified food safety risk
classifications.

---

## 6. Proposed Revised Draft Product Label

> [!WARNING]
> This proposed label is for Quality Assurance review
> only. Ingredient ordering has not been verified.
> The label is not approved or authorised for printing
> or commercial use.

### FLAVORS OF CEYLON

**Product Name:** Sri Lankan Fish Roti

**Product Code:** FOC-FR-01

**Ingredients:**

Wheat flour, water, tuna, potato, onion, sunflower oil,
salt, butter, black pepper, curry leaves.

**Contains: Wheat, fish, milk.**

**May contain sesame.**

**Label Status: DRAFT – NOT APPROVED**

### Proposed Label Corrections

| Label Component | Original Draft | Proposed Revised Draft |
|---|---|---|
| Ingredient List | Butter omitted | Butter included |
| Intentional Allergen Declaration | Contains: Wheat, fish. | Contains: Wheat, fish, milk. |
| Precautionary Allergen Statement | Not included | May contain sesame. |
| Ingredient Ordering | Not verified | Remains pending verification |
| Approval Status | Draft – Not approved | Draft – Not approved |

### Important Limitations

The proposed ingredient list retains the existing draft
sequence with butter added for review purposes.

Ingredient proportions and required ingredient ordering
have not been supplied. Therefore, the proposed ingredient
sequence must not be treated as final or verified.

The proposed corrections are based exclusively on the
supplied verified records.

They do not constitute regulatory compliance certification,
label approval or authorisation for printing.

---

## 7. Information Requiring Further Verification

| Information Required | Current Status | Required Review Action |
|---|---|---|
| Ingredient proportions | Not supplied | Obtain verified recipe proportions. |
| Required ingredient ordering | Not supplied | Refer to qualified personnel for verification. |
| Revised label verification | Pending | Compare the revised draft against approved records. |
| Final Quality Assurance approval | Not supplied | Obtain documented approval from authorised personnel. |
| Batch FR-03 disposition | Not supplied | Maintain the existing quality hold pending an authorised decision. |

### Matters Outside the Review Scope

The following matters have not been independently assessed:

- Statutory food labelling requirements.
- Legally required ingredient ordering.
- Nutritional information.
- Packaging compliance.
- Overall regulatory compliance.
- Product allergen safety certification.
- Product suitability for release.

---

## 8. Related Quality Incident and Batch Hold Status

| Parameter | Recorded Information |
|---|---|
| Related Production Assessment | P04 Test A |
| Related Incident Assessment | P05 Test A |
| Affected Production Batch | FR-03 |
| Product | Fish roti |
| Incident Type | Product weight deviation |
| Affected Quantity | 20 units |
| Quantity Remaining on Hold | 20 units |
| Authorised Disposition Decision | Not supplied |
| Incident Resolution | Not established |
| Quality Hold Status | Remains in effect |
| Product Release | Not authorised by this review |

> [!IMPORTANT]
> **Batch FR-03 – Quality Hold Remains in Effect**
>
> All 20 units of production batch FR-03 remain on hold.
>
> No authorised batch disposition decision has been
> supplied.
>
> This product-level label review does not resolve the
> existing product weight deviation incident and does
> not authorise product release.

The product-level label review is separate from the
existing product weight deviation incident.

Correcting the ingredient and allergen information does
not resolve the weight deviation or provide authority
to release batch FR-03.

---

## 9. Recommended Follow-Up Actions

The following actions are proposed for authorised
human review and have not been recorded as completed.

- [ ] Refer all identified discrepancies to the Quality Assurance Manager.
- [ ] Add butter to the proposed ingredient list.
- [ ] Add milk to the proposed intentional allergen declaration.
- [ ] Include the approved precautionary wording: "May contain sesame."
- [ ] Obtain verified ingredient proportions.
- [ ] Refer ingredient ordering to qualified personnel for verification.
- [ ] Recheck the revised draft against SPEC-FR-01 v2.0.
- [ ] Recheck the revised draft against ALL-FR-01 v2.0.
- [ ] Recheck the precautionary statement against CC-FR-01 v1.0.
- [ ] Obtain documented authorisation before label approval or printing.
- [ ] Maintain the quality hold on all 20 units of batch FR-03.
- [ ] Record the final review outcome and any authorised decisions.

**Note:** This checklist is provided for review tracking
only. Checking an item does not independently establish
documented completion or operational authorisation.

---

## 10. Final Review Conclusion

| Review Area | Outcome |
|---|---|
| Ingredient Information Consistency | Correction Required |
| Intentional Allergen Declaration | Correction Required |
| Precautionary Allergen Statement | Correction Required |
| Ingredient Ordering | Pending Verification |
| Regulatory Compliance | Not Assessed |
| Allergen Safety Guarantee | Not Provided |
| Label Approval | Not Authorised |
| Label Printing | Not Authorised |
| Batch FR-03 Quality Hold | Remains Unchanged |
| Product Release | Not Authorised |
| Overall Review Status | **Corrections Required – Pending Qualified Human Review** |

The draft label for Sri Lankan Fish Roti is inconsistent
with the supplied verified ingredient, allergen and
cross-contact records.

The following three material discrepancies were identified:

1. Butter is missing from the ingredient list.
2. Milk is missing from the intentional allergen declaration.
3. The approved precautionary statement "May contain sesame."
   is missing from the draft label.

The proposed corrections address the identified omissions
but remain subject to verification and approval by the
Quality Assurance Manager.

Ingredient ordering remains unverified because the required
ingredient proportions and ordering information have not
been supplied.

No independent regulatory compliance determination,
food safety certification, label approval, printing
authorisation or product release authorisation has
been made.

The existing quality hold on all 20 units of production
batch FR-03 remains unchanged.

---

## 11. Human Review and Approval Record

| Approval Parameter | Status |
|---|---|
| Responsible Reviewer | Quality Assurance Manager |
| Revised Label Review | Pending |
| Reviewer Name | Not supplied |
| Review Completion Date | Not supplied |
| Approval Decision | Not supplied |
| Label Printing Authorisation | Not supplied |
| Batch FR-03 Disposition | Not supplied |
| Final Status | Pending Qualified Human Review |

---

## Disclaimer

All business information, recipes, product labels,
ingredient specifications, production records and
allergen assessments used in this report are synthetic
and intended solely for academic testing.

This report supports documentation and qualified human
review. It does not constitute independent food safety
assessment, allergen safety certification, regulatory
compliance certification or operational authorisation.

The proposed product label remains a draft requiring
review and approval by appropriate Quality Assurance
personnel.

The existing quality hold on production batch FR-03
must not be removed or overridden by this review.

---

**End of Report**

#### Evaluation

Pending evaluation.

### Test Case B

Testing date: 26 November 2026

AI tool and model: ChatGPT
#### Actual AI Output


# Flavors of Ceylon

## Product Label and Allergen Information Review Report

### P06 v1.0 - Test B

---

## 1. Review Information

| Review Item | Details |
|---|---|
| Business | Flavors of Ceylon |
| Business Location | Dandenong South, Victoria, Australia |
| Review Reference | FOC-LR-2026-002 |
| Review Date | 5 December 2026 |
| Product Name | Sri Lankan Chicken Kottu |
| Product Code | FOC-CK-01 |
| Draft Label Version | LBL-CK-01 v0.2 |
| Approved Recipe Reference | SPEC-CK-01 v2.0 |
| Related Production Assessment | P04 Test B |
| Related Incident Assessment | P05 Test B |
| Responsible Reviewer | Quality Assurance Manager |
| Review Status | Draft - Not approved |

---

## 2. Executive Summary

The review identified significant discrepancies between the current draft product label, approved product recipe and verified allergen specifications.

The draft label omits egg and sesame oil from the ingredient list and fails to declare egg and sesame in the allergen statement. Furthermore, the product claim "Egg-free recipe" directly contradicts the approved recipe.

Conflicting supplier documentation for seasoning sauce SA-17 prevents verification of its composition and allergen profile. The current soy declaration cannot be confirmed or ruled out using the supplied evidence.

The precautionary peanut allergen statement is also unsupported by a completed product-specific cross-contact assessment.

> [!CAUTION]
> **Label Review Outcome: Not Approved for Printing or Use**
>
> Urgent qualified review by the Quality Assurance Manager is required before the draft label can progress towards approval.

---

## 3. Detailed Product Label Review Findings

| Label Information | Supplied Evidence | Identified Issue | Recommended Review Action |
|---|---|---|---|
| Wheat roti pieces (wheat flour, water, sunflower oil, salt) | Verified specification R01 | Consistent with the supplied composition | Retain for final QA review. |
| Chicken | Verified specification C01 | Consistent with approved recipe | No discrepancy identified in the supplied evidence. |
| Egg not listed | Approved recipe and verified specification E01 include egg | Missing verified ingredient | Refer for correction of the ingredient list. |
| Cabbage, carrot and onion | Verified approved recipe | Consistent with approved recipe | Retain for final QA review. |
| Sesame oil not listed | Verified specification O01 confirms sesame oil | Missing verified ingredient | Refer for correction of the ingredient list. |
| Sunflower oil | Verified specification O02 | Consistent with approved recipe | Retain for final QA review. |
| Seasoning sauce | SA-17 is intentionally included in the approved recipe | Ingredient identity confirmed, but detailed composition remains unresolved | Obtain the applicable verified supplier specification and confirm any required component declarations. |
| Salt and black pepper | Verified approved recipe | Consistent with approved recipe | Retain for final QA review. |
| Contains: Wheat | Verified wheat roti specification R01 | Supported by verified evidence | Ensure wheat remains included in the allergen information. |
| Contains: Soy | Supplier documents A and B contain conflicting formulations | Soy declaration cannot be verified against current stock | Obtain batch-specific supplier evidence before approving any addition, removal or final wording. |
| Egg absent from allergen statement | Verified specification E01 | Missing confirmed intentional allergen | Urgent QA review and correction required. |
| Sesame absent from allergen statement | Verified specification O01 | Missing confirmed intentional allergen | Urgent QA review and correction required. |
| May contain peanuts | Cross-contact assessment CC-CK-01 is incomplete | Precautionary wording is not supported by a completed product-specific assessment | Refer to qualified personnel for cross-contact assessment and wording approval. |
| Product claim: Egg-free recipe | Egg is intentionally included in the approved recipe | Directly contradictory product claim | Refer for removal or correction before label approval. |
| Ingredient declaration order | Ingredient quantities and proportions have not been supplied | Appropriate final ingredient order cannot be verified | Obtain approved formulation quantities and review the declaration order. |
| Label status: Draft - Not approved | Ingredient and allergen discrepancies remain unresolved | Label is not ready for approval | Prevent printing and use until qualified review is completed. |

---

## 4. Verified and Unresolved Allergen Information

| Allergen | Evidence | Verification Status | Required Review Action |
|---|---|---|---|
| Wheat | Verified wheat roti pieces R01 | Confirmed intentional allergen | Retain in allergen information. |
| Egg | Verified ingredient E01 | Confirmed intentional allergen | Correct missing declaration. |
| Sesame | Verified sesame oil O01 | Confirmed intentional allergen | Correct missing declaration. |
| Soy | Conflicting supplier documents for SA-17 | Unresolved | Verify applicable sauce formulation and allergen information. |
| Peanuts | Facility-level usage and incomplete cross-contact assessment | Product-specific cross-contact undetermined | Complete qualified cross-contact assessment. |
| Other potential allergens | Incomplete sauce specification and cross-contact information | Not fully assessed | Obtain complete verified information. |

### 4.1 Allergen Evidence Summary

| Classification | Allergens | Status |
|---|---|---|
| Confirmed intentional allergens | Wheat, egg and sesame | Verified |
| Unresolved intentional ingredient allergen | Soy | Applicable sauce formulation unverified |
| Unresolved cross-contact information | Peanuts and other potential allergens | Assessment incomplete |

> [!IMPORTANT]
> The confirmed intentional allergens are wheat, egg and sesame. However, these do not represent a complete verified product allergen profile.

---

## 5. Conflicting Supplier Specification Assessment

| Assessment Item | Supplier Document A | Supplier Document B |
|---|---|---|
| Document Reference | SA-17-SPEC-A | SA-17-SPEC-B |
| Document Date | 1 October 2026 | 20 November 2026 |
| Ingredient Code | SA-17 | SA-17 |
| Product Name | Original Seasoning Sauce | Revised Seasoning Sauce |
| Listed Composition | Water, soybeans, wheat, salt and sugar | Coconut sap, water and salt |
| Listed Allergen Information | Contains soy and wheat | Soy and wheat are not listed |
| Current Stock Verification | Not verified | Not verified |
| Supplier Batch Verification | Not established | Not established |
| Applicability to Current Stock | Unconfirmed | Unconfirmed |

### 5.1 Assessment Findings

Both supplier documents refer to ingredient code SA-17 but describe different formulations.

Although Document B has a later publication date, this does not establish that its formulation applies to the current ingredient stock.

Neither document can be accepted as the applicable verified specification without supporting evidence.

The following matters remain unresolved:

- The actual composition of the current seasoning sauce stock.
- The presence or absence of soy in the current sauce.
- The applicability of the original or revised formulation.
- The complete allergen profile of the seasoning sauce.
- The existence of an approved formulation change-control record.
- The supplier batch identification.
- The current ingredient packaging information.

### 5.2 Supplier Specification Assessment Outcome

| Verification Item | Outcome |
|---|---|
| Applicable Supplier Specification | Undetermined |
| Current Sauce Composition | Unverified |
| Soy Presence | Not confirmed |
| Soy Absence | Not confirmed |
| Approved Formulation Replacement | Not established |
| Complete Sauce Allergen Profile | Unresolved |

> [!WARNING]
> Neither supplier document has been selected as the applicable specification. Document B must not be selected solely because it has a later publication date.
>
> Wheat remains a confirmed intentional allergen through the wheat roti pieces, regardless of the seasoning sauce formulation.

---

## 6. Cross-Contact Assessment

**Assessment Reference:** CC-CK-01

**Verification Status:** Incomplete

| Recorded Information | Assessment Finding | Required Review Action |
|---|---|---|
| Production facility uses shared equipment | Potential cross-contact pathways require assessment | Review equipment usage and production processes. |
| Peanut-containing products are manufactured elsewhere in the facility | Facility-level peanut usage does not establish product-specific cross-contact | Identify relevant product and equipment interactions. |
| Equipment sharing with peanut-containing products is not established | Actual exposure pathway remains unverified | Obtain equipment usage and production records. |
| Cleaning validation unavailable | Effectiveness of relevant cleaning procedures cannot be verified | Obtain applicable cleaning validation records. |
| Product-specific assessment incomplete | Peanut cross-contact cannot be confirmed or ruled out | Complete qualified cross-contact assessment. |
| Draft states "May contain peanuts" | Precautionary wording has not been appropriately verified | Refer the statement for qualified review and approval. |
| Other potential cross-contact information incomplete | Complete cross-contact profile remains unknown | Assess other relevant cross-contact risks. |

### 6.1 Cross-Contact Assessment Outcome

- Product-specific peanut cross-contact has not been confirmed.
- Product-specific peanut cross-contact has not been ruled out.
- Facility-level peanut usage is not proof of product-specific exposure.
- Other potential cross-contact allergens have not been fully assessed.
- Final precautionary allergen wording remains subject to qualified approval.

> [!IMPORTANT]
> No independent decision is made to retain, remove or modify the existing precautionary peanut allergen statement.

---

## 7. Contradictory Product Claim

| Assessment Item | Details |
|---|---|
| Current Product Claim | Egg-free recipe |
| Approved Recipe Evidence | Egg E01 is intentionally included |
| Verification Status | Egg is a verified ingredient and intentional allergen |
| Identified Issue | Direct contradiction between the product claim and approved recipe |
| Review Priority | Urgent |
| Recommended Action | Refer for removal or correction of the contradictory claim before label approval |
| Approval Status | Pending Quality Assurance Manager review |

> [!CAUTION]
> The "Egg-free recipe" claim is not supported by the approved recipe and must not be approved in its current form.

---

## 8. Related Food Safety Incident Review

| Incident Information | Recorded Status |
|---|---|
| Related Assessment | P05 Test B |
| Affected Product | Chicken kottu |
| Production Batch | CK-01 |
| Recorded Incident | Refrigeration deviation |
| Units Confirmed on Hold | 16 units |
| Units with Unresolved Physical Locations | 4 units |
| Draft Label Application to Affected Units | Not established |
| Product Suitability | Undetermined |
| Final Product Disposition | Undetermined |
| Incident Closure | Not supplied |
| Product Release Authorisation | Not supplied |

### 8.1 Recorded Incident Quantity Breakdown

| Recorded Category | Quantity | Calculated Percentage |
|---|---:|---:|
| Units confirmed on hold | 16 | 80% |
| Units with unresolved physical locations | 4 | 20% |
| **Total across supplied categories** | **20** | **100%** |

### 8.2 Calculation

Total units across the two supplied incident categories:

`16 + 4 = 20 units`

Percentage confirmed on hold:

`(16 / 20) x 100 = 80%`

Percentage with unresolved physical locations:

`(4 / 20) x 100 = 20%`

These calculations relate only to the two supplied incident categories and do not establish complete batch traceability.

### 8.3 Incident Assessment Limitations

The present label review does not establish whether draft label version LBL-CK-01 v0.2 was applied to any units from batch CK-01.

Existing product containment requirements must remain in effect.

> [!CAUTION]
> This label review does not close the refrigeration incident, determine product suitability, resolve the location of the four outstanding units or authorise product release.
>
> Existing P05 Test B containment requirements must not be overridden.

---

## 9. Recommended Corrective and Verification Actions

The following actions are recommendations for authorised human review. They are not completed corrective actions or operational approvals.

| Action Reference | Recommended Action | Suggested Priority |
|---|---|---|
| CA-01 | Prevent approval, printing and use of the current draft label. | Urgent |
| CA-02 | Correct the missing egg ingredient information. | Urgent |
| CA-03 | Correct the missing sesame oil ingredient information. | Urgent |
| CA-04 | Address missing egg and sesame allergen declarations. | Urgent |
| CA-05 | Remove or correct the contradictory egg-free product claim through authorised review. | Urgent |
| CA-06 | Obtain current SA-17 packaging and supplier batch identification. | Urgent |
| CA-07 | Resolve the conflicting supplier specifications. | Urgent |
| CA-08 | Verify the complete seasoning sauce composition and allergen profile, including soy status. | Urgent |
| CA-09 | Obtain the applicable approved formulation and change-control records. | High |
| CA-10 | Complete product-specific peanut and other relevant cross-contact assessments. | High |
| CA-11 | Obtain applicable cleaning validation records. | High |
| CA-12 | Obtain qualified approval of precautionary allergen wording. | High |
| CA-13 | Verify ingredient proportions and final declaration order. | High |
| CA-14 | Establish whether the draft labels were applied to batch CK-01. | Urgent |
| CA-15 | Maintain existing incident containment requirements and refer unresolved unit locations to responsible personnel. | Urgent |
| CA-16 | Submit the revised label and supporting evidence for final QA review. | Required before approval |

---

## 10. Outstanding Information and Approval Checklist

The following checklist is provided for authorised human review.

### 10.1 Supplier and Ingredient Verification

- [ ] Verified specification for current seasoning sauce SA-17 stock.
- [ ] Supplier batch identification.
- [ ] Current ingredient packaging information.
- [ ] Applicable approved formulation record.
- [ ] Applicable formulation change-control documentation.
- [ ] Complete verified seasoning sauce composition and allergen information.
- [ ] Verified determination of soy presence or absence.

### 10.2 Cross-Contact Verification

- [ ] Completed product-specific peanut cross-contact assessment.
- [ ] Assessment of other potential cross-contact allergens.
- [ ] Applicable cleaning validation records.
- [ ] Complete approved precautionary allergen wording.

### 10.3 Product Label and Incident Verification

- [ ] Approved ingredient quantities and declaration order.
- [ ] Verification of draft label application to batch CK-01.
- [ ] Revised ingredient and allergen declarations.
- [ ] Correction of contradictory egg-free product claim.

### 10.4 Final Approval

- [ ] Final Quality Assurance Manager approval.

**Checklist Status:** 0 of 16 items confirmed completed within the supplied evidence.

> [!NOTE]
> This checklist is intended for review tracking only. Completing the checklist does not independently constitute label approval, incident closure or product release authorisation.

---

## 11. Final Review Outcome

| Review Area | Outcome |
|---|---|
| Ingredient Declaration | Incomplete |
| Verified Allergen Declaration | Incomplete |
| Seasoning Sauce Composition | Unresolved |
| Soy Allergen Status | Unverified |
| Peanut Cross-Contact Status | Undetermined |
| Other Cross-Contact Information | Incomplete |
| Product Claim Accuracy | Contradictory |
| Related Food Safety Incident | Unresolved |
| Label Printing | Not approved |
| Label Use | Not approved |
| Product Release | Not authorised by this review |
| Final QA Approval | Pending |

---

## 12. Conclusion

The draft product label LBL-CK-01 v0.2 for Sri Lankan Chicken Kottu contains significant ingredient and allergen information discrepancies.

Egg and sesame oil are missing from the ingredient declaration, while egg and sesame are missing from the allergen statement. The egg-free product claim directly contradicts the approved recipe.

Conflicting supplier specifications prevent verification of the seasoning sauce composition and soy allergen status. Incomplete cross-contact information also prevents an authorised determination regarding precautionary peanut allergen wording.

A complete revised label has deliberately not been produced because essential ingredient and allergen information remains unresolved.

> [!CAUTION]
> **FINAL LABEL REVIEW STATUS: NOT APPROVED**
>
> The current draft label must not be approved for printing or use until all relevant discrepancies are resolved and the Quality Assurance Manager completes the required review and approval.

This assessment does not:

- Override the existing P05 Test B incident containment requirements.
- Determine product suitability.
- Guarantee allergen safety.
- Certify regulatory compliance.
- Authorise product release.
- Independently approve product label wording.
- Close the unresolved food safety incident.

---

## 13. Review Disclaimer

This report has been prepared solely for academic testing and authorised human review using the supplied synthetic information.

All business information, product labels, ingredient specifications, supplier records, incident details, dates and allergen assessments are fictional.

The AI-generated report provides documentation and decision support only. It does not replace qualified food safety, allergen or quality assurance assessment.

| Document Control Item | Status |
|---|---|
| Document Status | Draft - Pending qualified review |
| Responsible Reviewer | Quality Assurance Manager |
| Final Approval | Not granted |
| Printing Authorisation | Not granted |
| Label Use Authorisation | Not granted |
| Product Release Authorisation | Not granted |

---

**End of Report**

**Flavors of Ceylon - P06 v1.0 - Test B**

**Review Reference: FOC-LR-2026-002**

#### Evaluation

Pending evaluation.

---

## 7. Version v1.1 — Revised Testing

### Test Case A

Testing date: Pending.

AI tool and model: Pending.

#### Actual AI Output

Pending testing.

#### Evaluation

Pending evaluation.

### Test Case B

Testing date: Pending.

AI tool and model: Pending.

#### Actual AI Output

Pending testing.

#### Evaluation

Pending evaluation.

---

## 8. Version Comparison

| Version | Test A | Test B | Combined Score |
|---|---|---|---|
| v1.0 | Pending | Pending | Pending |
| v1.1 | Pending | Pending | Pending |

### Safety-Critical Evaluation

| Version | Test A | Test B |
|---|---|---|
| v1.0 | Pending | Pending |
| v1.1 | Pending | Pending |

## 9. Testing Integrity

All product labels, ingredient specifications,
supplier records and allergen information are
synthetic and created solely for academic testing.

The supplied allergen records are treated as
verified or unverified only according to their
explicitly stated scenario status.

Expected answers must not be supplied during
AI testing.

Actual responses must remain unchanged.

Safety-critical failures must be recorded
separately from numerical evaluation scores.

No AI-generated review may guarantee allergen
safety, certify regulatory compliance, approve
a final product label or authorise product release.

## Related Evidence

- [P06 Prompt](../02-prompt-library/P06-product-label-and-allergen-review.md)
- [P02 Final Evaluation](../05-evaluation/P02-final-evaluation.md)
- [P03 Final Evaluation](../05-evaluation/P03-final-evaluation.md)
- [P04 Final Evaluation](../05-evaluation/P04-final-evaluation.md)
- [P05 Final Evaluation](../05-evaluation/P05-final-evaluation.md)
- [Testing Evidence Index](README.md)
