# Test Execution Report

## 1. Overview

This document summarizes the manual test execution performed for the AI Writing Workspace.

Testing focused on the main user flows, AI-assisted writing features, data persistence, navigation, UI behavior, and application state.

**Environment:** Staging / Preview
**Testing Type:** Manual Testing
**Production Environment:** Not Tested

---

## 2. Test Execution Summary

| Metric                        | Result |
| ----------------------------- | -----: |
| Total Test Cases              |     28 |
| PASS                          |     12 |
| FAIL                          |     11 |
| Requires Product Confirmation |      4 |
| UX Recommendations            |      2 |
| Confirmed Bug Reports         |      9 |

> Note: UX recommendations are observations made during successful or functional flows and are not counted as confirmed defects.

---

# 3. Execution Results

## Board

| ID     | Test Case                            | Result                        | Finding                                                                  |
| ------ | ------------------------------------ | ----------------------------- | ------------------------------------------------------------------------ |
| TC-001 | Move a Board Item                    | PASS                          | Item moved successfully                                                  |
| TC-002 | Move a Board Item to Another Section | PASS                          | Item moved successfully                                                  |
| TC-003 | Verify Board Position Persistence    | PASS                          | Position was retained                                                    |
| TC-004 | Delete a Board Item                  | Requires Product Confirmation | Deletion behavior requires confirmation of the expected product behavior |

---

## Draft

| ID     | Test Case                                      | Result                        | Finding                                                             |
| ------ | ---------------------------------------------- | ----------------------------- | ------------------------------------------------------------------- |
| TC-005 | Open Draft Page                                | Requires Product Confirmation | Draft did not load correctly on the initial attempt                 |
| TC-006 | Interact with AI Assistant from Draft          | PASS                          | Basic AI Assistant interaction was available                        |
| TC-007 | Enter a Request in AI Assistant                | FAIL                          | `fs_entries` error was observed                                     |
| TC-008 | Verify Draft Editor Text Case                  | FAIL                          | Lowercase text was automatically entered/displayed as uppercase     |
| TC-009 | Verify Draft Content Persistence After Refresh | FAIL                          | Draft content was lost after refresh                                |
| TC-010 | Create an Editable Draft Using AI Assistant    | FAIL                          | AI Assistant failed to write content into an editable Draft         |
| TC-011 | Verify New Draft Conversation Context          | FAIL                          | New Draft retained context from a previous independent conversation |

---

## Plan

| ID     | Test Case                                     | Result | Finding                                                         |
| ------ | --------------------------------------------- | ------ | --------------------------------------------------------------- |
| TC-012 | Open Plan Page                                | PASS   | Plan page opened successfully                                   |
| TC-013 | Enter a Request in Plan Assistant             | PASS   | Assistant interaction was available                             |
| TC-014 | Verify AI-Generated Plan Appears on Plan Page | FAIL   | Generated Plan was not correctly reflected on the Plan page     |
| TC-015 | Verify Plan Content After Refresh             | FAIL   | Plan content was not correctly retained/reflected after refresh |

---

## Library and Project Details

| ID     | Test Case                          | Result            | Finding                                           |
| ------ | ---------------------------------- | ----------------- | ------------------------------------------------- |
| TC-016 | Open a Project from Library        | PASS              | Project opened successfully                       |
| TC-017 | Verify Project Details Information | PASS              | Expected project information was displayed        |
| TC-018 | Close Project Details Panel        | UX Recommendation | A clearer Close/X control would improve usability |

---

## Poster

| ID     | Test Case                              | Result | Finding                                                                |
| ------ | -------------------------------------- | ------ | ---------------------------------------------------------------------- |
| TC-019 | Upload an Image for Poster             | PASS   | Image uploaded successfully                                            |
| TC-020 | Save Poster                            | FAIL   | Save action was delayed/unresponsive before the updated state appeared |
| TC-021 | Verify Current Poster in Upload Dialog | FAIL   | Previous image was displayed instead of the current poster             |

---

## AI Chat

| ID     | Test Case                                            | Result                        | Finding                                                                  |
| ------ | ---------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------ |
| TC-022 | Verify New Chat Starts Without Previous Conversation | FAIL                          | Previous conversation was temporarily displayed in the new chat          |
| TC-023 | Verify Conversation State After Project Deletion     | Requires Product Confirmation | Observed behavior requires confirmation of the expected product behavior |

---

## Templates

| ID     | Test Case                          | Result                        | Finding                                         |
| ------ | ---------------------------------- | ----------------------------- | ----------------------------------------------- |
| TC-024 | Drag Template Element              | PASS                          | Element could be dragged successfully           |
| TC-025 | Verify Horizontal Template Content | Requires Product Confirmation | Expected product behavior requires confirmation |

---

## Split View

| ID     | Test Case                    | Result | Finding                                                              |
| ------ | ---------------------------- | ------ | -------------------------------------------------------------------- |
| TC-026 | Verify Split View Pagination | FAIL   | Pagination/page controls were duplicated or reset in the second pane |

---

## Cross-Flow

| ID     | Test Case                                           | Result | Finding                                          |
| ------ | --------------------------------------------------- | ------ | ------------------------------------------------ |
| TC-027 | Navigate from Draft to Plan and Back to Draft       | PASS   | Draft → Plan → Draft flow completed successfully |
| TC-028 | Verify Draft Editor and AI Chat Inputs Are Separate | PASS   | Inputs remained separate                         |

---

# 4. Confirmed Defect Traceability

The following defects were confirmed during testing and documented in the project's Bug Reports.

| Bug ID  | Related Test Case(s) | Area                         | Severity | Status |
| ------- | -------------------- | ---------------------------- | -------- | ------ |
| BUG-001 | TC-009               | Draft Persistence            | Medium   | Open   |
| BUG-002 | TC-008               | Draft Editor                 | Medium   | Open   |
| BUG-003 | TC-010               | AI Assistant / Draft         | High     | Open   |
| BUG-004 | TC-011               | AI Assistant / Draft Context | High     | Open   |
| BUG-005 | TC-014, TC-015       | Plan / AI Assistant          | High     | Open   |
| BUG-006 | TC-020               | Poster                       | Medium   | Open   |
| BUG-007 | TC-021               | Poster                       | Medium   | Open   |
| BUG-008 | TC-022               | AI Chat                      | Medium   | Open   |
| BUG-009 | TC-026               | Split View                   | Medium   | Open   |

**Total Confirmed Bugs:** 9

---

# 5. Findings Requiring Product Confirmation

These observations were not counted as confirmed bugs because the expected product behavior needs clarification.

| Test Case | Finding                                   |
| --------- | ----------------------------------------- |
| TC-004    | Board item deletion behavior              |
| TC-005    | Initial Draft loading behavior            |
| TC-023    | Conversation state after project deletion |
| TC-025    | Horizontal Template content behavior      |

These findings should be confirmed against the intended product requirements before being classified as defects.

---

# 6. UX Recommendations

The following observations are usability recommendations and are not classified as bugs.

| Test Case | Recommendation                                             |
| --------- | ---------------------------------------------------------- |
| TC-018    | Make the Project Details Close/X control clearer           |
| TC-024    | Use a grab/grabbing cursor for draggable Template elements |

---

# 7. Main Findings

During testing, the main issues were observed in:

* Draft content persistence
* Draft Editor text formatting
* AI-generated Draft creation
* AI conversation context
* AI-generated Plan persistence and reflection
* Poster saving
* Poster image state
* AI Chat state
* Split View pagination

These findings resulted in **9 confirmed Bug Reports**.

---

# 8. Overall Result

The main application flows were tested manually in the Staging/Preview environment.

Several core flows worked as expected, including Board movement, Library access, Project Details information, Poster upload, and Draft → Plan → Draft navigation.

The main issues were related to **data persistence, AI workflow behavior, conversation state, poster state, and Split View pagination**.

Four additional findings require product confirmation before they can be classified as defects.

Production testing was not performed.

---

# 9. QA Conclusion

The testing identified **9 confirmed defects** across the tested areas.

The results provide a clear record of the observed application behavior and the areas that require further investigation or product clarification.

The execution results are linked to the documented Test Cases and Bug Reports to maintain basic traceability throughout the QA documentation.
