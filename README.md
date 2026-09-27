# 🌐 God's Eye View

> **A real-time 3D geospatial intelligence dashboard for exploring live public-world data on an interactive globe.**

Explore aircraft, ships, satellites, earthquakes, fires, weather, public cameras, infrastructure, radio stations, transit and more — all through one interactive spatial interface.

## 🚀 Live Demo

### **[🌍 Open God's Eye View](https://gods-eye-view-1lsi.onrender.com/)**

No installation required. Open the deployed application and start exploring the globe.

---

## ✨ Overview

**God's Eye View** is an interactive geospatial visualization platform built around a 3D globe.

The application combines multiple public and open data sources into a single interface so users can explore the world from a global view down to individual geographic entities.

Instead of switching between separate websites for flights, satellites, weather, earthquakes and other datasets, the project brings these sources together into one visual environment.

### What you can explore

* ✈️ Live aircraft
* 🛳️ Vessels and maritime activity
* 🛰️ Satellites and orbital objects
* 🌍 Earthquakes
* 🔥 Active fires
* 🌦️ Weather information
* 🌬️ Wind conditions
* 📹 Public camera locations
* 📡 Radio stations
* 🚆 Public transportation
* 🚲 Bike-sharing availability
* 🚀 Space missions
* 🏗️ Infrastructure
* 🗺️ Maps and geographic data
* 🧭 Routes and geographic measurements
* 🌐 Global geographic context

---

# 🎯 Project Goals

The project focuses on three main ideas:

### 1. One interface for many datasets

Public geographic information is distributed across hundreds of services.

God's Eye View provides a common visual layer for exploring those datasets.

### 2. Spatial understanding

Tables are useful, but geographic relationships are often easier to understand visually.

The application allows users to see:

* where objects are located
* how they move
* what exists nearby
* how different datasets overlap
* how events relate to geography

### 3. Experimentation

The project is designed to be explored, modified and extended.

Developers can add new:

* data sources
* map layers
* visualizations
* controls
* geographic datasets
* analysis tools

---

# 🧭 Main Features

## ✈️ Live Aircraft

Track aircraft using publicly available aviation data.

Aircraft can be visualized directly on the globe with information such as:

* position
* altitude
* heading
* speed
* callsign
* aircraft metadata
* movement history where available

The interface can interpolate between incoming data points to make movement appear smoother.

---

## 🛰️ Satellite Tracking

Explore satellites and orbital objects using publicly available orbital information.

The satellite layer can display:

* satellite positions
* orbital paths
* satellite categories
* selected satellite information

The project uses orbital propagation techniques to calculate satellite positions between observations.

---

## 🚢 Maritime Data

Explore available vessel information from supported AIS sources.

Depending on the configured provider and available coverage, users can inspect:

* vessel positions
* vessel movement
* vessel metadata
* maritime activity

Coverage depends on the underlying data provider.

---

## 🌍 Earthquakes

The earthquake layer visualizes recent seismic activity.

Users can inspect geographic earthquake events and compare them with other layers such as:

* population areas
* infrastructure
* weather
* transportation
* geographic regions

Earthquake information is sourced from public seismic data providers.

---

## 🔥 Active Fires

The project can visualize active fire detections from supported satellite-based fire datasets.

Useful information may include:

* detection location
* detection time
* intensity-related information
* surrounding geographic context

Fire data should be treated as observational data rather than an emergency-response system.

---

## 🌦️ Weather

The weather system can visualize multiple types of atmospheric information.

Supported concepts include:

* wind
* precipitation
* satellite cloud imagery
* lightning
* weather observations
* cyclone information

The globe can be used to understand weather patterns geographically rather than through isolated weather charts.

---

## 📹 Public Cameras

Supported public camera sources can be displayed geographically.

Camera information may include:

* camera position
* source
* estimated viewing direction
* coverage area
* available live imagery

Camera locations and coverage depend on the underlying public source.

---

## 📻 Radio

The radio layer connects geographic locations with publicly available radio station information.

Users can explore stations geographically and move between broadcasters using the interactive globe.

---

## 🚆 Transit

Where supported by available public feeds, the project can visualize:

* buses
* trains
* trams
* metros
* ferries

Transit availability depends on the supported geographic feeds.

---

## 🚲 Bike Sharing

The application can display public bike-sharing station information where GBFS feeds are available.

Depending on the provider, users may see:

* station locations
* available bikes
* available spaces
* station status

---

# 🗺️ Interactive Globe

The application is built around an interactive geographic environment.

Users can:

* zoom from global scale to local areas
* rotate the globe
* change viewing angles
* select geographic objects
* track objects
* switch visualization layers
* inspect geographic information
* change map providers
* create geographic routes

The interface is designed to make large amounts of spatial information understandable without requiring a traditional GIS application.

---

# 🎛️ Visualization Modes

The application includes visual modes designed for different viewing conditions.

Examples include:

* Normal
* CRT
* Night Vision
* FLIR / Thermal-style visualization
* Noir
* Snow
* Tactical HUD

These modes are primarily visual effects and should not be interpreted as actual sensor data.

---

# 🎯 Object Tracking

Users can select supported objects and focus the camera on them.

Depending on the selected data source, tracked objects can expose information such as:

```text
Position
Altitude
Speed
Heading
Identifier
Source
Last Update
Additional Metadata
```

The globe can keep the selected object centered while the user changes camera orientation or visualization settings.

---

# 🧭 Directions

The application can generate geographic routes using supported routing services.

Depending on the selected mode, routes can represent:

* walking
* driving
* cycling

Routes are visualized directly over the geographic environment.

---

# 📏 Geographic Measurements

The globe can also be used to understand geographic distances.

Users can measure relationships between geographic points and visualize them directly on the map.

Example:

```text
Location A
     │
     │ geographic distance
     │
Location B
```

---

# 🎙️ Voice Interaction

Optional voice functionality can be connected through an AI provider.

When configured, voice commands can be used for operations such as:

```text
Take me to Tokyo.

Show aircraft near this location.

Turn on the satellite layer.

Switch to night vision.

Zoom out to the globe.

Track that aircraft.
```

Voice capabilities depend on the configured AI provider and available API access.

The application is designed so that the core globe remains usable without voice functionality.

---

# 🧠 AI-Assisted Scene Understanding

When the optional AI functionality is configured, the application can provide contextual information about the current scene.

The system can combine available application state such as:

* geographic coordinates
* active layers
* selected objects
* map scale
* geographic context

with an AI interface.

AI-generated information should always be treated as an assistant layer rather than an authoritative source.

---

# 🏗️ Technology Stack

## Frontend

| Technology | Purpose                       |
| ---------- | ----------------------------- |
| JavaScript | Application logic             |
| HTML       | Application structure         |
| CSS        | UI and visualization styling  |
| Vite       | Development and build tooling |
| CesiumJS   | 3D geographic visualization   |

## Data & APIs

The project can integrate with multiple public or third-party services depending on configuration.

Examples include:

* OpenSky
* adsb.lol
* CelesTrak
* USGS
* NASA FIRMS
* NOAA
* ECMWF
* OpenStreetMap
* OSRM
* Radio Browser
* GBFS feeds
* GTFS-Realtime feeds
* public transportation APIs
* public camera APIs
* Launch Library

Provider availability and quotas can change over time.

---

# 🏛️ Architecture

A simplified view of the application architecture:

```text
                    ┌──────────────────────┐
                    │      Web Browser     │
                    │                      │
                    │  HTML / CSS / JS     │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │       CesiumJS       │
                    │    3D Globe Engine   │
                    └──────────┬───────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
        ┌───────────┐    ┌───────────┐    ┌───────────┐
        │   Maps    │    │  Layers   │    │   UI/HUD  │
        └───────────┘    └─────┬─────┘    └───────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
         Aircraft          Satellites       Weather
              │                │                │
              ▼                ▼                ▼
          Vessels          Earthquakes        Fires
              │                │                │
              └────────────────┼────────────────┘
                               ▼
                    ┌──────────────────────┐
                    │   Public Data APIs   │
                    └──────────────────────┘
```

---

# 📁 Project Structure

The repository follows a modular JavaScript architecture.

```text
gods-eye-view/
│
├── .github/
│   └── workflows/
│
├── .agents/
│
├── build/
│
├── config/
│
├── docs/
│
├── pinokio/
│
├── public/
│
├── scripts/
│
├── server/
│
├── src/
│   ├── data/
│   │   ├── local_data/
│   │   └── ...
│   │
│   ├── layers/
│   │   └── ...
│   │
│   ├── scenes/
│   │   └── ...
│   │
│   ├── voice/
│   │   └── ...
│   │
│   ├── main.js
│   ├── ui.js
│   ├── hud.js
│   ├── keySetup.js
│   └── mapStackController.js
│
├── tools/
│
├── .env.example
├── index.html
├── package.json
├── package-lock.json
├── style.css
├── vite.config.js
├── CHANGELOG.md
├── CONTRIBUTING.md
├── DATA_SOURCES.md
├── SECURITY.md
├── TESTING.md
└── README.md
```

---

# ⚡ Getting Started

## Requirements

Install:

* Node.js
* npm
* Git

Recommended Node.js versions should match the versions supported by the project configuration.

Check your installation:

```bash
node --version
npm --version
git --version
```

---

# 📥 Installation

Clone the repository:

```bash
git clone https://github.com/yashwantsingh4115/gods-eye-view.git
```

Enter the project directory:

```bash
cd gods-eye-view
```

Install dependencies:

```bash
npm ci
```

---

# 🩺 Check the Environment

Run the project diagnostics:

```bash
npm run doctor
```

This can help identify configuration and provider-related problems before starting the application.

---

# ▶️ Start Development Server

Run:

```bash
npm run dev
```

Then open:

```text
http://localhost:4173
```

The exact port may depend on the project's current Vite configuration.

---

# 🔐 Environment Variables

Some functionality requires external provider credentials.

Create a local environment file when required:

```bash
cp .env.example .env
```

On Windows PowerShell:

```powershell
Copy-Item .env.example .env
```

Never commit secrets to GitHub.

Example structure:

```env
# Example only
OPENAI_API_KEY=
CESIUM_ION_TOKEN=
AISSTREAM_API_KEY=
NASA_FIRMS_API_KEY=
TOMTOM_API_KEY=
OPENSKY_CLIENT_ID=
OPENSKY_CLIENT_SECRET=
```

Only configure variables that are actually required by the functionality you intend to use.

---

# 🔑 Optional Providers

The application is designed so that API keys are optional for many features.

| Provider       | Possible Usage                                     |
| -------------- | -------------------------------------------------- |
| Cesium ion     | 3D terrain and additional geographic visualization |
| Google Maps    | Google mapping services                            |
| OpenAI         | Voice and AI-assisted interaction                  |
| AISStream      | Maritime data                                      |
| NASA FIRMS     | Active fire data                                   |
| TomTom         | Traffic-related data                               |
| OpenSky        | Additional aircraft access                         |
| Launch Library | Additional space mission data                      |

Provider pricing, quotas, authentication requirements and terms can change.

Always check the provider's current documentation before deploying a production application.

---

# ☁️ Deployment

The project can be deployed to a compatible Node.js hosting platform.

The current deployed version is hosted on Render:

## 🌐 Production

**https://gods-eye-view-1lsi.onrender.com/**

### Basic Render workflow

```text
GitHub Repository
       │
       ▼
     Render
       │
       ▼
   Build Project
       │
       ▼
 Start Node/Vite Server
       │
       ▼
 Public Web Application
```

For production deployments:

1. Connect the GitHub repository.
2. Configure the required build/start commands.
3. Add required environment variables.
4. Deploy.
5. Verify the application and API integrations.

Do not expose private API keys through frontend JavaScript.

---

# 🛡️ Security

Security is important because this application can interact with multiple external services.

### Never commit:

```text
.env
API keys
private tokens
client secrets
credentials
access tokens
```

Use environment variables for sensitive configuration.

For browser-exposed provider keys, configure provider-side restrictions whenever supported.

Examples include:

* domain restrictions
* API restrictions
* quota limits
* usage alerts

Application-level rate limiting is not a replacement for provider billing controls.

---

# ⚠️ Data Accuracy

God's Eye View visualizes information obtained from public and third-party sources.

That means information can be:

* delayed
* incomplete
* unavailable
* approximate
* modeled
* interpolated
* incorrectly reported by the upstream source

Therefore, the application should **not** be used as the sole source for:

* flight navigation
* maritime navigation
* emergency response
* medical decisions
* safety-critical operations
* law-enforcement decisions
* financial decisions
* other operationally critical decisions

Always verify important information using authoritative sources.

---

# 🔒 Privacy & Responsible Use

This project is intended for geographic visualization and exploration of publicly available information.

The application should not be used to:

* identify private individuals
* track individuals
* perform unauthorized surveillance
* bypass access controls
* obtain private information
* misuse public datasets

Public availability of data does not automatically make every use appropriate.

Use the project responsibly and respect the terms of the underlying data providers.

---

# 📊 Data Sources

The project can combine information from several public and third-party datasets.

Examples include:

### Geographic

* OpenStreetMap
* Cesium
* Esri
* Google mapping services where configured

### Aviation

* OpenSky
* adsb.lol

### Space

* CelesTrak
* Launch Library

### Environment

* USGS
* NASA FIRMS
* NOAA
* ECMWF

### Transportation

* GTFS
* GTFS-Realtime
* GBFS
* public transportation feeds

### Routing

* OSRM
* OpenStreetMap

### Radio

* Radio Browser

The exact source, license, attribution and limitations of each dataset should be checked in:

```text
DATA_SOURCES.md
```

---

# 🧪 Development

Useful commands:

```bash
npm install
```

```bash
npm run dev
```

```bash
npm run doctor
```

```bash
npm run build
```

```bash
npm run preview
```

Available scripts depend on the current `package.json`.

Check them with:

```bash
npm run
```

---

# 🧩 Adding a New Data Layer

A new layer can generally follow this pattern:

```text
Data Provider
     │
     ▼
API / Dataset
     │
     ▼
Data Processing
     │
     ▼
Layer Module
     │
     ▼
Cesium Entities / Primitives
     │
     ▼
Interactive Globe
```

A good layer should define:

* data source
* update frequency
* geographic coordinate handling
* entity representation
* metadata
* loading state
* error handling
* attribution
* provider limitations

---

# 💡 Example Layer Ideas

The architecture can be extended with additional public datasets.

Potential additions:

* weather stations
* wildfire perimeters
* flood monitoring
* volcano activity
* astronomical observations
* public transportation systems
* renewable energy infrastructure
* public environmental sensors
* oceanographic observations
* geographic boundaries
* disaster information

New integrations should respect the source provider's API terms and licensing.

---

# 🤝 Contributing

Contributions are welcome.

Before opening a pull request:

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Test the application.
5. Check formatting and linting where applicable.
6. Update documentation when necessary.
7. Open a pull request.

Example:

```bash
git checkout -b feature/new-layer
```

Make your changes and commit them:

```bash
git add .
git commit -m "feat: add new data layer"
```

Push the branch:

```bash
git push origin feature/new-layer
```

Then open a Pull Request on GitHub.

---

# 🐛 Bug Reports

When reporting an issue, include:

```text
Operating System:
Node.js Version:
npm Version:
Browser:
Steps to Reproduce:
Expected Behaviour:
Actual Behaviour:
Console Error:
Relevant Configuration:
```

Do not include API keys or other secrets in an issue.

---

# 📚 Documentation

Additional project documentation:

```text
README.md
CONTRIBUTING.md
DATA_SOURCES.md
SECURITY.md
TESTING.md
CHANGELOG.md
```

These files should be consulted for detailed development, security and data-source information.

---

# 🌐 Useful Links

### 🚀 Live Application

**[Open God's Eye View](https://gods-eye-view-1lsi.onrender.com/)**

### 💻 GitHub Repository

**[View Source Code](https://github.com/yashwantsingh4115/gods-eye-view)**

### 🐛 Issues

**[Report a Bug / Request a Feature](https://github.com/yashwantsingh4115/gods-eye-view/issues)**

### 🔀 Pull Requests

**[View Pull Requests](https://github.com/yashwantsingh4115/gods-eye-view/pulls)**

---

# 🧠 Why This Project?

Modern geographic information is fragmented across many independent systems.

One service shows aircraft.

Another shows earthquakes.

Another shows weather.

Another shows satellites.

Another shows roads.

Another shows public cameras.

Another shows ships.

God's Eye View attempts to create a common spatial interface where these datasets can be explored together.

The goal isn't simply to display more data.

The goal is to make **relationships between data visible**.

---

# 🗺️ Project Vision

```text
                 THE WORLD
                     │
                     ▼
             ┌───────────────┐
             │ Public Signals │
             └───────┬───────┘
                     │
       ┌─────────────┼─────────────┐
       │             │             │
       ▼             ▼             ▼
    Aviation      Weather      Satellites
       │             │             │
       ├─────────────┼─────────────┤
       │             │             │
       ▼             ▼             ▼
    Maritime      Events       Infrastructure
       │             │             │
       └─────────────┼─────────────┘
                     ▼
              ┌──────────────┐
              │ GOD'S EYE VIEW│
              └───────┬──────┘
                      │
                      ▼
             Interactive 3D Globe
```

---

# 📜 License

This repository is distributed under the license included in:

```text
LICENSE
```

Individual third-party datasets, APIs, imagery and bundled assets may have separate licenses and usage restrictions.

Always review:

```text
DATA_SOURCES.md
```

before redistributing third-party data or assets.

---

# ⭐ Support the Project

If you find the project useful:

* ⭐ Star the repository
* 🐛 Report bugs
* 💡 Suggest features
* 🔧 Submit improvements
* 📚 Improve documentation
* 🔀 Open Pull Requests

Every contribution helps improve the project.

---

# 🌍 God's Eye View

**Explore the world.**

**Understand the signals.**

**Build on top of open data.**

### 🚀 [Launch the Live Application](https://gods-eye-view-1lsi.onrender.com/)

---

<div align="center">

### 🌐 God's Eye View

**Interactive • Open Data • Geospatial • 3D**

Built for exploration, experimentation and learning.

</div>
