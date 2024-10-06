# Patients-No-show-Analysis
## Project Overview
The **No-Show Appointments Analysis** project examines a dataset of medical appointments to identify factors influencing patients missing their scheduled appointments. By analyzing patient demographics, health conditions, and communication factors, the project aims to uncover patterns that can help reduce no-show rates and improve healthcare efficiency.
## Data sourses
- KaggleV2-May-2016.csv
## Tools
- **Programming Language**: Python
- **Libraries**:
  - `pandas` for data cleaning, manipulation, and analysis.
  - `NumPy` for numerical operations.
  - `matplotlib` and `seaborn` for visualizations.
  - `datetime` for handling date-related features.

## Data Cleaning and Preparation
The dataset contains 110,527 rows with features such as patient demographics, appointment scheduling details, and health-related information. The following steps were taken to clean and prepare the data:
1. **Irrelevant Columns**: Dropped columns like 'PatientId' and 'AppointmentID', which were not necessary for the analysis.
2. **Handling Missing Data**: No significant missing data required imputation.
3. **Age Correction**: Removed one row with a negative age value.
4. **Date Conversion**: Converted the 'ScheduledDay' and 'AppointmentDay' columns to datetime objects for easier manipulation.
5. **Feature Engineering**: Created a new column to calculate the difference in days between the scheduling date and the appointment date.

## Exploratory Data Analysis (EDA)
Exploratory Data Analysis was conducted to understand the relationships between different factors and the likelihood of missing an appointment. Key analysis steps included:
- Visualization of attendance patterns based on various medical conditions (e.g., hypertension, diabetes, alcoholism).
- Investigating the impact of SMS reminders on appointment attendance.


## Data Analysis
Several key factors were analyzed to determine their influence on no-show appointments. These include:
1. **Disabilities**: Patients with multiple disabilities showed a higher probability of missing their appointments, though the sample size of such patients was small.
2. **Chronic Health Conditions**: Patients without hypertension or diabetes were more likely to miss their appointments.
3. **SMS Reminders**: Surprisingly, patients who received SMS reminders were about 10% more likely to miss their appointments.

## Results
The key findings from the data analysis are as follows:
1. Patients with four disabilities are the most likely to miss appointments, although the sample size for this group is relatively small.
2. Patients without hypertension and those without diabetes are more prone to missing their appointments.
3. Unexpectedly, patients who received SMS reminders were more likely to miss their appointments compared to those who did not receive reminders.

## Recommendations
1. **Disability and Chronic Conditions**: Tailor interventions for patients with multiple disabilities and those without chronic conditions like hypertension or diabetes, as they show a higher no-show rate.
2. **SMS Effectiveness**: Reassess the effectiveness of SMS reminders as they currently seem to be associated with higher no-show rates.
3. **Future Research**: Expand the analysis to include larger datasets and longer time frames to validate the findings and generate more comprehensive insights.

## Limitations
1. **Time Frame**: The dataset covers a short period from November 2015 to June 2016, limiting the ability to generalize the results over time.
2. **Sample Size**: The dataset is relatively small, which may limit the accuracy of the conclusions and patterns drawn.
3. **Frequent No-Show Patients**: Further investigation is needed into patients with a history of frequent no-shows to understand their behavior better.
4. **Feature Granularity**: Some potentially influential features (e.g., the severity of the condition or socioeconomic status) were not included in the dataset.
