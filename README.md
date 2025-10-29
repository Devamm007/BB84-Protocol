# Hackathon Problem - BB84
Simulation App Repo: https://github.com/Devamm007/BB84-simulation-app
Simulation Demo: https://bb84-simulation-app.vercel.app/

## Team Name: Biskit
Members-
- 24f2000828@ds.study.iitm.ac.in
- ishitapurk14@gmail.com
- kushalpandey923@gmail.com

## Our Solutiom:
### Python Notebook-
The BB84 protocol is a foundational QKD method that allows two parties to generate a shared secret key over an insecure quantum channel while detecting eavesdroppers. <a href="https://github.com/ISAQC-QFF25/hackathon-bb84-biskit/blob/main/Notebook_functions.md">(used/created function's info)</a>

*This notebook simulates the protocol under various conditions:*
- Ideal Channel: No noise or eavesdropping.
- Noisy Channel: Natural quantum noise (e.g., depolarizing and readout errors).
- Eavesdropping Attack: Simulated interception by Eve, increasing readout noise.

*Key features:*
- Uses Qiskit-Aer for quantum circuit simulation.
- Supports configurable parameters like number of qubits, noise probability, eavesdropping probability , and more.
- Outputs detailed metrics, including QBER (with a threshold of 0.11 for detecting issues (commonly used)).
- Generates plots to analyze QBER and detection rates across varying noise/eavesdropping levels.

*Requirements:*
- Python (3.0 or latest)
- Jupyter Notebook / VS Code / Google Colab (```!pip install numpy matplotlib qiskit qiskit-aer```)
  - numpy
  - matplotlib
  - qiskit
  - qiskit-aer
- Setting locally
  - ```python3 -m venv <virtual-enviornment folder name>```
  - (Windows)```source <path-to-venv>/scripts/activate``` OR (Linux)```source <path-to-venv>/bin/activate```
  - ```pip install numpy matplotlib qiskit qiskit-aer```

### Simulation Application (to run locally)
- install all dependencies from requirements.txt using ```pip install -r requirements.txt```
- start the application after installing dependencies and being present in the directory containing app.py, run ```python app.py``` OR ```python3 app.py```

**OR**
### Lovable generated application (error-prone)
- https://bb84-whispers.lovable.app/

---
[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/J8PBj6Ui)
*Note: There is no autograder for this problem. Your solution will be manually reviewed.*
