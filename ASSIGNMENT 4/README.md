# FastAPI Internship — Assignment 4

Cart System Implementation

## Overview

This assignment implements a complete shopping cart system using FastAPI.
The API supports adding items to the cart, viewing cart contents, removing items, and performing checkout operations.

All endpoints were tested using Swagger UI.

## Features Implemented

### Q1 — Add Items to Cart

Endpoint: POST /cart/add

Products Added:

* Wireless Mouse (qty 2)
* Notebook (qty 1)

Subtotal calculations verified.

### Q2 — View Cart

Endpoint: GET /cart

Cart response includes:

* items list
* item_count
* grand_total

Grand total verified manually.

### Q3 — Error Handling

Tested cases:

* Adding out-of-stock product (USB Hub) → 400 error
* Adding invalid product id → 404 error

### Q4 — Update Existing Cart Item

Adding the same product again updates quantity instead of creating duplicates.

Example:
Wireless Mouse quantity updated to 3.

### Q5 — Remove and Checkout Flow

Steps completed:

* Notebook removed from cart
* Checkout performed successfully
* Cart cleared after checkout
* Order stored in orders list

### Q6 — Multi Customer Flow

Simulated two customers placing orders sequentially.

Orders correctly recorded in GET /orders endpoint.

### Bonus — Empty Cart Checkout

Checkout with empty cart correctly returns:

400 Bad Request
CART_EMPTY

## Technologies Used

* Python
* FastAPI
* Swagger UI
* REST APIs

## Author

Submitted as part of FastAPI Internship Training — Assignment 4

