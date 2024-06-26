# Drowsiness and Yawn Detection with OpenCV 👁️💤

This application uses OpenCV, dlib, and Pygame to detect drowsiness and count yawns in real-time using your webcam.

## Overview ℹ️

The program monitors facial landmarks and eye blink patterns to determine if the user is drowsy or active. It also tracks yawns and provides real-time feedback.

## Features 🚀

- **Real-time Face Detection:** Detects faces using dlib's frontal face detector.
  
- **Facial Landmark Detection:** Utilizes dlib's shape predictor to locate facial landmarks, including eyes.
  
- **Eye Blink Detection:** Calculates eye aspect ratio (EAR) to detect blinks and monitor drowsiness.
  
- **Yawn Detection:** Tracks yawn events based on mouth movement.

## Requirements 🛠️

- **Python 3.x**
- **OpenCV:** `pip install opencv-python`
- **dlib:** `pip install dlib`
- **Pygame:** `pip install pygame`
- **Numpy:** `pip install numpy`
- **Imutils:** `pip install imutils`

## Setup and Usage 📦

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your/repository.git
   cd repository-folder
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download the dlib Face Landmark Model:**
   Download the shape predictor model ("shape_predictor_68_face_landmarks.dat") from [dlib's model repository](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2) and place it in the project directory.

4. **Run the Application:**
   ```bash
   python app.py
   ```

5. **Interact:**
   - The application will open your webcam feed.
   - It will detect your face, track eye blinks, and count yawns.
   - Real-time status messages (active, drowsy, sleeping) will be displayed on the screen.

## Adjustments 🛠️

- **Thresholds:** Adjust EAR thresholds (`ear < 0.20` for sleep detection) based on your observation and environment.
- **Music:** Change or modify the alert music ("music.wav") as per your preference.

## Contributing 🤝

Contributions are welcome! Please fork the repository and submit pull requests for improvements or bug fixes.
