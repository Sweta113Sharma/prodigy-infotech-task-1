# 🧮 Calculator Functional & Boundary Testing

This repository contains the comprehensive **Test Suite and Verification Cases** for a standard calculator application, conducted as part of the **Prodigy InfoTech QA Internship (Task 1)**.

The objective of this task is to design detailed, structured test cases covering basic arithmetic operations, decimal math, operator precedence (BODMAS), invalid input handling, and large-value boundary scenarios.

---

## 📋 General Information

<div align="center">

![Tester](https://img.shields.io/badge/Tester-Sweta%20Kumari-ff69b4?style=flat-square&logo=github)
![Application](https://img.shields.io/badge/Application-Calculator-blue?style=flat-square)
![Test Type](https://img.shields.io/badge/Test%20Type-Functional%20%26%20Boundary%20Checks-orange?style=flat-square)
![Status](https://img.shields.io/badge/Status-Completed-success?style=flat-square)

</div>

---

## 📂 Test Suite Index

| Test Case ID | Test Scenario | Input Category | Expected Result Type |
|---|---|---|---|
| **TC_ADD_01** | Addition with Positive Numbers | Valid (Integers) | Exact Sum (`12`) |
| **TC_SUB_01** | Subtraction with Negative Result | Valid (Integers) | Negative Integer (`-5`) |
| **TC_MUL_01** | Multiplication with Decimals | Valid (Decimals) | Exact Product (`10`) |
| **TC_DIV_01** | Division by Zero | Invalid (Divide-by-zero) | Error / Block Message |
| **TC_INV_01** | Invalid Input (Non-numeric Characters) | Invalid (String symbols) | Error / Input Block |
| **TC_BODMAS_01** | BODMAS / Order of Operations | Valid (Expressions) | Correct Precedence Output (`14`) |
| **TC_DIV_02** | Division with Decimal Result | Valid (Integers) | Exact Decimal Quotient (`2.5`) |
| **TC_LARGE_01** | Large Number Calculation | Boundary (Overflow check) | Graceful Large Sum / Handling |

---

## 🧪 Detailed Test Cases

### 📥 1. Valid Input Scenarios

#### **Test Case ID:** `TC_ADD_01`
*   **Test Description:** Verify addition of two positive integers.
*   **Preconditions:** Calculator application is open and cleared.
*   **Test Steps:**
    1. Enter `5`
    2. Press the `+` operator key
    3. Enter `7`
    4. Press the `=` action key
*   **Expected Result:** The display output shows **`12`**.

#### **Test Case ID:** `TC_SUB_01`
*   **Test Description:** Verify subtraction resulting in a negative number.
*   **Preconditions:** Calculator application is open and cleared.
*   **Test Steps:**
    1. Enter `3`
    2. Press the `-` operator key
    3. Enter `8`
    4. Press the `=` action key
*   **Expected Result:** The display output shows **`-5`**.

#### **Test Case ID:** `TC_MUL_01`
*   **Test Description:** Verify multiplication of decimal numbers.
*   **Preconditions:** Calculator application is open and cleared.
*   **Test Steps:**
    1. Enter `2.5`
    2. Press the `×` operator key
    3. Enter `4`
    4. Press the `=` action key
*   **Expected Result:** The display output shows **`10`**.

#### **Test Case ID:** `TC_DIV_02`
*   **Test Description:** Verify division resulting in a decimal value.
*   **Preconditions:** Calculator application is open and cleared.
*   **Test Steps:**
    1. Enter `5`
    2. Press the `÷` operator key
    3. Enter `2`
    4. Press the `=` action key
*   **Expected Result:** The display output shows **`2.5`**.

---

### ⚠️ 2. Invalid & Edge Cases

#### **Test Case ID:** `TC_DIV_01`
*   **Test Description:** Verify division by zero handling.
*   **Preconditions:** Calculator application is open and cleared.
*   **Test Steps:**
    1. Enter `9`
    2. Press the `÷` operator key
    3. Enter `0`
    4. Press the `=` action key
*   **Expected Result:** The display shows an error message like **`"Cannot divide by zero"`** or **`"Error"`**.

#### **Test Case ID:** `TC_INV_01`
*   **Test Description:** Verify error display when trying to enter non-numeric characters.
*   **Preconditions:** Calculator application is open.
*   **Test Steps:**
    1. Attempt to enter `"abc"`
    2. Press the `+` operator key
    3. Enter `5`
    4. Press the `=` action key
*   **Expected Result:** The system blocks the alphabetical inputs, or the display shows an error message like **`"Invalid input"`** or **`"Error"`**.

---

### 🧠 3. Precedence & Boundary Scenarios

#### **Test Case ID:** `TC_BODMAS_01`
*   **Test Description:** Verify expression evaluation follows the standard BODMAS / order of operations rules.
*   **Preconditions:** Calculator application supports multi-operator expression parsing.
*   **Test Steps:**
    1. Enter `2`
    2. Press the `+` operator key
    3. Enter `3`
    4. Press the `×` operator key
    5. Enter `4`
    6. Press the `=` action key
*   **Expected Result:** The display shows **`14`** (since multiplication is evaluated before addition: `2 + (3 × 4) = 14`).

#### **Test Case ID:** `TC_LARGE_01`
*   **Test Description:** Verify handling of large number calculations to detect overflow.
*   **Preconditions:** Calculator application is open.
*   **Test Steps:**
    1. Enter `999999999`
    2. Press the `+` operator key
    3. Enter `1`
    4. Press the `=` action key
*   **Expected Result:** The display shows **`1000000000`** (or handles the large value range gracefully without crashing).
