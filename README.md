# Vegetable Sorting Robot

## Overview
This project implements an automated vegetable sorting system that combines computer vision with Arduino-controlled actuation. The system identifies vegetables, evaluates their quality, and sorts them into the appropriate containers based on ripeness or spoilage. It demonstrates the integration of perception, analysis, and robotics for practical applications in agriculture and food processing.

## Features
- Vegetable recognition using OpenCV
- Quality assessment for ripeness and spoilage
- Arduino-controlled sorting mechanism
- Fully automated workflow integrating vision, analysis, and actuation
- Modular and extensible system for new vegetable types

## System Architecture
[Camera] --> [Vision Module (OpenCV)] --> [Assessment Module (Ripeness/Spoilage Detection)] --> [Control Module (Python)] --> [Arduino Actuation] --> [Sorting Containers]

## Module Description

### 1. Vision Module
- Captures images of incoming vegetables
- Detects vegetable type using computer vision techniques such as color, shape, and texture analysis
- Outputs a classification label for each vegetable

### 2. Assessment Module
- Evaluates vegetable quality:
  - Spoiled
  - Unripe
  - Ripe
- Uses visual cues such as color, texture, and visible defects
- Sends assessment results to the control module

### 3. Control Module
- Acts as the bridge between perception and physical actuation
- Receives classification and assessment results
- Sends commands to the Arduino to trigger the sorting mechanism

### 4. Arduino Actuation
- Receives signals from the control module via serial communication
- Controls motors or servos to direct vegetables into the appropriate containers
- Ensures timing and precision for accurate sorting

### 5. Sorting Containers
- Separate bins for:
  - Spoiled vegetables
  - Unripe vegetables
  - Ripe vegetables

## Workflow
1. A vegetable is placed in the input area.
2. The camera captures an image and sends it to the Vision Module.
3. The Vision Module identifies the vegetable type.
4. The Assessment Module analyzes its quality.
5. The Control Module sends actuation commands to the Arduino.
6. The Arduino moves the vegetable to the corresponding container.
7. The system resets and becomes ready for the next vegetable.

## Purpose
- Automate quality control in agriculture and food processing
- Reduce manual labor in sorting and packaging workflows
- Demonstrate the integration of computer vision and robotics in a practical system
- Serve as a testbed for AI-assisted industrial automation projects

## Installation & Usage
1. Clone the repository:
   ```bash
   git clone <your-repository-link>
   ```
2. Install the required Python libraries.
3. Upload the Arduino code to the microcontroller.
4. Run the Python vision and control script.
5. Place vegetables in the input area and monitor the sorting process.
   git clone <repository-url>
