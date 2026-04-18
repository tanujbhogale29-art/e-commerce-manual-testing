# 📊 Test Summary Report — E-Commerce Website

**Project:** E-Commerce Website Manual Testing  
**Prepared By:** Tanuj Bhogale  
**Date:** March 2026  
**Version:** 1.0

---

## 1. Executive Summary

Manual testing was performed on 4 modules of an E-Commerce website — Login, Search, Cart, and Checkout. A total of **15 test cases** were executed, **8 bugs** were identified, reported, fixed by the development team, and verified through regression testing. The application is stable and ready for release.

---

## 2. Test Execution Summary

| Metric | Count |
|--------|-------|
| Total Test Cases Written | 15 |
| Total Test Cases Executed | 15 |
| ✅ Passed | 7 |
| ❌ Failed | 8 |
| ⏭️ Skipped | 0 |
| 🐛 Bugs Found | 8 |
| 🔁 Bugs Fixed & Verified | 8 |
| **Final Build Status** | ✅ **PASS** |

---

## 3. Module-wise Summary

| Module | Total TCs | Pass | Fail | Bugs |
|--------|-----------|------|------|------|
| Login | 4 | 2 | 2 | 2 |
| Search | 3 | 1 | 2 | 1 |
| Cart | 4 | 2 | 2 | 2 |
| Checkout | 4 | 2 | 2 | 3 |
| **Total** | **15** | **7** | **8** | **8** |

---

## 4. Bug Severity Summary

| Severity | Count |
|----------|-------|
| 🔴 Critical | 1 (BUG-006) |
| 🟠 High | 5 (BUG-002, 004, 005, 007, 008) |
| 🟡 Medium | 2 (BUG-001, 003) |
| 🟢 Low | 0 |

---

## 5. Bug List

| Bug ID | Module | Summary | Severity | Status |
|--------|--------|---------|----------|--------|
| BUG-001 | Login | No error on wrong password | Medium | ✅ Fixed |
| BUG-002 | Login | Accepts blank spaces as input | High | ✅ Fixed |
| BUG-003 | Search | Results shown for empty/invalid search | Medium | ✅ Fixed |
| BUG-004 | Cart | Accepts 0 and negative quantity | High | ✅ Fixed |
| BUG-005 | Cart | Total not updating on qty change | High | ✅ Fixed |
| BUG-006 | Checkout | Order placed with empty cart | Critical | ✅ Fixed |
| BUG-007 | Checkout | No validation on expired card | High | ✅ Fixed |
| BUG-008 | Checkout | Wrong amount on confirmation page | Medium | ✅ Fixed |

---

## 6. Regression Testing Summary

All 8 failed test cases were re-executed after bug fixes:

| TC | Bug Fixed | Regression Result |
|----|-----------|-------------------|
| TC02 | BUG-001 | ✅ Pass |
| TC03 | BUG-002 | ✅ Pass |
| TC06 | BUG-003 | ✅ Pass |
| TC07 | BUG-003 | ✅ Pass |
| TC09 | BUG-004 | ✅ Pass |
| TC10 | BUG-005 | ✅ Pass |
| TC13 | BUG-007 | ✅ Pass |
| TC14 | BUG-008 | ✅ Pass |
| TC15 | BUG-006 | ✅ Pass |

---

## 7. Test Closure Checklist

- [x] All test cases executed
- [x] All bugs reported with proper severity/priority
- [x] All bugs fixed and regression tested
- [x] Test artifacts saved (Test Plan, Test Cases, Bug Reports)
- [x] Test Summary Report prepared
- [x] Project ready for release ✅

---

## 8. Lessons Learned

- Boundary value inputs (0, negative, max) are common sources of bugs
- Direct URL navigation can bypass frontend validations — always test this
- Empty field validation is often missed by developers
- Regression testing is essential after every bug fix

---

**Signed Off By:** Tanuj Bhogale — QA Tester  
**Date:** March 2026
