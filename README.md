# 🌾 Cropalytix

**An AI-powered smart agriculture platform for Pakistani farmers.**

Cropalytix brings crop disease detection, an Urdu voice assistant, live weather advisory, and mandi (market) price tracking together in one easy-to-use web platform, so farmers can make faster, better-informed decisions about their crops.

> Final Year Project · Department of Computer Science · University of Central Punjab (UCP), Lahore

---

## 👥 Project Team

| Name | Roll No. |
|---|---|
| Muhammad Abdullah | L1F23BSCS0328 |
| Muhammad Freed Alam | L1F23BSCS0337 |
| Nida Mukhtar | L1F23BSCS1127 |

**Project Advisor:** Mr. Numan Aslam

---

## ✨ Features

- **🍃 Crop Disease Detection** – Upload a leaf photo and get a likely diagnosis, severity, and treatment guidance from a CNN trained on the PlantVillage dataset.
- **🎙️ Urdu Voice Assistant** – Ask questions by speaking in Urdu or English and hear the answer back, with no typing needed.
- **⛅ Weather Advisory** – Live forecast for the farmer's location with plain-language farming advice on spraying, irrigation, and harvest timing.
- **🏷️ Mandi Price Feed** – Track crop rates across markets before deciding where to sell.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React.js |
| Backend | Flask (Python), Node.js / Express |
| Database | MongoDB |
| Auth & Storage | Firebase |
| ML Model | Convolutional Neural Network (CNN), PlantVillage dataset |
| Weather Data | OpenWeather API |
| Methodology | Agile (iterative sprints) |

---

## 📁 Repository Structure

```
cropalytix/
├── prototype/      # Clickable farming-themed UI prototype (HTML/CSS/JS)
├── frontend/       # React web application
├── backend/        # Flask / Express APIs, database and Firebase config
├── ml-model/       # CNN training notebooks and scripts
├── docs/           # IEEE research paper, slides, diagrams, project documents
├── .gitignore
└── README.md
```

---

## 🚀 Getting Started

### Run the UI prototype

The prototype needs no backend, database, or dataset.

```bash
cd prototype
# Option 1: simply open index.html in Chrome or Edge
# Option 2: serve it locally
python3 -m http.server 8000
# then visit http://localhost:8000
```

**What's live vs. simulated in the prototype:**

| Module | Status |
|---|---|
| Weather Advisory | Live (Open-Meteo API, no key required) |
| Voice Assistant | Live (browser Web Speech API) |
| Disease Detection | Simulated until the trained CNN is connected |
| Mandi Prices | Simulated until a market-data API is connected |

### Run the full application *(coming soon)*

```bash
# Backend
cd backend
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
python app.py

# Frontend
cd frontend
npm install
npm start
```

### Environment variables

Create a `.env` file in `backend/` (never commit this file):

```
OPENWEATHER_API_KEY=your_key_here
MONGODB_URI=your_connection_string
FIREBASE_CONFIG=path_to_your_firebase_config
```

---

## 🗺️ Roadmap

- [x] UI prototype with farming-themed design
- [x] IEEE-format research paper
- [ ] Train CNN on the PlantVillage dataset
- [ ] Connect the model to the Flask inference endpoint
- [ ] Integrate MongoDB and Firebase authentication
- [ ] Connect a live mandi price data source
- [ ] Offline / low-bandwidth mode
- [ ] Field testing with real farmers

---

## 🤝 Contributing

1. Create a branch: `git checkout -b feature/your-feature-name`
2. Commit your changes: `git commit -m "Add your feature"`
3. Push the branch: `git push origin feature/your-feature-name`
4. Open a Pull Request into `main`

---

## 📄 License

This project was developed for academic purposes as a Final Year Project at the University of Central Punjab.

---

<p align="center">Built with 🌱 for Pakistan's farmers</p>
