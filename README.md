# GitHub Webhook Listener Project

This project demonstrates a simple GitHub webhook listener built using Python (Flask), MongoDB, and JavaScript frontend. It listens for GitHub push events and displays them on a live webpage.

---

## 📁 Project Structure

- `action-repo` → A sample GitHub repo to trigger push events
- `webhook-repo` → The Flask app that receives webhook data, stores it in MongoDB, and displays events on a webpage

---

## 🚀 How It Works

1. A push is made to `action-repo`
2. GitHub sends a webhook event to the Flask server via ngrok
3. Flask stores event data in MongoDB
4. The frontend (`index.html`) fetches the latest events every 15 seconds and displays them live

---

## 🔧 Tech Stack

- **Frontend:** HTML, CSS, JS
- **Backend:** Python (Flask)
- **Database:** MongoDB
- **Other:** ngrok (to expose local server), GitHub Webhooks

---

## ⚙️ How to Run

1. Clone this repo:
    ```bash
    git clone https://github.com/prity2407/webhook-repo.git
    cd webhook-repo
    ```

2. Install requirements:
    ```bash
    pip install -r requirements.txt
    ```

3. Run MongoDB (must be installed):
    ```bash
    mongod
    ```

4. Start Flask server:
    ```bash
    python app.py
    ```

5. Start ngrok (replace path with yours):
    ```bash
    ngrok http 5000
    ```

6. Add the ngrok URL to your GitHub webhook:
    ```
    https://<your-ngrok-url>/webhook
    ```

---

## 📸 Screenshot

![Preview](screenshot.png)

---

## ✅ Features

- Real-time GitHub push event capture
- MongoDB storage of webhook data
- UI auto-refreshes to show latest events

---

## 📌 Future Improvements

- Handle pull request and merge events
- Deploy Flask app to Render/Railway
- Add authentication & logging

---

## 📬 Author

**Preety Sriwastava**  
Full Stack Developer 💻  
