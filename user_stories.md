**Title:**
_As a [user role], I want [feature/goal], so that [reason]._

**Acceptance Criteria:**
1. [Criteria 1]
2. [Criteria 2]
3. [Criteria 3]

**Priority:** [High/Medium/Low]
**Story Points:** [Estimated Effort in Points]
**Notes:**
- [Additional information or edge cases]
- 
** Admin User stories for Access and Functionality
  1. Log in to the system
        _As an admin user, I want to log into the portal with username and password to manage the platform securely
           Acceptance criteria:
              - system should log me in with valid credential
              - system should deny access if the log in credential doesn't match
  3. Log out from the system
        _As an admin user. I want to log out from the portal using log out button to protect the systeme.
           Acceptance criteria:
              - log out button should securely log me out from the system
  5. Add Doctors to the Portal
        _As an admin user, I can add doctors to the portal
           Acceptance criteria:
              - system should have option to add doctors
              - System should show message that doctors have been added successfully
              - System should show a current doctors list, including the new doctor, marked     
  7. Delete Doctors from the portal
         _As an admin user, I can delete a doctor from the portal who no longer available
           Acceptance criteria:
                 - System should have option to delete doctors
                 - System should show message that doctors have been deletec successfully
                 - System should show a current list of Doctors, excluding the deleted doctor
  9. Able to run stored procedures 
         _As an admin users, I can run stored procedures in MSQL CLI to get the number of appointments and track usage statistics
           Acceptance Criteria:
                 - system should allow to admin users to run stored procedures           

** Patient User Storines for Booking and Managing Appointments
      1. View list of doctors without logging in to explore options before registering
            _As a new patient, I will be able to see the doctor list as a guest user
               Acceptance criteria:
                  - System should have a menu option to show the doctors list in the home page
                  - Clicking on the menu "View Doctors" will open the doctors list page
      2. Sign up using your email and password to book appointments
            _As a new patient, I will be able to sign up using my email and setting up a password
               Acceptance criteria:
                  - When I click on to the sign-up link in the home page, system will take me to the sign-up page where I can set my username and password
                  - system will confirm that an account has been created through email
      3. Log into the portal to manage you bookings
            _As a registered patient, I will be able to manage my appointments, make new appointment, change appointment and cancel appointment
                Acceptance criteria:
                  - System will allow to make new appointment
                  - System will allow to change appointment
                  - System will allow to cancel appointment
                  - System will confirm appointment status by sending email 
      4. Log out from the system to secure account
            _As a registered patient I will be able to log out from the system
              Acceptance criteria:
                    - system should log me out by clicking the log out button
                    - a message will be shown that log out is successful
      5. View my upcoming appointments so that I can prepare myself
            _As a registered patient, I will be able to see my upcoming appointments
               Acceptance criteria:
                     - System will show in patient dashboard a list of upcoming appointments sorted by date

** Doctor User Stories for managing availability and appointments
        - Doctors will be able to make themselves available or not available for a particular time
        - Doctors can see all the appointments along with patient details
        - Doctors will be able to edit the appoinments as needed to change their availability
        - Doctors can create, edit and delete prescriptions


       
