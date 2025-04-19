##📡 IoT Based Earthquake Monitoring and Alerting System Using Machine Learning

This project leverages IoT sensors, microcontroller-based data collection, and machine learning to detect seismic events in real-time. It provides early warnings using visual and auditory alerts and dashboards for monitoring.
___

##🔧 Components Overview

✅ **Python Scripts**
serial_reader.py – Connects to Arduino and fetches real-time sensor data.

data_preprocessing.py – Cleans, scales, and reshapes data for model input.

model_inference.py – Loads trained ML models (LSTM/GRU/RNN) and predicts seismic activity.

flask_app.py – Serves a live web dashboard for visualization.

gui_app.py – Optional desktop GUI using Tkinter.

✅ Arduino Sketches
seismic_sensors.ino – Reads vibration, accelerometer, and temperature data.

Sends formatted strings to Python via USB serial communication.

✅ Machine Learning Models
Trained on labeled sensor datasets.

Models used: LSTM, GRU, and RNN.

Stored in .h5 format for real-time predictions.

___

##⚙️ How to Run
On Arduino
Upload seismic_sensors.ino using Arduino IDE.

Connect board via USB and ensure correct COM port.

Open Serial Monitor (optional, for debugging).


On Python Environment
Install dependencies:
pip install numpy pandas matplotlib tensorflow flask scikit-learn pyserial

Run the system:

bash
Copy
Edit
python flask_app.py  # for web dashboard
python gui_app.py    # for desktop GUI
____

📡 Alerting Mechanism
Normal Activity: LED glows green, no alert sound.

Abnormal Activity: Buzzer + red LED flash.

Alerts can also be integrated with:

Email (SMTP)
____

📊 Visualizations
Real-time graphs using matplotlib for:

Vibration

AccX, AccY, AccZ

Temperature

Predicted Label (Normal/Abnormal)

Accessible through Flask web interface or Tkinter GUI.
___

🧠 Tech Stack
Hardware: Arduino Uno, SW-420 Vibration Sensor, ADXL345 Accelerometer, Temperature Sensor, Buzzer, LEDs

Software: Python, Flask, Tkinter, TensorFlow/Keras

Models: RNN, LSTM, GRU

Tools: Arduino IDE, Visual Studio Code
___
📌 Future Scope
Use ESP32 for wireless sensor data transmission

Deploy Flask app to cloud (Heroku/AWS)

Add GPS and map-based visual alerts

Build mobile app for instant notifications
___
📩 Contact
For queries or collaboration, reach out to:

ramya003ramya@gmail.com

msharmila030@gmail.com

