# 📝 Flask To-Do List API

This is a simple RESTful API built with Flask for managing a To-Do list. It supports CRUD operations: Create, Read, Update, and Delete to-do items. Data is stored in memory using Python lists and dictionaries.

---

## 🚀 Features

- Get all to-do items
- Get a specific item by ID
- Add a new item
- Update an existing item
- Delete an item
- Test all endpoints easily using Postman

---

## 🛠️ Requirements

- Python 3.6+
- Flask

Install Flask using pip if you haven't:

```bash
pip install Flask
```
By default, the server will run at:
http://127.0.0.1:5000/

##📬 API Endpoints
###1. GET all items
URL: /items

Method: GET

Response: List of all to-do items.

###2. GET item by ID
URL: /items/<id>

Method: GET

Response: A specific item or error message.

###3. POST a new item
URL: /items

Method: POST

Body: JSON
``
{
  "name": "New Item",
  "description": "Details about the item"
}
``
Response: Updated list of items.

###4. PUT (update) an item
URL: ``/items/<id>``

Method: PUT

Body: JSON

json
``
{
  "name": "Updated Name",
  "description": "Updated description"
}``
Response: Updated item.

###5. DELETE an item
URL: ``/items/<id>``

Method: DELETE

Response: Message confirming deletion.

##🧪 Testing with Postman
You can use Postman to test all API routes:

Open Postman.

Set the method (GET, POST, PUT, DELETE).

Enter the URL (e.g., http://127.0.0.1:5000/items/1).

For POST/PUT, switch to the Body tab > raw > JSON, and provide the data.

Hit Send to see the result.

##📌 Notes
This app stores data in memory; all changes will be lost once the server restarts.

For persistent storage, consider using a database like SQLite, PostgreSQL, or MongoDB.

