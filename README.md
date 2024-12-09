# ST10459259WALCIRESFERNANDO_IMAD_PRATICUM
The **World of student life** is a simple Android application designed to making budget management an engaging way for students to track and control their daily experience.


## **Features**
- **Splash Screen**: A welcoming screen with options to start the app or exit.
- **Main Screen**:
  - Input and save your morning and afternoon run distances.
  - Add notes for each entry.
  - Calculate the average Spent days
  - Navigate to a detailed summary of all recorded runs.
  

## **Pseudocode**
#### **Splash Screen**
1. Display app name, student name, and student number.
2. Show logo.
3. Provide two buttons:
   - **Start**: Navigate to the Main Screen.
   - **Exit**: Close the app.
   - 
4. Wait for user interaction.
#### **Main Screen**
1. Display input fields:
   - Morning run distance.
   - Afternoon run distance.
   - Notes.
2. Show buttons:
   - **Submit**:
     1. Validate inputs.
     2. Save input data in arrays:
        - Morning speding array.
        - Afternoon speding array.
        - expense Notes array.
     3. Clear input fields.
   - **Clear**:
     - Reset input fields to empty.
    
      

1. **Calculate Average Spending**:
   - Initialize variables:
     - totalSpending = 0
     - daysWithData = number of days with input data
   - For each day:
     - Get morning and afternoon spending values
     - If the values are valid (not null or empty):
       - Add morning and afternoon spending to totalSpending
     - Otherwise:
       - Display error message "Please fill in all fields!"
   - Calculate the average spending:
     - averageSpending = totalSpending / daysWithData
   - Display the average spending:
     - Show "Average Spending: R$ {averageSpending}"

2. **View Details**:
   - When the "View Details" button is pressed:
     - Navigate to the details screen
     - Pass the data for the days, morning and afternoon spending, and expense notes to the details screen

3. **Handle Invalid Inputs**:
   - If the user leaves a field empty or enters a non-numeric value:
     - Display an error message "Please fill in all fields correctly!"


Usage
Splash Screen:
Press Start to proceed to the main screen.
Press Exit to close the app.
Main Screen:
Enter your morning and afternoon spending amounts and any notes.
Press Submit to save the data.
Press Clear to reset the input fields.
Press Calculate Average to view the average spending.
Press View Details to see a summary of all spending data.
Detailed View Screen:
View all recorded spending data in a scrollable list.
Press Back to Main to return to the main screen.

## **Pseudocode**##

Splash Screen
Display app name, student name, and student number.
Show logo.
Provide two buttons:
Start: Navigate to the Main Screen.
Exit: Close the app.
Wait for user interaction.
Main Screen
Display input fields:
Morning spending amount.
Afternoon spending amount.
Notes.
Show buttons:
Submit:
Validate inputs.
Save input data in arrays:
Morning spending array.
Afternoon spending array.
Notes array.
Clear input fields.
Clear:
Reset input fields to empty.
Calculate Average:
Loop through morning and afternoon spending arrays.
Compute the total spending.
Divide the total spending by the number of days to get the average.
Display the average spending.

View Details:
Navigate to the Detailed View Screen.
Handle invalid inputs by displaying an error message.
Detailed View Screen
Retrieve and display:
Day-wise morning spending amount.
Day-wise afternoon spending amount.
Notes for each day.
Provide navigation:
Back: Return to the Main Screen.
Data Handling
Use parallel arrays:
Morning spending: morningSpending[].
Afternoon spending: afternoonSpending[].
Notes: notes[].
Use loops:
To iterate through arrays and compute the weekly average spending.
To display detailed spending data.
Navigation Logic
Splash Screen:
If "Start" is clicked, open Main Screen.
If "Exit" is clicked, close the app.

Main Screen:
If "View Details" is clicked, open Detailed View Screen.
Detailed View Screen:
If "Back" is clicked, return to Main Screen.
Error Handling
For input fields:
If morning or afternoon spending is empty or not a number, display an error message.
For calculating average:
Ensure arrays are not empty before calculating.
For navigation:
Prevent navigation if critical data is missing.


## **Technologies Used**
- **Kotlin**: Programming language for Android development.
- **Android SDK**: Tools and libraries for building Android applications.
- **Android Studio**: Integrated development environment (IDE) for Android.


## **Screenshots**
### 1. **Splash Screen**
![image](https://github.com/user-attachments/assets/fc39909b-2aea-4e9c-975c-7952f60d19c5)


### 2. **Main Screen**
![image](https://github.com/user-attachments/assets/728ab6f9-9cd3-48e1-9d75-e3fa73cd0dee)

### 3. **Detailed View Screen**
![image](https://github.com/user-attachments/assets/1fc2511d-0ab2-4050-935a-6fae375776b2)

### **Prerequisites**
- Android Studio (latest version recommended).
- Basic knowledge of Android development using Kotlin.

