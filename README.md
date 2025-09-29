# Assignment03-Flask-and-MongoDB


This project is a simple web application built with Python and the Flask framework. It demonstrates two key functionalities: creating a basic API endpoint and handling web form submissions with a database connection.

## Features

This application is divided into two main parts based on the assignment requirements:

1.  [cite_start]**JSON API Endpoint**[cite: 1]:
    * An API route at `/api` is available via the `GET` method.
    * [cite_start]This endpoint reads a list of user data from a static `data.json` file located in the `backend` directory[cite: 2].
    * [cite_start]It returns the data as a JSON response, as shown in the project screenshot[cite: 44, 46, 49, 63].

2.  [cite_start]**Data Submission Form with MongoDB**[cite: 72]:
    * [cite_start]The main page (`/`) displays a "Signup Page" with a form for a user's name and password[cite: 89, 92].
    * When the form is submitted, the data is sent to the `/submit` route via the `POST` method.
    * [cite_start]The application then inserts the submitted data into a collection in a MongoDB Atlas database[cite: 72].
    * [cite_start]Upon successful submission, the user is shown a success message[cite: 73, 97].

## Technologies Used

* **Backend:** Python, Flask
* **Database:** MongoDB Atlas, PyMongo
* **Frontend:** HTML, CSS

## Setup and Installation

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
    cd your-repository-name
    ```

2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required dependencies:**
    ```bash
    pip install Flask pymongo
    ```

4.  **Configure MongoDB:**
    * Make sure you have a MongoDB Atlas account and a cluster set up.
    * In the `app.py` file, replace the placeholder connection string with your actual MongoDB Atlas connection URI.

5.  **Run the application:**
    ```bash
    python app.py
    ```
    [cite_start]The application will be running on `http://127.0.0.1:5000`[cite: 70].

## How to Use

* **View the API:** Open your browser and navigate to `http://127.0.0.1:5000/api` to see the JSON data.
* **Submit Data:** Open `http://127.0.0.1:5000/` in your browser, fill out the form, and click "Submit". [cite_start]You can then check your MongoDB Atlas collection to see the newly added data[cite: 173, 176, 179].
