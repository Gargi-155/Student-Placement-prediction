
# 🎓 Student Placement Prediction System

An end-to-end Machine Learning web application that predicts whether a student is likely to be placed based on academic performance, technical skills, communication ability, resume quality, and placement preparation.

The application is built using **Flask** and powered by a **Random Forest Classifier** trained on placement data. It is fully containerized with **Docker**, making deployment consistent across development and production environments.

---

## 👨‍💻 Author

**Name:** - Gargi
**Course:** - B.Tech Computer Science Engineering
**Registration number** - 23BCE11333

---

## 🚀 Live Demo

**Live Application:**
[https://student-placement-predictor-app-6rll.onrender.com](https://student-placement-prediction-4a1f.onrender.com/)

**GitHub Repository:**
[https://github.com/YOUR_USERNAME/Student-Placement_Predictor_App](https://github.com/Gargi-155/Student-Placement-prediction)

---

# 📌 Features

* Predicts campus placement probability in real time
* User-friendly web interface built with Flask
* Random Forest Machine Learning model
* Dockerized for reproducible deployment
* Production-ready deployment using Render
* Responsive frontend using HTML and CSS

---

# 🛠️ Tech Stack

| Category            | Technology    |
| ------------------- | ------------- |
| Language            | Python 3      |
| Framework           | Flask         |
| Machine Learning    | Scikit-learn  |
| Data Processing     | Pandas, NumPy |
| Model Serialization | Pickle        |
| Web Server          | Gunicorn      |
| Containerization    | Docker        |
| Deployment          | Render        |

---

# 📂 Project Structure

```text
Student-Placement-Predictor/
│
├── static/
│   └── style.css
│
├── templates/
│   └── index.html
│
├── app.py
├── train.py
├── placement_model.pkl
├── requirements.txt
├── Dockerfile
├── .gitignore
└── README.md
```

---

# 📊 Input Features

The prediction model uses the following student attributes:

| Feature              | Description                       |
| -------------------- | --------------------------------- |
| CGPA                 | Academic performance (0–10)       |
| Communication Skills | Communication rating (0–10)       |
| Resume Score         | Resume quality score (0–10)       |
| Coding Score         | Programming proficiency (0–10)    |
| Placement Attendance | Placement training attendance (%) |

---

# 🎯 Model Output

The trained model returns one of two predictions:

| Prediction        | Meaning                          |
| ----------------- | -------------------------------- |
| **Placed 🎉**     | Student is likely to be placed   |
| **Not Placed 😔** | Student is unlikely to be placed |

---

# ⚙️ Running the Project Locally

## 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Student-Placement_Predictor_App.git

cd Student-Placement_Predictor_App
```

---

## 2. Create a Virtual Environment

Using Conda:

```bash
conda create -n placement python=3.10

conda activate placement
```

Or using venv:

```bash
python -m venv venv
```

Activate:

Windows

```bash
venv\Scripts\activate
```

Linux/Mac

```bash
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Train the Model

```bash
python train.py
```

This generates:

```
placement_model.pkl
```

---

## 5. Run the Application

```bash
python app.py
```

Open your browser:

```
http://127.0.0.1:5000
```

---

# 🐳 Docker Deployment

## Build the Docker Image

```bash
docker build -t student-placement-app .
```

## Run the Container

```bash
docker run -p 10000:10000 student-placement-app
```

Visit:

```
http://localhost:10000
```

---

# ☁️ Deployment

The application is deployed on **Render** using Docker.

Deployment workflow:

1. Push changes to the **main** branch.
2. Render automatically detects the update.
3. Docker builds the application image.
4. Gunicorn starts the Flask application.
5. The latest version becomes available online.

---

# 🤖 Machine Learning Pipeline

1. Load placement dataset
2. Perform preprocessing
3. Split training and testing data
4. Train a Random Forest Classifier
5. Serialize the trained model using Pickle
6. Load the model in Flask
7. Generate predictions from user inputs

---

# 📸 Application Preview

*Add screenshots of your application here.*

---

# 📄 License

This project is intended for educational and portfolio purposes.

---

## ⭐ Future Improvements

* User authentication
* Model confidence score
* Performance analytics dashboard
* REST API endpoints
* Multiple ML model comparison
* Database integration
* CI/CD pipeline with GitHub Actions


