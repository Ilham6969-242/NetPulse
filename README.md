# NetPulse
A real-time network traffic and Geo-IP radar that visualizes active system sockets, bandwidth telemetry, and process-level connections on a dark-mode browser dashboard.
"Step 1: Download this repository."

"Step 2: Run pip install -r requirements.txt"

"Step 3: Run sudo uvicorn main:app --port 8000"

"Step 4: Open http://localhost:8000 in your browser."

Live Socket Inspection: Tracks active network connections and maps them to the specific system processes (e.g., chrome, ssh, python3) owning the traffic.

Real-Time Geo-IP Mapping: Resolves public destination IPs in batches and streams them over WebSockets to draw glowing arcs on a Leaflet.js world map.

Live Protocol & Bandwidth Telemetry: Tracks upload/download throughput and port distribution (HTTP/HTTPS/DNS/SSH) on rolling Chart.js dashboards.

Anomaly Alert Engine: Automatically flags sudden outbound connection bursts or traffic originating on non-standard ports.

Snapshot Replay Mode: Records 60 seconds of live WebSocket telemetry into a portable JSON file, enabling instant, installation-free demo hosting on GitHub Pages.
