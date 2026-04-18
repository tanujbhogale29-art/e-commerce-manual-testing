# 🔍 Test Cases — Search Module

**Module:** Search  
**Tester:** Tanuj Bhogale  
**Date:** March 2026

---

## TC05 — Valid Product Search

| Field | Details |
|-------|---------|
| **Test Case ID** | TC05 |
| **Module** | Search |
| **Test Case Title** | Search with valid product name |
| **Type** | Positive |
| **Precondition** | User is on homepage |
| **Test Steps** | 1. Click search bar <br> 2. Type: `Laptop` <br> 3. Press Enter or click Search |
| **Expected Result** | Relevant products displayed |
| **Actual Result** | Products listed correctly ✅ |
| **Status** | ✅ Pass |
| **Bug ID** | — |

---

## TC06 — Invalid/Gibberish Search

| Field | Details |
|-------|---------|
| **Test Case ID** | TC06 |
| **Module** | Search |
| **Test Case Title** | Search with random gibberish text |
| **Type** | Negative |
| **Precondition** | User is on homepage |
| **Test Steps** | 1. Click search bar <br> 2. Type: `xyzabc123!!!` <br> 3. Press Enter |
| **Expected Result** | "No results found" message |
| **Actual Result** | Page showed unrelated products ❌ |
| **Status** | ❌ Fail |
| **Bug ID** | [BUG-003](../bug-reports/BUG-003.md) |

---

## TC07 — Empty Search

| Field | Details |
|-------|---------|
| **Test Case ID** | TC07 |
| **Module** | Search |
| **Test Case Title** | Search with empty search bar |
| **Type** | Negative |
| **Precondition** | User is on homepage |
| **Test Steps** | 1. Click search bar <br> 2. Leave it blank <br> 3. Press Enter |
| **Expected Result** | Validation message or no action |
| **Actual Result** | All products displayed on empty search ❌ |
| **Status** | ❌ Fail |
| **Bug ID** | [BUG-003](../bug-reports/BUG-003.md) |
