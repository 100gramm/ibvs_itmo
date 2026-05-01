# IBVS ITMO: Image-Based Visual Servoing

This repository contains a team project developed at ITMO University focused on **Image-Based Visual Servoing (IBVS)**

## Project Description
The goal of this project is to implement a control pipeline where a robot's state is determined through a visual feedback loop. Using cameras in a simulated environment, the system extracts key features to calculate control signals, bypassing traditional odometry where necessary.

### Key Technologies
* **Physics Simulation:** MuJoCo
* **Computer Vision:** OpenCV (for feature extraction and image processing)
* **Language:** Python 3.9+

---

## Installation Guide

Follow these steps to set up the environment and run the project locally.

### 1. Prerequisites
Ensure you have the following installed:
* [Python 3.9+](https://www.python.org/downloads/)
* [MuJoCo](https://github.com/google-deepmind/mujoco/releases) (Note: Modern versions are installed via pip, but ensure your system drivers are up to date).

### 2. Clone the Repository
```bash
git clone [https://github.com/knigstein/ibvs_itmo.git](https://github.com/knigstein/ibvs_itmo.git)
cd ibvs_itmo
```

### 3. Create a Virtual Environment
It is highly recommended to use a virtual environment to avoid dependency conflicts.
```bash
# Create environment
python -m venv venv

# Activate on Windows
.\venv\Scripts\activate

# Activate on Linux/macOS
source venv/bin/activate
```

### 4. Install Dependencies
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

---

## Usage and Workflow

### Running the Simulation
To launch the main simulation environment and see the pre-trained agent or the CV pipeline in action:
```bash
python main.py
```


## Project Structure

* `models/` – Saved weights for RL agents (Stable Baselines3 exports).
* `envs/` – Custom Gymnasium environments for the MuJoCo simulation.
* `cv_modules/` – Scripts for image processing, masking, and feature detection.
* `utils/` – Helper functions for coordinate transformations and logging.
* `main.py` – The main entry point for running the demonstration.

---

## License
This project is licensed under the MIT License.
```
