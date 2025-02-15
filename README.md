# Voice-Controlled Arduino Robot 🤖🔊  

This project implements a **voice-controlled robot** using an **Arduino Leonardo**, powered by **machine learning-based speech recognition** with **Singular Value Decomposition (SVD)** and **Principal Component Analysis (PCA)**. The system captures and processes voice commands, sending control signals to the robot via **serial communication**.

## 🔧 Hardware Components
- 🛠 **Microcontroller**: Arduino Leonardo
- 🔊 **Microphone Module**: Captures voice commands
- ⚙️ **Motors**: DC motors with a motor driver for movement
- 🔋 **Power**: External power supply for stable operation
- 📡 **Communication**: Serial data transfer between PC and Arduino

## 🖥 Software Tools
- **Jupyter Notebook**: For voice signal processing and feature extraction
- **Python Libraries**: `numpy`, `scipy`, `sklearn`, `librosa`, `pyserial`
- **Machine Learning**: **SVD** & **PCA** for feature reduction and classification
- **Arduino IDE**: For motor control firmware

## 🚀 How It Works
1. **Voice Signal Processing**  
   - Captures voice commands using a **microphone module**.
   - Converts speech into a numerical feature matrix using **MFCC (Mel-Frequency Cepstral Coefficients)**.
   
2. **Feature Extraction with SVD & PCA**  
   - **SVD** decomposes the feature matrix for dimensionality reduction.
   - **PCA** finds the most important features for classification.

3. **Command Classification**  
   - Trains an ML model to recognize commands like `forward`, `backward`, `left`, `right`, and `stop`.
   - Uses **KNN or SVM classifiers** for real-time prediction.

4. **Arduino Control**  
   - The predicted command is sent via **serial communication** (`pyserial`).
   - Arduino executes corresponding motor actions.
## Demo
Here’s a screenshot of the project:
video's link: (https://drive.google.com/file/d/1pHrXH5elPMvx0C1SMg8o44wD7MbwBJkG/view?usp=drive_link)
(https://github.com/Dao1213/Voice-Controlled-Arduino-Robot/blob/main/IMG_9990.jpg)
(https://github.com/Dao1213/Voice-Controlled-Arduino-Robot/blob/main/IMG_9996.jpg)
