## Description

Feeding Canadian Kids is a non-profit organization that takes in applications from after-school *Programs*, which are in need of food for kids, and *Restaurants*, which are looking to donate food. The *Admins* from Feeding Canadian Kids would then browse new applications and manually fill in the information that a *Restaurant* or *Program* provided into an excel sheet. Then, manually pair them up according to the dates when they can deliver or accept food.

The problem we are trying to solve is that their current process is manual, and as they are trying to expand their program, it would be very hard for admins at Feeding Canadian Kids to continue to complete everything manually.

The web-application we are creating is meant to automate their current registration process and make the pairing process easier. We enable the end-users, *Programs* and *Restaurants*, to register accounts and then fill their profiles with their information and schedules. Then, the *Admins* can see all the applications and create new pairings accordingly.

# Development requirements
## Instructions for Mac OS:

### Install and use Python 3.6

### Install Miniconda: `brew install --cask miniconda`

### Close Git repository: git clone [OUR_REPOSITORY_URL]

### Make sure you're branch is master

### Type `conda create --name djangoEnv` in your terminal and press Enter

### Confirm location by typing 'y' in your terminal.

### Type `conda activate djangoEnv` in your terminal and press Enter.

### Type `conda install python=3.6` in your terminal and press Enter.

### Confirm installation by typing 'y'.

### pip3 install django==1.11

### python -m django --version

### should say 1.11


### Type 'y' to confirm installation.

### Type `pip install django-misaka` in your terminal and press Enter.

### Type `pip install django-bootstrap3` in your terminal and press Enter.

### Type `pip install django-braces` in your terminal and press Enter.

### Type `pip install pymysql` in your terminal and press Enter.

### Type `pip install pillow` in your terminal and press Enter.

### Type `pip install faker` and press Enter.

### pip install resources

### pip install requests

### pip install staty

### Type ./run.sh to run the shell script that will make migrations and run the application

### If you want to populate database with some data before testing, type python populate_db.py

### Running Django server can be turned off by typing Ctrl + C.

&nbsp;

You can run this application on any modern Operating System that supports Python 3.6. Additional installations need to be done to run the project:
* First you need to install conda on your machine. Instructions for how to install can be found here: https://docs.conda.io/projects/conda/en/latest/user-guide/install/macos.html
* Create a new folder, call it [YOUR_FOLDER_NAME]
* Open console and navigate to [YOUR_FOLDER_NAME]
* Clone our GitHub repository into your folder by using 
   * git clone [OUR_REPOSITORY_URL]
* Make sure you're branch is master
* Navigate into folder called "team-project-feeding-canadian-kids-team-1"
* Navigate into project called "project"
* Type conda create --name djangoEnv in your terminal and press Enter
* Confirm location by typing 'y' in your terminal
* Type conda activate djangoEnv in your terminal and press Enter
* Type conda install python=3.6 in your terminal and press Enter
* Confirm installation by typing 'y'
* Type conda install django=1.11 in your terminal and press Enter
* Type 'y' to confirm installation
* Type pip install django-misaka in your terminal and press Enter
* Type pip install django-bootstrap3 in your terminal and press Enter
* Type pip install django-braces in your terminal and press Enter
* Type pip install pymysql in your terminal and press Enter
* Type pip install pillow in your terminal and press Enter
* Type pip install faker and press Enter
* Type ./run.sh to run the shell script that will make migrations and run the application
* If you want to populate database with some data before testing, type python populate_db.py
* Running Django server can be turned off by typing Ctrl + C

## Key Features
Our product consists of two almost-separate applications. We have designed the admin and end-user portals. Here we list the features of each:

**Admin Portal**: 
1.    Multiple admins can log in to their accounts.
2.    There, they can access new notifications (which are updated in real-time)
3.    They can access a settings page in which they can change their profile information. 
4.    In the settings page, they can add additional admin accounts. 
5.    They can access pages with lists of individual programs and restaurants. 
6.    They can manually add and edit new programs and restaurants.
7.    They can access the users' information, reply to their requests, 
8.    They can accept/deny new-account applications. 
9.    They can visit pairings, review them, make new ones, and remove the selected ones.
10.    Then can review and accept/deny requests made by users.
 
**End-users**:
1.    End-users of two kinds (Restaurant owners and Program representatives) can sign-up, login, and make an application to become a partner. 
2.    After their application is reviewed, if they are accepted by Feeding Canadian Kids’ admins, the end-users can access their dashboard.
3. Users, they can see their information and their schedule. 
4. Users can access their pairing with other partners.
5. Users can make requests to Feeding Canadian Kids admins.
6. Users can edit their requests.
7. Users can access the settings page, in which they can change their account information. 




## Instructions

Our instructions will walk you through different areas of our application and will help you to get familiar with its functionality.

* Step 0: go to http://farazkhosh.pythonanywhere.com
* Step 1: Login/Signup
   + Navigate to the landing page, which corresponds to address "/".
   + You will see a sign-up page for users. Your next task is to create a new account. Enter your first name, last name, a valid email address, and password. 
       + You can use the following data if you want: 
       + Sample credentials: 
           + First name: John
           + Last name: Davis
           + email: johndavis@gmail.com
           + password: 123456789
           + Select restaurant for the type
    + You don't have to these sample credentials, as our account system is fully functional.
   
   + Click sign up.

   + You should be navigated to the home page, from where you can submit an application. 

* Step 2: Submit the application
  + Now that you've created an account, you need to provide the information for the fields in the form in order to create a restaurant account. We provide sample information that you can enter here, but you are not required to enter the same information.
      + Restaurant name: Subway
      + Current position: owner
      + Your phone number 6471112233
      + How many meals: 5
      + Uber Eats: Yes
      + Health & Safety Certificate: All Good
      + Address: nowhere street 99
      + What days are required: select Monday
      + Start time: 9:00 AM
      
  + Click 'Submit'
  + You will see the page that says: 
 'Thank for submitting your application!
  We will work to get back to you within 48 business hours.'
  
  + Congratulations! You have successfully applied to become a restaurant! Now you need to wait for the admin to review your application.

  + Let's now log in as an admin into the admin portal!

* Step 3: Log out
   + Go to http://farazkhosh.pythonanywhere.com/logout in order to sign out of your user account.


* Step 4: Admin Login
    + Navigate to the landing page, which corresponds to address http://farazkhosh.pythonanywhere.com/admin/login.
    + Here you need to enter admin login information
        + You can use the following email and password to login as admin:
            + Email: demo_admin@fck.com
            + Password: 123456789

+ Click 'login'. You will be automatically redirected to the admin's homepage after you log into the admin portal.
      
            
* Step 5: Admin Homepage
     * After logging in, the admin user would be brought to the address "http://farazkhosh.pythonanywhere.com/admin" which is the homepage.
         * The homepage displays the schedule for that current day
         * From the homepage is where the admin user can navigate to all the other features.

* Step 6: Admin Applications Page 
    + Now navigate to the applications page: http://farazkhosh.pythonanywhere.com/admin/applications/, find the application with your restaurant's name, and click on the blue 'Review' button beside it.


* Step 7: Review your own application!
    + Now, you should see all the information that you have provided in the Restaurant Application! You should also see a table at the bottom of the page that shows the schedule that you have specified in your application. Of course, you want to accept your own application, so click the 'Accept' button! 
    + Congratulations! You have just accepted your own application! 
    + To verify that it actually worked, go to http://farazkhosh.pythonanywhere.com/admin/applications/ and take a look at the first table. You will see that the name of your restaurant has disappeared from the application table! It means that the application was reviewed, and its status is not "Pending" anymore. In our case, the status of your application will be "Accepted"!


* Step 8: Restaurants page
    + Go to http://farazkhosh.pythonanywhere.com/admin/restaurants/
    + Here, you should be able to see the name of your restaurant, the application for which you have just approved. Congratulations! Now you're officially a restaurant owner!


* Step 9: Log out from the admin portal
    + Go to http://farazkhosh.pythonanywhere.com/admin/logout/ to sign out. 

* Step 10: Log into your restaurant account
    + You have created this account in step 1. You will need to provide your email and password to log in. Go to http://farazkhosh.pythonanywhere.com/login and click a small blue button at the bottom that says 'Log In'. It has 'Already a user?' besides it. 
    + After you click the button, the login form should be displayed.
    + Enter your email and password in the correct fields.
    + Click 'LOGIN'.
    + After you click login, you should be redirected to your user homepage, which is at the following address: http://farazkhosh.pythonanywhere.com/
    + You should be able to see your current schedule in the 'Schedule' table. The table called 'Program information' should be empty at this point, since you haven't been paired with any programs.

* Step 11: Creating a new request:
    + Go to http://farazkhosh.pythonanywhere.com/requests/
    + This is the page where you can submit requests of various types, such as "Schedule change", etc.
    + Click on the blue "New Request" button to begin! 
    + After you click the "New Request" button, you should be redirected to http://farazkhosh.pythonanywhere.com/requests/new, where you need to fill in the form for your new request! 
    + There are 4 types of requests currently available: 'Profile', 'Schedule', 'Partner Change', 'Other'. When we submit a request, admins will receive and read it, and then they may or may not accept or deny it. If admins choose to accept the request, they will need to perform the changes asked by request. In case admins deny a request, they will need to write a message to the user that explains why the request was denied.
    + Let's submit a request for Schedule change! 
    + Select 'Schedule' for the 'Type of Request'.
    + Select Monday in your answer to 'What schedule would you like to change to?'
    + Select 11:00 AM as a start time.
    + Click on 'Submit Request' to submit your request.
    + After clicking the button, you should be redirected to http://farazkhosh.pythonanywhere.com/requests/, where you can see all of your requests.
    + Notice that the status of your request is 'In Review', which means that admins haven't approved your request yet.
    + But what if we have changed our mind, and now we want to start at 8:00 AM ?! No problem! You can always edit your request! We explain how you can do it in the next step.

* Step 12: Editing a request
    + Click on 'Edit' button beside your newly submitted request. 
    + You will be redirected to a new page where you will be able to edit your request! 
    + Click on time and change it to 8:00 AM
    + Now click 'Save Changes' to modify your request!
    + After you click the button, you should be redirected to http://farazkhosh.pythonanywhere.com/requests/

* Step 13: Log out
    * Click on your name in the upper right corner (to the right of a profile image).
    * Click 'Logout' button in the drop-down menu.
    * You should be redirected to the signup/login page/
    * Congratulations! At this point, you have completed the set of instructions for the user side of our application!


* Step 14: Login into the admin portal
    + Go to http://farazkhosh.pythonanywhere.com/admin/login
    + Here you need to enter admin login information
        + You can use the following email and password to login as admin:
            + Email: demo_admin@fck.com
            + Password: 123456789

  + Click 'login'. You will be automatically redirected to the admin's homepage after you log into the admin portal.

* Step 15: View notifications

    * The admin user can view notifications by clicking the bell in the top right, which shows all current new notifications present. 
    * Notifications are updated in real-time, so when a new request or application is added to the system, the admin will get a notification. 

* Step 16: View Settings Page
    * The admin user can go to the settings page by clicking on their icon in the top right corner of the screen and then clicking on settings. 
    * Here, the admin can change their icon, name, email.
    * Here, the admin can also add additional admins.
    * Here you can change the admin profile name by entering a new first and last name and clicking submit. You can do the same with email and password.
        * Once this is changed, you must use the new email and password to log in. And the old email and password will become invalid. 

* Step 17: View list of Programs or Restaurants
    * The admin user can click on the side menu bar for a list of restaurants or a list of programs. 
    * Here, admins can manually add new restaurants and new programs on each page, respectively. They can click "Add New Restaurant" or "Add New Program" in the top right of the table, and this will bring them to a form to fill in the information about the main contact, and the restaurant or program.
        * The restaurant and program will both be automatically approved if added manually.

* Step 18: Pair Programs and Restaurants together
    * The admin user can click on pairings in the side menu bar, and reach the pairings page.
        * Here, the admin user can select a pairing and remove it by clicking the remove pairing button.
        * The admin user is also able to create a new pairing by clicking add new pairing button.
            * Admin should select a restaurant and a program from two tables before clicking the add pairing button.

* Step 19: Accepting/Denying Applications
    * The admin user can view applications that are pending by going to the URL http://farazkhosh.pythonanywhere.com/admin/applications. 
        * Here, the admin user can view all pending applications sorted in two tables. One for restaurants, and the other one for programs. 
        * The user can click on review button beside each of them, and their profile will be brought up. 
            * On the profile page, the admin can accept the application or deny it.
                * If the admin denies an application, they can leave a note on the reason the application was rejected. This reason will be shown to a user the next time they log. That user will also need to resubmit their application.


## Licences
* We are applying MIT License to our codebase.
 
* MIT license allows us to modify the original source code, which provides us with additional flexibility in terms of planning further development strategy. MIT license also allows Feeding Canadian Kids to claim copyright in case their property rights are violated.

* Our decision was to use MIT license for our project because it is very permissive and also because it allows for our project to be freely distributed. MIT license provides us with additional flexibility in terms of modifying our project, which allows us to worry more about the product and less about paperwork.



