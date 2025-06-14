📦 Flask Inventory CRUD App

This is a simple web application that allows users to manage inventory items. Built with Flask, SQLAlchemy, MySQL, Docker, and styled using Bootstrap 5, it enables full CRUD (Create, Read, Update, Delete) operations with a clean UI.
🚀 Features

    View all inventory items

    Add new items

    Edit existing items

    Delete items

    Responsive and minimal Bootstrap UI

    Dockerized with MySQL integration

🧱 Tech Stack

    Backend: Python, Flask, SQLAlchemy

    Frontend: Jinja2, HTML5, Bootstrap 5

    Database: MySQL 8.0

    Containerization: Docker & Docker Compose

📁 Project Structure

flaskinventory/
├── app/
│   ├── __init__.py         # App factory & DB setup
│   ├── models.py           # SQLAlchemy model for Inventory
│   ├── routes.py           # Flask routes (CRUD logic)
│   ├── templates/          # HTML templates (Jinja2)
│   │   ├── base.html
│   │   ├── index.html
│   │   ├── add.html
│   │   └── edit.html
├── app.py                  # Entrypoint for the app
├── Dockerfile              # Docker config for Flask app
├── docker-compose.yml      # Defines Flask & MySQL services
├── requirements.txt        # Python dependencies
└── README.md               # You're reading it!

⚙️ Requirements

    Python 3.x

    Docker + Docker Compose

🧪 How to Run (Docker)

    Clone the repository

git clone https://github.com/your-username/flaskinventory.git
cd flaskinventory

Build and start the containers

    docker-compose up --build

    Access the app
    Visit: http://localhost:5000

🗄️ Database Schema: Inventory
Field	Type	Notes
id	Integer	Primary Key (Auto)
name	String(80)	Required
price	Float	Required
mac_address	String(17)	Unique, Required
serial_number	String(50)	Unique, Required
manufacturer	String(50)	Required
description	Text	Optional
🔗 Routes
Route	Description
/	List all inventory items
/add	Add a new item
/edit/<int:id>	Edit an existing item
/delete/<int:id>	Delete an item
📸 UI Screenshots

    (Optional – Add screenshots if submitting or posting on GitHub)

📃 License

This project is provided for educational purposes as part of a technical test.
