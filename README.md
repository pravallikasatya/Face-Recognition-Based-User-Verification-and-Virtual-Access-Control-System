<div align="center">

# 🔐 Face Recognition-Based User Verification and Virtual Access Control System

### AI-Powered Facial Identification using Python & OpenCV

![Python](https://img.shields.io/badge/Python-3.x-blue)
![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green)
![Face Recognition](https://img.shields.io/badge/Face-Recognition-purple)
![Google Colab](https://img.shields.io/badge/Google-Colab-orange)

**Capture • Detect • Recognize • Verify**

</div>

---

## 📌 1. Project Overview

The "Face Recognition-Based User Verification and Virtual Access Control System" is
a computer vision project developed using Python, OpenCV, and
face recognition techniques.

The system captures a user's face through a webcam, registers
authorized users, and verifies their identity by comparing the
captured face with previously registered face encodings.

Based on the comparison, the system displays an access-granted
or access-denied result and simulates a virtual door lock.

This project is implemented as a software-based prototype using
Google Colab, with temporary storage during the active session.

---

## 🌍 2. Real-World Problem and Proposed Solution

### 🔴 Real-World Problem

Traditional access verification methods, such as keys, cards,
and passwords, can be lost, forgotten, shared, or misused.

Manual identity verification can also take time and may require
human supervision.

### 🟢 Proposed Solution

This project demonstrates a face-based user verification system
that can:

- Capture a user's face using a webcam.
- Register authorized users.
- Generate facial encodings for recognition.
- Compare a captured face against registered users.
- Display verification results.
- Simulate virtual access granting and denial.
- Maintain temporary access logs during the session.

The prototype demonstrates the concept of facial verification.
It does not physically unlock a door or replace a production-grade
security system.

---

## 🎯 3. Aim and Objectives

### Aim

To develop a webcam-based face recognition and user verification
prototype that identifies registered users and simulates
access control using Python and computer vision.

### Objectives

- To capture face images through a webcam.
- To register and identify authorized users.
- To extract and store facial encodings temporarily.
- To recognize registered users through face comparison.
- To verify user identity and display access decisions.
- To simulate virtual unlocking and relocking.
- To maintain temporary verification and access logs.
- To demonstrate a practical application of computer vision.

---

## 🛠️ 4. Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| OpenCV | Image capture and computer vision |
| Face Recognition | Facial encoding and matching |
| NumPy | Numerical operations and array processing |
| Google Colab | Cloud-based notebook environment |
| JavaScript Webcam Capture | Browser webcam access in Colab |
| Matplotlib | Optional visualization of results |

---
## 🏗️ 5. System Architecture and Workflow

### System Architecture

```text
        ┌───────────────────────┐
        │         User          │
        └──────────┬────────────┘
                   │
                   ▼
        ┌───────────────────────┐
        │ Webcam Image Capture  │
        └──────────┬────────────┘
                   │
                   ▼
        ┌───────────────────────┐
        │ Face Detection        │
        └──────────┬────────────┘
                   │
                   ▼
        ┌───────────────────────┐
        │ Facial Encoding       │
        └──────────┬────────────┘
                   │
                   ▼
        ┌───────────────────────┐
        │ Compare Registered    │
        │ Face Encodings        │
        └──────────┬────────────┘
                   │
                   ▼
        ┌───────────────────────┐
        │ Identity Matched?     │
        └───────┬────────┬──────┘
                │        │
               Yes       No
                ▼        ▼
        ┌────────────┐ ┌────────────┐
        │ Access     │ │ Access     │
        │ Granted    │ │ Denied     │
        └─────┬──────┘ └────────────┘
              │
              ▼
        ┌────────────┐
        │ Virtual    │
        │ Unlock     │
        └─────┬──────┘
              │
              ▼
        ┌────────────┐
        │ Virtual    │
        │ Relock     │
        └────────────┘
```

### Workflow

1. **Initialization:** Import the required libraries and initialize the system.
2. **User Registration:** Capture a face image and register the user's name.
3. **Face Encoding:** Extract and temporarily store the facial encoding.
4. **Verification:** Capture a new image and compare it with registered encodings.
5. **Identity Matching:** Determine whether the captured face matches a registered user.
6. **Access Decision:** Display access granted or denied.
7. **Virtual Access Simulation:** Simulate unlocking and relocking for an authorized user.
8. **Access Logging:** Display verification records from the current session.
## ⚙️ 6. Installation and Execution Instructions

### Requirements

- Python 3
- Google account
- Google Colab
- Webcam-enabled computer
- Internet connection for installing dependencies

### Running the Project in Google Colab

1. Open the project notebook in Google Colab.
2. Install the required libraries:

   ```python
   !pip install opencv-python numpy face-recognition
   ```

3. Import the required libraries and execute the initialization cells.
4. Allow webcam access when prompted by the browser.
5. Register a user by entering a name and capturing a face image.
6. Capture a new image for identity verification.
7. Run the face comparison process and view the verification result.
8. Check the virtual access simulation and temporary access logs.

### Running the Notebook

1. Open the `.ipynb` notebook in Google Colab.
2. Select **Runtime → Run all**, or execute cells in order.
3. Follow the prompts for registration and verification.
4. Grant webcam permission when requested.

**Note:** The project uses temporary session storage. Registered face data may be lost when the Colab runtime is reset or disconnected.

## 🧪 7. Results and Test Cases

The following test cases describe the expected behavior
of the Face Recognition and User Verification System.

| Test Case | Test Scenario | Expected Result | Status |
|-----------|---------------|-----------------|--------|
| TC01 | Register a new user with a detectable face | User registered successfully | ⏳ Pending |
| TC02 | Verify a registered user | Access Granted | ⏳ Pending |
| TC03 | Verify an unregistered user | Access Denied | ⏳ Pending |
| TC04 | Capture an image without a detectable face | No face detected message | ⏳ Pending |
| TC05 | Verify before registering any user | Access Denied | ⏳ Pending |
| TC06 | View access logs | Display current session logs | ⏳ Pending |
| TC07 | Complete the virtual unlock duration | Virtual door relocks automatically | ⏳ Pending |

### 📊 Results

| Metric | Result |
|--------|--------|
| User Registration | To be tested |
| Face Detection | To be tested |
| Face Recognition | To be tested |
| User Verification | To be tested |
| Access Control Simulation | To be tested |
| Access Log Generation | To be tested |

**Note:** Update the status and results after executing
and testing the notebook. These are expected outcomes,
not verified test results.

## ⚠️ 8. Limitations and Future Enhancements
Limitations
- The project is a software-based prototype and does not
  physically control a door.
- Face images and encodings are stored temporarily during
  the active session.
- Data may be lost when the Colab runtime resets.
- Recognition performance may vary with lighting,
  camera quality, facial pose, and image clarity.
- Basic face matching is not equivalent to secure
  biometric authentication.
- The prototype does not include production-grade
  liveness detection or anti-spoofing.
- Webcam access depends on browser permissions and
  device availability.
Future Enhancements
- Implement continuous video-based face recognition.
- Integrate a database for authorized user management.
- Add secure, consent-based enrollment and deletion.
- Implement liveness detection and anti-spoofing.
- Integrate physical access hardware for a controlled
  demonstration.
- Add role-based user access and an administrative interface.
- Improve error handling and verification reporting.
- Deploy the application as a web-based system.

## 👩‍💻 9. Author and Contact Links

**Pravallika Satya Bokka**

B.Tech – Computer Science and Engineering (Data Science)  
Raghu Engineering College, Visakhapatnam

