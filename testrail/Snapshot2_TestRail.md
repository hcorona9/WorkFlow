# TestRail — Snapshot 2 Test Run Report

> **Instructions:** After completing your TestRail test run, go to **Reports → Summary (Run tab)**
> and export/screenshot the summary. Replace this file with that export, or paste the summary
> content below.

---

## Test Run: Snapshot 2 — Email Notification System

**Project:** QTC WFQ Administrator Application  
**Sprint:** Snapshot 2  
**Feature Under Test:** Email Notification System  
**Tester(s):** *(Add names)*  
**Date:** *(Add date)*

---

## Test Cases

| ID | Title | Type | Expected Result | Status |
|---|---|---|---|---|
| T-01 | Task assigned — notification sent | Positive | Assignee receives email with correct subject and body | *(Pass/Fail)* |
| T-02 | Task reassigned — notification sent to new assignee | Positive | New assignee receives email; old assignee does not | *(Pass/Fail)* |
| T-03 | Task completed — admin notified | Positive | Admin receives task completed email | *(Pass/Fail)* |
| T-04 | Step created — admin notified | Positive | Admin receives step created email | *(Pass/Fail)* |
| T-05 | SMTP failure — operation still succeeds | Negative | Task assignment succeeds; error logged; no UI error shown | *(Pass/Fail)* |
| T-06 | Notifications disabled flag — no email sent | Negative | Setting `Notifications:Enabled: false` suppresses all emails | *(Pass/Fail)* |
| T-07 | Email subject format correct | Positive | Subject matches `[WFQ] Task Assigned: {TaskName}` format | *(Pass/Fail)* |
| T-08 | Email body contains workflow link | Positive | Email body includes a valid URL to the workflow details page | *(Pass/Fail)* |
| T-09 | Read-only action — no notification sent | Negative | Viewing a workflow or step does not trigger any email | *(Pass/Fail)* |
| T-10 | Completed task cannot be reassigned | Negative | Reassign button disabled/hidden for completed tasks | *(Pass/Fail)* |

---

## Summary
<img width="721" height="247" alt="ss2" src="https://github.com/user-attachments/assets/670f3aba-abaa-4153-803f-ac5a0e7a1ba4" />
<img width="716" height="347" alt="ss2p2" src="https://github.com/user-attachments/assets/480b694f-52d3-42e0-8182-022ac04b1c52" />



- **Total Tests:** 10  
- **Passed:** *6*  
- **Failed:** *4*  
- **Blocked/Skipped:** *N/A*

---

## Notes / Defects Found
*N/A*
