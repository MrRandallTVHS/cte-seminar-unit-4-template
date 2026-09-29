# Test Cases

Run and document each test after the microservices and orchestrator are running.

## Test 1: Update Inventory

Begin with 5 units of `Laptop` in inventory. The command below adds 5 more
units, so the resulting stock should be 10.

Example command:

```text
curl -X PUT http://localhost:5001/inventory/Laptop -H "Content-Type: application/json" -d "{\"quantity\": 5}"
```

Expected response format:

```text
{"message":"Laptop stock updated."}
```

## Test 2: Check Inventory

Example command:

```text
curl -X GET http://localhost:5001/inventory/Laptop
```

Expected response format:

```text
{"item":"Laptop","stock":10}
```

## Test 3: Process Payment

Example command:

```text
curl -X POST http://localhost:5000/checkout -H "Content-Type: application/json" -d "{\"item\":\"Laptop\",\"quantity\":2,\"method\":\"credit_card\",\"amount\":2000}"
```

Expected response format:

```text
{"message":"Processed 2000 via Credit Card."}
```
