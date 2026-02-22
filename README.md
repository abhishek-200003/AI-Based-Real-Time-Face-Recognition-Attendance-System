📌 Overview

SmartAttend is a real-time face recognition attendance system built using Python and computer vision techniques. The system detects and recognizes faces from a live webcam feed and automatically records attendance with timestamps in a CSV file while preventing duplicate entries during a session.

🎯 Problem Statement

Manual attendance tracking is time-consuming and prone to manipulation.
This project automates attendance marking using facial recognition, reducing human effort and improving reliability.

⚙️ How It Works

Pre-registered images are loaded and encoded.

The webcam captures live video.

Faces are detected and encoded in real-time.

Encodings are compared using distance-based matching.

If a match is found:

The name is displayed.

The current timestamp is recorded.

Attendance is written to a CSV file.

Duplicate entries are prevented within a single session.

🛠️ Tech Stack

Python

OpenCV

face_recognition (dlib-based model)

NumPy

CSV (for attendance storage)

📂 Project Structure
SmartAttend/
│── mark.ipynb
│── attendance.csv
│── requirements.txt
│── README.md
│── images/
│    └── .gitkeep
📥 Training Images Setup

Create a folder named images/ in the project directory.

Place one image per person inside the folder.

Example:

images/
│── Dev.jpg
│── Karthick.jpg
│── Michael.jpg

The file name should match the person's name.
The system extracts names from file names automatically.

🔐 Privacy Notice

For privacy and ethical reasons, real training images are not included in this repository.

Facial images are considered biometric data.
Users must provide their own images with proper consent before using the system.

This repository is intended for educational and demonstration purposes only.

🚀 Installation

Clone the repository:

git clone <your-repository-link>

Install dependencies:

pip install -r requirements.txt

Add your training images to the images/ folder.

Run the program:

python mark.py
✨ Features

✔ Real-time face detection
✔ Face encoding and recognition
✔ Automatic timestamp logging
✔ Duplicate attendance prevention
✔ Lightweight CSV-based storage



📄 License

This project is created for educational and demonstration purposes.

Now let me challenge you a bit:

Right now your system prevents duplicates only
