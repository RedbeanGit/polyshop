# Inventory

#### GET /products

- Description: Retrieves all InventoryProducts.
- Request:
  - Headers: None
  - Body: None
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Array of InventoryProduct objects

#### GET /products/{productId}

- Description: Retrieves a specific InventoryProduct.
- Request:
  - Headers: None
  - URL Parameters: productId
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Product object
  - 404 Not Found

#### POST /products

- Description: Creates a new InventoryProduct.
- Request:
  - Headers: Content-Type: application/json
  - Body: InventoryProduct object
- Response:
  - 201 Created
    - Content-Type: application/json
    - Body: InventoryProduct object
  - 400 Bad Request

#### PUT /products/{productId}

- Description: Updates a specific InventoryProduct.
- Request:
  - Headers: Content-Type: application/json
  - URL Parameters: productId
  - Body: InventoryProduct object
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Updated InventoryProduct object
  - 400 Bad Request
  - 404 Not Found
