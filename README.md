# 🗨️ ChatterBox

ChatterBox is a simple chat application designed to smooth Communication betweeen users with the help of Docker Compose, Nginx, Node.js, and PostgreSQL. It includes numbers of tables such as user registration, login with JWT-based authentication, and real-time-style chat message handling.

---

Chaticus/
├── Backend/          # Node.js + Express backendAPI +sql+package.json    + server.json
├── Frontend/         # Static HTML/CSS/JS frontend served by Nginx
├── Database/         # SQL files for initial database schema and content
├── .env              # Environment variables for PostgreSQL and pgAdmin
└── docker-compose.yml


---

# 🚀 How to Run It

>  Make sure [Docker Desktop] is running.

1. Open a terminal in the `ChatterBox` folder.
2. Run: docker-compose up--build

To *reset the database* (drops data and reloads SQL):
docker-compose down --volumes
docker-compose build --no-cache
docker-compose up


---

# 🌐 App Features

- ✅ User registration and login (secure password hashing with bcrypt)
- ✅ JWT-based token authentication
- ✅ PostgreSQL multi-table schema: 'users', 'messages'
- ✅ Message posting & retrieval with timestamps
- ✅ Fully containerized architecture using Docker Compose
- ✅ Custom Nginx reverse proxy config

| Component | URL                       |
|----------|----------------------------|
| Frontend | http://localhost:8080      |
| Backend  | http://localhost:3000/chat |
| pgAdmin  | http://localhost:5050      |

---

# 🛠️ Technologies Used

- **Frontend**: HTML, CSS, Vanilla JS
- **Backend**: Node.js, Express
- **Database**: PostgreSQL
- **Other**: Docker, Docker Compose, pgAdmin, bcrypt, jsonwebtoken

---

# 📝 Credentials (Default)

- pgAdmin: `admin@chaticus.com` / `admin`
- PostgreSQL DB: `chaticus`, user: `postgres`, password from `.env`

---

# 📬 API Endpoints

- `POST /api/register` – Register a user
- `POST /api/login` – Login and get JWT token
- `POST /api/messages` – Post a chat message (auth required)
- `GET  /api/messages` – Get all chat messages

---

# 🧪 Sample Data

Loaded via `Database/001_content.sql`:
- 1 user account
- 3 sample messages

---
# 👾 Errors v/s Expectations 

- I faced lot of errors , firstly when i was edited my all files after that i faced backend crash , i was able to solve that issue but i was stuck at the last part and it was show me previous data in all files.
- Next i was faced when i was run the command then in docker file when i was click my application i was not found my backend port number.
- After struggle with lot of errors finally i was open my multiple application.
- I expected it to be simple to a multitable website which will have a login system and ausers interface which will save chats according to user id.


THANKS 
---------------------------------------------------------------------------
