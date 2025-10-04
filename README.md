# Green Parking App

Eco-friendly web application for 4-wheeler parking management with admin and user functionality, developed using Flask, SQLite, HTML, CSS, and Bootstrap.

##  Project Structure

```
green_parking_app/
├── app.py
├── database.py
├── requirements.txt
├── README.md
├── openapi.yaml       
├── static/
│   └── style.css
├── templates/
│   ├── home.html
│   ├── login.html
│   ├── register.html
│   ├── admin_dashboard.html
│   ├── user_dashboard.html
│   ├── add_parking_lot.html
│   └── edit_parking_lot.html
```

##  Features

- Admin and user authentication/authorization
- Eco-friendly parking lot creation & management (admin)
- Automatic spot allocation for bikes, EVs, and cars
- Spot booking and release with green tracking (user)
- Parking cost and CO₂ savings calculations
- Green points and badge reward system
- Responsive, modern dashboard interfaces
- Display of daily eco-tips
- Optional REST API endpoints with YAML definition
- Database created and managed programmatically

##  Tech Stack

- **Backend:** Flask, SQLite3
- **Frontend:** Jinja2 (HTML templates), CSS, Bootstrap
- **APIs:** JSON (Flask), OpenAPI (YAML)
- **Database:** SQLite (auto-generated - no manual setup required)

##  Setup & Installation

### Requirements

- Python 3.8+
- pip

### Dependency Installation

From the root of your project:

```bash
pip install Flask
```

Or if you use a `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### Database

The database (`green_parking.db`) is generated automatically on first run.  
You can delete this file at any time to reset all user data and parking lots.

## ▶️ Running the Application

1. **Initialize the database** (automatic on run)
2. **Start the Flask server:**

   ```bash
   python app.py
   ```

3. **Open your browser and visit:**

   ```
   http://localhost:5000/
   ```

## 👑 Admin Access

- **Username:** admin
- **Password:** admin123

(Admin user is created automatically, no registration required.)

## 🧑‍💻 User Access

1. Register a new user via the Register link.
2. Login using your newly created credentials.

## 🔑 Core Functionalities

- **Admin Dashboard:** Create/edit/delete parking lots, see all users, view stats
- **User Dashboard:** Book or release spots (auto-allocation), see usage & green stats
- **Booking Logic:** 10% of spots for bikes, 20% for EVs, 70% for cars
- **Eco Features:** Add solar/EV/recycling options per lot; earn green points for eco parking
- **Gamification:** Green points, eco badge rewards
- **Charts & Analytics:** (if implemented) API endpoints and dashboards for stats

## 🌐 API Documentation

If you enable REST API endpoints, see your `openapi.yaml` file for specs.

Example endpoint (GET):

```
/api/parking_stats
```

## 📝 Project Notes

- No environment files (`venv`), Python bytecode, or secret files should be included in submission.
- To reset the app to default: stop the server, delete `green_parking.db`, and restart the app.
- Frontend automatically adapts to various devices thanks to responsive CSS.

## ❓ Troubleshooting

- If you encounter "database not found" errors, ensure you have write access to the folder.
- If styles don't display, make sure `style.css` is in the correct folder (`static/`).
- For any issues, restart the app and database by deleting `green_parking.db`.

## 📄 License

*For academic/Hackathon use only.*

## 🏅 Credits

Created by: **[Your Name]**  
For: Vehicle Parking App – University Mini Project.

**Enjoy using Green Parking – park with a purpose! 🌱**
