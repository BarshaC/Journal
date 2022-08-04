#Section 0: FlaskProject

##Section 1: Overview
- Learning journals are often named for a specific purpose and/or format–a creative writing journal, for example. 
Even a personal blog is a kind of journal, and can thus become a learning journal if the blogging is done in order to promote, deepen, or extend learning of some kind.
-uses jinja template to dynamically build HTML pages using python concepts 
such as variables, loops, lists and so on. 

##Section 2: Why I built this project?
-Learning to make website using flask
- connect back end programming to front end 

##Section 3: Explaining templates
All the templates are the entended from the layout.html
home.html
- includes all the html code for the home page
login.html
- includes frame for the login detail 
layout.html
-basic layout for the whole website
register.html
-basic layout for the new users to register
writejourney.html
-Edit the post which include forms which can help with the editing and posting

##Section 4: Explaining python files
*forms.py: 
-uses wtforms so the user can enter the input and help with the form
-RegistrationForm() includes variables like username, email, password, confirm password and submit which are responsible to make a from with these heading so the users can sign up for their accounts
-LoginForm() includeds variables like email, password which user can use to login
-UpdateAccountForm() is mainly respondible to updating the account username and email for the users
*routes.py: using app routes which can allow the pages to connect from one wepage to another 
- home() is responsible to show the journals. I have used paginate in order to fit certain number of journal post on one page and the other posts get shifted to the other page.
-about() is the about page. Note, I have not completed on the about page. Because, that was the motive of my project as I had proposed. But, I will be adding on to features like about page and calenders and side page in the days come.
-update_post() is responsible for routing the update to the another page which is actually a for updating the journals.
-delete_post() is responsible for routing to the dialogue box which has option to either to delete or update the post.
-register() functions to anchor to signup.html
-login() functions to anchor login.html
-logout() functions as to achor to login.html so the user ends up in the login page after logging up.
-account() functions only and only if the user has logged in the page.
-save_picture() funtions emails the user to browse through the PC using app.root_path and os.path
*models.py: uses the db in order to manage the users and the username
-User() makes the database for the credentials for the user like login credentials,posts, password,email, username and image_file
-Posts() makes the columns and add the data like the title of the posts and the actual content so the user can extract it when needed


