---
title: CycloEval
publishDate: 2025-01-20
img: /assets/cycloEvalecran.png
img_alt: Screenshot of the CycloEval web interface
description: |
  CycloEval analyzes smartphone sensor data mounted on a bicycle to assess riding conditions and detect impacts. The project combines frontend, backend, and cloud technologies to collect, process, and visualize sensor data in real time.
tags:
  - React
  - Python
  - REST API
  - CI/CD
  - Docker
---

### CycloEval

##### Description
CycloEval processes smartphone sensor logs captured on a bicycle to evaluate ride quality and flag shocks. It features a modern frontend, a FastAPI backend, and automated deployment pipelines.

##### Features
- **Data Collection**: Uses the Sensor Logger app to record accelerometer, gyroscope, and GPS streams.  
- **Data Processing**: FastAPI endpoints analyze sensor streams to detect impacts and compute ride-condition metrics.  
- **Visualization**: Interactive map view showing ride paths and detected shocks in real time.

##### Requirements
- Node.js 18+ and npm or pnpm  
- Python 3.8+ with FastAPI & Uvicorn  
- Docker & Docker Compose  

##### Installation

**Frontend**  
1. Navigate to the `client` folder:
   cd client
2. Create a `.env` file:
3. Install dependencies and start the dev server:

   - npm install
   - npm run dev


**Backend**

1. Install Python dependencies:

   pip install -r server/requirements.txt
   
2. Launch the FastAPI server:

   uvicorn server.main:app --host 127.0.0.1 --port 8000 --reload


**Full Stack Deployment**
Use Docker Compose to build and run all services:

- docker-compose down
- docker-compose up --build -d


To force recreate (drops the database):

- docker-compose down
- docker-compose up --build --force-recreate -d


Check logs for CI/CD and services:

- tail -f local_api.log
- docker logs fastapi_backend
- docker logs vite_frontend

