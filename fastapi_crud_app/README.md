## Welcome to the Steve's FastAPI CRUD API! with Swagger built-in!
---
# Instructions to work with the app:

# Use the following command to execute uvicorn locally with reload option:

# > uvicorn app:app --reload

# Use the following command to execute tests:

# > pytest test_app.py --disable-warnings -v
---
Use - /docs to access the swagger interface when the app is running
---

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

3. List All Items
   
   GET /items/
   
   Returns a list of all items.

4. Get Item by ID
   
   GET /items/{item_id}
   
   Replace {item_id} with the integer ID of the item.

5. Update Item by ID
   
   PUT /items/{item_id}
   
   JSON Body Example:
   
   {
   "name": "Updated Item",
   "description": "Updated description",
   "price": 15.0,
   "quantity": 3
   }

6. Delete Item by ID

---

Note: If anyone wants to try running this locally, please use "pip install" to install the following dependencies:
fastapi
uvicorn
python-json-logger
pytest
httpx

   DELETE /items/{item_id}
   
   Replace {item_id} with the integer ID of the item.
