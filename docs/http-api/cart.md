# Cart

#### GET /cart

- Description: Retrieves the list of CartProducts in the cart.
- Request:
  - Headers: None
  - Body: None
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Array of CartProduct objects

#### POST /cart/add

- Description: Adds a CartProduct to the cart.
- Request:
  - Headers: Content-Type: application/json
  - Body: CartProduct object
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Added CartProduct object

#### POST /cart/remove

- Description: Removes a CartProduct from the cart.
- Request:
  - Headers: Content-Type: application/json
  - Body: CartProduct object
- Response:
  - 200 OK
    - Content-Type: application/json
    - Body: Removed CartProduct object
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
