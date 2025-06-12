# -Task-Manager-System-CodeIgniter-4-
Task Manager System (CodeIgniter 4) A simple web-based task manager built with PHP (CodeIgniter 4), MySQL, and Bootstrap-style UI. Supports user authentication, task management, role-based access control, file uploads, and a RESTful API.


⚙️ Installation & Setup
✅ Prerequisites:
XAMPP / Apache / PHP 8.x

MySQL

Composer (for CodeIgniter dependencies)

🛠 Setup Steps:
Clone the project

bash
Copy
Edit
git clone https://github.com/your-username/taskmanager.git
Move the project to your XAMPP htdocs folder:

makefile
Copy
Edit
C:\xampp\htdocs\taskmanager\
Create a MySQL database:

Name: taskmanager

Import the provided taskmanager.sql file in phpMyAdmin

Update the .env file:

pgsql
Copy
Edit
database.default.hostname = localhost
database.default.database = taskmanager
database.default.username = root
database.default.password =
database.default.DBDriver = MySQLi
Access the system in your browser:

arduino
Copy
Edit
http://localhost/taskmanager/public
🔐 Default Roles
Role	Permissions
Admin	Add, Edit, Delete, Upload
User	Add, Edit, Upload (No delete)

🔌 RESTful API Endpoints
Method	Endpoint	Description	Access
GET	/api/tasks	Get all tasks	All users
GET	/api/tasks/{id}	Get task by ID	All users
POST	/api/tasks	Create task	Logged in
PUT	/api/tasks/{id}	Update task	Logged in

⚠️ API requests use session-based authentication. For full protection, you can add API tokens later.

📤 File Uploads
Supported types: .jpg, .jpeg, .png, .pdf

Max size: 2 MB

Files stored in: writable/uploads/

📷 Screenshots (optional)
Add screenshots of:

Login Page

Dashboard

Upload Section

API response (JSON in browser)

👤 Author
Your Name
GitHub Profile

📄 License
MIT License (or your preferred license)
