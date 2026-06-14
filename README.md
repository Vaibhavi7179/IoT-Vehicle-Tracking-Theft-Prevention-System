# 🚗 IoT Vehicle Tracking & Theft Prevention System

An intelligent software-based IoT Vehicle Tracking & Theft Prevention System developed using Python, Streamlit, Folium, Geopy, and ReportLab. This project simulates real-time GPS tracking, geofencing, vehicle monitoring, theft detection, alert generation, and location history analytics through an interactive dashboard.

---

## 📌 Project Overview

Vehicle theft remains a major concern worldwide. This project provides a smart solution that continuously tracks vehicle movement, monitors geofenced areas, and generates theft alerts whenever the vehicle leaves a predefined safe zone.

The system simulates GPS data and visualizes vehicle movement on an interactive map while maintaining historical logs and generating reports.

---

## ✨ Features

### 🚗 Vehicle Tracking
- Real-time GPS location simulation
- Continuous vehicle movement monitoring
- Google Maps integration

### 📍 Geofencing
- Define safe vehicle zones
- Monitor vehicle boundaries
- Detect unauthorized movement

### 🚨 Theft Detection
- Automatic theft alerts
- Out-of-zone notifications
- Real-time monitoring

### 📊 Dashboard
- Live vehicle status
- Interactive Folium maps
- Current location display
- Location history table

### 📄 Reporting
- CSV log generation
- PDF report generation
- Vehicle movement history

---

## 🛠️ Technology Stack

| Technology | Purpose |
|------------|----------|
| Python | Core Development |
| Streamlit | Dashboard |
| Folium | Interactive Maps |
| Geopy | Distance Calculation |
| Pandas | Data Processing |
| ReportLab | PDF Reports |
| CSV | Data Storage |

---

## 📂 Project Structure

```text
IoT-Vehicle-Tracking-Theft-Prevention-System/
│
├── main.py
├── requirements.txt
│
├── python_simulation/
│   ├── gps_simulator.py
│   ├── geofence.py
│   ├── alerts.py
│   └── logger.py
│
├── dashboard/
│   └── app.py
│
├── data/
│   └── location_history.csv
│
└── reports/
    └── generate_report.py
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/IoT-Vehicle-Tracking-Theft-Prevention-System.git
```

### Navigate to Project

```bash
cd IoT-Vehicle-Tracking-Theft-Prevention-System
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Project

### Start Vehicle Tracking

```bash
python main.py
```

This will:

- Simulate GPS coordinates
- Track vehicle movement
- Detect geofence violations
- Generate alerts
- Save data to CSV
- Generate PDF reports

---

### Launch Dashboard

```bash
cd dashboard

python -m streamlit run app.py
```

Dashboard URL:

```text
http://localhost:8501
```

---

## 📍 Geofence Configuration

Modify the safe zone in:

```python
SAFE_LOCATION = (19.0760, 72.8777)

SAFE_RADIUS = 200
```

Where:

- SAFE_LOCATION = Center of geofence
- SAFE_RADIUS = Allowed distance in meters

---

## 🚨 Theft Detection Logic

The system continuously calculates the distance between:

- Safe Location
- Current Vehicle Location

If:

```python
distance > SAFE_RADIUS
```

Then:

```text
THEFT ALERT GENERATED
```

---

## 📊 Dashboard Preview

Features:

- Vehicle Status
- Current Coordinates
- Interactive Map
- Theft Alerts
- Location History
- Real-Time Monitoring

---

## 📄 Generated Reports

### CSV Report

Stores:

- Timestamp
- Latitude
- Longitude
- Distance
- Status
- Alert Type

### PDF Report

Contains:

- Vehicle Tracking History
- Theft Events
- Location Logs

---

## 🧪 Test Scenarios

### Scenario 1

Vehicle Parked

Expected:

```text
SAFE
```

### Scenario 2

Normal Movement

Expected:

```text
TRACKING ACTIVE
```

### Scenario 3

Vehicle Leaves Geofence

Expected:

```text
GEOFENCE ALERT
```

### Scenario 4

Vehicle Theft Simulation

Expected:

```text
THEFT DETECTED
```

---

## 📈 Future Enhancements

- ESP32 Integration
- GPS NEO-6M Module
- MQTT Communication
- Cloud Deployment
- SMS Alerts
- Mobile Application
- AI-Based Theft Prediction
- Real-Time Vehicle Immobilization

---

## 🎯 Learning Outcomes

This project demonstrates:

- Internet of Things (IoT)
- GPS Tracking Systems
- Geofencing Technology
- Data Visualization
- Python Development
- Dashboard Design
- Report Generation
- Software Simulation

---

## 👩‍💻 Author

**Vaibhavi S K**

Computer Science & Engineering Student

---

## ⭐ Support

If you found this project useful:

⭐ Star this repository

🍴 Fork this repository

📢 Share it with others

---

## 📜 License

This project is developed for educational and academic purposes.
