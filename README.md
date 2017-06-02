# How To Run
## Setting Up WebSide server locally
See [README](https://github.com/AdherencePillProject/WebSide/blob/master/AdherencePillProject/README.MD) file of WebSide

## Setting Up web_cloud app locally
See [README](https://github.com/AdherencePillProject/web_cloud/blob/master/README.md) file of web_cloud

## Setting Up Android app
1. Install [Android Studio](https://developer.android.com/studio/index.html)
2. Download the [Android project](https://github.com/AdherencePillProject/ADP_Android)
3. See README file of Android app


# Roadmap

## Introduction
We have achieved most of functionalities on Android part, while a good amount of jobs on website are not work now, which is the main direction that we want to work forwards. In the following weeks, we hope we can achieve the following milestones:
1. **Make sure the correctness of data-binding**
2. **Ensure the validation of key services/executions**
3. **Optimize UI to improve user experience**




## Milestone 1: Correctness of data-binding
First, we should check the correctness of data-binding across the app. In this section, we focus on verifying the displayed data should be the same, without considering the validation of executions. 

**[User](Data-binding/User.md)**
- [ ] web/login
- [ ] Android/login
- [ ] Database/User

**Doctor-Patient relation**
- [ ] Doctor/Doctor home
- [ ] Doctor/Patient Prescription
- [ ] Doctor/Patient Graph
- [ ] Database/PatientDoctor


**Appointment**
- [ ] Doctor/Doctor Home
- [ ] Patient/Appointment
- [ ] Database/Appointment


**Patient’s Prescription (Specific time in current day) (HH:mm:ss)**
- [ ] Doctor/Patient Graph
- [ ] Doctor/Patient Prescription
- [ ] Patient/Patient Home
- [ ] Patient/Medcine Cabinet
- [ ] Android/TodayFragment
- [ ] Database/Prescription


**Patient’s Prescription (Schedule) (yy:MM:dd)**
- [ ] Doctor/Patient Graph
- [ ] Doctor/Patient Prescription
- [ ] Android/Calendar
- [ ] Database/Prescription


**Patient’s Medicine**
- [ ] Patient/Medcine Cabinet
- [ ] Android/MedcationFragment
- [ ] Database/Prescription - Patient - Bottle


**BottleUpdate**
- [ ] Patient/Patient Home
- [ ] Android/TodayFragment
- [ ] DatabaseUpdates




**REST API**


GET
- [ ] /logout
- [ ] /account/email
- [ ] /account/password
- [ ] /doctor/patients
- [ ] /doctor/patients/prescription
- [ ] /doctor/appointments
- [ ] /patient
- [ ] /patient/appointment
- [ ] /patient/prescription
- [ ] /patient/pills


POST
- [ ] /login
- [ ] /doctor
- [ ] /doctor/patient/prescription
- [ ] /doctor/appointment
- [ ] /patient
- [ ] /patient/appointment


PUT
- [ ] /account/password
- [ ] /account/info


DELETE
- [ ] /doctor/patient/prescription




## Milestone 2: Validation of Key Services/Executions
Second, we need to check the validation of app’s service. This section should take a week.


**Make Appointment**
- [ ] Doctor/Doctor Home
- [ ] Patient/Appointment
- [ ] Database/Appointment




**Add/Delete Prescription**
- [ ] Doctor/Patient Prescription
- [ ] Patient/Patient Home
- [ ] Patient/Medcine Cabinet
- [ ] Android/TodayFragment
- [ ] Database/Prescription


**User**
- [ ] web/login (the window of user type does not work)
- [ ] web/sign up
- [ ] forget password
- [ ] Android/login
- [ ] Database/User


**Notification Of Prescription**
- [ ] Android/AlertService
- [ ] Android/TodayFragment


**Update Pill Taken Data**
- [ ] Android/ZentriService
- [ ] Android/NextAtivity/onClick
- [ ] Database/Update
- [ ] Android/TodayFragment UI


## Milestone 3: UI Optimization
Third, we will move to optimize UI to improve UX. Following are parts of UI elements we are supposed to add. We may need to decide to add more UI elements in two weeks.


**Android/TodayFragment**
- [ ] Categorize data into four groups: morning, afternoon, evening, bedtime
- [ ] Add interval bars


**web_cloud/Patient/Patient Home**
- [ ] Categorize data into four groups: morning, afternoon, evening, bedtime
- [ ] Add interval bars


**web_cloud/doctor/Patient Graph**
- [ ] search bar
- [ ] prescription view (optimize y axis)


**web_cloud/doctor/Patient Prescription**
- [ ] search bar


**web_cloud/doctor/Doctor Home**
- [ ] search bar
- [ ] number of entries
- [ ] threshold value





## Future Works
In the future (probably July), after we finish above basic functionalities, we want to add some new features. Generally, we will focus on three directions:

1. **Database migration and improvement**
- [ ] migrate to AWS
- [ ] In database, store dosage and prescription name separately, update patient prescriptions page (and other relevant pages?) accordingly
- [ ] Larger database
- [ ] 10-15 patients for doctor


2. **Implement other data-binding circles**
- [ ] Display schedule on Android
- [ ] Display patient’s doctor on Android
- [ ] Show reasonable list of medication
- [ ] Doctor home table should display medication adherence %


3. **Write unit test classes**
- [ ] Write Junit test classes for activities in Android
- [ ] Write unit test classes for services in web_cloud 
- [ ] Write unit test classes for controllers and routes in WebSide


4. **Add new features:**
- [ ] Implement local database in mobile
- [ ] Add setting on Android
- [ ] Add setting on web_cloud
- [ ] Doctor’s suggestion should have menu options
