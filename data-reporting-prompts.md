# 📊 Data & Reporting Prompts

> Prompts for Excel formulas, data analysis, and reporting automation.

[← Back to Main Library](../README.md)

---

### 6.1 Excel Formula Builder for Timesheet Analysis

**When to use:** You manage employee timesheets in Excel and need formulas to summarize approval status counts and total hours per employee across two sheets.

```
I am building an Excel timesheet analysis. I have:
- Detail sheet name: [e.g., "TimeSheetReportManager"]
  - Employee names in column: [e.g., B]
  - Status values in column: [e.g., K] — values are "Approved", "Pending", "Rejected"
  - Hours logged in column: [e.g., L]
- Analysis sheet name: [e.g., "Timesheets Analysis"]
  - Employee names listed starting at cell: [e.g., P4]
  - I want output columns for: Approved count, Pending count, Rejected count, Total Hours

Provide:
1. COUNTIFS formula for each status (Approved / Pending / Rejected) referencing the employee name dynamically
2. SUMIFS formula for total hours per employee
3. The custom cell format to apply to the Total Hours column so values over 24 hours display correctly
4. Exact steps to implement: headers, row 1 formulas, how to drag down for all employees
5. A verification step to cross-check formula results using Excel's filter function

Use cell references, not hardcoded names. Make all formulas copy-paste ready.
```

**Tags:** `Excel` `timesheet` `formulas` `COUNTIFS` `SUMIFS` `reporting` `management`

---

*[← Back to Main Library](../README.md)*
