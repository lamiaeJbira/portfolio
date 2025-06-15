---
title: Public Transport Management System (TEC)
publishDate: 2023-12-28 00:00:00
img: /assets/air-auto-railway-transport-silhouette-260nw-2155243835.webp
img_alt: A bus picking up passengers at a city bus stop
description: |
  Learn how to manage passenger boarding and alighting in public buses using object-oriented programming. This guide walks through porting a C application to Java incrementally, focusing on creating abstract classes for vehicles and passengers.
tags:
  - Java
  - Object-Oriented Programming
  - Public Transport System
---

## Public Transport Management System (TEC)

> Efficiently handle passenger interactions in a bus system using Java.

This project ports an existing C application to Java with an object-oriented approach. It’s developed incrementally through a series of practical exercises, concentrating on managing passenger boarding and alighting in public buses.

### Prerequisites

To get started, you will need:

- **Java SE Development Kit (JDK) 8u221 or later**  
- **Make** for build automation  
- **Linux environment** (development optimized for Linux)

### Project Overview

The goal is to manage passenger boarding and alighting events in buses. Each bus maintains a list of passengers and notifies them at each stop. Passengers respond by requesting to disembark or change their seating status (e.g., seated, standing).

Key design elements include abstract classes for `Vehicle` and `Passenger`. For each exercise stage, a separate Git branch with factory patterns is available via:

git checkout TD<exercise-number>factory
`

Currently, the system defines multiple `Boarding` behaviors (4 types) and `Stop` behaviors (5 types), combined by three passenger types. Running the global test suite (`TestsGlobaux`) exercises all passenger scenarios.

### Project Structure

* **Makefile**: Automates compilation
* **README**: This documentation
* **src/**: Java source files for core classes
* **tst/**: Unit tests for main classes
* **build/tec/**: Compiled class files for the `tec` package
* **report/**: Final project report (PDF)

### Build & Run

1. **Compile the project**
   - make
2. **Run tests**
- make test 
3. **Clean build artifacts**
   - make clean
   



