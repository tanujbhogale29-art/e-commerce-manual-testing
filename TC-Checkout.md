# 💳 Test Cases — Checkout Module

**Module:** Checkout  
**Tester:** Tanuj Bhogale  
**Date:** March 2026

---

## TC12 — Valid Checkout

| Field | Details |
|-------|---------|
| **Test Case ID** | TC12 |
| **Module** | Checkout |
| **Test Case Title** | Complete checkout with valid details |
| **Type** | Positive |
| **Precondition** | User logged in, item in cart |
| **Test Steps** | 1. Go to Cart <br> 2. Click Checkout <br> 3. Enter valid address <br> 4. Enter valid card: `4111 1111 1111 1111` <br> 5. Click Place Order |
| **Expected Result** | Order placed, confirmation page shown |
| **Actual Result** | Order placed successfully ✅ |
| **Status** | ✅ Pass |
| **Bug ID** | — |

---

## TC13 — Expired Card

| Field | Details |
|-------|---------|
| **Test Case ID** | TC13 |
| **Module** | Checkout |
| **Test Case Title** | Checkout with expired credit card |
| **Type** | Negative |
| **Precondition** | Item in cart |
| **Test Steps** | 1. Go to Checkout <br> 2. Enter valid address <br> 3. Enter expired card with past date: `01/22` <br> 4. Click Place Order |
| **Expected Result** | Error: "Card is expired. Please use a valid card." |
| **Actual Result** | Order placed without any validation ❌ |
| **Status** | ❌ Fail |
| **Bug ID** | [BUG-007](../bug-reports/BUG-007.md) |

---

## TC14 — Empty Address Field

| Field | Details |
|-------|---------|
| **Test Case ID** | TC14 |
| **Module** | Checkout |
| **Test Case Title** | Checkout with empty delivery address |
| **Type** | Negative |
| **Precondition** | Item in cart |
| **Test Steps** | 1. Go to Checkout <br> 2. Leave address field blank <br> 3. Enter valid card <br> 4. Click Place Order |
| **Expected Result** | Validation error: "Address is required" |
| **Actual Result** | Confirmation page showed wrong/empty address ❌ |
| **Status** | ❌ Fail |
| **Bug ID** | [BUG-008](../bug-reports/BUG-008.md) |

---

## TC15 — Checkout with Empty Cart

| Field | Details |
|-------|---------|
| **Test Case ID** | TC15 |
| **Module** | Checkout |
| **Test Case Title** | Place order with empty cart |
| **Type** | Negative |
| **Precondition** | Cart is empty |
| **Test Steps** | 1. Empty the cart <br> 2. Navigate to `/checkout` directly via URL <br> 3. Click Place Order |
| **Expected Result** | Error: "Your cart is empty" or redirect to cart page |
| **Actual Result** | Order placed with ₹0 total ❌ |
| **Status** | ❌ Fail |
| **Bug ID** | [BUG-006](../bug-reports/BUG-006.md) |
