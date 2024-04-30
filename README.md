# Django- Email-Authentication Form
 A simple form is created using HTML/CSS and authenticated via email using **python Django Framework**


Here, a simple form is created where a user can signup, login and signout. Some important steps and features:

- A user cannot signIn if he/she hasn't sign up first.

- While signing up, a user must be carefully not to enter same username or email which is already registred or in used in the form. 
  As all the data will be stored in the database and if the form identifies the same username or email then, user is prompt an error message and redirected home page.

- After filling up the form and the signup button is click, a message will be prompt to user asking to verify the email.

- Now, user must go to their mail where 2 messages would already had been send. One message is a welcome message and 
 another mail is for confirming and verifying the email of user.

- After verifying the mail (i.e. by clicking the link ), the user'd be finally logged in into the form.

- there will be a signout button which helps user to signout from form.

- Once the user has been signed up in the form, they can use their log in information(i.e. username and password) to logged in into the form again.

- All the data entered by the user are stored in database which is only accessable to admin.


**Everything used:**
- Django mail to send mails for registration
- **_Six is used to generate unique token (pip install siz)_**
- view.py contains all the api for all the function to work.
- while for generating _token_, it is written in token.py file seperately


NOTE: if user tries to log in into the form without verifying their email then they would be directly redirect to home page with an message as "bad credentials".
