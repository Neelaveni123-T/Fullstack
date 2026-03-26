# Flask Feedback App

A simple Flask application with user authentication and feedback system.

## Features

- User registration and login
- Feedback submission and display
- Modern responsive UI
- MongoDB database integration

## Local Development

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Start MongoDB:
   ```bash
   mongod --dbpath /path/to/your/db
   ```

3. Run the application:
   ```bash
   python app.py
   ```

4. Open http://localhost:5000

## Default Login

- Username: `admin`
- Password: `1234`

## Deployment on Render

1. Push your code to a Git repository
2. Connect your repository to Render
3. Render will automatically detect the `render.yaml` configuration
4. Set up the following environment variables in Render:
   - `MONGODB_URI`: Your MongoDB connection string
   - `DB_NAME`: Your database name (default: `flask_db`)
   - `SECRET_KEY`: Your Flask secret key (Render can generate this)

## Environment Variables

- `SECRET_KEY`: Flask secret key for sessions
- `MONGODB_URI`: MongoDB connection string
- `DB_NAME`: Database name
- `PORT`: Port number (default: 5000)

## Project Structure

```
├── app.py              # Main Flask application
├── requirements.txt    # Python dependencies
├── render.yaml         # Render configuration
├── templates/          # HTML templates
│   ├── landing.html    # Landing page
│   ├── logni.html      # Login page
│   ├── register.html   # Registration page
│   └── feedback.html   # Feedback page
└── README.md           # This file
```
