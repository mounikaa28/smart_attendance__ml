# Smart Attendance ML – Attendance Prediction System

## About the Project

Smart Attendance ML is a machine learning-based attendance prediction system designed to help college students monitor their attendance and understand their attendance trends.

In many colleges, attendance records are updated periodically, making it difficult for students to track their current attendance and determine how many more classes they need to attend to reach the required attendance percentage.

This project aims to simplify attendance monitoring by providing attendance calculations, trend analysis, and machine learning-based predictions to help students make informed decisions.

## Objectives

- Calculate the current attendance percentage.
- Compare current and previous attendance records.
- Analyze changes in attendance over time.
- Estimate the number of additional classes required to reach a target attendance percentage.
- Use machine learning to support attendance prediction.
- Identify attendance risk levels based on the implemented criteria.
- Provide a simple and user-friendly interface for attendance monitoring.

## Features

- **Attendance Calculation:** Calculates attendance percentage using available attendance data.
- **Attendance Comparison:** Compares attendance across different periods.
- **Attendance Trend Analysis:** Shows changes in attendance over time.
- **Target Attendance Estimation:** Helps estimate the number of classes required to reach a target percentage.
- **Risk Assessment:** Identifies attendance risk levels according to the application's rules.
- **Machine Learning Integration:** Uses a trained machine learning model for attendance-related predictions.
- **Backend API:** Connects the application with the machine learning service.

## Technologies Used

- **Frontend:** [Add your frontend technology]
- **Backend:** Node.js and Express.js
- **Machine Learning Service:** Python and FastAPI
- **Model Storage:** Pickle (`.pkl`)
- **API Server:** Uvicorn
- **Version Control:** Git and GitHub

## System Architecture

The system consists of a user interface, a backend API, and a machine learning service.

1. The user enters the required attendance information.
2. The backend processes the request.
3. The machine learning service receives the required input.
4. The trained model generates a prediction when applicable.
5. The application displays the attendance information and supported results to the user.

## Machine Learning Model

The project uses a trained machine learning model stored in the following location:

`ml-service/models/smart_attendance_model.pkl`

The model is loaded by the machine learning service to generate predictions based on the features used during training.

Model performance can be evaluated using metrics such as R² score, Root Mean Squared Error (RMSE), and Mean Absolute Error (MAE), where appropriate. Actual evaluation values should be added after testing the model on suitable test data.

## Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Munazza-08/Smart_Attendance_ML.git
```

### 2. Navigate to the Project Directory

```bash
cd Smart_Attendance_ML
```

### 3. Set Up the Machine Learning Service

Navigate to the directory containing the FastAPI application and install its dependencies.

```bash
pip install -r requirements.txt
```

Create and activate a Python virtual environment if required.

### 4. Start the Machine Learning Service

Run the following command from the directory containing the appropriate FastAPI entry point:

```bash
uvicorn main:app --reload --port 8000
```

The service will run at `http://localhost:8000` if the application starts successfully.

If interactive API documentation is enabled, it can be accessed at `http://localhost:8000/docs`.

### 5. Start the Backend

Navigate to the backend directory, install the dependencies, and start the application using the scripts defined in its `package.json`.

```bash
npm install
npm start
```

### 6. Start the Frontend

Navigate to the frontend directory and install the required dependencies.

```bash
npm install
npm run dev
```

Open the local URL displayed in the terminal.

**Note:** The commands and directory names should match the actual project structure and configuration.

## Example Attendance Analysis

An illustrative example of attendance analysis is shown below.

| Metric | Example Value |
|---|---:|
| Current Attendance | 66.67% |
| Previous Attendance | 70.00% |
| Change in Attendance | -3.33 percentage points |
| Target Attendance | 75% |
| Attendance Risk | At Risk |

These values are examples only. Actual results depend on the attendance data provided and the application's calculations.

## Applications

- Helps students monitor their attendance.
- Supports attendance planning throughout the semester.
- Provides insights into attendance trends.
- Helps students identify potential attendance risks.
- Demonstrates the application of machine learning to an educational problem.

## Future Enhancements

- Subject-wise attendance analysis.
- Improved monthly attendance predictions.
- Attendance trend visualizations.
- Enhanced model evaluation and validation.
- Improved API error handling.
- Additional testing and deployment improvements.

These are potential future improvements and may not be implemented in the current version.

## License

No license has been specified yet. A suitable license can be added if the project is intended for open-source distribution.

---

**Smart Attendance ML — Making attendance tracking more informative through machine learning.**
