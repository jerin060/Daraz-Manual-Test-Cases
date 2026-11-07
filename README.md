<h1 align="center">🛒 Daraz – Manual Test Case Suite</h1>

<p align="center">
  Manual functional test design for the <b>Daraz</b> e-commerce website<br>
  <i>Test Scenarios · Test Cases · Test Data</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Testing-Manual-blue" alt="Manual">
  <img src="https://img.shields.io/badge/Modules-8-orange" alt="8 modules">
  <img src="https://img.shields.io/badge/Test%20Cases-72-brightgreen" alt="72 test cases">
  <img src="https://img.shields.io/badge/Tool-Excel%20%2F%20Google%20Sheets-green" alt="Excel">
</p>

---

## 📌 About
A manual testing project that designs test documentation for the main customer journey on **Daraz**: from creating an account to paying for an order. It follows the standard QA flow:

```
Test Scenario  →  Test Case  →  Test Data
(what to test)    (how to test)  (what data to use)
```

> **Scope:** test case writing only (no automation). Application under test: [Daraz](https://www.daraz.com.bd).

## 🧩 Modules Covered
| Module | What is tested |
|---|---|
| Registration | New account creation, field validation, OTP, duplicate account |
| Login | Valid / invalid login, empty fields, logout |
| Search | Keyword search, no result, filter and sort |
| Product Details | Price, description, images, variants |
| Cart | Add, remove, update quantity, voucher |
| Wishlist | Add, remove, move to cart |
| Checkout | Address, order summary |
| Payment | Payment method selection (COD, bKash, Nagad, card) |

## 📊 Test Coverage
| Module | Scenarios | Test Cases | High | Medium | Low |
|---|:-:|:-:|:-:|:-:|:-:|
| Registration | 8 | 14 | 5 | 7 | 2 |
| Login | 7 | 10 | 6 | 3 | 1 |
| Search | 5 | 9 | 2 | 4 | 3 |
| Product Details | 6 | 8 | 3 | 3 | 2 |
| Cart | 5 | 9 | 3 | 6 | 0 |
| Wishlist | 4 | 6 | 2 | 3 | 1 |
| Checkout | 5 | 8 | 3 | 5 | 0 |
| Payment | 5 | 8 | 3 | 4 | 1 |
| **Total** | **45** | **72** | **27** | **35** | **10** |

Every test case covers positive, negative or boundary behaviour. Techniques used: equivalence partitioning, boundary value analysis and error guessing.

## 📁 File Structure
```
daraz-manual-test-cases/
├── README.md
├── test-artifacts/
│   └── Daraz_Test_Cases.xlsx        # Main workbook
```

**Workbook sheets**
| Sheet | Contents |
|---|---|
| **Test Scenario** | Scenario ID, module, description, type, priority, number of test cases |
| **Test Cases** | Step, action, expected result, status, actual result, priority, scenario ID, test data ID |
| **Test Data** | Data ID, module, test case ID, field, data type (valid / invalid / boundary), value |

## 🚀 How to Use
1. Open `test-artifacts/Daraz_Test_Cases.xlsx` in Excel or Google Sheets.
2. Pick a test case and read its **Prereq.** row.
3. Get the input values from the **Test Data** sheet (use the Test Data ID).
4. Run the steps and compare the result with **Expected Result**.
5. Set **Status** (`Success`, `Failed`, `Block/Skip`) and write any difference in **Actual Result**.
6. Log each failure in new document.

## 🏷️ Conventions
| Item | Format | Example |
|---|---|---|
| Scenario | `TS-<MODULE>-<nn>` | `TS-LOG-02` |
| Test case | `TC-<MODULE>-<nn>` | `TC-CRT-02` |
| Test data | `TD-<MODULE>-<nn>` | `TD-PAY-04` |

**Priority:** `High` core flow · `Medium` validation / secondary flow · `Low` minor behaviour

## ⚠️ Notes
- Steps and expected results are based on the Daraz Bangladesh website and should be re-checked on the live site before execution, as labels, messages and payment options can change.
- All test data is dummy. Use sandbox payments and never enter real card or wallet details.

## 👩‍💻 Author
**Jarin Akther**

| | |
|---|---|
| 📧 Email | [jarinakther55@gmail.com](mailto:jarinakther55@gmail.com) |
| 💻 GitHub | https://github.com/jerin060|
| 🔗 LinkedIn | www.linkedin.com/in/jarin-akther |

<sub>Educational project. Not affiliated with or endorsed by Daraz.</sub>
