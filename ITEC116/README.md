# FastAPI Development Labs  

This repository contains five lab activities demonstrating API development using FastAPI. Each folder corresponds to a specific activity, covering fundamental concepts such as API functionality, authentication, and versioning.  

## Lab Activities  

### 1. Factorial API  

**Overview:**  
Developed a simple API to compute the factorial of a given number using FastAPI.  

- Implemented a loop-based factorial calculation.  
- **Endpoint:** `/factorial/{number}`  
- If the input was 0, the API returned `{ "result": false }`.  
- Gained experience in handling dynamic URL parameters.  

### 2. To-Do List API  

**Overview:**  
Implemented a CRUD-based API to manage a to-do list, utilizing HTTP methods like GET, POST, PATCH, and DELETE.  

- Created a dictionary-based task management system.  
- **Endpoints:**  
  - `GET /tasks/{task_id}` → Retrieve a task.  
  - `POST /tasks` → Add a new task.  
  - `PATCH /tasks/{task_id}` → Update a task.  
  - `DELETE /tasks/{task_id}` → Remove a task.  
- Practiced request validation, response formatting, and HTTP method usage.  

### 3. JSON Handling API  

**Overview:**  
Focused on processing and structuring JSON data within an API.  

- Implemented an API to fetch user posts along with related comments.  
- **Endpoint:** `GET /detailed_post/{userID}`  
- Retrieved and structured nested JSON responses effectively.  

### 4. API Versioning & Authentication  

**Overview:**  
Explored API versioning, authentication mechanisms, and error handling.  

- Implemented multiple API versions for improved maintainability.  
- Added API key authentication using environment variables.  
- **Error Handling:**  
  - `404 Not Found` → When a requested task is missing.  
  - `201 Created` → When a new task is successfully added.  
  - `204 No Content` → When a task is updated or deleted.  
- Applied best practices for securing and structuring API responses.  

### 5. API Deployment  

**Overview:**  
Deployed the API to a cloud platform (Render) and ensured its functionality in a live environment.  

- Successfully deployed the Lab 4 API on Render.  
- Implemented API key authentication for security.  
- **Deployed API:**  
  - Hosted at `itec116_<surname>.onrender.com`.  
  - Configured authentication using environment variables.  

## Setup Instructions  

1. Install dependencies:  
   ```sh
   pip install fastapi uvicorn python-dotenv
   ```  
2. Navigate to the desired activity folder.  
3. Run the FastAPI server:  
   ```sh
   uvicorn main:app --reload
   ```  
4. Access API documentation:  
   - [Swagger UI](http://127.0.0.1:8000/docs)  

**Localhost:** `127.0.0.1`
