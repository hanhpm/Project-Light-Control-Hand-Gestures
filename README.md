# Light Controlling Using Hand Gestures

A project that uses hand gesture recognition to control lights, integrating Google's MediaPipe Gesture Recognizer with a deep learning-based Multi-Layer Perceptron (MLP) model. This project provides an innovative way to interact with devices through predefined hand gestures.

---

## Features

- **Hand Gesture Recognition**: Detects and classifies predefined hand gestures in real-time.
- **Light Control**: Controls lights based on recognized gestures.
- **Real-Time Deployment**: Supports simulation and real-world implementation with relay modules.
- **Customizable Classes**: Easily modify gesture classes via a YAML configuration file.

---

## Installation and Process to run the follow-up command 

### Prerequisites

1. Install **Python 3.10**.
2. Install dependencies using the `requirements.txt` file:

```bash
conda create -n gesture_env python=3.10
conda activate gesture_env
pip install -r requirements.txt
```

---
## Data collection 

```bash 
python generate_landmark_data.py
```
---
### Train the model 
1. Load and preprocess the data: The dataset will be loaded from the .csv files generated earlier.

2. Train and validate the model: Use PyTorch to train the Multi-Layer Perceptron (MLP) model.

3. Evaluate the model: Test the trained model on the test dataset to ensure accuracy.
---
### Deployment
Command to run deployment:

```bash 
python detect_simulation.py
```

Modify the script to set the mode:

```bash
device = False  # Simulation mode
# device = True  # Real hardware mode
```
---

## License
This project is licensed under the MIT License. See the LICENSE file for details.






