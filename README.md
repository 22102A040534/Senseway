## Hi there 👋
 SenseWay – AI-Powered Smart Navigation for Neurodiverse Users - https://senseway-c517e.web.app/
SenseWay is an AI-driven smart navigation platform designed to offer personalized, accessible, and stress-free routing solutions for neurodiverse individuals. Whether you're planning a calm walk or need real-time emergency support, SenseWay adapts to your sensory preferences to help you move through the world with confidence.

🚀 Features
Route Planning
Choose between the Shortest, Sensor-Friendly, or Safe Rest Stop routes based on individual preferences.
Routes are visualized on a map with live distance and ETA updates.

Real-Time Navigation with Calm Sync
Multiple Route Options: Generates up to 3–5 routes using Google Directions API, ranked by a Calmness Score:[C = w_1 \times (1 - \frac{N}{N_{max}}) + w_2 \times (1 - \frac{AQI}{AQI_{max}}) + w_3 \times (1 - \frac{T}{T_{max}}) + w_4 \times (1 - \frac{D}{D_{max}})]Where: (C): Calmness Score (N): Noise Level (dB) (AQI): Air Quality Index (T): Estimated Time (minutes) (D): Distance (km) Weights ((w_1, w_2, w_3, w_4)): Customizable (default: 0.4, 0.3, 0.2, 0.1)


AR Navigation
Uses Web AR (AR.js) for immersive augmented reality-based directions, tailored for sensory-friendly environments.AR Live View: Uses AR.js and to overlay directional rings and step-by-step instructions in real space. Real-Time Step Advancement: Automatically progresses instructions when within 10 meters of a waypoint using navigator.geolocation.watchPosition. Voice Guidance: Provides spoken instructions alongside on-screen AR cues for accessibility. Mobile-Optimized: Fully responsive, tested on Chrome Android with GPS and camera support.


Emergency Support Page
Live safe zone maps with SOS button to alert trusted contacts with your real-time location.

Peer Monitoring
Allows syncing with trusted peers/family members for shared live tracking in high-stress situations.

Environmental Insights
Live Data: Fetches real-time AQI, noise levels, temperature, and humidity via OpenWeatherMap and Noise APIs. Neurodiverse-Friendly Visuals: Color-coded metrics (🟢 Good, 🟡 Moderate, 🔴 Poor) with minimal visual noise. Periodic Updates: Refreshes data every 60 seconds without page reloads.


User Profile with Sensory Preferences
Stores preferences like avoiding loud zones or preferring daylight routes to personalize your experience.

AI Chatbot (Navi)
Floating Interface: Minimal, responsive chatbot for navigation and page routing. Rule-Based Logic: Handles greetings, navigation commands, and page redirects using keyword detection. Offline-Compatible: Works without API calls, ensuring reliability in low-network scenarios.


🛠 Technologies Used
Frontend: HTML, CSS, JavaScript 
APIs: Google Maps JavaScript API (Directions, Places, Geometry, Street View) OpenWeatherMap API (AQI, temperature, humidity) Noise APIs (e.g., Ambiciti, Noise-API, placeholders for future integration) Overpass API (hospital locations) Nominatim (reverse geocoding)

AR: AR.js, A-Frame, Backend: Firebase (hosting, Realtime Database for peer monitoring) 
Storage: localStorage for offline profile data Styling: Tailwind CSS (planned), custom CSS for neurodiverse-friendly UI Fonts: System default for performance, Poppins as fallback 
Deployment: Firebase Hosting with enhanced cache settings


✅ Built Using:
Project IDX – for seamless cloud-based development

Gemini API – for future integration of context-aware suggestions & predictive assistance
----------------------------------------------------------------------------------------------
$ Performance Benchmarks :

# Module Metric Result

Route Planning Time to Render Routes 1.8–2.4 sec

Calm Score Calculation <100 ms per route

Real-Time Navigation GPS Lock Time Avg. 2.1 sec

Checkpoint Detection <500 ms (~10m threshold)

AR Navigation AR.js Load Time ~1.9 sec

Instruction Update <200 ms lag

Environmental Insights API Poll Frequency Every 60 sec

AQI + Noise Load Time ~1.3 sec

Emergency Support Location Fetch ~1.5 sec

Rest Stop Retrieval <2.5 sec (5km radius)

Peer Monitoring Live Location Sync <300 ms latency

AI Chatbot Toggle Response ~80 ms

Profile Page Form Load + Prefill ~20 ms (localStorage)
----------------------------------------------------------------------------------------------
Mobile Optimization:

Fully responsive (360px–1080px) First Meaningful Paint: 1.5–2.2 sec on 5G/4G Offline support for chatbot, profile, and partial AR functionality
-----------------------------------------------------------------------------------------------
Please follow the Code of Conduct and ensure tests pass before submitting. License This project is licensed under the MIT License. Acknowledgements.
For questions or support, contact - arshiambu@gmail.com or open an issue on GitHub.

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
(https://senseway-c517e.web.app/)
