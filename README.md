# Doctolib Test

## Instructions A sunderstood from the guidlelines :
This code provides an algorithm that checks the availabilities of an agenda depending of
the events attached to it by checking availability on opening dates and if opening days are recurring weekly and exclude reserved times,
The main method has a start date for input and is looking for the availabilities of the next 7 days.

They are two kinds of events:
 * `opening`, are the openings for a specific day and they can be recurring week by week.
 * `appointment`, times when the doctor is already booked.
 
 So I did the following :
 
  * **Step 1**: I changed the order of events to be applying opening dates before reserving the appointments, to fix the issues for test.
  * **Step 2**: I assumed that there is no appoitment can be reserved from 12:30 to 13:00 so the result should be 9:30,10:00,11:30,12:00.
  * **Step 3**: Regarding to Test Case no 3 , the opening day was 2018 and recurring week is true , and the checking the availabiity on                   day 2014 that is the same day of the week , so the result showed the all day available and I modified the test case to fit                 with date .
  * **Step 4**: Allow the function to return availabilities on as many days as requested


