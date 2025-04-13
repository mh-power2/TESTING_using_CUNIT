# Welcome to my Testing project using Cunit

## First a breif about the project and how it works
### 2 SW Users Description 
The software is designed to deal with 2 types of users 
1. Admin Mohamed Tarek: 
This user type is used to manage the Software and can do the 
following: 
* Register new user account to the Software 
* Delete user account from the Software  
* Check all available Courses Registrations  
* Print all user’s information including login credentials 
* Print Specific user information including login credentials 
This user Type should login at the startup with a secret Token 
defined in the File Sec.h  
2. Normal User (Student) 
This user type is used to interact with the Software and can do the 
following: 
a. Create Account 
i. Entering his personal info and login credentials to have 
an account on the Software 
b. Login to Account  (after successful login user can:) 
* Logout from his Account 
* change his password 
* see his info (not including username and password 
* Reserve a course from an announced list of courses 
* Show his Enrolled Courses

### SW Components
1. APP 
This Component Contains the Main App Logic that mainly Detects 
the User Type (illustrated in section 2) 
a. Admin User: 
* Verifies the credentials of the Admin  
* Note: To Login as an Admin use the token: 10203040 
you can change it in the file Sec.h 
* If successful verification it goes to Admin Page 
b. Customer User: 
i. Load the User Page to (Login/Create Account) 
c. Wrong Entry / Admin not verified: 
i. Terminate the Software 
2. BackEnd 
* This component is the main logic of the application which is 
responsible for Running the Logic of: 
* Admin Page  
The home page after Admin Successful verification
* Customer Page 
The home page if the user type is Customer to Login or 
Create Account
* Student Page 
Running the Home Page for the Student after a Successful 
Login 
* Also The Backend Component Also responsible for getting the 
choices from the user, Checking it and verifying it’s correctness, 
then Adding/Removing/Invoking the Data to/from Database 
Component if needed.
* Course Registration: 
This Component is used by The Backend Component to make a 
reservation for a student, Show the List of available courses and 
show the list of courses that a specific student is registered to. 
 
* Create Account 
This component is used by The Backend component to take a form 
from the User/Admin to create an account after the verification of 
the Input form. 
and if verified it adds / removes the Account from the Database. 
 
* CUnit 
This Component is the CUnit Library Header/Source files  
* DB 
This is the Data Base Manager Component which is responsible for 
Receiving Requests from the Backend Component and making 
CRUD operations to the Database itself   
* Note: CRUD (Create/Read/Update/Delete) 
it also contains the DB info which contains the definition of the DB 
Variables which contains the Data elements (Users info, Login 
Credentials, ..etc.). 
 
* Final Project 
This Folder Contains the output file of building the whole project 
 
* Generic 
This Component contains the header files contains the declaration 
of the Data Types used in our Software and the info about the size 
of users allowed in the SW, the number of Available courses and 
some other important definitions  
 
* Login  
This component is used by the Backend component to handle the 
login functionality in the Software it performs the following: 
a. Detecting User Type 
b. Verifying the Admin Token to Login 
c. Verifying the User Attempt to Login 
 
* Security 
This Component Contains the Definition of the Admin Security 
Token used for Admin Login Verification
11. Tests 
This Component is used to perform the testing on the Application 
Software it contains initial test cases and test suites.  
 
* Main.c 
This is the File that contains the main function that starts the 
Application or the Test
* Tests 
This Component is used to perform the testing on the Application 
Software using Cunit

# Everything is commented and there is a TXT file you should read before running have fun :)
