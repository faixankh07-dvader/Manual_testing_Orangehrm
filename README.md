# OrangeHRM Manual Testing Project

Manual QA project testing the core **Login**, **PIM (Employee Information Management)**, and **Leave** modules of the [OrangeHRM Open Source Demo](https://opensource-demo.orangehrmlive.com), a live public HR management system used for QA practice.

## Objective

Demonstrate the manual testing lifecycle end-to-end: test planning, test case design, execution, defect reporting, and summary reporting — using professional QA documentation standards.

## Scope

- **Login / Authentication** — valid/invalid login, field validation, session handling
- **PIM** — add/search/edit/delete employee records
- **Leave** — apply for leave, view requests, approve/reject flow, filtering

## Results at a glance

| Module | Test Cases | Pass | Fail |
|---|---|---|---|
| Login | 12 | 11 | 1 |
| PIM | 12 | 11 | 1 |
| Leave | 12 | 9 | 3 |
| **Total** | **36** | **30** | **5** |

**4 defects found** — 1 High, 2 Medium, 1 Low. Full details in `docs/Test_Cases.xlsx` → **Bug Reports** tab.

Notable finding: **BUG_003** — Approve/Reject actions were not accessible for pending leave requests on the Admin's Leave List view, blocking the core leave-approval workflow (flagged for re-verification, as it may be a permission artifact of the shared public demo rather than an app defect).

## Repository Structure

```
docs/
  Test_Plan.md       → Scope, approach, environment, entry/exit criteria
  Test_Cases.xlsx     → Full test documentation (5 tabs):
                          - Execution Summary (results + observations)
                          - Login Module (12 test cases)
                          - PIM Module (12 test cases)
                          - Leave Module (12 test cases)
                          - Bug Reports (4 defects, full repro steps)
```

## Tools Used

- Manual black-box testing (positive, negative, boundary test design)
- Microsoft Excel for test case management and reporting

## Author

M Faizan Khan
