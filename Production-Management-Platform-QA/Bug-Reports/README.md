# Bug Reports — Production Management Platform

This folder contains the documented defects identified during manual QA testing of the Production Management Platform.

## Defect Summary

| Bug ID  | Area                  | Severity | Status |
| ------- | --------------------- | -------- | ------ |
| BUG-001 | Director Availability | High     | Fixed  |
| BUG-002 | Project Management    | Medium   | Open   |
| BUG-003 | Production Budget     | High     | Fixed  |
| BUG-004 | Invoice Management    | Medium   | Open   |
| BUG-005 | Sales Activity        | Medium   | Open   |
| BUG-006 | UI / Usability        | Medium   | Open   |

## Bug Reports

### BUG-001 — Event Cannot Be Added to Director Availability

**Severity:** High
**Status:** Fixed

An Availability Event could not be added successfully to Director Availability.

The issue was fixed and successfully retested.

[View BUG-001](BUG-001-event-cannot-be-added-to-director-availability.md)

---

### BUG-002 — Project Details Fail to Load for a Specific Project

**Severity:** Medium
**Status:** Open

Project Details failed to load for one specific project while other projects opened normally.

The issue remained reproducible during retesting.

[View BUG-002](BUG-002-project-details-fail-to-load.md)

---

### BUG-003 — Expense Not Included in Budget Total

**Severity:** High
**Status:** Fixed

An added expense was not correctly reflected in the Budget Sub-total and Total Budget.

The issue was fixed and successfully retested.

[View BUG-003](BUG-003-expense-not-included-in-budget-total.md)

---

### BUG-004 — Negative Invoice Amount Displays `[object Object]`

**Severity:** Medium
**Status:** Open

A negative invoice amount resulted in `[object Object]` instead of a readable validation message.

[View BUG-004](BUG-004-negative-invoice-amount-object-object.md)

---

### BUG-005 — Meeting Activity View Displays Call Activities

**Severity:** Medium
**Status:** Open

The Meeting activity view displayed both Meeting and Call activities instead of only Meeting activities.

[View BUG-005](BUG-005-meeting-view-displays-call-activities.md)

---

### BUG-006 — Button Text Becomes Unreadable on Hover

**Severity:** Medium
**Status:** Open

Button text became difficult to read on hover because the text and background had insufficient contrast.

[View BUG-006](BUG-006-button-text-unreadable-on-hover.md)

---

## Defect Statistics

| Metric          | Count |
| --------------- | ----: |
| Total Defects   |     6 |
| Fixed           |     2 |
| Open            |     4 |
| High Severity   |     2 |
| Medium Severity |     4 |

## Retesting Summary

Two defects were successfully fixed and verified through retesting:

* BUG-001 — Director Availability Event creation
* BUG-003 — Production Budget calculation

BUG-002 was retested but remained reproducible.

No retest result was documented for BUG-004, BUG-005, or BUG-006.

---

> All project names, data, and identifying information have been anonymized for portfolio purposes.
