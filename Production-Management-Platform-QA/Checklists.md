# QA Checklists — Production Management Platform

## Project Management

* [ ] Projects page opens successfully
* [ ] Project Details load correctly
* [ ] Project information is displayed consistently
* [ ] Project stage information is displayed correctly
* [ ] Project data remains available after refresh

## Director Availability

* [ ] Director can be selected
* [ ] Availability section opens
* [ ] Add Event drawer opens
* [ ] Event statuses are available
* [ ] Valid start date is accepted
* [ ] Valid end date is accepted
* [ ] End date earlier than start date is rejected
* [ ] Optional project field works
* [ ] Optional notes field works
* [ ] Created event appears in Availability

## Production Budget

* [ ] Production Budget opens
* [ ] Expense category can be selected
* [ ] Expense values can be entered
* [ ] Prep value is accepted
* [ ] Days value is accepted
* [ ] Sub-total is calculated correctly
* [ ] Total Budget is calculated correctly
* [ ] Saved values remain correct after refresh

## Invoice Management

* [ ] New Invoice form opens
* [ ] Required fields are validated
* [ ] Valid invoice can be created
* [ ] Negative amount is rejected
* [ ] Negative amount displays a readable validation message
* [ ] Duplicate invoice number is rejected
* [ ] Duplicate validation message is readable
* [ ] Invoice information is saved correctly

## Sales Activities

* [ ] Call activity can be opened
* [ ] Meeting activity can be opened
* [ ] Activity type is displayed correctly
* [ ] Call view displays Call activities
* [ ] Meeting view displays only Meeting activities
* [ ] Activity counters match displayed records

## Files / Cloud Import

* [ ] Files section opens
* [ ] Import from Cloud is accessible
* [ ] Set up in Settings navigation works
* [ ] Cloud integration settings open
* [ ] Action buttons are visible
* [ ] Button text is readable in normal state
* [ ] Button text remains readable on hover
* [ ] Hover state maintains sufficient contrast

## Validation & Error Handling

* [ ] Invalid input is rejected
* [ ] Validation messages are readable
* [ ] Technical object representations are not displayed to users
* [ ] Error messages clearly explain the problem
* [ ] Invalid data does not create unintended records

## Regression / Retesting

* [ ] Previously reported bugs are retested after fixes
* [ ] Fixed functionality remains stable
* [ ] Related functionality is checked after a fix
* [ ] No new regression is introduced
