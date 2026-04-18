# 🛒 Test Cases — Cart Module

**Module:** Cart  
**Tester:** Tanuj Bhogale  
**Date:** March 2026

---

## TC08 — Add Single Item to Cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC08 |
| **Module** | Cart |
| **Test Case Title** | Add a single product to cart |
| **Type** | Positive |
| **Precondition** | User is logged in |
| **Test Steps** | 1. Search for a product <br> 2. Click "Add to Cart" <br> 3. Open Cart |
| **Expected Result** | Product appears in cart with correct price |
| **Actual Result** | Product added correctly ✅ |
| **Status** | ✅ Pass |
| **Bug ID** | — |

---

## TC09 — Add Zero Quantity

| Field | Details |
|-------|---------|
| **Test Case ID** | TC09 |
| **Module** | Cart |
| **Test Case Title** | Set product quantity to 0 in cart |
| **Type** | Boundary |
| **Precondition** | Product is in cart |
| **Test Steps** | 1. Open Cart <br> 2. Change quantity to `0` <br> 3. Click Update |
| **Expected Result** | Error: "Quantity must be at least 1" or item removed |
| **Actual Result** | Cart accepted 0 quantity, total became ₹0 ❌ |
| **Status** | ❌ Fail |
| **Bug ID** | [BUG-004](../bug-reports/BUG-004.md) |

---

## TC10 — Add Very High Quantity (9999)

| Field | Details |
|-------|---------|
| **Test Case ID** | TC10 |
| **Module** | Cart |
| **Test Case Title** | Set product quantity to 9999 |
| **Type** | Boundary |
| **Precondition** | Product is in cart |
| **Test Steps** | 1. Open Cart <br> 2. Change quantity to `9999` <br> 3. Click Update |
| **Expected Result** | Price updates to 9999 × unit price |
| **Actual Result** | Price did not update, showed old total ❌ |
| **Status** | ❌ Fail |
| **Bug ID** | [BUG-005](../bug-reports/BUG-005.md) |

---

## TC11 — Remove Item from Cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC11 |
| **Module** | Cart |
| **Test Case Title** | Remove a product from cart |
| **Type** | Positive |
| **Precondition** | Product is in cart |
| **Test Steps** | 1. Open Cart <br> 2. Click "Remove" on a product |
| **Expected Result** | Product removed, cart total updated |
| **Actual Result** | Product removed correctly ✅ |
| **Status** | ✅ Pass |
| **Bug ID** | — |
