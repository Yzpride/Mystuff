# Use case model
## 1 Use Case Diagram
 

## 2 Use case descriptions
As can be seen from the use case diagram, there is only one user (i.e. George P. Burdell) and below are the descriptions for each use case:

### Use case 1: Enter/Edit current job 

Requirements: This use case will allow the user to enter (if it is the first time) or edit all the details of their current job.

Pre-conditions: The app is started and the user is presented with the main menu.

Post-conditions: The current job information is updated and saved.

Scenarios: <br>
If the current job is present, the system displays the details of the current job and prompts the user to select the desired activities: 1) edit, 2) delete, 3) save and exit, and 4) cancel and exit.  <br>
•	If the user selects edit, the system allows the user to modify the details of the current job. <br>
•	If the user selects delete, the system allows the user to delete all details of the current job. The system also internally changes the current job status to not present. Then the user is brought back to the main menu (use case ends). <br>
•	If the user selects save and exit, the system allows the user to save the current details and exit the interface back to the main menu (use case ends).  <br>
•	If the user selects cancel and exit, the system ignores the user entered details and exit the interface back to the main menu (use case ends). <br>

If the current job is not present, the system prompts the user to select the desired activities: 1) add, 2) save and exit, and 3) cancel and exit.  <br>
•	If the user selects add, the system allows the user to enter the details of the current job. <br>
•	If the user selects save and exit, the system allows the user to save the job details. The system also internally changes the current job status to present, and exit the interface back to the main menu (use case ends).  <br>
•	If the user selects cancel and exit, the system ignores the user entered details and exit the interface back to the main menu (use case ends).  <br>

### Use case 2: Enter job offers

Requirements: this use case will allow the user to enter or edit all the details of their job offers and compare the job offer against the current job (if present).

Pre-conditions: the app is started and the user is presented with the main menu.

Post-conditions: the job offer information is updated and saved. Comparison results against the current job are displayed. 

Scenarios: <br>
If the current job is present, the system prompts the user to select the desired activities: 1) add offer, 2) save and compare with current job, 3) save and exit, and 4) cancel and exit.  <br>
•	If the user selects add offer, the system provides a user interface and allows the user to add the details of the job offer. <br>
•	If the user selects save and compare with current job, the system displays the job comparison results and prompts the user to return back to main menu (use case ends). <br>
•	If the user selects save and exit, the system allows the user to save the job details and exit back to main menu (use case ends). <br>
•	If the user selects cancel and exit, the system ignores the user entered details and exit the interface back to the main menu (use case ends). <br>

If the current job is not present, the system prompts the user to select the desired activities: 1) add offer, 2) save and exit, and 3) cancel and exit.  <br>
•	If the user selects add offer, the system provides a user interface and allows the user to add the details of the job offer. <br>
•	If the user selects save and exit, the system allows the user to save the job details and exit back to main menu (use case ends). <br>
•	If the user selects cancel and exit, the system ignores the user entered details and exit the interface back to the main menu (use case ends). <br>

### Use case 3: Adjust the comparison settings

Requirements: this use case will allow the user to assign integer weights to factors for comparing jobs. 

Pre-conditions: the app is started and the user is presented with the main menu.

Post-conditions: the comparison settings have been updated. 

Scenarios: <br>
The system displays the current comparison settings and prompts the user to select the desired activities: 1) adjust the comparison settings, 2) save and exit, 3) cancel and exit. <br>
•	If the user selects adjust the comparison settings, the system allows the user to enter the integer weights to those factors.  <br>
•	If the user selects save and exit, the system allows the user to save the factor weights and exit back to main menu (use case ends).  <br>
•	If the user selects cancel and exit, the system ignores the user entered details and exit the interface back to the main menu (use case ends). <br>

### Use case 4: Compare job offers

Requirements: this use case will allow user to compare two jobs.

Pre-condition: the app is started and the user is presented with the main menu.

Post-conditions: comparison results between two jobs have been displayed. 

Scenarios: <br>
The system verifies how many jobs (including both current job and job offers) are available.  <br>
If there are no jobs available, the compare job offers use case should be disabled in the system.  <br>
If there is only one job available, the system displays the job details and prompts the user to return to the main menu and enter another job.  <br>
If there are at least two jobs available, the system displays a list of job offers including the current job (if present) and prompts the user to select two jobs to compare and trigger the comparison.  <br>
The system displays the comparison results and then prompts the user to select the desired activities: 1) perform another comparison, and 2) exit <br>
•	If the user selects perform another comparison, the system return the user back to the displayed the job list and prompts the user to do another selection <br>
•	If the user selects exit, the system exits back to the main menu (use case ends).  <br>
