# 📚 BookRec-Summarizer: AI-Powered Book Discovery

An intelligent system designed to enhance the reading experience by providing personalized book recommendations and instant, concise summaries. Leveraging machine learning, this project helps users discover new books tailored to their tastes and quickly grasp the essence of any title, making informed choices faster.

<img width="1600" height="813" alt="image" src="https://github.com/user-attachments/assets/d6ebe51f-2c7e-4bd0-b838-192bafc4eca6" />


## ✨ Key Features

-   **Personalized Recommendations:** Employs a Scikit-learn based machine learning model to suggest books based on user preferences and reading history.
-   **Instant Summaries:** Implements a text summarization feature to provide quick, concise insights into a book's content.
-   **Hybrid Backend:** Utilizes a powerful combination of **Flask** for serving the ML model and **Node.js** for handling primary backend logic and API requests.
-   **Clean & Interactive Frontend:** A user-friendly interface built with HTML, CSS, and JavaScript for a smooth and intuitive user experience.

## ⚙️ How It Works: Architecture Overview

This project uses a microservice-oriented architecture to separate concerns and ensure scalability.

1.  **Frontend (HTML/CSS/JS):** The user interacts with this clean interface to search for books or get recommendations.
2.  **Node.js Backend (Main Server):** Acts as the primary API gateway. It handles user-facing requests, manages routing, and communicates with the Flask microservice for ML-specific tasks.
3.  **Flask Backend (ML Microservice):** A dedicated Python service that hosts the recommendation and summarization models. It exposes simple API endpoints that the Node.js server can call to get predictions or summaries.

```

[User] \<--\> [Frontend] \<--\> [Node.js API Gateway] \<--\> [Flask ML Service]

````

## 🛠️ Technology Stack

-   **Frontend:** `HTML5`, `CSS3`, `JavaScript`
-   **Backend:** `Node.js`, `Flask`
-   **Machine Learning / Data Science:** `Scikit-learn`, `Pandas`, `NumPy`
-   **Database:** `(Specify your database, e.g., MongoDB, PostgreSQL, or state if using flat files like CSV)`

## 🚀 Getting Started

Follow these instructions to set up and run the project on your local machine.

### Prerequisites

Make sure you have the following installed:
-   Node.js & npm (v18.x or later)
-   Python (v3.9 or later) & pip
-   Git

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/your-github-username/your-repo-name.git](https://github.com/your-github-username/your-repo-name.git)
    cd your-repo-name
    ```

2.  **Set up the Flask ML Service (Python):**
    ```sh
    # Navigate to the Flask backend directory
    cd flask-backend

    # Create and activate a virtual environment
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

    # Install Python dependencies
    pip install -r requirements.txt

    # Start the Flask server (usually runs on [http://127.0.0.1:5000](http://127.0.0.1:5000))
    flask run
    ```
    *Note: You may need to create a `requirements.txt` file by running `pip freeze > requirements.txt` after installing Flask, Pandas, NumPy, and Scikit-learn.*

3.  **Set up the Main Server (Node.js):**
    (Open a new terminal window)
    ```sh
    # Navigate to the Node.js backend directory
    cd node-backend

    # Install npm dependencies
    npm install

    # Start the Node.js server (usually runs on http://localhost:3000)
    npm start
    ```

4.  **Launch the Frontend:**
    The frontend is served by the Node.js server. Open your browser and navigate to:
    **http://localhost:3000**

You should now have the application running locally!

## 📁 Project Structure

````

.
├── flask-backend/          \# Python Flask ML Service
│   ├── app.py              \# Main Flask application
│   ├── models/             \# Saved ML models (.pkl files)
│   ├── data/               \# Datasets (e.g., .csv files)
│   └── requirements.txt    \# Python dependencies
│
├── node-backend/           \# Node.js Main Server
│   ├── server.js           \# Main server file
│   ├── routes/             \# API routes
│   ├── package.json        \# Node.js dependencies
│   └── ...
│
├── frontend/               \# Frontend files
│   ├── index.html
│   ├── style.css
│   └── script.js
│
└── README.md               \# This file

```

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project.
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the Branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

## 📧 Contact

AYUSH SAINI- (https://www.linkedin.com/in/ayush-saini-2579a6265/) - ayushsaini7033@gmail.com

Project Link: [https://github.com/ayushsa24/book-recommendation-summarization.git]

```
