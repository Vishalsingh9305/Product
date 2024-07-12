# Product-SaveForLater

## Objective

The objective of this assessment is to work with ReST APIs, understand asynchronous programming, and build interactive web pages using JavaScript.

## Instructions

### HTML Structure

Create two sections/lists in your HTML page:

- **Products:** To display the list of products.
- **Save for Later:** To display the list of saved items.

### JavaScript Functions

Create the following functions in `public/js/script.js`:

#### `getProducts()`

Fetch products from `http://localhost:3000/products`. Populate them in the DOM under `<ul id="products">`. Return a promise with the JSON response from the API.

#### `getsaveforlater()`

Fetch saved items from `http://localhost:3000/saveforlater`. Populate them in the DOM under `<ul id="save-for-later">`. Return a promise with the JSON response from the API.

#### `addsaveforlater(id)`

Click event handler for the "Add to Save for Later" button corresponding to each product. Take the id of a product as input, copy the respective product to the "Save for Later" section. Post the product to `db.json` via `http://localhost:3000/saveforlater`. Return a promise with the complete list of saved items loaded on the page.

#### `deletesaveforlater(id)`

Function to delete a product from the save for later list by passing the id.

## Running the Project

1. **Start the JSON server:**
   ```bash
   json-server --watch db.json --port 3000
2. **Start a html file**
