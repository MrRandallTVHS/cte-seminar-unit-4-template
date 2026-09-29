# Service Contracts

These contracts define the minimum behavior expected from the Task 2 services. Students may choose the internal implementation, but the required endpoints and response purpose should remain clear and consistent.

## Inventory Service

Run on port `5001`.

For the required test sequence, initialize the service with 5 units of
`Laptop`. This makes the inventory update test produce a stock total of 10
after 5 additional units are added.

### Update Stock

- Method: `PUT`
- Path: `/inventory/<item>`
- JSON body: `{ "quantity": number }`
- Purpose: Add the specified quantity to the item's stock.

### Check Stock

- Method: `GET`
- Path: `/inventory/<item>`
- Purpose: Return the item name and current stock.

## Payment Service

The payment service should provide a clear operation for processing a payment. It should accept an amount and payment method and return a success or error response.

## Cart Service

The cart service should provide a clear operation for adding an item and quantity to a cart. It should return a success or error response and should not directly own inventory or payment logic.

## Orchestrator

Run the checkout entry point on port `5000`.

### Checkout

- Method: `POST`
- Path: `/checkout`
- JSON body: `{ "item": "Laptop", "quantity": 2, "method": "credit_card", "amount": 2000 }`
- Purpose: Coordinate the required service calls and return the overall result.

The orchestrator should coordinate the workflow. It should not duplicate all of the business logic from the individual services.
