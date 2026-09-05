# QA Checklists — Production Management Platform

## Project Management

* [ ] Projects page opens successfully
* [ ] Existing project can be selected
* [ ] Project Details page opens
* [ ] Project Details load successfully
* [ ] Different projects can be opened
* [ ] Similar project records display their own data
* [ ] Project stage is displayed consistently
* [ ] Project information remains available after refresh
* [ ] Project data is not mixed between records

## Director Availability

* [ ] Director can be selected
* [ ] Availability section opens
* [ ] **+ EVENT** button is available
* [ ] Add Event form opens
* [ ] Event status options are displayed
* [ ] Valid start date is accepted
* [ ] Valid end date is accepted
* [ ] End date earlier than start date is rejected
* [ ] Optional Project field works correctly
* [ ] Optional Notes field works correctly
* [ ] Valid Event can be created
* [ ] Created Event appears in Availability
* [ ] Previously reported Event creation issue is retested after fix

## Production Budget

* [ ] Production Budget opens
* [ ] Expense category can be selected
* [ ] Expense item can be added
* [ ] Expense values can be entered
* [ ] Prep value is accepted
* [ ] Days value is accepted
* [ ] Sub-total is calculated correctly
* [ ] Total Budget is calculated correctly
* [ ] Expense is included in budget totals
* [ ] Saved budget values remain correct after refresh
* [ ] Previously reported calculation issue is retested after fix

## Invoice Management

* [ ] New Invoice form opens
* [ ] Required fields are validated
* [ ] Valid invoice can be created
* [ ] Negative amount is rejected
* [ ] Negative amount displays a readable validation message
* [ ] Duplicate invoice number is validated
* [ ] Duplicate validation message is readable
* [ ] Decimal monetary values are handled correctly
* [ ] Large positive amount is handled according to supported rules
* [ ] Validation does not expose internal object representations
* [ ] Invoice data is saved correctly

## Sales Activities

* [ ] Sales Activity area opens
* [ ] Call activity can be opened
* [ ] Meeting activity can be opened
* [ ] Activity type is displayed correctly
* [ ] Call view displays Call activities
* [ ] Meeting view displays only Meeting activities
* [ ] Activity counters are displayed
* [ ] Activity counters are consistent with displayed records
* [ ] Different activity types are correctly filtered
* [ ] Activity views do not display unrelated activity types

## Files / Cloud Import

* [ ] Files section opens
* [ ] Import from Cloud is accessible
* [ ] Set up in Settings navigation works
* [ ] Cloud integration settings open
* [ ] Relevant action button is visible
* [ ] Button text is readable in normal state
* [ ] Button text remains readable on hover
* [ ] Hover state maintains sufficient contrast
* [ ] Action button remains visually identifiable during interaction

## Validation & Error Handling

* [ ] Invalid input is rejected
* [ ] Required field validation is displayed
* [ ] Validation messages are readable
* [ ] Error messages clearly explain the problem
* [ ] Technical object representations are not displayed to users
* [ ] Invalid data does not create unintended records
* [ ] Validation behavior is consistent across tested forms

## Data Consistency

* [ ] Saved values remain correct after refresh
* [ ] Related displayed values remain synchronized
* [ ] Project data is consistent across views
* [ ] Budget values remain consistent after saving
* [ ] Activity type and displayed records remain consistent
* [ ] No unrelated records appear in filtered views

## Exploratory Testing

* [ ] Similar records were compared
* [ ] Different activity types were compared
* [ ] Invalid input was tested
* [ ] Negative values were tested
* [ ] Boundary-style monetary values were explored
* [ ] Calculation behavior was investigated
* [ ] UI hover states were checked
* [ ] Unexpected application responses were investigated
* [ ] Suspicious behavior was investigated before reporting
* [ ] False positives were excluded from Bug Reports

## Regression / Retesting

* [ ] BUG-001 — Director Availability Event creation retested
* [ ] BUG-003 — Production Budget calculation retested
* [ ] Fixed functionality remains stable
* [ ] Related functionality is checked after a fix
* [ ] No new regression is introduced
* [ ] Previously reported defects are tracked separately
* [ ] Confirmed defects are documented with reproducible steps

## QA Documentation

* [ ] Test Cases are documented
* [ ] Test Scenarios are documented
* [ ] QA Checklist is maintained
* [ ] Exploratory Testing findings are documented
* [ ] Confirmed defects have Bug Reports
* [ ] Retest results are documented where applicable
* [ ] Project documentation is anonymized
* [ ] Project status is marked as ongoing
