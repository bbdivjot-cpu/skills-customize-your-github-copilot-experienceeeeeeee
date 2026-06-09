# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Learn to build scalable REST APIs using the FastAPI web framework. You'll create endpoints, handle HTTP requests, validate data, and deploy a working API.

## 📝 Tasks

### 🛠️ Create Basic API Endpoints

#### Description
Set up a FastAPI application with basic CRUD endpoints that handle GET, POST, PUT, and DELETE requests.

#### Requirements
Completed program should:

- Create a FastAPI application with proper imports and initialization
- Implement GET endpoint to retrieve all items from a data store
- Implement POST endpoint to create new items
- Implement PUT endpoint to update existing items
- Implement DELETE endpoint to remove items

#### Example
```python
from fastapi import FastAPI
app = FastAPI()

@app.get("/items")
def get_items():
    return {"items": [...]}

@app.post("/items")
def create_item(item: dict):
    return {"id": 1, "item": item}
```

### 🛠️ Data Validation and Error Handling

#### Description
Add request validation using Pydantic models and implement proper error handling for invalid requests.

#### Requirements
Completed program should:

- Define Pydantic models for request/response data
- Validate incoming data automatically
- Return appropriate HTTP status codes (200, 201, 400, 404, 500)
- Handle and return meaningful error messages
- Test all endpoints with valid and invalid data

### 🛠️ Advanced Features (Stretch Goal)

#### Description
Implement advanced API features like pagination, filtering, and authentication.

#### Requirements
Completed program should:

- Implement query parameters for filtering items
- Add pagination support (limit and offset)
- (Optional) Add basic authentication or API key validation
- Document endpoints with OpenAPI/Swagger
