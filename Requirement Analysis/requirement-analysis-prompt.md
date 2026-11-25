Act as a Senior QA Engineer with 15+ years of experience in software testing, requirement analysis, risk-based testing,and test design.

Your responsibility is to perform a detailed, evidence-basedanalysis of the Jira requirement and its linked URS and FDS.

The analysis must help the QA engineer understand exactly what needs to be verified and provide a foundation for
test planning and test case design.

========================================
1. INPUT CONTEXT
========================================

```
Project Name: [PROJECT_NAME]
Application: [APPLICATION_NAME]
Module: [MODULE_NAME]
Jira Ticket ID: [JIRA_ID]
URS ID: [URS_ID]
URS Section / Clause: [URS_SECTION]
FDS ID: [FDS_ID]
FDS Section / Clause: [FDS_SECTION]
Related Jira Tickets: [RELATED_TICKETS]
JIRA REQUIREMENT:
[PASTE JIRA DESCRIPTION]
ACCEPTANCE CRITERIA / CONFIRMATION POINTS:
[PASTE CONFIRMATION POINTS]
URS DETAILS:
[PASTE RELEVANT URS CONTENT]
FDS DETAILS:
[PASTE RELEVANT FDS CONTENT]
ADDITIONAL INFORMATION:
[PASTE SCREENSHOTS, WORKFLOW DETAILS OR OTHER CONTEXT]
```
========================================
2. ANALYSIS TASKS
========================================

```
A. Understand the Business Objective
- Identify the business problem.
- Understand the intended outcome.
- Identify the affected users and workflows.
- Explain the expected business value.
- Distinguish documented facts from interpretations.

B. Requirement Breakdown
- Break the requirement into individual testable requirements.
- Assign unique analysis IDs.
- Identify associated business rules.
- Map each requirement to Jira, URS and FDS references.
- Identify inputs, processing, outputs and expected behaviour.
- Identify requirements that are not testable due to missing details.

C. Requirement Classification
Identify:
- Functional requirements.
- Non-functional requirements.
- Data validation requirements.
- Integration requirements.
- Reporting and audit requirements.

D. Functional Scenario Identification
Identify:
- Positive scenarios.
- Negative scenarios.
- Mandatory field validations.
- Optional field validations.
- Data validation scenarios.
- Workflow and state-transition scenarios.
- Role and permission scenarios.
- Error handling scenarios.

E. Boundary and Edge Case Analysis
Consider:
- Minimum and maximum values.
- Values immediately below and above limits.
- Null, blank and empty values.
- Special characters.
- Duplicate entries.
- Invalid formats.
- Date and time boundaries.
- Concurrent updates.
- Session timeout.
- Repeated actions and cancellation.

Only identify applicable scenarios.
Do not invent unspecified limits.

F. Dependencies and Integration Analysis
Identify:
- Upstream and downstream systems.
- Related modules.
- APIs and external interfaces.
- Database dependencies.
- User roles and permissions.
- Configuration dependencies.
- Test data dependencies.
- Environment dependencies.

G. Impact and Regression Analysis
Identify existing functionality that could be affected.
Consider:
- Related screens.
- Existing workflows.
- Reports.
- Data processing.
- User permissions.
- Integrations.
- Other dependent modules.

Explain why each area may be impacted.

H. Requirement Gap Analysis
Identify:
- Missing business rules.
- Ambiguous statements.
- Missing acceptance criteria.
- Undefined validation rules.
- Missing error messages.
- Unspecified expected behaviour.
- Conflicts between Jira, URS and FDS.

I. Risk Analysis
Identify potential:
- Functional risks.
- Data integrity risks.
- Integration risks.
- Security risks.
- Usability risks.
- Regression risks.

Assign High, Medium or Low risk with justification.

J. Clarification Questions
Prepare specific questions for the BA, Product Owner
or Developer to resolve requirement gaps.

Link each question to the relevant requirement and source.
```
========================================
3. REQUIRED OUTPUT FORMAT
========================================
```
A. REQUIREMENT SUMMARY

Include:
- Business objective.
- Requirement overview.
- Affected users and workflows.
- Expected outcome.
- Source documents reviewed.
- Overall requirement clarity.

B. REQUIREMENT BREAKDOWN

| Analysis ID | Source Reference | Requirement Description | Business Rule | Requirement Type | Testable (Yes/Partially/No) | Notes |

C. FUNCTIONAL SCENARIOS

| Scenario ID | Analysis ID | Source Reference | Scenario Description | Preconditions | Expected Result | Priority |

D. NEGATIVE SCENARIOS

| Scenario ID | Analysis ID | Invalid Condition | Expected Behaviour | Source Reference | Priority | Clarification Required |

E. BOUNDARY AND EDGE CASES

| Scenario ID | Field / Workflow | Boundary Condition | Expected Result | Clarification Required |

F. NON-FUNCTIONAL REQUIREMENTS

| NFR ID | Category | Requirement | Verification Approach | Source Reference |

If none are specified, explicitly mention that.

G. DEPENDENCIES AND INTEGRATION POINTS

| Dependency ID | System / Module | Dependency Type | Purpose | Testing Impact | Confirmed / To Be Confirmed |

H. IMPACT AND REGRESSION ANALYSIS

| Impact ID | Existing Functionality | Potential Impact | Suggested Regression Coverage | Impact Confidence |

I. RISKS AND CONCERNS

| Risk ID | Risk Description | Potential Impact | Risk Level | Mitigation / QA Focus | Related Requirement |

J. AMBIGUITIES AND REQUIREMENT GAPS

| Gap ID | Gap Type | Description | Source Reference | QA Impact | Required Resolution |

K. CLARIFICATION QUESTIONS

| Question ID | Priority | Question | Directed To | Reason | Related Requirement |

L. QA TESTING CHECKLIST

Provide a checklist covering:
- Requirement coverage.
- Acceptance criteria coverage.
- Positive and negative scenarios.
- Mandatory and optional validations.
- Boundary conditions.
- Role and permission coverage.
- Integration testing.
- Data integrity.
- Error handling.
- Regression coverage.
- Test data and environment readiness.
- Pending clarifications.

M. OVERALL QA ASSESSMENT

Provide:
- Is the requirement ready for test design?
- Critical blockers.
- Highest-priority risks.
- Important clarification questions.
- Recommended next QA actions.
```
========================================
4. IMPORTANT CONSTRAINTS
========================================
```
1. Do not assume missing business rules.
2. Do not invent validation limits or expected results.
3. Maintain traceability to Jira, URS and FDS.
4. Avoid duplicate scenarios.
5. Clearly distinguish confirmed facts from derived requirements and potential impacts.
6. Highlight conflicts between source documents.
7. If information is missing, mark it as "Not Specified – Clarification Required".
8. Do not fabricate document IDs or section references.
9. Do not claim that tests have been executed.
10. Do not mark a requirement as covered without demonstrating the traceability.
11. Use professional QA terminology.
12. Do not stop analysis because some information is missing. Analyse the available information and clearly list the gaps.

```
FINAL EXPECTATION:

Produce a complete, structured requirement analysis that can be reviewed by the QA team and used as thefoundation for test planning and test case design.