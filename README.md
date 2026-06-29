🦀 Rust Rhai API

A Rust project demonstrating how to build APIs using Actix Web while executing business logic dynamically with the Rhai scripting engine.

Instead of hardcoding calculations directly into Rust, this project loads logic from external .rhai scripts, making the application more flexible and easier to extend.

⸻

✨ Features

* Build REST APIs using Actix Web
* Execute dynamic logic using Rhai scripts
* Separate application logic from Rust code
* URL parameter handling
* Perform arithmetic operations through API endpoints
* Fast and lightweight backend architecture

⸻

🚀 Project Overview

This application receives API requests, extracts input values, executes Rhai scripts, and returns results.

Workflow:

Client Request
      ↓
Actix Web API
      ↓
Extract Route Parameters
      ↓
Pass Values to Rhai Engine
      ↓
Execute Script File
      ↓
Return Response

⸻

🛠 Tech Stack

* Rust 🦀
* Actix Web
* Rhai
* Tokio

⸻

📦 Dependencies

[dependencies]
actix-web = "4"
rhai = "1"
tokio = { version = "1", features = ["full"] }

⸻

💻 API Endpoints

Multiply Numbers

GET /multiply/{num1}/{num2}

Example:

http://127.0.0.1:8080/multiply/5/6

Response:

30

⸻

Add Numbers

GET /add/{num1}/{num2}

Example:

http://127.0.0.1:8080/add/10/20

Response:

30

⸻

💻 Project Structure

Rust-Rhai-API
│
├── src
│   ├── main.rs
│   ├── add.rhai
│   └── multiply.rhai
│
├── Cargo.toml
├── Cargo.lock
├── README.md
└── .gitignore

⸻

▶ Getting Started

Clone the repository:

git clone https://github.com/Hellboy28D/Rust-Rhai-API.git

Move into the project:

cd Rust-Rhai-API

Run the application:

cargo run

Server starts on:

http://127.0.0.1:8080

⸻

🎯 Learning Goals

This project helped me understand:

✅ Building REST APIs with Actix Web
✅ Route parameter extraction
✅ Dynamic scripting using Rhai
✅ Separating logic from application code
✅ Request-response flow in backend systems
✅ Rust ecosystem tooling

⸻

🚀 Future Improvements

* Add subtraction and division endpoints
* Add error handling for invalid inputs
* Load scripts dynamically from folders
* Add authentication
* Support custom user scripts
* Docker deployment support

⸻

Built with 🦀 + APIs + scripting + curiosity
