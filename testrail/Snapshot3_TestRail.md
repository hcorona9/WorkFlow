# TestRail — Snapshot 3 Test Run Report

> **Instructions:** After completing your TestRail test run, go to **Reports → Summary (Run tab)**
> and export/screenshot the summary. Replace this file with that export, or paste the summary
> content below.

---

## Test Run: Snapshot 3 — Workflow Export / Report Generation

**Project:** QTC WFQ Administrator Application  
**Sprint:** Snapshot 3  
**Feature Under Test:** Workflow Export (PDF and CSV)  
**Tester(s):** *(Add names)*  
**Date:** *(Add date)*

---

## Test Cases

| ID | Title | Type | Expected Result | Status |
|---|---|---|---|---|
| T-01 | Export PDF — workflow with steps and tasks | Positive | PDF downloads successfully; contains workflow name, steps table, tasks table | *(Pass/Fail)* |
| T-02 | Export CSV — workflow with tasks | Positive | CSV downloads successfully; contains correct columns and data rows | *(Pass/Fail)* |
| T-03 | PDF file name format correct | Positive | File named `{WorkflowName}_Report_{YYYY-MM-DD}.pdf` | *(Pass/Fail)* |
| T-04 | CSV file name format correct | Positive | File named `{WorkflowName}_Tasks_{YYYY-MM-DD}.csv` | *(Pass/Fail)* |
| T-05 | Export PDF — workflow with no steps | Edge Case | PDF downloads; steps section shows "No steps have been added to this workflow." | *(Pass/Fail)* |
| T-06 | Export CSV — workflow with no tasks | Edge Case | CSV downloads; file contains header row only with no data rows | *(Pass/Fail)* |
| T-07 | Export does not modify database | Negative | No records are created, updated, or deleted after export | *(Pass/Fail)* |
| T-08 | Export requires admin authorization | Security | Accessing export URL without `?is_admin=true` returns Access Denied | *(Pass/Fail)* |
| T-09 | Admin stays on Workflow Details page after export | Positive | Page does not navigate away; file download triggers in browser | *(Pass/Fail)* |
| T-10 | PDF is readable in standard PDF viewer | Positive | PDF opens correctly in browser PDF viewer and Adobe Acrobat | *(Pass/Fail)* |
| T-11 | CSV is compatible with Excel / Google Sheets | Positive | CSV opens correctly in Excel and Google Sheets without formatting errors | *(Pass/Fail)* |
| T-12 | Export button shows loading state during generation | Positive | Button shows spinner and is disabled while file is being generated | *(Pass/Fail)* |
| T-13 | Export error — server failure shows toast | Negative | If generation fails, red error toast appears; page remains functional | *(Pass/Fail)* |

---

## Summary

*(Paste your TestRail Run Summary report screenshot or export here after completing the test run.)*

- **Total Tests:** 13  
- **Passed:** *(fill in)*  
- **Failed:** *(fill in)*  
- **Blocked/Skipped:** *(fill in)*

---

## Notes / Defects Found

*(Document any bugs or issues discovered during this test run here.)*
