# BUG-002 — Project Details Fail to Load for a Specific Project

**Area:** Project Management
**Type:** Functional
**Severity:** Medium
**Environment:** Test Environment

## Preconditions

Multiple projects are available in the Projects list.

## Steps to Reproduce

1. Open the **Projects** page.
2. Open the affected project.
3. Wait for the Project Details page to load.
4. Compare the result with other available projects.

## Actual Result

Project Details fail to load for one specific project.

Other projects open normally, including another project with a similar name.

## Expected Result

Every valid project should open its Project Details page successfully.

## Impact

Users cannot access or manage the affected project's information.

## Retest

The issue remained reproducible during retesting in the test environment.
