# Catalog

#### GET /products

- Description: Retrieves the list of all CatalogProducts in the catalog.
- Request:
  - Headers: None
  - Body: None
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Array of CatalogProduct objects

#### GET /products/{productId}

- Description: Retrieves a CatalogProduct with the specified ID.
- Request:
  - Headers: None
  - URL Parameters: productId
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: CatalogProduct object
  - 404 Not Found

#### POST /products

- Description: Creates a new CatalogProduct.
- Request:
  - Headers: Content-Type: application/json
  - Body: CatalogProduct object
- Response:
  - 201 Created
    - Content-Type: application/json
    - Body: CatalogProduct object
  - 400 Bad Request
