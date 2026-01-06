# 🎓 Smart University Fee System (AI Facial Recognition)

A Final Year Project (FYP) that automates university fee collection using **AI Face Recognition**.
This system replaces manual ID checks with biometric login, allows online fee payments, and generates PDF receipts automatically.

---

## 🛠️ Prerequisites (What you need installed)
Before running this project, make sure you have these two installed on your computer:

1.  **Python (v3.8 or later):** [Download Here](https://www.python.org/downloads/)
    * *Note during install:* Check the box **"Add Python to PATH"**.
2.  **Node.js (v14 or later):** [Download Here](https://nodejs.org/)

---

## 🚀 How to Run the Project (Step-by-Step)

### Step 1: Download & Organize Files (Important!)
1.  Click the **Green "Code" button** above and select **Download ZIP**.
2.  Extract (Unzip) the downloaded file.
3.  **Create a new folder** on your desktop (or anywhere) named:
    > **Smart University Fee System**
4.  **Move all the extracted files** (the `backend` folder, `frontend` folder, and any other files) into this new **Smart University Fee System** folder.
5.  Open this **Smart University Fee System** folder in **VS Code** (or your terminal).

---

### Step 2: Setup the Backend (Python)
This handles the Face Recognition and Database.

1.  Open your terminal/command prompt inside the main folder.
2.  Navigate to the **backend** folder:
    ```bash
    cd backend
    ```
3.  Install the required libraries:
    ```bash
    pip install flask flask-cors opencv-python numpy fpdf insightface onnxruntime
    ```
4.  Initialize the Database (Create tables):
    ```bash
    python init_db.py
    ```
    *(You will see a message: "Tables created successfully")*

5.  **Start the Server:**
    ```bash
    python app.py
    ```
    ✅ **Success:** You should see `Running on http://127.0.0.1:5000`.
    *(Keep this terminal open! Do not close it.)*

---

### Step 3: Setup the Frontend (React)
This handles the User Interface (Website).

1.  Open a **NEW** terminal window (keep the Python one running).
2.  Navigate to the **frontend** folder:
    ```bash
    cd frontend
    ```
3.  Install the dependencies (This installs React, Axios, etc.):
    ```bash
    npm install
    ```
    *(This might take 1-2 minutes. Wait for it to finish.)*

4.  **Start the Website:**
    ```bash
    npm start
    ```
    ✅ **Success:** Your browser will automatically open `http://localhost:3000`.

---

## 📖 User Guide (How to Use)

### 1. Register a New Student
* Go to **"New Admission"** on the home page.
* Enter Name, Roll No, Department, etc.
* **Upload a clear photo** of your face.
* Click Register. (The system will assign you a Challan ID and generate a fee bill).

### 2. Student Login (Face ID)
* Go to **"Student Portal"**.
* Enter your **Challan ID** (e.g., `NIDA-11-7`).
* The camera will turn on. **Look at the camera.**
* If your face matches, you will be logged in to your Dashboard.

### 3. Pay Fees & Download Receipt
* On the Dashboard, you will see your **"Current Dues"**.
* Click **"Pay Now"**.
* Once paid, click the **"Receipt"** button to download your PDF.

### 4. Admin Login
* Go to **"Admin Portal"**.
* **Username:** `admin`
* **Password:** `admin123`
* Here you can see total revenue and student lists.

---

## ⚠️ Troubleshooting (Common Errors)

* **Error: `Module not found` in Python?**
    * Make sure you ran the `pip install` command inside the `backend` folder.
* **Error: Website is blank?**
    * Make sure the backend terminal is running `python app.py`.
* **Face not recognizing?**
    * Ensure good lighting when registering and logging in.
    * Ensure you are entering the correct Challan ID.

---

## 📜 License
This project was developed for educational purposes (Final Year Project).
