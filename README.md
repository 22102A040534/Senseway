## Hi there 👋
 SenseWay – AI-Powered Smart Navigation for Neurodiverse Users
SenseWay is an AI-driven smart navigation platform designed to offer personalized, accessible, and stress-free routing solutions for neurodiverse individuals. Whether you're planning a calm walk or need real-time emergency support, SenseWay adapts to your sensory preferences to help you move through the world with confidence.

🚀 Features
Route Planning
Choose between the Shortest, Sensor-Friendly, or Safe Rest Stop routes based on individual preferences.
Routes are visualized on a map with live distance and ETA updates.

Real-Time Navigation
Powered by OpenStreetMap + OSRM, this mode offers full-screen map navigation with verbal cues, real-time position updates, and multiple travel modes (walk, cycle, train, car).

AR Navigation
Uses Web AR (AR.js) for immersive augmented reality-based directions, tailored for sensory-friendly environments.

Emergency Support Page
Live safe zone maps with SOS button to alert trusted contacts with your real-time location.

Peer Monitoring
Allows syncing with trusted peers/family members for shared live tracking in high-stress situations.

User Profile with Sensory Preferences
Stores preferences like avoiding loud zones or preferring daylight routes to personalize your experience.

🛠 Technologies Used
🌐 Frontend:
HTML5, CSS3, JavaScript

Leaflet.js for map rendering

Material UI for responsive design

🧠 Backend:
Node.js + Express

MongoDB / Firebase for data & peer syncing

📍 APIs & Integration:
OpenStreetMap + OSRM for routing

Leaflet Routing Machine for alternate routes

Speech Synthesis API for verbal cues

AirVisual API + Noise API for environmental data

Geolocation API + OpenMaps for safe zone detection

Firebase Hosting + Auth (Google Sign-In)

✅ Built Using:
Project IDX – for seamless cloud-based development

Gemini API – for future integration of context-aware suggestions & predictive assistance

📂 Repository Structure
pgsql
Copy
Edit
📁 public/
├── index.html
├── style.css
├── script.js
├── ar-navigation/
├── emergency-support/
├── profile/
├── peer-monitoring/
└── assets/
🔗 Live Demo
Hosted on Firebase: https://your-project-id.web.app (incognito mode)

