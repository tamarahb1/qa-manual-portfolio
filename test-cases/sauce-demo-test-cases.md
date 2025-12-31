# Manual Test Cases – Sauce Demo (https://www.saucedemo.com)

## Test Data
- Valid user: standard_user
- Password: secret_sauce
- Invalid user: invalid_user
- Invalid password: wrong_password

---

### TC-001 – Valid Login
**Preconditions:** User is on login page  
**Steps:**
1. Enter username: standard_user
2. Enter password: secret_sauce
3. Click Login  
**Expected Result:** User is redirected to the Products page.

---

### TC-002 – Invalid Login (Wrong Credentials)
**Preconditions:** User is on login page  
**Steps:**
1. Enter username: invalid_user
2. Enter password: wrong_password
3. Click Login  
**Expected Result:** Error message is displayed and user remains on login page.

---

### TC-003 – Login Required Validation
**Preconditions:** User is on login page  
**Steps:**
1. Leave username blank
2. Leave password blank
3. Click Login  
**Expected Result:** Validation error is displayed (username required).

---

### TC-004 – Logout
**Preconditions:** User is logged in on Products page  
**Steps:**
1. Open menu (hamburger icon)
2. Click Logout  
**Expected Result:** User is logged out and returned to login page.

---

### TC-005 – Products Page Loads Successfully
**Preconditions:** User is logged in  
**Steps:**
1. Observe Products page content  
**Expected Result:** Product list is visible with item names, prices, and Add to cart buttons.

---

### TC-006 – Add Single Item to Cart (From Products Page)
**Preconditions:** User is logged in on Products page  
**Steps:**
1. Click “Add to cart” on any product  
**Expected Result:** Button changes to “Remove” and cart badge shows 1.

---

### TC-007 – Remove Item from Products Page
**Preconditions:** One item added to cart  
**Steps:**
1. Click “Remove” on the same product  
**Expected Result:** Button changes back to “Add to cart” and cart badge updates.

---

### TC-008 – Cart Badge Updates with Multiple Items
**Preconditions:** User is logged in  
**Steps:**
1. Add 2 different items to cart  
**Expected Result:** Cart badge displays 2.

---

### TC-009 – View Cart Page
**Preconditions:** User is logged in  
**Steps:**
1. Click the cart icon  
**Expected Result:** Cart page loads showing selected items.

---

### TC-010 – Remove Item from Cart Page
**Preconditions:** At least one item in cart  
**Steps:**
1. Go to cart page
2. Click Remove on an item  
**Expected Result:** Item is removed from cart and cart list updates.

---

### TC-011 – Continue Shopping from Cart
**Preconditions:** User is on cart page  
**Steps:**
1. Click “Continue Shopping”  
**Expected Result:** User is returned to Products page.

---

### TC-012 – Start Checkout
**Preconditions:** At least one item in cart  
**Steps:**
1. Go to cart page
2. Click Checkout  
**Expected Result:** Checkout: Your Information page is displayed.

---

### TC-013 – Checkout Info Required Field Validation
**Preconditions:** User is on Checkout: Your Information page  
**Steps:**
1. Leave First Name blank
2. Enter Last Name and Zip
3. Click Continue  
**Expected Result:** Error message displays indicating First Name is required.

---

### TC-014 – Complete Checkout Flow Successfully
**Preconditions:** At least one item in cart; user on Checkout: Your Information page  
**Steps:**
1. Enter First Name, Last Name, Zip
2. Click Continue
3. Verify Checkout Overview page loads
4. Click Finish  
**Expected Result:** Confirmation page displays “Thank you for your order!”

---

### TC-015 – Checkout Cancel (Overview Page)
**Preconditions:** User is on Checkout Overview page  
**Steps:**
1. Click Cancel  
**Expected Result:** User returns to Products page and cart remains unchanged.
