# Exploratory Testing — Production Management Platform QA

## Objective

Exploratory testing was used to investigate application behavior beyond predefined test cases and identify unexpected functional, validation, data, and UI issues.

## Areas Explored

### Project Management

Explored project opening, Project Details loading, project information, and behavior across multiple projects.

**Finding:**
A specific project failed to load its Project Details while other projects opened successfully.

### Director Availability

Explored event creation, available statuses, date selection, optional fields, and invalid date ranges.

**Finding:**
An issue was identified where an Availability Event could not initially be added. The issue was later fixed and successfully retested.

### Production Budget

Explored expense entry, Prep and Days values, Sub-total, and Total Budget calculations.

**Finding:**
Expenses were initially not correctly reflected in budget totals. The issue was fixed and successfully retested.

### Invoice Management

Explored invoice creation and validation using invalid and boundary-style inputs.

**Finding:**
A negative invoice amount resulted in `[object Object]` instead of a readable validation message.

### Sales Activity

Explored Call and Meeting activities and compared the behavior of different activity types.

**Finding:**
The Meeting activity view displayed both Meeting and Call activities instead of filtering to the selected activity type.

### Files / Cloud Import

Explored navigation to Cloud integration settings and interaction with action buttons.

**Finding:**
A button's hover state caused the white text to blend into a white background, making the action difficult to read.

## Exploratory Testing Techniques

* Comparing similar records
* Testing invalid input
* Testing boundary-style values
* Comparing different activity types
* Checking UI state changes
* Verifying data consistency
* Retesting previously reported issues
* Investigating unexpected application responses

## Key Findings

Exploratory testing helped identify issues that were not limited to basic happy-path functionality, including:

* Data loading problems
* Business logic calculation issues
* Validation and error-handling problems
* Incorrect activity filtering
* UI contrast and usability issues

## Conclusion

Exploratory testing provided additional coverage beyond predefined scenarios and helped identify defects across multiple application modules.

The project remains ongoing, and additional exploratory findings may be documented as new functionality is tested.
