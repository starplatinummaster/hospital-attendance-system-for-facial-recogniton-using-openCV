
# Facial Detection Software
  
This project demonstrates a **facial detection and attendance management system** built using Python, OpenCV, and Tkinter, integrating GUI-based user flows for patients, staff, and administrators.

---

## 📖 Introduction
Face detection is a computer vision technology used to locate and identify human faces in digital images or video frames.  
This project leverages **Haarcascade Classifiers (OpenCV)** to detect human faces in real-time via a laptop camera. It also integrates a GUI for user registration and authentication, enabling:

- Staff sign-in and attendance tracking  
- Patient sign-in and specialist consultation booking  
- Administrator access to view and manage records  

The system captures facial features, stores attendance/registration details in CSV files, and ensures a semi-contactless authentication mechanism.

---

## 🖥️ System Requirements
To run the project successfully, the following are required:

- Operating System with **Python 3.7 (32-bit)**  
- **OpenCV** for computer vision and face detection  
- **Tkinter** for GUI interface  
- **NumPy & Pandas** for data handling  
- **winsound** (Windows only, for audio alerts)  
- At least **5 MB of disk space**  
- Laptop/PC with keyboard, mouse, and an in-built/external **camera**

---

## 🔄 Workflow
The system follows the flow:

1. User chooses entry type (Staff / Patient / Administrator / Create Account).  
2. Program activates the camera to detect a face.  
3. If a face is detected:
   - Attendance or registration is recorded in respective CSV files.  
   - An audio beep confirms detection.  
4. Administrators can view staff and patient data.  
5. Patients can book appointments with specialists.  

---

## 🛠️ Features & Functions
### Core Functions
- **`main()`** → Entry point; displays options for staff, patient, admin, and registration.  
- **`Face()`** → Handles facial detection, captures images, and triggers audio feedback.  
- **`Patiententry()` / `staffentry()`** → User login for patients or staff.  
- **`Admin_Space()`** → Restricted access to staff and patient data for administrators.  
- **`createnewwindow()`** → Enables account registration (staff/patient).  

### Data Handling
- Staff details stored in **`doctor.csv`**  
- Patient details stored in **`patient.csv`**  
- Attendance records stored in **`Attendance.csv`**

---

## 📦 Modules Used
- `cv2` → OpenCV face detection (Haarcascades)  
- `winsound` → Audio beep on face detection (Windows only)  
- `tkinter` → GUI interface  
- `numpy` & `pandas` → Data storage and processing  
- `time` & `datetime` → Attendance timestamping  

---

## ▶️ Running the Project
1. Clone or download the project files.  
2. Ensure the following CSV files exist in the root directory:
   - `doctor.csv`
   - `patient.csv`
   - `Attendance.csv`
3. Install dependencies:
   ```bash
   pip install opencv-python numpy pandas
   
4.  **Run the program:**

    ```bash
    python main.py
    ```

5.  **Use the GUI to navigate between:**
    *   Staff sign-in
    *   Patient sign-in
    *   Administrator login
    *   Account creation

---

### 📸 Sample Outputs

*   Staff login screen
*   Patient login and specialist booking
*   Admin dashboard for viewing records
*   Account registration confirmation

---

## 🚧 Constraints & Future Scope

### Current Limitations

*   Only face detection (no recognition yet).
*   Runs primarily on Windows (`winsound` dependency).

### Planned Enhancements

*   Upgrade from detection to face recognition for more robust authentication.
*   Add feedback and rating system for patients post-consultation.
*   Extend to voice authentication using phonocardiography.
*   Integrate emergency alerts (e.g., auto-contacting blood donors).
*   Enhance usability and portability across platforms.


