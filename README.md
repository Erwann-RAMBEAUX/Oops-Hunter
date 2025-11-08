# Oops Hunter - Sensitive Data Leak Detector

![Python](https://img.shields.io/badge/Python-3.11-blue.svg)
![Flask](https://img.shields.io/badge/Flask-black.svg)
![Tesseract](https://img.shields.io/badge/Tesseract-OCR-lightgrey.svg)
![Status](https://img.shields.io/badge/Status-Academic%20Project-lightgreen.svg)

A web application designed to analyze documents and detect the presence of sensitive data. This project provides a detailed analysis history and assigns a risk score to users based on their submissions.

> **Note:** This is a group academic project developed as part of the PPII (Multidisciplinary IT Engineering Project) module at Télécom Nancy.

## Table of Contents
1. [Key Features](#key-features)
2. [Technologies Used](#technologies-used)
3. [Prerequisites](#prerequisites)
4. [Installation](#installation)
5. [Running and Usage](#running-and-usage)

---

## 🎯 Key Features

* **Document Analysis:** Detects the presence of sensitive data (configurable) in uploaded files.
* **Supported File Types:** `.pdf`, `.md`, `.docx`, `.xlsx`, `.txt`.
* **Analysis History:** Maintains a detailed log of all analyses performed by users.
* **User Risk Scoring:** Assigns a score to users based on the number of documents with data leaks they have submitted.
* **Admin Panel:** Allows for managing user accounts and configuring the types of sensitive data to search for.
    * *Note: In the current version, only the addition of new data types based on regex algorithms is fully functional.*

## 🛠️ Technologies Used

* **Backend:** Python, Flask
* **Frontend:** HTML, CSS, Bootstrap
* **OCR (Optical Character Recognition):** Tesseract
* **Python Dependencies:** See `requirements.txt`

## 📋 Prerequisites

Before you begin, ensure you have the following installed on your system:

* **Python** (v3.11.5 or higher)
* **Tesseract OCR**
    * Follow the [official documentation](https://tesseract-ocr.github.io/tessdoc/Installation.html) to install it on your operating system.

## 🚀 Installation

Follow these steps to set up the development environment:

1.  Clone this repository to your local machine:
    ```bash
    git clone https://github.com/Erwann-RAMBEAUX/Oops-Hunter
    ```

2.  Create and activate a Python virtual environment:
    ```bash
    # Create the environment
    python -m venv venv
    
    # Activate on macOS/Linux
    source venv/bin/activate
    
    # Activate on Windows (PowerShell/CMD)
    .\venv\Scripts\activate
    ```

3.  Install the required Python dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## ▶️ Running and Usage

1.  Launch the Flask application from your terminal:
    ```bash
    flask --app index run
    ```

2.  Open your browser and navigate to `http://127.0.0.1:5000` (or the address shown in your terminal).

3.  Log in with one of the demo accounts:

    **Account 1:**
    * **Email:** `antoine.delacroix@gmail.com`
    * **Password:** `password`

    **Account 2:**
    * **Email:** `marie.dubois@gmail.com`
    * **Password:** `securepass`

4.  Use the interface to add a document and click "Analyze".
5.  View the analysis results or navigate to the history to see past scans.
6.  Explore the "Administration" section to manage accounts and data types.
