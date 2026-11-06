# Moods and Stresses (Power Apps)

As a health care provider, we are concerned about the moods and stress levels of our patients. We want to use our data to understand how many patients may not be doing well based on their daily check-ins.

## Data Dictionary

### Patients

The [patients.csv](patients.csv) file contains one row per patient.

| Field | Description |
| --- | --- |
| `external_patient_id` | Unique identifier for the patient |
| `user_name` | Patient's username |
| `full_name` | Patient's full name |

### Daily Check-ins

The [daily_checkins.csv](daily_checkins.csv) file contains patients' daily mood and stress readings.

| Field | Description |
| --- | --- |
| `external_checkin_id` | Unique identifier for the check-in |
| `external_patient_id` | Identifier linking the check-in to a patient in `patients.csv` |
| `checkin_date` | Date of the check-in |
| `mood` | Mood rating from 1 (very bad) to 5 (great) |
| `stress` | Stress rating from 1 (low stress) to 5 (very stressed) |

## Assignment

1. Upload or import both provided CSV files into a data source that can be used by Power Apps.
2. Build a Power Apps app that uses the uploaded data to answer this question:

   **How many patients had two or more bad days during the week beginning May 7, 2017?**

   For this assignment:

   - A patient has a **bad day** when either:
     - their mood rating is 1 or 2; or
     - their mood rating is 3 and their stress rating is 4 or 5.
   - Each patient should be counted no more than once.
3. The app must clearly display the resulting number of patients. How you design the rest of the app is up to you.
