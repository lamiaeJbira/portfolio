---
title: Secure Micromobility Route Planning API
publishDate: 2024-04-11 00:00:00
img: /assets/WhatsApp Image 2024-08-23 at 4.15.04 p.m..jpeg
img_alt: Safe routes for micromobility devices
description: |
  This API provides dynamically generated safe routes for e-scooter and bicycle users on the Pessac-Talence-Gradignan campus, taking into account real-time factors such as traffic, lighting, and weather.
tags:
  - API
  - Micromobility
  - Safety
---

## Secure Micromobility Route Planning API

##### Summary
This API addresses the growing need for safer routes for e-scooter and bicycle users on the Pessac-Talence-Gradignan campus. By factoring in traffic density, street lighting, weather data, and user preferences, it delivers optimized, secure routes that enhance both safety and user experience.

##### Key Features
- **Dynamic Route Computation**: Real-time calculation of optimal paths based on safety metrics.  
- **RESTful Endpoints**: Easy-to-use API for integration with mobile or web clients.  
- **Live Data Integration**: Traffic, lighting, and weather feeds update routes on the fly.  
- **Route Statistics**: Provides detailed metrics (distance, estimated time, safety score).  
- **User Preferences**: Customize routing based on speed, lighting level, or minimal traffic.  
- **Incident Reporting**: Users can flag hazards and contribute to route safety improvements.  
- **Comprehensive Documentation**: Swagger/OpenAPI spec and code examples included.

##### Git Workflow
- **feature/&lt;name&gt;**: New feature development  
- **develop**: Daily integration, bug fixes, and testing  
- **main**: Stable branch for system tests and release candidates  
- **production**: Production-ready code after final validation  

**Commit Convention**  
Stage your changes, then run:

./commit.sh


This script formats commit messages and runs automated tests.

##### Deployment & Branching

1. **Develop Features** on `feature/&lt;name&gt;`.
2. **Merge to develop** without pull request for daily iterations.
3. **Open PR to main** once `develop` is stable.
4. **PR from main to production** after passing release tests.

##### Setup & Installation

1. **Quick Linux Setup**

   - ./setup.sh

2. **Virtual Environment (optional but recommended)**

   - python3 -m venv venv
   - source venv/bin/activate   # (or venv\Scripts\activate on Windows)

3. **Install Dependencies**

- pip install -r requirements.txt
- 
5. **Generate Graph**

   - python3 creation.py

6. **Run the API**

   - python3 app.py



