# MakeMyTrip

Installation : 
1. There is a pom.xml file in the project which contains the dependencies required to run the project.

2. Java details
   java 9.0.4
   Java(TM) SE Runtime Environment (build 9.0.4+11)
   Java HotSpot(TM) 64-Bit Server VM (build 9.0.4+11, mixed mode)

Test Cases covered for login scenario: 
Positive test cases
1. Login scenario with valid email and valid password.
2. Verify login window UI.
3. Verify create new account link on login window.
4. Verify reset password link on login window.
5. Verify 'login via OTP link' on login window and back arrow of 'enter OTP' window.
6. Verify back arrow on password window of login page.
7. Verify re-send OTP link on password window of login page.
8. Verify get OTP to login with mobile link on login page.
9. Login scenario with valid mobile number and valid password.

Negative test cases
1. Login scenario with invalid email and verify error message.
2. Login scenario with valid email and invalid password.
3. Login scenario with blank username.
4. Login scenario with valid email and blank password.

Note : 1. I have not covered negative test cases for login with mobile number due to time constraints.
       2. some part of the automation script contains static wait again for the same reason.
       3. I have not written test functionality for back arrow that is on verify your email id page that pops up after                   clicking on 'or login via OTP' link. 
       4. Multiple tries to login with mobile number with password by ignoring the OTP part results in error that says 
          "Token threshold is reached.: Country Code: 91 National Number: displays the number here used to generate OTP"(This            is again not covered).
       5. On thge same page with the above error message, when you click on resend OTP, System throws an other error, i.e 
           "Looks like we are facing some technical issues, please try again in some time(uncovered).
           
Validations covered for round trip booking are:
1. Verify application launch.
2. Verify click on search button redirects to flight search page.
3. Verify departure flight is from 'Goa' to 'Mumbai'.
4. Verify Total fare is matching the addition of individual flight fare.
5. Verify review page is displayed.
4. Verify return flight is from 'Mumbai' to 'Goa'.

*****Let me know if you find any issue to run the project.*******
