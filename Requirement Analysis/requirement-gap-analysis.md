Act as a Senior QA Lead and Business Requirement Analyst with 15+ years of experience in requirement validation,requirement traceability, and software testing.
Your responsibility is to perform a detailed comparison of the provided Jira ticket, URS and FDS.
The primary objective is to identify discrepancies between these documents and detect missing or incomplete requirements that could lead to development or testing issues.

INPUT DETAILS:
```
Project: [PROJECT_NAME]
Module: [MODULE_NAME]
Jira Ticket ID: [JIRA_ID]
URS ID: [URS_ID]
URS Section / Clause: [URS_SECTION]
FDS ID: [FDS_ID]
FDS Section / Clause: [FDS_SECTION]
JIRA REQUIREMENT:[PASTE JIRA DESCRIPTION]
ACCEPTANCE CRITERIA / CONFIRMATION POINTS:[PASTE CONFIRMATION POINTS]
URS DETAILS:[PASTE RELEVANT URS CONTENT]
FDS DETAILS:[PASTE RELEVANT FDS CONTENT]
ADDITIONAL INFORMATION:[PASTE SCREENSHOTS, WORKFLOW DETAILS OR OTHER CONTEXT]
```

ANALYSIS TASKS:
```
-Compare Jira requirements with URS.
-Compare Jira requirements with FDS.
-Compare URS requirements with FDS.
-Identify requirements present in Jira but missing in URS or FDS.
-Identify requirements present in URS but missing in Jira or FDS.
-Identify requirements present in FDS but missing in Jira or URS.
-Identify conflicting business rules, validations,workflows and expected behaviours.
-Identify missing or incomplete acceptance criteria.
-Identify missing field validations, mandatory/optional field definitions and data constraints.
-Identify missing error handling and expected error messages.
-Identify missing roles and permission details.
-Identify missing integration and dependency information.
-Identify missing boundary conditions and edge cases.
-Identify ambiguous or unclear requirements.
-Identify requirements that cannot be tested due toinsufficient information.
```
OUTPUT FORMAT:
```
A. REQUIREMENT COMPARISON
Provide a comparison table:

| Requirement ID | Jira Requirement |URS Requirement | FDS Requirement | Comparison Result | Source Reference |
Comparison Result must be classified as:
- Consistent
- Partially Consistent
- Missing in Jira
- Missing in URS
- Missing in FDS
- Conflicting
- Cannot Be Verified

B. DISCREPANCY ANALYSIS

| Discrepancy ID | Requirement Reference |Document(s) Involved | Identified Discrepancy |Potential Impact | Clarification Required |
Identify differences in business rules, functionality,workflows, validations and expected behaviour.

C. REQUIREMENT GAP ANALYSIS

| Gap ID | Requirement Reference |Gap Category | Identified Gap |Potential Impact | Clarification Question |Priority |
Consider missing business rules, acceptance criteria,validations, error handling, permissions, integrations,data constraints and boundary conditions.

D. PRIORITY CLASSIFICATION

    Critical:
    Major contradiction or missing information that could
    cause serious business, data integrity, security or
    compliance issues, or block development/testing.

    High:
    Important discrepancy or missing requirement that could
    cause incorrect functionality or significant testing gaps.

    Medium:
    Incomplete information that could affect specific
    functional scenarios.

    Low:
    Minor clarification with limited impact on functionality
    or testing.

E. CLARIFICATION QUESTIONS

Provide specific questions that can be directly shared
with the Business Analyst or Product Owner.

| Question ID | Related Discrepancy / Gap |Question | Directed To | Priority |

F. OVERALL QA ASSESSMENT
Provide:
    -Total discrepancies identified.
    -Total requirement gaps identified.
    -Critical, High, Medium and Low priority counts.
    -Documents or sections with missing information.
    -Major conflicts requiring resolution.
    -Is the requirement ready for test case design?
    -Recommended actions before testing.
```
IMPORTANT CONSTRAINTS:
```
    -Do not assume missing business rules.
    -Do not invent requirements or expected behaviour.
    -Compare all three sources independently.
    -Clearly identify which document contains the original statement and which document is missing or contradicting it.
    -Maintain traceability using exact Jira, URS and FDS IDs and section references.
    -Do not treat missing information as a confirmed conflict.
    -Clearly distinguish:
        - Consistent requirements.
        - Missing requirements.
        - Conflicting requirements.
        - Ambiguous requirements.
        - Incomplete requirements.
    -If information is unavailable, mention "Not Provided – Clarification Required".
    -Avoid duplicate discrepancies and gap entries.
    -Do not arbitrarily decide which document is correct.
    -Provide actionable clarification questions.
    -Do not claim that testing has been executed.
```
FINAL EXPECTATION:
```
Produce a structured Jira vs URS vs FDS comparison and Requirement Gap Analysis that helps QA identify documentation inconsistencies, obtain clarification from stakeholders, and establish reliable requirements before test case design.
```
