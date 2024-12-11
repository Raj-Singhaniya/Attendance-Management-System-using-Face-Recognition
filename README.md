
# Attendance Management System using Face Recognition

## Overview
The **Attendance Management System** is a Python-based application that leverages face recognition technology to automate the process of tracking student attendance. This project uses OpenCV for face detection and recognition, along with a user-friendly graphical interface built with Tkinter. It includes features for capturing images for training, real-time face recognition, and managing attendance records efficiently.
# Problem Statement
To develop an automated attendance management system using face recognition technology. The system aims to reduce manual errors, improve attendance accuracy, and ensure the authenticity of student/staff attendance in classrooms or workplaces.
# Software Requirements
Prerequisites
-> Python installed.
-> Required libraries: tinker, tensorflow (or PyTorch), opencv-python, pillow, and numpy.





## Features
- **Face Recognition**: Automatically recognize students' faces and mark their attendance.
- **Image Capture**: Capture and save images for training the recognition model.
- **Manual Attendance**: Option to manually fill attendance records.
- **CSV Export**: Generate attendance reports in CSV format.
- **Database Integration**: Store attendance records in a MySQL database.

# Applications
-> Automated Student Attendance: Track student attendance in real-time during class, reducing manual errors and time spent on roll calls.
  Exam Halls and Assessments: Ensure that only registered students are taking exams, preventing impersonation.
-> Parent-Teacher Communication: Alert parents about their child's attendance via SMS or email notifications.
-> Event Tracking: Monitor student participation in extracurricular activities, seminars, or campus events.
-> Employee Attendance: Automate the clock-in/clock-out process for employees using facial recognition, eliminating the need for manual punch 
   cards or RFID tags.
-> Remote Attendance: For employees working remotely or in hybrid setups, face recognition can verify their attendance from home.


# Future Scope
-> AI-Powered Recognition Models: As face recognition algorithms improve, attendance systems will become more accurate, even in challenging 
   conditions like low lighting, crowded environments, or non-frontal face views.
-> Cloud-Based Systems: Future attendance management systems will increasingly shift to cloud-based platforms, allowing organizations to 
    manage attendance across multiple locations, track remote employees, and access real-time data from anywhere.
->  Mobile Attendance Management: With more powerful mobile devices, face recognition attendance systems could become more portable. Future     
    applications may allow employees or students to mark their attendance using smartphones, reducing the need for fixed hardware like 
    attendance kiosks.

---

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/attendance-management-system.git
cd attendance-management-system
```

### 2. Install Required Packages
Ensure Python is installed on your system, then install the necessary dependencies:
```bash
pip install -r requirements.txt
```

### 3. Set Up MySQL Database
- Create a MySQL database to store attendance records.
- Update the database connection details in the code as needed.

### 4. Download Haarcascade
Download the Haarcascade XML file for face detection from the [OpenCV GitHub repository](https://github.com/opencv/opencv) and place it in the project directory.

---

## Usage

### 1. Capture Images
- Run `main_Run.py` to open the GUI.
- Enter the student's enrollment number and name.
- Click on **"Take Images"** to capture their face images.

### 2. Train the Model
- After capturing images, click on **"Train Images"** to train the face recognition model.

### 3. Automatic Attendance
- Select **"Automatic Attendance"** to start the face recognition process using the webcam.

### 4. Manual Attendance
- Use the **"Manually Fill Attendance"** option to manually fill attendance records.

### 5. View Registered Students
- Access the admin panel to view the list of registered students and their details.

---

## Directory Structure
```plaintext
Attendance Management System using Face Recognition/
│
├── TrainingImage/               # Directory to store training images
├── TrainingImageLabel/          # Directory to save trained model
├── StudentDetails/              # Directory to save student details CSV
├── Attendance/                  # Directory to save attendance records
├── haarcascade_frontalface_default.xml  # Haarcascade file for face detection
├── requirements.txt             # Required Python packages
├── main_Run.py                  # Main application file
├── training.py                  # Script for training the face recognition model
├── testing.py                   # Script for testing face recognition
├── mini_app.py                  # Simple GUI application for capturing images
├── app.py                       # Streamlit app for attendance visualization
└── README.md                    # Project documentation

