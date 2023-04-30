# Order

#### GET /orders

- Description: Retrieves all orders.
- Request:
  - Headers: None
  - Body: None
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Array of order objects

#### GET /orders/{orderId}

- Description: Retrieves an order with the specified ID.
- Request:
  - Headers: None
  - URL Parameters: orderId
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Order object
  - 404 Not Found

#### GET /orders/{orderId}/products

- Description: Retrieves the OrderProducts of an order with the specified ID.
- Request:
  - Headers: None
  - URL Parameters: orderId
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Array of OrderProduct objects
  - 404 Not Found
