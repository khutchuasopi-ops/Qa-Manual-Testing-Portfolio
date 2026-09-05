# Test Cases — Production Management Platform QA

## 1. Project Management

### TC-001 — Open Project from Projects List

**Area:** Project Management
**Priority:** High

**Steps:**

1. Open the Projects page.
2. Select an existing project.
3. Open the project.

**Expected Result:**
The selected project opens successfully.

---

### TC-002 — Load Project Details

**Area:** Project Management
**Priority:** High

**Steps:**

1. Open the Projects page.
2. Select an existing project.
3. Wait for Project Details to load.

**Expected Result:**
Project Details load successfully.

---

### TC-003 — Compare Project Details Across Projects

**Area:** Project Management
**Priority:** Medium

**Steps:**

1. Open one existing project.
2. Verify that Project Details load.
3. Return to the Projects list.
4. Open another project.
5. Compare the loading behavior.

**Expected Result:**
All valid projects should open their Project Details successfully and consistently.

---

### TC-004 — Verify Project Stage Display

**Area:** Project Management
**Priority:** Medium

**Steps:**

1. Open an existing project.
2. Review the project stage.
3. Navigate away from the project.
4. Open the project again.
5. Compare the displayed stage.

**Expected Result:**
The project stage should be displayed consistently.

---

### TC-005 — Verify Project Data After Refresh

**Area:** Project Management
**Priority:** Medium

**Steps:**

1. Open an existing project.
2. Review the displayed project information.
3. Refresh the page.
4. Review the project information again.

**Expected Result:**
Project information remains available and consistent after refresh.

---

### TC-006 — Compare Similar Project Records

**Area:** Project Management
**Priority:** Medium

**Steps:**

1. Open the Projects list.
2. Identify two available projects with similar information.
3. Open each project separately.
4. Compare their displayed details.

**Expected Result:**
Each project should display its own correct information without mixing data between records.

---

## 2. Director Availability

### TC-007 — Open Director Availability

**Area:** Director Availability
**Priority:** High

**Steps:**

1. Open the Director section.
2. Select a Director.
3. Open the Availability section.

**Expected Result:**
The selected Director's Availability section opens successfully.

---

### TC-008 — Open Add Availability Event Form

**Area:** Director Availability
**Priority:** High

**Steps:**

1. Open a Director's Availability.
2. Click **+ EVENT**.

**Expected Result:**
The Add Event form opens successfully.

---

### TC-009 — Create Availability Event with Valid Data

**Area:** Director Availability
**Priority:** High

**Steps:**

1. Open the Add Event form.
2. Enter valid Event information.
3. Select valid start and end dates.
4. Submit the Event.

**Expected Result:**
The Event is created successfully and appears in the Director's Availability.

---

### TC-010 — Verify Availability Event Status Options

**Area:** Director Availability
**Priority:** Medium

**Steps:**

1. Open the Add Event form.
2. Review the available Event status options.

**Expected Result:**
The available status options are displayed correctly and can be selected as applicable.

---

### TC-011 — Validate Valid Availability Dates

**Area:** Director Availability
**Priority:** High

**Steps:**

1. Open the Add Event form.
2. Enter a valid start date.
3. Enter a valid end date after the start date.
4. Submit the Event.

**Expected Result:**
The valid date range is accepted.

---

### TC-012 — Reject Invalid Availability Date Range

**Area:** Director Availability
**Priority:** High

**Steps:**

1. Open the Add Event form.
2. Enter a valid start date.
3. Enter an end date earlier than the start date.
4. Submit the Event.

**Expected Result:**
The invalid date range is rejected and appropriate validation is displayed.

---

### TC-013 — Verify Optional Availability Fields

**Area:** Director Availability
**Priority:** Medium

**Steps:**

1. Open the Add Event form.
2. Enter the required Event information.
3. Leave optional Project and Notes fields empty.
4. Submit the Event.

**Expected Result:**
Optional fields should not prevent valid Event creation.

---

### TC-014 — Retest Availability Event Creation

**Area:** Director Availability
**Priority:** High

**Steps:**

1. Open a Director's Availability.
2. Click **+ EVENT**.
3. Enter valid Event information.
4. Submit the Event.
5. Review the Availability list.

**Expected Result:**
The Event is created successfully and remains visible in Availability.

**Retest Result:**
The previously identified Event creation issue was fixed and successfully retested.

---

## 3. Production Budget

### TC-015 — Open Production Budget

**Area:** Production Budget
**Priority:** High

**Steps:**

1. Open a project.
2. Navigate to Production Budget.
3. Open an existing budget.

**Expected Result:**
The Production Budget opens successfully.

---

### TC-016 — Select Expense Category

**Area:** Production Budget
**Priority:** Medium

**Steps:**

1. Open an existing Production Budget.
2. Add or edit an expense item.
3. Select an available expense category.

**Expected Result:**
The expense category can be selected successfully.

---

### TC-017 — Enter Expense Values

**Area:** Production Budget
**Priority:** High

**Steps:**

1. Open an expense item.
2. Enter valid expense-related values.
3. Save the budget.

**Expected Result:**
The entered expense values are accepted and saved.

---

### TC-018 — Validate Prep Value

**Area:** Production Budget
**Priority:** Medium

**Steps:**

1. Open an expense item.
2. Enter a valid Prep value.
3. Save the budget.

**Expected Result:**
The Prep value is accepted and reflected in the budget calculation.

---

### TC-019 — Validate Days Value

**Area:** Production Budget
**Priority:** Medium

**Steps:**

1. Open an expense item.
2. Enter a valid Days value.
3. Save the budget.

**Expected Result:**
The Days value is accepted and reflected in the budget calculation.

---

### TC-020 — Calculate Budget Sub-total

**Area:** Production Budget
**Priority:** High

**Steps:**

1. Open an existing Production Budget.
2. Add an expense item.
3. Enter valid expense values.
4. Save the budget.
5. Review the Sub-total.

**Expected Result:**
The Sub-total reflects the applicable expense correctly.

---

### TC-021 — Calculate Total Budget

**Area:** Production Budget
**Priority:** High

**Steps:**

1. Open an existing Production Budget.
2. Add an expense item.
3. Enter valid expense values.
4. Save the budget.
5. Review Total Budget.

**Expected Result:**
Total Budget reflects the applicable expense correctly.

---

### TC-022 — Verify Expense Is Included in Budget Total

**Area:** Production Budget
**Priority:** High

**Steps:**

1. Open an existing Production Budget.
2. Add an expense item.
3. Enter valid expense-related values.
4. Save the budget.
5. Compare the expense with the Sub-total and Total Budget.

**Expected Result:**
The added expense is included correctly in the corresponding budget calculations.

**Retest Result:**
The previously identified calculation issue was fixed and successfully retested.

---

### TC-023 — Verify Budget Values After Refresh

**Area:** Production Budget
**Priority:** Medium

**Steps:**

1. Open an existing Production Budget.
2. Enter valid expense values.
3. Save the changes.
4. Refresh the page.
5. Review the expense and total values.

**Expected Result:**
Saved values remain correct and the displayed totals remain consistent after refresh.

---

## 4. Invoice Management

### TC-024 — Open New Invoice Form

**Area:** Invoice Management
**Priority:** High

**Steps:**

1. Open Invoice Management.
2. Select the option to create a new invoice.

**Expected Result:**
The New Invoice form opens successfully.

---

### TC-025 — Create Invoice with Valid Data

**Area:** Invoice Management
**Priority:** High

**Steps:**

1. Open the New Invoice form.
2. Enter valid values in all required fields.
3. Enter a valid invoice amount.
4. Submit the invoice.

**Expected Result:**
The invoice is created successfully.

---

### TC-026 — Validate Required Invoice Fields

**Area:** Invoice Management
**Priority:** High

**Steps:**

1. Open the New Invoice form.
2. Leave a required field empty.
3. Submit the form.

**Expected Result:**
The application prevents submission and displays appropriate validation.

---

### TC-027 — Reject Negative Invoice Amount

**Area:** Invoice Management
**Priority:** Medium

**Steps:**

1. Open the New Invoice form.
2. Enter valid values in required fields.
3. Enter `-100` in the Amount field.
4. Submit the invoice.

**Expected Result:**
The invoice is rejected and a clear validation message explains that negative amounts are not allowed.

**Actual Result:**
The application displayed `[object Object]` instead of a readable validation message.

---

### TC-028 — Validate Duplicate Invoice Number

**Area:** Invoice Management
**Priority:** Medium

**Steps:**

1. Open the New Invoice form.
2. Enter an invoice number that already exists.
3. Complete the remaining required fields.
4. Submit the invoice.

**Expected Result:**
The invoice is rejected and a readable validation message explains the duplicate invoice number.

---

### TC-029 — Verify Decimal Invoice Amount Handling

**Area:** Invoice Management
**Priority:** Medium

**Steps:**

1. Open the New Invoice form.
2. Enter valid required information.
3. Enter a decimal amount with multiple decimal places.
4. Submit the invoice.
5. Review the displayed amount.

**Expected Result:**
The application processes and displays the amount according to its supported monetary precision.

**Observed Result:**
A value with extended decimal precision was displayed rounded to the supported monetary format.

---

### TC-030 — Verify Large Invoice Amount Handling

**Area:** Invoice Management
**Priority:** Medium

**Steps:**

1. Open the New Invoice form.
2. Enter valid required information.
3. Enter a large positive invoice amount.
4. Submit the invoice.

**Expected Result:**
The application accepts the value if it is within the supported business rules and displays it correctly.

**Observed Result:**
No confirmed defect was identified during testing.

---

## 5. Sales Activities

### TC-031 — Open Call Activity

**Area:** Sales Activity
**Priority:** Medium

**Steps:**

1. Open the Sales Activity area.
2. Select a Call activity.

**Expected Result:**
The Call activity opens successfully.

---

### TC-032 — Open Meeting Activity

**Area:** Sales Activity
**Priority:** Medium

**Steps:**

1. Open the Sales Activity area.
2. Select a Meeting activity.

**Expected Result:**
The Meeting activity opens successfully.

---

### TC-033 — Verify Call Activity Filtering

**Area:** Sales Activity
**Priority:** Medium

**Steps:**

1. Open a Call activity.
2. Review the displayed activity records.
3. Review the activity counters.

**Expected Result:**
The Call view displays only Call activities and the counters correspond to the displayed activity type.

**Observed Result:**
The Call view correctly displayed only Call activities.

---

### TC-034 — Verify Meeting Activity Filtering

**Area:** Sales Activity
**Priority:** Medium

**Steps:**

1. Open a Meeting activity.
2. Review the displayed activity records.
3. Review the activity counters.

**Expected Result:**
The Meeting view displays only Meeting activities.

**Actual Result:**
The Meeting view displayed both Meeting and Call activities.

---

### TC-035 — Compare Call and Meeting Views

**Area:** Sales Activity
**Priority:** Medium

**Steps:**

1. Open a Call activity and review the displayed records.
2. Return to the activity list.
3. Open a Meeting activity.
4. Compare the displayed records.

**Expected Result:**
Each activity view should preserve the selected activity type and display only relevant records.

**Actual Result:**
Call filtering worked correctly, while Meeting filtering displayed unrelated Call activities.

---

## 6. Files / Cloud Import

### TC-036 — Open Cloud Import

**Area:** Files / Cloud Import
**Priority:** Medium

**Steps:**

1. Open the Files section.
2. Click **Import from Cloud**.

**Expected Result:**
The Cloud Import functionality opens successfully.

---

### TC-037 — Navigate to Cloud Integration Settings

**Area:** Files / Cloud Import
**Priority:** Medium

**Steps:**

1. Open Files.
2. Click **Import from Cloud**.
3. Click **Set up in Settings**.

**Expected Result:**
The user is navigated to the relevant Cloud integration settings.

---

### TC-038 — Verify Action Button Normal State

**Area:** UI / Usability
**Priority:** Medium

**Steps:**

1. Navigate to the relevant Cloud integration settings.
2. Locate the action button.
3. Review the button in its normal state.

**Expected Result:**
The button and its text are clearly visible and readable.

---

### TC-039 — Verify Action Button Hover State

**Area:** UI / Usability
**Priority:** Medium

**Steps:**

1. Navigate to the relevant Cloud integration settings.
2. Locate the action button.
3. Move the mouse over the button.
4. Compare the normal and hover states.

**Expected Result:**
The button text remains readable and maintains sufficient contrast against the hover background.

**Actual Result:**
The background became white while the text remained white, making the text practically unreadable.

---

## 7. Cross-Module / Regression

### TC-040 — Verify Data Consistency After Save and Refresh

**Area:** Cross-Module / Regression
**Priority:** High

**Steps:**

1. Open a module containing editable project-related data.
2. Enter valid data.
3. Save the changes.
4. Navigate away from the current page.
5. Return to the same record.
6. Refresh the page.
7. Compare the displayed data with the saved values.

**Expected Result:**
Saved data remains consistent after navigation and refresh, and no unexpected changes or data loss occur.
