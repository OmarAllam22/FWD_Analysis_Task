# FWD_Analysis_Task:
A data analysis task during my Future Work is Digital Scholarship provided by the Egyptian Ministry of Communications and Information Technology.
_________________________________
## 1- Dataset Description:
- This dataset collects information from 100k medical appointments in Brazil and is focused on the
question of whether patients show up for their appointment. Several characteristics about the patient
are included in each row.
- The data has 110527 rows and 14 columns.
_______________
## 2- InMind Questions:
- General Questions related to the existence of:
1. missing values?
2. wrong datatypes for columns?
3. complete duplicates in the data?
4. outliers in each column?

- Univariate Questions:

1. Which `Gender` is more healthier than the other depending on number of enteries?
2. Which `Age` values are valid or there are values like 1000..,etc?
3. Which disease among `Hipertension`, `Diabetes` and `Alcoholism` is most dominant?

- Bivariate Questions:
1. Is the number of `PatientId` same as `AppointmentID` or may be more than one
appointment for the same patient?
2. Does Receiving `Scholarship` has strong effect on not cancelling the appointment or
not?
3. Does the period between `AppointmentDay` and `ScheduleDay` has effect on cancelling
the appointment?
_______________
## 3- Conclusion:
### 1. Reached Results:
I went through a 110527-row and 14-column dataset about medical 
appointments inBrazil to discover which features affects the meeting being
Canceled or not.
#### First, the data must be cleaned and I:
1. dropped `AppointmentID` and `HandCap` Columns.
2. replaced `PatientId` values with `0 -> 62298` values.
3. renamed `No-show` to `Canceled` for avoiding confusion.
4. changed the datatypes for `Scholarship`, `Hipertension`, `Diabetes`, `Alcoholism` and
`SMS_received`.
5. replaced wrong values in the `Age` column.
#### Then, I came with some insights from the analysis that:
1. In our sample, `Females` care with their health more than `Males` as they reserved 
moreappointments.
2. The most dominant disease in our sample is `Diabetes`.
3. % of `Alcohol` additction is, by far, higher in `Males` than `Females`.
4. Receiving `Scholarship` has strong effect on not cancelling the appointment.
5. Longer`ReservationPeriod` _period between `AppointmentDay` and `ScheduledDay`
contributes to those cancelled appointments.
6. `Gender` has no notable effect on cancelling appointments.
#### After that, I concluded the main objective that:
Receiving financial `Scholarship` & getting shorter `ReservationPeriod` for the 
appointment arethe most two features that may tend to lower the number of Canceled
appointments
### 2. Limitations:
1. `Handcap` has no documentation in the kaggle description & its name has no translation so 
it may be important but we cannot understand it.
2. Discription of data on kaggle shows that `SMS_received` is a field indicates number of 
message received but in this data it is only binary field with either **0** or **1** which 
may reflect misleading understand.
(Thanks
