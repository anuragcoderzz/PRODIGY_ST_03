# Test Cases for SauceDemo E-commerce Website

## Overview
These test cases are created for the SauceDemo e-commerce website (https://www.saucedemo.com/) to verify its core functionalities: login, browsing products, adding to cart, and checkout. The test cases cover both positive and negative scenarios.

## Test Case 1: Successful Login with Valid Credentials
- **Test Case ID**: TC_01  
- **Test Description**: Verify that a user can log in successfully with valid credentials.  
- **Preconditions**: User is on the SauceDemo login page (https://www.saucedemo.com/).  
- **Test Steps**:  
  1. Enter username as "standard_user".  
  2. Enter password as "secret_sauce".  
  3. Click the "Login" button.  
- **Expected Results**: User is redirected to the products page, and the product listings are displayed.

## Test Case 2: Failed Login with Invalid Credentials
- **Test Case ID**: TC_02  
- **Test Description**: Verify that a user cannot log in with invalid credentials.  
- **Preconditions**: User is on the SauceDemo login page.  
- **Test Steps**:  
  1. Enter username as "invalid_user".  
  2. Enter password as "wrong_password".  
  3. Click the "Login" button.  
- **Expected Results**: Error message displayed: "Epic sadface: Username and password do not match any user in this service".

## Test Case 3: Browsing Products After Login
- **Test Case ID**: TC_03  
- **Test Description**: Verify that a user can browse products after logging in.  
- **Preconditions**: User is logged in and on the products page.  
- **Test Steps**:  
  1. Scroll through the product listings.  
  2. Verify that product names, descriptions, prices, and images are visible.  
- **Expected Results**: All products are displayed with their names, descriptions, prices, and images visible.

## Test Case 4: Adding Product to Cart
- **Test Case ID**: TC_04  
- **Test Description**: Verify that a user can add a product to the cart.  
- **Preconditions**: User is logged in and on the products page.  
- **Test Steps**:  
  1. Select a product (e.g., "Sauce Labs Backpack").  
  2. Click the "Add to cart" button for that product.  
  3. Click the cart icon to view the cart.  
- **Expected Results**: The selected product (e.g., "Sauce Labs Backpack") is added to the cart and visible in the cart page.

## Test Case 5: Successful Checkout with Valid Details
- **Test Case ID**: TC_05  
- **Test Description**: Verify that a user can complete the checkout process with valid details.  
- **Preconditions**: User is logged in, has added at least one product to the cart, and is on the cart page.  
- **Test Steps**:  
  1. Click the "Checkout" button.  
  2. Enter first name as "John".  
  3. Enter last name as "Doe".  
  4. Enter postal code as "12345".  
  5. Click the "Continue" button.  
  6. Review the order summary and click the "Finish" button.  
- **Expected Results**: Checkout completion page is displayed with a message: "Thank you for your order!".

## Test Case 6: Checkout with Missing Details
- **Test Case ID**: TC_06  
- **Test Description**: Verify that the checkout process fails if required details are missing.  
- **Preconditions**: User is logged in, has added at least one product to the cart, and is on the checkout information page.  
- **Test Steps**:  
  1. Leave the first name field blank.  
  2. Enter last name as "Doe".  
  3. Enter postal code as "12345".  
  4. Click the "Continue" button.  
- **Expected Results**: Error message displayed: "Error: First Name is required".