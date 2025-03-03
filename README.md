# GESTION DES TACHES

GESTION DES TACHES is a simple CRUD (Create, Read, Update, Delete) application built with FASTAPI. This application allows users to manage their tasks efficiently.

## Features

- Create new tasks
- Read existing tasks
- Update task details
- Delete tasks

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/gestion-des-taches.git
   cd gestion-des-taches
Create a virtual environment and activate it:

Copy
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
Install the required dependencies:

Copy
pip install -r requirements.txt
Run the application:

Copy
uvicorn main\:app --reload
The application will be available at http://127.0.0.1:8000.

Usage
Create a new task:

Copy
POST /tasks/
Example request body:

Copy
{
  "title": "Task Title",
  "description": "Task Description",
  "completed": false
}
Read all tasks:

Copy
GET /tasks/
Read a single task:

Copy
GET /tasks/{task_id}
Update a task:

Copy
PUT /tasks/{task_id}
Example request body:

Copy
{
  "title": "Updated Task Title",
  "description": "Updated Task Description",
  "completed": true
}
Delete a task:

Copy
DELETE /tasks/{task_id}
Contributing
Contributions are welcome! Please open an issue or submit a pull request.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contact
If you have any questions or suggestions, feel free to reach out to omarbouhdiida@gmail.com.

