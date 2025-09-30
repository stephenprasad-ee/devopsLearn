# Welcome to the Steve's FastAPI CRUD API! with Swagger built-in!

# Instructions to work with the app:

# Use the following command to execute uvicorn locally with reload option:

# > uvicorn app:app --reload

# Use the following command to execute tests:

# > pytest test_app.py --disable-warnings -v


## Available Endpoints:

1. Health Check
   GET /health
   Returns the health status of the API with timestamp.

2. Create Item
   POST /items/
   
   JSON Body Example:
   
   {
   "name": "Sample Item",
   "description": "A description",
   "price": 10.5,
   "quantity": 2
   }

4. List All Items
   GET /items/
   
   Returns a list of all items.

6. Get Item by ID
   GET /items/{item_id}
   
   Replace {item_id} with the integer ID of the item.

7. Update Item by ID
   PUT /items/{item_id}
   
   JSON Body Example:
   
   {
   "name": "Updated Item",
   "description": "Updated description",
   "price": 15.0,
   "quantity": 3
   }

8. Delete Item by ID
   DELETE /items/{item_id}
   
   Replace {item_id} with the integer ID of the item.
