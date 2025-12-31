# Bug Report Samples – Sauce Demo (https://www.saucedemo.com)

> Note: These are sample bug reports created for portfolio demonstration purposes
using a public demo application and fictional data.

---

## BUG-001 – Login error message does not clearly indicate which field is missing
**ID:** BUG-001  
**Title:** Login validation message is unclear when username and password are both blank  
**Environment:** Web | Desktop | Chrome  
**Severity:** Medium  
**Priority:** Medium  
**Preconditions:** User is on login page

**Steps to Reproduce:**
1. Navigate to https://www.saucedemo.com
2. Leave Username blank
3. Leave Password blank
4. Click **Login**

**Expected Result:**
A clear message should display indicating both username and password are required
(or indicate all missing required fields).

**Actual Result:**
A generic validation message displays that does not clearly communicate all missing fields
(only one field requirement is implied).

**Notes:**
Usability improvement: clearer messaging reduces confusion and re-attempts.

---

## BUG-002 – Cart badge count does not immediately update after rapid add/remove actions
**ID:** BUG-002  
**Title:** Cart badge count may not reflect accurate item count after rapid add/remove clicks  
**Environment:** Web | Desktop | Firefox  
**Severity:** Low  
**Priority:** Low  
**Preconditions:** User is logged in on Products page

**Steps to Reproduce:**
1. Login with valid credentials
2. On Products page, rapidly click **Add to cart** then **Remove** on the same item multiple times
3. Observe cart badge count

**Expected Result:**
Cart badge should consistently reflect the current number of items in the cart.

**Actual Result:**
Cart badge may appear inconsistent (briefly shows incorrect count) before updating.

**Notes:**
This may be related to UI refresh timing/state sync.

---

## BUG-003 – Checkout required-field error is not visually prominent
**ID:** BUG-003  
**Title:** Checkout error message is easy to miss when a required field is blank  
**Environment:** Web | Desktop | Chrome  
**Severity:** Low  
**Priority:** Medium  
**Preconditions:** At leas

