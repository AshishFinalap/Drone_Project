# Autonomous Drone-Based Disaster Response & Rescue System

## Overview

An AI-powered autonomous drone system designed for disaster response and search-and-rescue operations. The project combines Graph Neural Networks (GNN), graph-based path planning, real-time telemetry, and an interactive web dashboard to assist rescue teams in navigating hazardous environments efficiently.

The system models the disaster area as a graph where locations are represented as nodes and possible drone movements as edges. Machine learning predicts safe traversal paths, while shortest-path algorithms generate optimal rescue routes.

---

## Features

- Graph-based disaster area modeling
- Graph Neural Network (GNN) for node prediction
- Shortest path planning using Dijkstra's Algorithm
- Interactive map-based monitoring dashboard
- Real-time drone telemetry support
- Rescue node visualization
- Dynamic graph generation from datasets
- Modular architecture for ROS2 integration
- Frontend built using React + TypeScript
- Python backend for AI model inference

---

## Project Architecture

```
Drone
   │
   ▼
Telemetry Data
   │
   ▼
Graph Construction
   │
   ▼
Graph Neural Network
   │
   ▼
Safe Node Prediction
   │
   ▼
Dijkstra Path Planning
   │
   ▼
Interactive Rescue Dashboard
```

---

## Tech Stack

### Frontend

- React
- TypeScript
- Vite
- Leaflet
- CSS

### Backend

- Python
- PyTorch
- NetworkX
- NumPy
- Pandas

### Machine Learning

- Graph Neural Networks (GNN)
- Node Classification
- Graph Processing

### Robotics

- ROS2 Compatible
- Drone Telemetry Interface

---

## Repository Structure

```
Drone_Project/

├── Frontend
│   ├── App.tsx
│   ├── DroneMap.tsx
│   ├── Header.tsx
│   └── Components
│
├── AI Models
│   ├── train.py
│   ├── predict.py
│   ├── gnn.py
│   ├── model_utils.py
│   └── node_predictor_model.pt
│
├── Graph Processing
│   ├── build_graph.py
│   ├── train_node_and_edge.py
│   └── synthetic_dataset.py
│
├── Data
│   ├── adjacency.csv
│   ├── nodes_features.csv
│   └── test_adjacency.csv
│
├── Telemetry
│   └── telemetry.py
│
└── Configuration
    ├── package.json
    ├── requirements.txt
    └── vite.config.ts
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/<your-username>/Drone_Project.git

cd Drone_Project
```

### Install Frontend

```bash
npm install
```

### Install Backend

```bash
pip install -r requirements.txt
```

---

## Running the Project

### Start Frontend

```bash
npm run dev
```

### Train GNN Model

```bash
python train.py
```

### Run Prediction

```bash
python predict.py
```

### Generate Graph

```bash
python build_graph.py
```

---

## Machine Learning Pipeline

1. Load graph dataset
2. Extract node features
3. Train Graph Neural Network
4. Predict safe rescue nodes
5. Build weighted graph
6. Compute optimal rescue path
7. Display results on dashboard

---

## Applications

- Disaster Management
- Search and Rescue
- Emergency Response
- Autonomous Drone Navigation
- Smart City Surveillance
- Hazard Zone Mapping

---

## Future Improvements

- Multi-drone coordination
- Live GPS integration
- Real-time obstacle avoidance
- Reinforcement Learning-based path planning
- Cloud deployment
- Live video streaming
- Edge AI optimization

---

## Requirements

- Python 3.10+
- Node.js 18+
- npm
- PyTorch
- NetworkX
- React
- TypeScript

---

## License

This project is released under the Apache 2.0 License.

---

## Acknowledgements

This project utilizes open-source tools and libraries including:

- PyTorch
- React
- Vite
- NetworkX
- Leaflet
- ROS2
