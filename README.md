# Attendance Management System 📚🎥✨  

### Overview 🌟  
Take student attendance to the next level! This system uses **facial recognition technology** to make attendance management seamless and efficient. With an intuitive GUI for administrators and integration with a MySQL database, tracking attendance has never been easier.  

💡 **Features at a Glance:**  
- 🚀 **Facial Recognition**: Leveraging OpenCV and face_recognition libraries.  
- 🗂️ **Database Integration**: All data stored securely in MySQL.  
- 📸 **Real-Time Monitoring**: Attendance marked using a live camera feed.  
- 🖥️ **Admin Dashboard**: Manage records effortlessly via a user-friendly GUI.  
- 📊 **Exportable Logs**: Attendance history saved in CSV format for easy access.  

---

## Technologies Used 🛠️  
- **Python 3.x** 🐍  
- **OpenCV** 🖼️ for image processing  
- **face_recognition** 👤 for matching faces  
- **MySQL** 🗃️ for database management  
- **Tkinter** 🖱️ for GUI design  
- **Pillow (PIL)** 📷 for handling images  

---

## Database Structure 🗃️  

### 📝 **`Atnd` Table:**  
| Column       | Description                  |  
|--------------|------------------------------|  
| **Name**     | Student's Name               |  
| **Time**     | Date and time of attendance  |  
| **RollNo**   | Student's unique identifier  |  

### 🎓 **`Course` Table:**  
| Column         | Description                  |  
|----------------|------------------------------|  
| **CourseID**   | Unique Course Identifier     |  
| **RollNo**     | Reference to the student     |  
| **Course_Name**| Name of the course           |  

### 🔗 **`Enrollment` Table:**  
| Column            | Description                  |  
|-------------------|------------------------------|  
| **Enrollment_ID** | Unique enrollment number     |  
| **RollNo**        | Reference to the student     |  
| **CourseID**      | Linked course identifier     |  

### 📋 **`Student_information` Table:**  
| Column          | Description                       |  
|-----------------|-----------------------------------|  
| **RollNo**      | Student’s unique identifier       |  
| **Name**        | Student’s full name              |  
| **CourseID**    | Linked course identifier          |  
| **EnrollmentID**| Linked enrollment identifier      |  
| **Attendance**  | Attendance percentage            |  

---

## How It Works ⚙️  
1. 📷 **Capture Faces**: Webcam detects faces in real-time.  
2. 🔍 **Match Faces**: Compares captured faces with pre-stored images.  
3. ✅ **Mark Attendance**: Matches are logged into the database.  
4. 👀 **Blink Detection**: Ensures students are present and attentive.  
5. 🖥️ **Admin Controls**: Modify or review attendance via GUI.  

---

## Requirements 📦  
Install the following libraries:  
- **OpenCV**: `pip install opencv-python`  
- **face_recognition**: `pip install face_recognition`  
- **MySQL Connector**: `pip install mysql-connector-python`  
- **Pillow**: `pip install pillow`  

💡 **Pro Tip**: Tkinter usually comes pre-installed with Python!  

---

## Getting Started 🚀  

1. 🛠️ **Setup**: Configure your MySQL database and create tables (SQL provided in the script).  
2. 📁 **Prepare Data**: Add known face images in the `faces_known` directory.  
3. ▶️ **Run the System**: Execute the Python script to start managing attendance!  

---

## Future Upgrades 🚀🔮  
- 📱 **Instant Alerts**: Notify students in real-time when their attendance is marked.  
- 🌈 **Better Recognition**: Improve facial recognition under varying lighting conditions.  
- 🖥️ **Online Portal**: Integrate with an online platform for broader accessibility.  

---

### Created With ❤️ By:  
**Avishikar Kannan N** 👨‍💻
