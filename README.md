# OPM-Hackathon-2025

## HSSE National Portal Web App

This is a full-stack web application for visualizing, reporting, and analyzing HSSE (Health, Safety, Security, Environment) incidents. The app includes a real-time dashboard, an AI-powered assistant, and an interactive incident map.

## 📁 Project Structure

```
├── app.py                  # Main Flask application
├── templates/
│   ├── index.html          # Dashboard interface
│   ├── map.html            # Interactive incident map page
│   ├── ai.html             # AI voice assistant UI
├── static/
│   └── uploads/            # Image upload directory
├── model/
│   └── best.pt             # YOLO model file for PPE detection
├── db/
│   └── hsse.db             # SQLite3 database with incident data
├── .env                    # Environment variables (for Gemini API)
```

## 🚀 Features

- 📊 **Dashboard**: HSSE metrics, trends, fines, construction data, news insights.
- 🧠 **Voice Assistant**: Gemini API integration for natural-language HSSE queries.
- 🗺️ **Incident Map**: Folium-based, interactive map with live markers and stats.
- 🧾 **Report Handling**: Allows incident reporting with image uploads and location data.
- 🧠 **YOLOv8 Analysis**: Detects safety gear violations (e.g., missing hard hats) in uploaded images.

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://your-repo-url.git
cd your-repo-folder
```

### 2. Create and Activate Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Add `.env` File

Create a `.env` file in the root directory:

```
GEMINI_API_KEY=your_google_gemini_api_key_here
```

### 5. Ensure Required Files Exist

- `model/best.pt` – Pretrained YOLOv8 model for object detection.
- `db/hsse.db` – SQLite database with tables: `reports`, `dashboard_metrics`, etc.
- `static/uploads/` – Folder for image uploads (auto-created if missing).

## ▶️ Run the Application

```bash
python app.py
```

Then visit:  
👉 http://127.0.0.1:5000

## 🧪 Testing the App

- Visit `/` for the dashboard  
- Visit `/map` for the incident map  
- Visit `/ai` for the voice-based assistant

## 🛠️ Built With

- **Flask** – Backend framework  
- **Jinja2** – Template rendering  
- **SQLite3** – Lightweight DB for incident storage  
- **Folium** – Map visualization  
- **YOLOv8 (Ultralytics)** – PPE violation detection  
- **Google Gemini API** – AI assistant responses  
- **Tailwind CSS** – Responsive frontend design  
- **Chart.js** – Trend chart visualization

## 📌 Notes

- Max file upload size: **50MB**
- Allowed image formats: `png`, `jpg`, `jpeg`, `gif`
- The assistant only responds based on internal/processed data – not external web info.

## References

"""
Portions of this script were generated using ChatGPT (OpenAI, 2025).
Prompt used: "Create a Flask route to handle file uploads and show a success message."
"""
**
// Code partially generated with ChatGPT (OpenAI, 2025)
// Prompt: "Create a dropdown menu that opens on hover"
This function was generated with the help of ChatGPT (OpenAI, 2025)
Prompt: "Write a Python function to scrape headlines from a news website"