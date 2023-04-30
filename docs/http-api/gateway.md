# Gateway

## Cart

#### GET /cart

- Description: Retrieves the list of Products in the cart.
- Request:
  - Headers: None
  - Body: None
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Array of Product objects

#### POST /cart/add

- Description: Adds a Product to the cart.
- Request:
  - Headers: Content-Type: application/json
  - Body: Product object
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Added Product object

#### POST /cart/remove

- Description: Removes a Product from the cart.
- Request:
  - Headers: Content-Type: application/json
  - Body: Product object
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Removed Product object
  - 400 Bad Request

#### POST /cart/checkout

- Description: Orders the products currently in the cart and empties the cart.
- Request:
  - Headers: Content-Type: application/json
  - Body: None
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Boolean indicating if the cart achieved to start the command process

## Order

#### GET /orders

- Description: Retrieves the list of Orders.
- Request:
  - Headers: None
  - Body: None
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Array of Order objects

#### GET /orders/{id}

- Description: Retrieves one Order.
- Request:
  - Headers: None
  - Body: None
  - URL Parameters: id
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: One Order object.
  - 404 Not Found

#### GET /orders/{id}/products

- Description: Retrieves the list of Products in a given Order.
- Request:
  - Headers: None
  - Body: None
  - URL Parameters: id
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Array of Product objects
  - 404 Not Found

## Product

#### GET /products

- Description: Retrieves the list of Products.
- Request:
  - Headers: None
  - Body: None
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Array of Product objects

#### GET /products/{id}

- Description: Retrieves one Product.
- Request:
  - Headers: None
  - Body: None
  - URL Parameters: id
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: One Product objects

#### POST /products

- Description: Create a new Product.
- Request:
  - Headers: Content-Type: application/json
  - Body: Product object
- Response:
  - 201 OK
    - Content-Type: application/json
    - Body: Created Product object
