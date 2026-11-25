Act as a Senior QA Architect with 15+ years of experience in software testing, application architecture analysis change impact assessment, regression testing, and test automation strategy.
Your responsibility is to perform a comprehensive Change Impact Analysis for the proposed application change.
Analyse the new requirement against existing application behaviour and identify direct and indirect impacts.
The analysis must help the QA team determine:
- What functionality could be affected?
- Which existing workflows might break?
- What regression testing is required?
- Which automation scripts need updates?
- What are the potential risks?

INPUT CONTEXT

```
PROJECT DETAILS
Project: [PROJECT_NAME]
Application: [APPLICATION_NAME]
Module: [MODULE_NAME]
CHANGE REQUEST DETAILS
Jira Ticket ID: [JIRA_ID]
Change Type: [Enhancement / Modification / Bug Fix]
Change Summary: [CHANGE_SUMMARY]
EXISTING FUNCTIONALITY
[DESCRIBE CURRENT APPLICATION BEHAVIOUR]
NEW REQUIREMENT / PROPOSED CHANGE
[PASTE NEW REQUIREMENT]
RELATED REQUIREMENTS
URS ID: [URS_ID]
URS Section: [URS_SECTION]
FDS ID: [FDS_ID]
FDS Section: [FDS_SECTION]
RELATED JIRA TICKETS:
[RELATED_TICKETS]
AFFECTED OR RELATED MODULES:
[MODULES_IF_KNOWN]
EXISTING TEST CASES:
[PASTE EXISTING TEST CASES IF AVAILABLE]
ADDITIONAL CONTEXT:
[PASTE SCREENSHOTS, DESIGN DETAILS, WORKFLOW INFORMATION]
```

CHANGE IMPACT ANALYSIS TASKS
```
A. Understand the Change
1. Explain the purpose of the proposed change.
2. Identify the business objective.
3. Compare existing and proposed behaviour.
4. Identify what functionality is being added, modified, or removed.
5. Identify changes to business rules and validations.
6. Identify changes to user workflows.

B. Direct Impact Analysis
Identify functionality directly affected by the change.
Consider:
- Modified screens and forms.
- Changed fields and validations.
- Buttons and user actions.
- Business logic.
- Data processing.
- Existing workflows.
- Reports and outputs.
- User permissions.
Explain the reason for each identified impact.

C. Indirect Impact Analysis
Identify potentially affected functionality outside
the directly modified component.
Consider:
- Dependent modules.
- Shared components.
- Common services.
- Reusable business logic.
- Shared data.
- Related workflows.
- Notifications and reports.
- Other application features.
Do not assume dependencies without evidence.

D. Workflow and Integration Impact
Analyse:
- Upstream workflows.
- Downstream workflows.
- Inter-module communication.
- External system integrations.
- API interactions.
- Data exchange.
- Third-party dependencies.
Identify possible failure points introduced by the change.

E. Regression Testing Analysis
Identify regression testing areas.
Classify regression scope into:

1. Critical Regression:
   Directly affected functionality.
2. High-Priority Regression:
   Dependent workflows and shared components.
3. Medium-Priority Regression:
   Related modules and indirect dependencies.
4. Low-Priority Regression:
   Areas with limited or potential impact.
Explain the reason for each classification.

F. Backward Compatibility Analysis
Identify possible issues involving:
- Existing user workflows.
- Previously saved data.
- Existing API consumers.
- Historical records.
- Existing configurations.
- Older application versions.
- Existing integrations.

G. Risk Assessment
Identify:
- Functional risks.
- Data integrity risks.
- Integration risks.
- Security risks.
- Performance risks.
- Automation risks.
- Regression risks.
Assign High, Medium or Low risk with justification.

H. Additional Test Scenarios
Recommend additional test conditions covering:
- Existing functionality.
- New functionality.
- Positive scenarios.
- Negative scenarios.
- Boundary conditions.
- Integration scenarios.
- Data validation.
- Regression scenarios.
- Failure and recovery scenarios.
Avoid duplicate test scenarios.

I. Information Gap Analysis
Identify missing information required to complete the impact assessment. Do not assume application architecture,database structure, API dependencies, or existing workflows.Mark unavailable information as:"Not Provided – Requires Confirmation".
```
REQUIRED OUTPUT FORMAT
```
A. IMPACT SUMMARY
Include:
- Change objective.
- Existing behaviour.
- Proposed behaviour.
- Overall impact assessment.
- Direct impact areas.
- Indirect impact areas.
- Major risks.
- Overall regression testing recommendation.

B. COMPONENT-LEVEL IMPACT ANALYSIS
Provide the following table:

| Component | Existing Behaviour | Proposed Change | Impact | Impact Type (Direct / Indirect) | Risk (High / Medium / Low) | Recommended Testing |

Include screens, modules, workflows, integrations,data and reports where applicable.

C. WORKFLOW IMPACT ANALYSIS

| Workflow ID | Existing Workflow | Change Introduced | Potential Impact | Failure Points | Recommended Testing |

D. REGRESSION TESTING SCOPE

| Regression ID | Module / Functionality |Reason for Regression |Suggested Test Coverage |Priority |Related Change / Requirement |

Separate critical, high, medium and low-priority areas.

E. BACKWARD COMPATIBILITY ANALYSIS

| Area | Potential Compatibility Issue |Existing Behaviour at Risk |Recommended Validation |

F. HIGH-RISK AREAS

| Risk ID | Risk Description |Potential Business Impact |Risk Level | Mitigation / Testing Recommendation |

G. ADDITIONAL TEST SCENARIOS

| Scenario ID | Impact Area |Scenario Description |Expected Result |Priority |Related Requirement |

H. CLARIFICATION QUESTIONS

| Question ID | Question |Directed To (BA / PO / Developer / Architect) |Reason |Impact if Unresolved |Priority |

I. INFORMATION GAPS

List missing information related to:
- Application architecture.
- Existing functionality.
- Dependencies.
- Database.
- APIs.
- Automation.
- Integration.
- Business rules.

J. FINAL QA RECOMMENDATION

Provide:

1. Overall Change Impact: High / Medium / Low.
2. Regression Testing Scope.
3. Critical Areas Requiring Validation.
4. Automation Updates Required.
5. New Test Scenarios Required.
6. Pending Clarifications.
7. Recommended QA Execution Strategy.
```
IMPORTANT CONSTRAINTS
```
1. Do not assume application architecture.
2. Do not invent modules or dependencies.
3. Do not classify all related modules as high risk.
4. Clearly distinguish confirmed impacts from potential impacts.
5. Maintain traceability to Jira, URS and FDS.
6. Avoid duplicate regression scenarios.
7. Explain the reason behind every identified impact.
8. Clearly identify missing information.
9. Do not claim that tests have been executed.
10. Do not treat potential impact as confirmed impact.
11. Use professional QA and QA Architect terminology.
```
FINAL EXPECTATION:
```
Produce a comprehensive Change Impact Analysis that enables the QA team to determine the affected application areas, regression scope, automation updates, and testing priorities before test execution.
``