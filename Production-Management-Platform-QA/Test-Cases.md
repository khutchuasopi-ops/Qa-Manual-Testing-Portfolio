# Test Cases — Production Management Platform QA

## TC-001 — Create Director Availability Event

**Area:** Director Availability
**Priority:** High

**Preconditions:**
A Director is available and the Availability section is accessible.

**Steps:**

1. Open the Director section.
2. Select a Director.
3. Open Availability.
4. Click **+ EVENT**.
5. Enter valid Event information.
6. Select valid start and end dates.
7. Submit the Event.

**Expected Result:**
The Event is created successfully and displayed in the Director's Availability.

---

## TC-002 — Validate Availability Event Date Range

**Area:** Director Availability
**Priority:** High

**Steps:**

1. Open the Add Event form.
2. Enter a valid start date.
3. Enter an end date earlier than the start date.
4. Submit the Event.

**Expected Result:**
The application rejects the invalid date range and displays appropriate validation.

---

## TC-003 — Open Project Details

**Area:** Project Management
**Priority:** High

**Steps:**

1. Open the Projects page.
2. Select an existing project.
3. Wait for Project Details to load.

**Expected Result:**
The selected project's details load successfully.

---

## TC-004 — Calculate Production Budget Total

**Area:** Production Budget
**Priority:** High

**Steps:**

1. Open Production Budget.
2. Select an expense category.
3. Enter valid Prep and Days values.
4. Save the budget.
5. Review Sub-total and Total Budget.

**Expected Result:**
The expense is correctly included in the Sub-total and Total Budget.

---

## TC-005 — Validate Negative Invoice Amount

**Area:** Invoice Management
**Priority:** Medium

**Steps:**

1. Open the New Invoice form.
2. Enter valid required information.
3. Enter a negative value in Amount.
4. Submit the invoice.

**Expected Result:**
The invoice is rejected and a clear validation message explains that negative amounts are not allowed.

---

## TC-006 — Validate Duplicate Invoice Number

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

## TC-007 — Filter Sales Activities by Type

**Area:** Sales Activity
**Priority:** Medium

**Steps:**

1. Open Sales Activity.
2. Open a Call activity.
3. Review the displayed activities.
4. Return to the activity list.
5. Open a Meeting activity.
6. Review the displayed activities.

**Expected Result:**
The selected activity type displays only the corresponding activities.

---

## TC-008 — Verify Button Hover Contrast

**Area:** UI / Usability
**Priority:** Medium

**Steps:**

1. Open Files.
2. Click Import from Cloud.
3. Click Set up in Settings.
4. Navigate to the relevant Cloud integration settings.
5. Locate the action button.
6. Hover over the button.

**Expected Result:**
The button text remains clearly readable and maintains sufficient contrast against the hover background.

---

## TC-009 — Validate Budget Values After Save

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

## TC-010 — Verify Error Message Readability

**Area:** Validation / Error Handling
**Priority:** Medium

**Steps:**

1. Open a form containing validation rules.
2. Enter invalid data.
3. Submit the form.
4. Review the displayed error message.

**Expected Result:**
The application displays a clear, user-readable validation message rather than an internal object or technical representation.
